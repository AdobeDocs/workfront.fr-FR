---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Niveaux d’autorisation pour [!DNL Workfront] pour Outlook
description: Le [!DNL Workfront for Outlook] Le module complémentaire requiert un accès en lecture/écriture à la boîte aux lettres. Le [!DNL Workfront for Outlook] l’intégration requiert les autorisations de niveau supérieur, car elle permet de télécharger les pièces jointes aux emails à partir du serveur d’échange Outlook et de les télécharger sur [!DNL Workfront], lorsque l’utilisateur envoie une demande à partir d’un courrier électronique contenant des pièces jointes.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Niveaux d’autorisation pour [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] nécessite le niveau le plus élevé des quatre niveaux d’autorisations autorisés dans [!DNL Outlook] modules complémentaires.

Pour plus d’informations sur les autorisations dans [!DNL Outlook] modules complémentaires, voir [Confidentialité, autorisations et sécurité pour [!DNL Outlook] add-ins](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) dans le [!DNL Microsoft] documentation.

Le [!DNL Workfront for Outlook] le module complémentaire requiert un accès en lecture/écriture à la boîte aux lettres (`ReadWriteMailbox`), qui est la portée d’autorisation la plus élevée.
Le [!DNL Workfront for Outlook] l’intégration requiert les autorisations de niveau supérieur, car elle permet de télécharger les pièces jointes aux emails à partir du [!DNL Outlook] Exchange server et chargez-les sur [!DNL Workfront], lorsque l’utilisateur envoie une demande à partir d’un courrier électronique contenant des pièces jointes. Pour que cette fonctionnalité fonctionne, [!DNL Workfront for Outlook] utilise la fonction `mailbox.getCallbackTokenAsync()` de [!DNL Office] API JavaScript complémentaire pour obtenir le jeton et l’utiliser pour télécharger les pièces jointes d’email à partir du serveur d’échange. La seule autorisation qui autorise l’utilisation de cette fonction est `ReadWriteMailbox`. Pour plus d’informations, voir [Confidentialité, autorisations et sécurité des modules complémentaires Outlook](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) dans la documentation de Microsoft.

Le [!DNL Workfront for Outlook] module complémentaire requiert également `ReadWriteItem` autorisation (incluse dans `ReadWriteMailbox`), qui est utilisé pour lire le corps de l’email et lire/mettre à jour les métadonnées de l’email :

* Lire le corps de l&#39;email :

   [!DNL Workfront for Outlook] lit le corps de l’email lorsqu’un utilisateur envoie la demande ou envoie le corps de l’email en tant que mise à jour à [!DNL Adobe Workfront] Objet.
* Lecture/mise à jour des métadonnées d’email :

   [!DNL Workfront for Outlook] met à jour les en-têtes de courrier électronique lorsqu’un utilisateur envoie une requête à partir d’un courrier électronique. Cela permet de stocker des informations sur les [!DNL Adobe Workfront] , de sorte que la prochaine fois que l’utilisateur ouvrira le module complémentaire pour le même courrier électronique, les informations sur les actions précédentes avec ce message s’affichent.

[!DNL Workfront for Outlook] accède à la boîte aux lettres d’un utilisateur uniquement lorsque celui-ci effectue une action dans le module complémentaire. Il ne dispose d’aucune fonctionnalité d’arrière-plan. Workfront for Outlook accède uniquement à la boîte aux lettres de l’utilisateur dans le scénario suivant :

* L’utilisateur tente d’envoyer une requête, de créer une tâche ou d’envoyer un courrier électronique comme mise à jour depuis [!DNL Workfront for Outlook] (Ouverture du module complémentaire et sélection d’une action)
   * [!DNL Workfront for Outlook] lit le corps du courrier électronique à remplir dans le formulaire à l’intérieur du module complémentaire.
   * [!DNL Workfront for Outlook] lit les métadonnées de courrier électronique pour afficher des informations sur le module complémentaire au sujet des actions précédentes effectuées dans le module complémentaire avec le même message.
* Lorsqu’un utilisateur envoie une requête, crée une tâche ou envoie un courrier électronique comme mise à jour à partir d’ [!DNL Workfront for Outlook] (en cliquant sur le bouton [!UICONTROL submit] sur le module complémentaire) :
   * [!DNL Workfront for Outlook] lit le corps du courrier électronique pour l’envoyer à Workfront sous forme de description de requête ou de commentaire.
   * [!DNL Workfront for Outlook] met à jour les métadonnées de courrier électronique pour stocker des informations sur les requêtes envoyées ou l’objet mis à jour.
   * [!DNL Workfront for Outlook] télécharge des pièces jointes de courrier électronique à partir du serveur Exchange pour les charger vers les requêtes envoyées, les tâches créées ou les objets mis à jour.
