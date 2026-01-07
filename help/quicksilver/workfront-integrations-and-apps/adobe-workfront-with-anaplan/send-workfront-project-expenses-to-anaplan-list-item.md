---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Envoyer les dépenses  [!DNL Adobe Workfront]  à un élément de la liste  [!DNL Anaplan] '
description: Ce scénario d’intégration partage les détails relatifs aux dépenses d’un projet  [!DNL Adobe Workfront]  avec un élément de liste budgétaire  [!DNL Anaplan] . Le partage de ces informations vous permet de tirer le meilleur parti de l’optimisation des dépenses et de l’analyse financière que fournit  [!DNL Anaplan] .
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 98%

---

# Envoyer les dépenses [!DNL Adobe Workfront] à un élément de liste [!DNL Anaplan]

Ce scénario d’intégration partage les détails relatifs aux dépenses d’un projet [!DNL Adobe Workfront] avec un élément de liste budgétaire [!DNL Anaplan]. Le partage de ces informations vous permet de tirer le meilleur parti de l’optimisation des dépenses et de l’analyse financière que fournit [!DNL Anaplan].

>[!IMPORTANT]
>
>Dans cet article, le terme « campagne » fait référence au cas d’utilisation de la campagne marketing que ce scénario représente, et n’est en aucun cas lié au connecteur Adobe Campaign [!DNL Workfront Fusion] ou à l’objet [!UICONTROL Campaign] de [!DNL Workfront], qui a récemment été supprimé.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package de workflow Adobe Workfront et tout package d’automatisation et d’intégration Adobe Workfront</p><p>Workfront Ultimate</p><p>Packages Workfront Prime et Select, avec l’achat supplémentaire de Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licences Adobe Workfront</td> 
   <td> <p>Standard</p><p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront Fusion</td> 
   <td>
   <p>Basé sur les opérations : aucune exigence de licence Workfront Fusion</p>
   <p>Basé sur un connecteur (hérité) : Workfront Fusion pour l’automatisation et l’intégration du travail </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Si votre organisation dispose d’un package Workfront Select ou Prime qui n’inclut pas l’automatisation et l’intégration de Workfront, elle doit acquérir Adobe Workfront Fusion.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, consultez [Conditions d’accès requises dans la documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences Adobe Workfront Fusion, consultez [Licences Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Événement de déclenchement

Ce scénario est planifié pour s’exécuter toutes les 15 minutes.

## Configuration [!DNL Workfront] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Workfront] :

* Un profil d’utilisateur ou d’utilisatrice dans [!DNL Workfront] nommé *Intégration Anaplan*, disposant de droits d’administration système.

  Pour plus d’informations sur la création d’un utilisateur ou d’une utilisatrice dans [!DNL Workfront], voir [Ajouter des utilisateurs ou des utilisatrices](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Un formulaire personnalisé **[!UICONTROL Résumé de campagne]** joint à l’objet de projet pour stocker les valeurs de données personnalisées que vous choisissez d’envoyer à [!DNL Anaplan].

  Le formulaire doit contenir les champs suivants :

  | Nom du champ | Type de champ |
  |---|---|
  | [!UICONTROL Date de la dernière transmission] | Date |
  | [!UICONTROL Notes d’intégration] | Zone de texte |

  Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configuration [!DNL Anaplan] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Anaplan] :

* Profil d’utilisateur ou d’utilisatrice dans [!DNL Anaplan] nommé Intégration **[!UICONTROL [!DNL Workfront]]**, disposant de droits d’administration système.
* Le modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* La liste du modèle [!DNL Anaplan] qui doit contenir les budgets des campagnes.
* Un fichier **[!UICONTROL Import des dépenses réelles Anaplan]** qui contient les colonnes suivantes, dans cet ordre :

   1. GUID de dépense [!UICONTROL [!DNL Workfront]]

   2. GUID du projet [!UICONTROL [!DNL Workfront]]

   3. [!UICONTROL Montant réel]

   4. [!UICONTROL Description]

   5. [!UICONTROL Type de dépenses]

   6. [!UICONTROL Date effective]

   7. [!UICONTROL Nom de la campagne]

   8. [!UICONTROL [!DNL Anaplan] ID d’élément de liste]

  Pour préparer le fichier Import des dépenses réelles [!UICONTROL [!DNL Anaplan]] :

   1. Copiez et collez le texte suivant dans un éditeur de texte ou [!DNL Excel].
   1. Enregistrez le fichier au format CSV.
   1. Chargez le fichier dans [!DNL Anaplan].

      Pour obtenir des instructions, consultez la documentation [!DNL Anaplan] sur l’import de données dans des modules provenant d’un fichier.

   1. Notez le nom que vous avez donné au fichier. Il sera utilisé lors du déploiement du modèle de scénario [!UICONTROL Fusion].

  Exemple de contenu CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* Un fichier d’import des dépenses prévues **[!UICONTROL [!DNL Anaplan]]**, contenant les colonnes suivantes, dans cet ordre :

   1. GUID de dépenses [!UICONTROL [!DNL Workfront]]

   2. GUID du projet [!UICONTROL [!DNL Workfront]]

   3. [!UICONTROL Montant réel]

   4. [!UICONTROL Description]

   5. [!UICONTROL Type de dépenses]

   6. [!UICONTROL Date effective]

   7. [!UICONTROL Nom de la campagne]

   8. ID d’élément de liste [!UICONTROL [!DNL Anaplan]]

  Pour préparer le fichier d’import des dépenses planifiées [!UICONTROL [!DNL Anaplan]] :

   1. Copiez et collez le texte suivant dans un éditeur de texte ou [!DNL Excel].
   1. Enregistrez le fichier au format CSV.
   1. Chargez le fichier sur Anaplan.

      Pour plus d’informations, consultez la documentation d’[!DNL Anaplan] relative à l’import de données dans les modules à partir d’un fichier.

   1. Notez le nom que vous avez donné au fichier. Il sera utilisé lors du déploiement du modèle de scénario [!UICONTROL Fusion].

  Exemple de contenu CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* Un processus d’**[!UICONTROL import de mise à jour de projet]** préparé pour exécuter l’import des données livrées dans un chargement de fichier.

>[!NOTE]
>
>Il existe des fichiers d’import distincts pour les dépenses prévues et effectives, afin qu’elles puissent être rapportées de manière indépendante, aux dates prévues et effectives respectivement.

Pour obtenir des instructions sur l’une de ces actions, voir la documentation d’[!DNL Anaplan].

## Déploiement sur [!DNL Fusion]

Procédez comme suit pour déployer ce scénario d’intégration dans votre compte [!DNL Fusion]. Cette opération ne doit être effectuée qu’après avoir terminé les configurations [!DNL Workfront] et [!DNL Anaplan] requises.

1. Accédez au menu [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur le modèle de scénario **[!UICONTROL Envoyer les mises à jour des dépenses Workfront à un élément de liste [!DNL Anaplan]]**.
1. Remplacez les valeurs de variable pour les variables [!DNL Anaplan] suivantes :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Nom de la variable</th> 
      <th>Remplacer la valeur par</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>L’identifiant de l’espace de travail du compte [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model ID] </td> 
      <td>L’identifiant du modèle de votre compte [!DNL Anaplan] et l’espace de travail sélectionné que vous souhaitez utiliser pour ce scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Le nom de la liste de votre compte [!DNL Anaplan] et l’espace de travail et le modèle sélectionnés que vous souhaitez utiliser pour ce scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Actual Expense Import]</td> 
      <td> <p>Le nom du fichier qui recevra les données des dépenses effectives du projet.</p> <p> (Exemple : WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Planned Expense Import]</td> 
      <td> <p>Le nom du fichier qui recevra les données des dépenses prévues du projet.</p> <p> (Exemple : WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>Le nom du processus qui exécutera l’import des données des dépenses du projet.</p> <p>(Exemple : WF Int - Load Project Expenses)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Vous trouverez des informations détaillées sur la configuration des fichiers et des processus dans la documentation de configuration d’[!DNL Anaplan].

1. Sélectionnez ou ajoutez un profil de connexion [!DNL Anaplan].
1. Mettez à jour tous les modules [!DNL Anaplan] restants avec une connexion [!DNL Anaplan], lorsque l’on vous y invite.
1. Sélectionnez ou ajoutez un profil de connexion [!DNL Workfront].
1. Mettez à jour tous les modules [!DNL Workfront] restants avec une connexion [!DNL Workfront], lorsqu’un message vous y invite.
1. Sur le module **[!UICONTROL Créer un fichier CVS de dépenses réelles]**, ajoutez une nouvelle structure de données pour mapper les attributs de projet aux colonnes CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. Sur le module **[!UICONTROL Créer un fichier CSV de dépenses prévues]**, ajoutez une nouvelle structure de données pour mapper les attributs de projet aux colonnes CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Autres modèles de scénario recommandés

Ce modèle de scénario est complété par les modèles de scénario d’optimisation des dépenses suivants qui peuvent également être déployés :

* [[!UICONTROL Envoyer des mises à jour de projet  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer des mises à jour des heures effectives  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Scénarios supplémentaires pour lier les demandes de budget :

* [[!UICONTROL Créer un élément de liste  [!DNL Anaplan]  à partir d’une demande de budget  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Appliquer une allocation de budget  [!DNL Anaplan]  à un projet  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scénarios supplémentaires pour lier des demandes de campagne :

* [[!UICONTROL Créer un élément de liste  [!DNL Anaplan]  à partir d’une demande de campagne  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Appliquer une allocation de budget  [!DNL Anaplan]  à une demande ou un projet de campagne  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
