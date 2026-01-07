---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Envoyer des mises à jour de projet  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] '
description: Ce scénario d’intégration partage la progression, le statut et les détails clés du calendrier d’un projet  [!DNL Adobe Workfront]  avec un élément de liste budgétaire  [!DNL Anaplan] . Le partage de ces informations vous permet de tirer le meilleur parti de l’optimisation des dépenses et de l’analyse financière que fournit  [!DNL Anaplan] .
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 98%

---

# Envoyer les mises à jour de projet [!DNL Adobe Workfront] à un élément de liste [!DNL Anaplan]

Ce scénario d’intégration partage la progression, le statut et les détails clés du calendrier d’un projet [!DNL Adobe Workfront] avec un élément de liste budgétaire [!DNL Anaplan]. Le partage de ces informations vous permet de tirer le meilleur parti de l’optimisation des dépenses et de l’analyse financière que fournit [!DNL Anaplan].

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

* Profil d’utilisateur ou d’utilisatrice dans [!DNL Workfront] nommé Intégration **[!UICONTROL [!DNL Anaplan]]**, disposant de droits d’administration système.

  Pour plus d’informations sur la création d’un utilisateur ou d’une utilisatrice dans [!DNL Workfront], voir [Ajouter des utilisateurs et des utilisatrices](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Formulaire personnalisé **[!UICONTROL Résumé de campagne]** joint à l’objet de projet pour stocker des valeurs de données personnalisées que vous choisissez d’envoyer à Anaplan.

  Les champs suivants sont des exemples de champs qui peuvent être inclus dans le formulaire personnalisé pour faciliter le mappage de données avec Anaplan, mais ils ne sont pas nécessaires pour ce scénario d’intégration :

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Nom du champ</th> 
     <th>Type de champ</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market Start Date]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>[!UICONTROL Paragraph Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Paragraph Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Inclut des options qui correspondent à vos processus.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Configuration [!DNL Anaplan] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Anaplan] :

* Profil d’utilisateur ou d’utilisatrice dans [!DNL Anaplan] nommé Intégration **[!UICONTROL [!DNL Workfront]]**, disposant de droits d’administration système.
* Modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* Liste du modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* Fichier **[!UICONTROL Import de mise à jour de projet]** contenant les colonnes suivantes, dans cet ordre :

1. [!UICONTROL itemID]

2. GUID du projet [!UICONTROL [!DNL Workfront]]

3. [!UICONTROL Nom de la campagne]

4. [!UICONTROL Pourcentage d&#39;achèvement]

5. [!UICONTROL Date de début prévue]

6. [!UICONTROL Date d’achèvement prévue]

7. [!UICONTROL Nombre d’heures prévues]

8. [!UICONTROL Coûts prévus]

9. [!UICONTROL Montant des dépenses prévues]

10. [!UICONTROL Coût réel de main-d’œuvre]

11. [!UICONTROL Coût prévu de main-d’œuvre]

12. [!UICONTROL Statut]

Pour préparer le fichier Import des dépenses prévues [!UICONTROL [!DNL Anaplan]], procédez comme suit :

1. Copiez et collez le texte suivant dans un éditeur de texte ou [!DNL Excel].
1. Enregistrez le fichier au format CSV.
1. Chargez le fichier sur Anaplan.

   Pour plus d’informations, consultez la documentation d’[!DNL Anaplan] relative à l’import de données dans les modules à partir d’un fichier.

1. Notez le nom que vous avez donné au fichier. Il sera utilisé lors du déploiement du modèle de scénario [!UICONTROL Fusion].

Exemple de contenu CSV

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>Les colonnes facultatives peuvent inclure les éléments suivants :

1. [!UICONTROL Vue d’ensemble de la campagne]

2. [!UICONTROL Message clé]

3. [!UICONTROL Date de début du marché]

4. [!UICONTROL Date de fin du marché]

5. [!UICONTROL Audience cible]

Incluez également tous les autres champs que vous souhaitez définir dans le mappage.

* Processus d’**[!UICONTROL import de mise à jour du projet]** préparé pour exécuter l’import de données fournies dans un fichier chargé.

Pour obtenir des instructions sur les actions décrites, consultez la documentation d’[!DNL Anaplan].

## Déployer vers [!DNL Workfront Fusion]

Pour déployer ce scénario d’intégration dans votre compte Fusion, procédez comme suit. Avant de commencer, assurez-vous d’avoir effectué la configuration requise de [!DNL Workfront] et d’[!DNL Anaplan].

1. Naviguez vers le menu [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur le modèle de scénario **[!UICONTROL Envoyer des mises à jour de projets Workfront à l’élément de liste [!DNL Anaplan]]**.
1. Remplacez les valeurs des variables [!DNL Anaplan] suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Nom de la variable</th> 
      <th>Remplacer la valeur par</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>ID d’un espace de travail de votre compte [!DNL Anaplan].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model ID] </td> 
      <td>ID d’un modèle de votre compte [!DNL Anaplan] et de l’espace de travail sélectionné.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Le nom de la liste de votre compte [!DNL Anaplan] et de l’espace de travail et du modèle sélectionnés.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Project Update Import]</td> 
      <td>Nom du fichier recevant les données de mise à jour du projet.<p>(Exemple : WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>Nom du processus exécutant l’import des données du projet.</p> <p>(Exemple : WF Int - Mettre à jour les détails de la campagne)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomain]</td> 
      <td>Sous-domaine de votre compte [!DNL Workfront]. Il permet de créer un lien vers votre projet [!DNL Workfront] dans une note qui peut être générée.</td> 
     </tr> 
    </tbody> 
   </table>

   Les détails de la configuration des fichiers et des processus sont fournis dans la documentation de configuration d’[!DNL Anaplan].

1. Sélectionnez ou ajoutez un profil de connexion [!DNL Anaplan].
1. Mettez à jour tous les modules [!DNL Anaplan] restants avec une connexion [!DNL Anaplan], lorsque l’on vous y invite.
1. Sélectionnez ou ajoutez un profil de connexion [!DNL Workfront].

   Le filtre est configuré pour extraire tous les projets liés incomplets et ceux qui ont été terminés au cours des 29 dernières minutes. Si vous modifiez la fréquence du scénario [!DNL Fusion], vous devrez mettre à jour cette valeur une fois que le modèle de scénario aura été déployé.

1. Dans le module **[!UICONTROL Créer un CSV de mise à jour de projets]**, ajoutez une nouvelle structure de données pour mapper les attributs du projet aux colonnes CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. Mettez à jour tous les modules [!DNL Workfront] restants avec une connexion [!DNL Workfront], lorsque l’on vous invite à le faire.

## Autres modèles de scénario recommandés

Ce modèle de scénario est complété par les modèles de scénario d’optimisation des dépenses suivants qui peuvent également être déployés :

* [[!UICONTROL Envoyer les mises à jour des heures effectives  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] ]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer les dépenses  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] ]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Scénarios supplémentaires pour lier les demandes de budget :

* [[!UICONTROL Créer un élément de liste  [!DNL Anaplan]  à partir d’une demande de budget  [!DNL Adobe Workfront] ]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Appliquer une allocation de budget  [!DNL Anaplan]  à un projet  [!DNL Adobe Workfront] ]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scénarios supplémentaires pour lier des demandes de campagne :

* [[!UICONTROL Créer un élément de liste  [!DNL Anaplan]  à partir d’une demande de campagne  [!DNL Adobe Workfront] ]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Appliquer une allocation de budget  [!DNL Anaplan]  à une demande ou un projet de campagne  [!DNL Adobe Workfront] ]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
