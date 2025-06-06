---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Niveaux d’autorisation de  [!DNL Workfront]  pour Outlook
description: Le module complémentaire  [!DNL Workfront for Outlook]  requiert un accès en lecture/écriture à la boîte de réception. L’intégration  [!DNL Workfront for Outlook]  requiert les autorisations les plus élevées, car elle permet de télécharger les pièces jointes aux e-mails à partir du serveur d’échange Outlook et de les charger sur  [!DNL Workfront], lorsque l’utilisateur ou utilisatrice envoie une demande à partir d’un e-mail contenant des pièces jointes.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 79%

---

# Niveaux d’autorisation pour [!DNL Workfront for Outlook]

>[!IMPORTANT]
>
>[Microsoft est en train de désactiver la prise en charge des jetons Exchange Online hérités](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) actuellement utilisés par le complément Workfront Outlook pour l&#39;authentification. Cette modification apportée par Microsoft a déjà commencé à affecter les clients et continuera à être déployée par phases jusqu’en octobre 2025.
>
>* **Une fois que Microsoft a complètement désactivé ces jetons, l’intégration de Workfront pour Microsoft Outlook ne fonctionne plus.**
>
>Dans le cadre de cette modification, Microsoft a pris la décision de modifier la manière dont les jetons sont réactivés. Après le **30 juin 2025**, les administrateurs ne pourront plus réactiver les jetons eux-mêmes. Seule la prise en charge de Microsoft peut accorder des exceptions. **Le 1er octobre 2025, les jetons hérités seront désactivés pour tous les clients. Les exceptions ne seront pas accordées.**


[!DNL Workfront for Outlook] nécessite le niveau le plus élevé des quatre niveaux d’autorisations autorisés dans les modules complémentaires [!DNL Outlook].

Pour plus d’informations sur les autorisations dans les modules complémentaires [!DNL Outlook], voir [Confidentialité, autorisations et sécurité pour les modules complémentaires  [!DNL Outlook] ](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) dans la documentation [!DNL Microsoft].

Le module complémentaire [!DNL Workfront for Outlook] requiert un accès en lecture/écriture à la boîte de réception (`ReadWriteMailbox`), soit le niveau d’autorisation le plus élevé.
L’intégration [!DNL Workfront for Outlook] requiert les autorisations les plus élevées, car elle permet de télécharger les pièces jointes aux e-mails à partir du serveur d’échange [!DNL Outlook] et de les charger sur [!DNL Workfront], lorsque l’utilisateur ou l’utilisatrice envoie une demande à partir d’un e-mail contenant des pièces jointes. Pour que cette fonctionnalité fonctionne, [!DNL Workfront for Outlook] utilise la fonction `mailbox.getCallbackTokenAsync()` de l’API JavaScript de module complémentaire [!DNL Office] pour obtenir le jeton et l’utiliser pour télécharger les pièces jointes d’e-mail à partir du serveur d’échange. La seule autorisation qui permet l’utilisation de cette fonction est `ReadWriteMailbox`. Pour plus d’informations, voir [Confidentialité, autorisations et sécurité des modules complémentaires Outlook](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) dans la documentation de Microsoft.

Le module complémentaire [!DNL Workfront for Outlook] requiert également l’autorisation `ReadWriteItem` (incluse dans `ReadWriteMailbox`), qui est utilisée pour lire le corps de l’e-mail et lire/mettre à jour les métadonnées de l’e-mail :

* Lire le corps de l’e-mail :

  [!DNL Workfront for Outlook] lit le corps de l’e-mail lorsqu’une personne envoie la demande ou envoie le corps de l’e-mail comme mise à jour de l’objet [!DNL Adobe Workfront].
* Lire/mettre à jour des métadonnées d’e-mail :

  [!DNL Workfront for Outlook] met à jour les en-têtes d’e-mail lorsqu’une personne envoie une demande à partir d’un e-mail. Cela permet de stocker des informations sur les objets [!DNL Adobe Workfront] envoyés, de sorte que la prochaine fois que l’utilisateur ou l’utilisatrice ouvrira le module complémentaire pour le même e-mail, les informations sur les actions précédentes avec cet e-mail s’afficheront.

[!DNL Workfront for Outlook] accède à la boîte de réception d’une personne uniquement lorsque celle-ci effectue une action dans le module complémentaire. Il ne dispose d’aucune fonctionnalité d’arrière-plan. Workfront for Outlook accède uniquement à la boîte de réception d’une personne dans le scénario suivant :

* La personne tente d’envoyer une demande, de créer une tâche ou d’envoyer un e-mail en tant que mise à jour depuis [!DNL Workfront for Outlook] (ouverture du module complémentaire et sélection d’une action).
   * [!DNL Workfront for Outlook] lit le corps de l’e-mail à remplir dans le formulaire à l’intérieur du module complémentaire.
   * [!DNL Workfront for Outlook] lit les métadonnées de l’e-mail pour afficher des informations sur le module complémentaire au sujet des actions précédentes effectuées dans le module complémentaire avec le même e-mail.
* Lorsqu’une personne envoie une demande, crée une tâche ou envoie un e-mail en tant que mise à jour depuis [!DNL Workfront for Outlook] (en cliquant sur le bouton [!UICONTROL Envoyer] sur le module complémentaire) :
   * [!DNL Workfront for Outlook] lit le corps de l’e-mail pour l’envoyer à Workfront sous forme de description de la demande ou de commentaire.
   * [!DNL Workfront for Outlook] met à jour les métadonnées de l’e-mail pour stocker des informations sur les demandes envoyées ou l’objet mis à jour.
   * [!DNL Workfront for Outlook] télécharge des pièces jointes de l’e-mail à partir du serveur d’échange pour les charger vers les demandes envoyées, les tâches créées ou les objets mis à jour.
