---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Niveaux d’autorisation pour  [!DNL Workfront] pour Outlook
description: Le module complémentaire  [!DNL Workfront for Outlook] nécessite un accès en lecture/écriture à la boîte aux lettres. L’intégration  [!DNL Workfront for Outlook] requiert les autorisations de niveau supérieur, car elle permet de télécharger des pièces jointes d’email à partir du serveur d’exchange Outlook et de les télécharger vers  [!DNL Workfront], lorsque l’utilisateur envoie une demande à partir d’un courrier électronique contenant des pièces jointes.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Niveaux d’autorisations pour [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] nécessite le plus haut des quatre niveaux d’autorisations autorisés dans les modules complémentaires [!DNL Outlook].

Pour plus d&#39;informations sur les autorisations dans les modules complémentaires [!DNL Outlook], consultez la section [Confidentialité, autorisations et sécurité pour les  [!DNL Outlook] modules complémentaires](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) dans la documentation [!DNL Microsoft].

Le module complémentaire [!DNL Workfront for Outlook] nécessite un accès en lecture/écriture à la boîte aux lettres (`ReadWriteMailbox`), qui est la portée d&#39;autorisation la plus élevée.
L&#39;intégration [!DNL Workfront for Outlook] nécessite les autorisations de niveau supérieur, car elle permet de télécharger les pièces jointes d&#39;email à partir du serveur d&#39;exchange [!DNL Outlook] et de les télécharger vers [!DNL Workfront], lorsque l&#39;utilisateur envoie une demande à partir d&#39;un email contenant des pièces jointes. Pour que cette fonctionnalité fonctionne, [!DNL Workfront for Outlook] utilise la fonction `mailbox.getCallbackTokenAsync()` de l’API JavaScript de complément [!DNL Office] pour obtenir le jeton et l’utiliser pour télécharger les pièces jointes d’email à partir du serveur d’exchange. `ReadWriteMailbox` est la seule autorisation qui autorise l’utilisation de cette fonction. Pour plus d’informations, voir [Confidentialité, autorisations et sécurité des modules complémentaires Outlook](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) dans la documentation Microsoft.

Le module complémentaire [!DNL Workfront for Outlook] nécessite également l’autorisation `ReadWriteItem` (incluse dans `ReadWriteMailbox`), qui est utilisée pour lire le corps de l’email et lire/mettre à jour les métadonnées de l’email :

* Lire le corps de l&#39;email :

  [!DNL Workfront for Outlook] lit le corps du courrier électronique lorsqu’un utilisateur envoie la demande ou envoie le corps du courrier électronique en tant que mise à jour vers [!DNL Adobe Workfront] Object.
* Lecture/mise à jour des métadonnées d’email :

  [!DNL Workfront for Outlook] met à jour les en-têtes de courrier électronique lorsqu’un utilisateur envoie une demande à partir d’un courrier électronique. Cela permet de stocker des informations sur l’objet [!DNL Adobe Workfront] envoyé. Dès lors, la prochaine fois que l’utilisateur ouvrira le module complémentaire pour le même courrier électronique, les informations sur les actions précédentes avec ce message s’afficheront.

[!DNL Workfront for Outlook] accède à la boîte aux lettres d’un utilisateur uniquement lorsque celui-ci effectue une action dans le module complémentaire. Il ne dispose d’aucune fonctionnalité d’arrière-plan. Workfront for Outlook accède uniquement à la boîte aux lettres de l’utilisateur dans le scénario suivant :

* L’utilisateur tente d’envoyer une requête, de créer une tâche ou d’envoyer un email comme mise à jour depuis [!DNL Workfront for Outlook] (Ouverture du module complémentaire et sélection d’une action).
   * [!DNL Workfront for Outlook] lit le corps du courrier électronique à remplir dans le formulaire à l’intérieur du module complémentaire.
   * [!DNL Workfront for Outlook] lit les métadonnées de courrier électronique pour afficher des informations sur le module complémentaire au sujet des actions précédentes effectuées dans le module complémentaire avec le même courrier électronique.
* Lorsqu’un utilisateur envoie une requête, crée une tâche ou envoie un courrier électronique comme mise à jour à partir de [!DNL Workfront for Outlook] (en cliquant sur le bouton [!UICONTROL envoyer] sur le module complémentaire) :
   * [!DNL Workfront for Outlook] lit le corps de l&#39;email pour l&#39;envoyer à Workfront en tant que description de requête ou commentaire.
   * [!DNL Workfront for Outlook] met à jour les métadonnées de courrier électronique pour stocker des informations sur les requêtes envoyées ou l’objet mis à jour.
   * [!DNL Workfront for Outlook] télécharge des pièces jointes de courrier électronique à partir du serveur exchange pour charger des requêtes envoyées, des tâches créées ou des objets mis à jour.
