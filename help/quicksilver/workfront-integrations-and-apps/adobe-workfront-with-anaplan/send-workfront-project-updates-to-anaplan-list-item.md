---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Envoyer les mises à jour du projet  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan]
description: Ce scénario d’intégration partage la progression, l’état et les détails de planification clés d’un projet  [!DNL Adobe Workfront] avec un élément de liste de budgets  [!DNL Anaplan] . Le partage de ces informations vous permet de mieux tirer parti de l’optimisation des dépenses et de l’analyse financière fournie par [!DNL Anaplan] .
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 6%

---

# Envoyer des mises à jour de projet [!DNL Adobe Workfront] à un élément de liste [!DNL Anaplan]

Ce scénario d’intégration partage la progression, l’état et les détails de planification clés d’un projet [!DNL Adobe Workfront] avec un élément de liste budgétaire [!DNL Anaplan]. Le partage de ces informations vous permet de mieux tirer parti de l’optimisation des dépenses et de l’analyse financière fournie par [!DNL Anaplan].

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

* Un profil utilisateur dans [!DNL Workfront] nommé **[!UICONTROL [!DNL Anaplan]Integration]**, disposant des droits d’administrateur système.

  Pour plus d&#39;informations sur la création d&#39;un utilisateur dans [!DNL Workfront], voir [Ajout d&#39;utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Un formulaire personnalisé **[!UICONTROL résumé de campagne]** joint à l’objet de projet pour stocker les valeurs de données personnalisées que vous choisissez d’envoyer à Anaplan.

  Les champs suivants représentent des exemples de champs qui peuvent être inclus dans le formulaire personnalisé pour faciliter le mappage des données vers Anaplan, mais ils ne sont pas nécessaires pour ce scénario d’intégration :

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Nom de champ</th> 
     <th>Type de champ</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL À La Date De Début Du Marché]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL À La Date De Fin Du Marché]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Présentation de Campaign]</td> 
     <td>[!UICONTROL Champ de texte de paragraphe]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Message de clé]</td> 
     <td>[!UICONTROL Champ de texte de paragraphe]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Audience Target]</td> 
     <td> <p>[!UICONTROL Liste déroulante]</p> <p>Incluez des options qui correspondent à vos processus.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer ou modifier un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Configuration [!DNL Anaplan] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Anaplan] :

* Un profil utilisateur dans [!DNL Anaplan] nommé **[!UICONTROL [!DNL Workfront]Integration]**, disposant des droits d’administrateur système.
* Le modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* Liste du modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* Un fichier **[!UICONTROL Project Update Import]** contenant les colonnes suivantes, dans cet ordre :

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] GUID de projet ]

3. [!UICONTROL Nom de la campagne]

4. [!UICONTROL Pourcentage d&#39;achèvement]

5. [!UICONTROL Date de début planifiée]

6. [!UICONTROL Date d’achèvement prévue]

7. [!UICONTROL Nombre d’heures prévues]

8. [!UICONTROL Coûts prévus]

9. [!UICONTROL Coût des dépenses planifiées]

10. [!UICONTROL Coût réel de la main-d’oeuvre]

11. [!UICONTROL Coût de main-d’oeuvre planifié]

12. [!UICONTROL Statut]

Pour préparer le fichier [!UICONTROL [!DNL Anaplan] d’importation des dépenses prévues ] :

1. Copiez et collez les éléments suivants dans un éditeur de texte ou [!DNL Excel]
1. Enregistrement du fichier au format CSV
1. Téléchargez le fichier dans Anaplan.

   Pour plus d’informations, consultez la documentation [!DNL Anaplan] sur l’importation de données dans des modules à partir d’un fichier.

1. Notez le nom que vous avez donné au fichier ; il sera utilisé lors du déploiement du modèle de scénario [!UICONTROL Fusion].

Exemple de contenu CSV

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>Les colonnes facultatives peuvent inclure :

1. [!UICONTROL Présentation de campagne]

2. [!UICONTROL Message clé]

3. [!UICONTROL Date de début du marché]

4. [!UICONTROL Date de fin du marché]

5. [!UICONTROL Public cible]

Incluez également tous les autres champs que vous souhaitez définir dans le mappage.

* Un processus **[!UICONTROL Project Update Import]** préparé pour exécuter l’importation de données livrées dans un téléchargement de fichier.

Pour obtenir des instructions sur l’une de ces actions, consultez la documentation [!DNL Anaplan].

## Déploiement sur [!DNL Workfront Fusion]

Effectuez les étapes suivantes pour déployer ce scénario d’intégration sur votre compte Fusion. Cette opération ne doit être effectuée qu’après avoir terminé la configuration [!DNL Workfront] et [!DNL Anaplan] requise.

1. Accédez au menu [!UICONTROL  Modèles] dans [!DNL Workfront Fusion] et cliquez sur le modèle de scénario **[!UICONTROL Envoyer les mises à jour du projet Workfront à [!DNL Anaplan] élément de liste]** .
1. Remplacez les valeurs de variable pour les variables [!DNL Anaplan] suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Nom de variable</th> 
      <th>Remplacer la valeur par</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>L’identifiant d’un espace de travail de votre compte [!DNL Anaplan].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID de modèle] </td> 
      <td>L’identifiant d’un modèle de votre compte [!DNL Anaplan] et l’espace de travail sélectionné.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Nom de la liste de votre compte [!DNL Anaplan] et de l’espace de travail et du modèle sélectionnés.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nom de fichier : Importation de mise à jour de projet]</td> 
      <td>Nom du fichier qui recevra les données de mise à jour du projet.<p>(Exemple : WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nom du processus : Importation de mise à jour de projet]</td> 
      <td> <p>Nom du processus qui exécutera l’importation des données du projet.</p> <p>(Exemple : WF Int - Mise à jour des détails d’une campagne)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomain]</td> 
      <td>Le sous-domaine de votre compte [!DNL Workfront]. Il est utilisé pour créer un lien vers votre projet [!DNL Workfront] dans une note qui peut être générée.</td> 
     </tr> 
    </tbody> 
   </table>

   Vous trouverez des détails sur la configuration des fichiers et des processus dans la documentation de configuration de [!DNL Anaplan].

1. Sélectionnez ou ajoutez un profil de connexion [!DNL Anaplan].
1. Mettez à jour tous les modules [!DNL Anaplan] restants avec une connexion [!DNL Anaplan] lorsque vous y êtes invité.
1. Sélectionnez ou ajoutez un profil de connexion [!DNL Workfront].

   Le filtre est configuré pour extraire tous les projets liés incomplets et ceux qui ont été terminés au cours des 29 dernières minutes. Si vous modifiez la fréquence du scénario [!DNL Fusion], vous souhaiterez mettre à jour cette valeur une fois le modèle de scénario déployé.

1. Sur le module **[!UICONTROL Build Projects Update CSV]** , ajoutez une nouvelle structure de données pour mapper les attributs de projet aux colonnes CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. Mettez à jour tous les modules [!DNL Workfront] restants avec une connexion [!DNL Workfront] lorsque vous y êtes invité.

## Autres modèles de scénario recommandés

Ce modèle de scénario est complété par les modèles de scénario d’optimisation des dépenses suivants qui peuvent également être déployés :

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] des mises à jour en heures réelles à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyez [!DNL Adobe Workfront] des dépenses à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Scénarios supplémentaires pour lier les requêtes de budget :

* [[!UICONTROL  Créez un  [!DNL Anaplan] élément de liste à partir d&#39;une  [!DNL Adobe Workfront] requête de budget]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL  Appliquez une  [!DNL Anaplan] allocation budgétaire à un [!DNL Adobe Workfront] projet]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scénarios supplémentaires pour lier des requêtes de campagne :

* [[!UICONTROL  Créez un  [!DNL Anaplan] élément de liste à partir d’une  [!DNL Adobe Workfront] requête de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL  Appliquez une  [!DNL Anaplan]  allocation budgétaire à une  [!DNL Adobe Workfront] requête de campagne ou projet de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
