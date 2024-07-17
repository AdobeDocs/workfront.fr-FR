---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Envoyer les dépenses  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan]
description: Ce scénario d’intégration partage les détails relatifs aux dépenses d’un projet  [!DNL Adobe Workfront] avec un élément de liste  [!DNL Anaplan] budget. Le partage de ces informations vous permet de mieux tirer parti de l’optimisation des dépenses et de l’analyse financière fournie par [!DNL Anaplan] .
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 5%

---

# Envoyer [!DNL Adobe Workfront] dépenses à un élément de liste [!DNL Anaplan]

Ce scénario d’intégration partage les détails liés aux dépenses d’un projet [!DNL Adobe Workfront] avec un élément de liste budgétaire [!DNL Anaplan]. Le partage de ces informations vous permet de mieux tirer parti de l’optimisation des dépenses et de l’analyse financière fournie par [!DNL Anaplan].

>[!IMPORTANT]
>
>&quot;Campaign&quot; dans cet article fait référence au cas d’utilisation de campagne marketing que ce scénario représente et n’est en aucun cas connecté au connecteur Adobe Campaign [!DNL Workfront Fusion] ou à l’objet [!UICONTROL Campaign] récemment obsolète dans [!DNL Workfront].

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td> <p>Workfront Fusion pour l’automatisation et l’intégration du travail </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

&#42;&#42; Pour plus d’informations sur les [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Événement de déclenchement

Ce scénario est planifié pour s’exécuter toutes les 15 minutes.

## Configuration [!DNL Workfront] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Workfront] :

* Un profil utilisateur de [!DNL Workfront] nommé *[!UICONTROL *[!DNL Anaplan] Integration]**, disposant des droits d’administrateur système.

  Pour plus d&#39;informations sur la création d&#39;un utilisateur dans [!DNL Workfront], voir [Ajout d&#39;utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Un formulaire personnalisé **[!UICONTROL résumé de campagne]** joint à l’objet de projet pour stocker les valeurs de données personnalisées que vous choisissez d’envoyer à [!DNL Anaplan].

  Le formulaire doit contenir les champs suivants :

  | Nom de champ | Type de champ |
  |---|---|
  | [!UICONTROL Date de dernière transmission] | Date |
  | [!UICONTROL Notes d’intégration] | Zone de texte |

  Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer ou modifier un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Configuration [!DNL Anaplan] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Anaplan] :

* Un profil utilisateur dans [!DNL Anaplan] nommé **[!UICONTROL [!DNL Workfront]Integration]**, disposant des droits d’administrateur système.
* Le modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* Liste du modèle [!DNL Anaplan] dans lequel vous souhaitez capturer les budgets de campagne.
* Un fichier **[!UICONTROL Anaplan Importation des dépenses réelles]** contenant les colonnes suivantes, dans cet ordre :

   1. [!UICONTROL [!DNL Workfront] GUID de dépenses ]

   2. [!UICONTROL [!DNL Workfront] GUID de projet ]

   3. [!UICONTROL Montant réel]

   4. [!UICONTROL Description]

   5. [!UICONTROL Type de dépense]

   6. [!UICONTROL Date d’entrée en vigueur]

   7. [!UICONTROL Nom de la campagne]

   8. [!UICONTROL [!DNL Anaplan] ID d’élément de liste ]

  Pour préparer le fichier [!UICONTROL [!DNL Anaplan] Importation des dépenses réelles] :

   1. Copiez et collez les éléments suivants dans un éditeur de texte ou [!DNL Excel].
   1. Enregistrez le fichier au format CSV.
   1. Téléchargez le fichier dans [!DNL Anaplan].

      Pour plus d’informations, consultez la documentation [!DNL Anaplan] sur l’importation de données dans des modules à partir d’un fichier.

   1. Notez le nom que vous avez donné au fichier ; il sera utilisé lors du déploiement du modèle de scénario [!UICONTROL Fusion].

  Exemple de contenu CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* Un fichier **[!UICONTROL [!DNL Anaplan]d’&#39;importation de dépenses planifiée]** contenant les colonnes suivantes, dans cet ordre :

   1. [!UICONTROL [!DNL Workfront] GUID de dépenses ]

   2. [!UICONTROL [!DNL Workfront] GUID de projet ]

   3. [!UICONTROL Montant réel]

   4. [!UICONTROL Description]

   5. [!UICONTROL Type de dépense]

   6. [!UICONTROL Date d’entrée en vigueur]

   7. [!UICONTROL Nom de la campagne]

   8. [!UICONTROL [!DNL Anaplan] ID d’élément de liste ]

  Pour préparer le fichier [!UICONTROL [!DNL Anaplan] d’importation des dépenses prévues ] :

   1. Copiez et collez les éléments suivants dans un éditeur de texte ou [!DNL Excel]
   1. Enregistrement du fichier au format CSV
   1. Téléchargez le fichier dans Anaplan.

      Pour plus d’informations, consultez la documentation [!DNL Anaplan] sur l’importation de données dans des modules à partir d’un fichier.

   1. Notez le nom que vous avez donné au fichier ; il sera utilisé lors du déploiement du modèle de scénario [!UICONTROL Fusion].

  Exemple de contenu CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* Un processus **[!UICONTROL Project Update Import]** préparé pour exécuter l’importation de données livrées dans un téléchargement de fichier.

>[!NOTE]
>
>Il existe des fichiers d&#39;import distincts pour les dépenses prévues et réelles afin qu&#39;elles puissent être rapportées indépendamment respectivement au cours des dates prévues et en vigueur.

Pour obtenir des instructions sur l’une de ces actions, consultez la documentation [!DNL Anaplan].

## Déploiement sur [!DNL Fusion]

Effectuez les étapes suivantes pour déployer ce scénario d’intégration sur votre compte [!DNL Fusion]. Cette opération ne doit être effectuée qu’après avoir terminé la configuration [!DNL Workfront] et [!DNL Anaplan] requise.

1. Accédez au menu [!UICONTROL  Modèles] dans [!DNL Workfront Fusion] et cliquez sur le modèle de scénario **[!UICONTROL Envoyer les mises à jour des dépenses Workfront à [!DNL Anaplan] élément de liste]** .
1. Remplacez les valeurs de variable pour les variables [!DNL Anaplan] suivantes :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Nom de variable</th> 
      <th>Remplacer la valeur par</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>L’identifiant de l’espace de travail de votre compte [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID de modèle] </td> 
      <td>L’identifiant du modèle de votre compte [!DNL Anaplan] et l’espace de travail sélectionné que vous souhaitez utiliser pour ce scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Le nom de la liste de votre compte [!DNL Anaplan] et l’espace de travail et le modèle sélectionnés que vous souhaitez utiliser pour ce scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nom de fichier : Importation des dépenses réelles]</td> 
      <td> <p>Nom du fichier qui recevra les données de dépenses réelles du projet.</p> <p> (Exemple : WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nom de fichier : Importation de dépenses planifiée]</td> 
      <td> <p>Nom du fichier qui recevra les données de dépenses planifiées du projet.</p> <p> (Exemple : WorkfrontUpdateLinkedProjects_ScheduleExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nom du processus : Importation de mise à jour de projet]</td> 
      <td> <p>Nom du processus qui exécutera l’importation des données de dépenses du projet.</p> <p>(Exemple : WF Int - Chargement des dépenses de projet)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Vous trouverez des détails sur la configuration des fichiers et des processus dans la documentation de configuration de [!DNL Anaplan].

1. Sélectionnez ou ajoutez un profil de connexion [!DNL Anaplan].
1. Mettez à jour tous les modules [!DNL Anaplan] restants avec une connexion [!DNL Anaplan] lorsque vous y êtes invité.
1. Sélectionnez ou ajoutez un profil de connexion [!DNL Workfront].
1. Mettez à jour tous les modules [!DNL Workfront] restants avec une connexion [!DNL Workfront] lorsque vous y êtes invité.
1. Sur le module **[!UICONTROL Créer les dépenses réelles CSV]** , ajoutez une nouvelle structure de données pour mapper les attributs de projet aux colonnes CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. Sur le module **[!UICONTROL Générer une dépense planifiée CSV]** , ajoutez une nouvelle structure de données pour mapper les attributs de projet aux colonnes CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Autres modèles de scénario recommandés

Ce modèle de scénario est complété par les modèles de scénario d’optimisation des dépenses suivants qui peuvent également être déployés :

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] des mises à jour de projet à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer [!DNL Adobe Workfront] des mises à jour en heures réelles à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Scénarios supplémentaires pour lier les requêtes de budget :

* [[!UICONTROL  Créez un  [!DNL Anaplan] élément de liste à partir d&#39;une  [!DNL Adobe Workfront] requête de budget]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL  Appliquez une  [!DNL Anaplan] allocation budgétaire à un [!DNL Adobe Workfront] projet]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scénarios supplémentaires pour lier des requêtes de campagne :

* [[!UICONTROL  Créez un  [!DNL Anaplan] élément de liste à partir d’une  [!DNL Adobe Workfront] requête de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL  Appliquez une  [!DNL Anaplan]  allocation budgétaire à une  [!DNL Adobe Workfront] requête de campagne ou projet de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
