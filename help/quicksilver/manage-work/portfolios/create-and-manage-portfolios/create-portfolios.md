---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Créer un portfolio
description: Un portfolio est un ensemble de projets qui se partagent les mêmes ressources, le même budget et le même planning. Les projets d’un portfolio sont suffisamment similaires pour utiliser le même groupe de ressources et être mesurés par rapport à la même carte de performance.
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 80%

---

# Créer un portfolio

<!--Audited: 7/2024-->

Un portfolio est un ensemble de projets qui se partagent les mêmes ressources, le même budget et le même planning. Les projets d’un portfolio sont suffisamment similaires pour utiliser le même groupe de ressources et être mesurés par rapport à la même carte de performance.

Vous pouvez utiliser des portfolios pour regrouper des projets qui appartiennent aux mêmes lignes de produits, divisions, services, entreprises ou autres unités opérationnelles.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p>
   <p>Actuelle : [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>[!UICONTROL Edit] l’accès aux portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Après avoir créé un portfolio, vous disposez par défaut des autorisations de gestion qui lui sont associées.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création de portefeuilles

Vous pouvez créer un portefeuille dans Workfront à l’aide de l’une des méthodes suivantes :

* Créez un portfolio à partir de zéro en commençant dans la zone Portfolios du menu principal. Cet article décrit comment créer un portfolio à partir de zéro.

* Importez un portefeuille à l’aide de Kickstarts.

  En tant qu’administrateur Workfront, vous pouvez importer des portefeuilles à l’aide d’un lancement.

  Pour plus d’informations sur l’import de données à l’aide de Kickstarts dans Workfront, consulter la section [Importer des données dans Adobe Workfront à l’aide d’un modèle de Kickstart](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

* Ajoutez des portfolios au fur et à mesure que vous les connectez à partir d’un type d’enregistrement dans Workfront Planning.

  Vous devez disposer d’une nouvelle licence Workfront et d’une licence Workfront Planning supplémentaire pour Workfront Planning.

  Pour plus d’informations sur l’accès à Workfront Planning, voir [Présentation de l’accès](/help/quicksilver/planning/access/access-overview.md).

  Pour plus d&#39;informations sur la création de portefeuilles en les ajoutant à des enregistrements, reportez-vous à la section « Créer des enregistrements au fur et à mesure que vous les connectez » de l&#39;article [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).


## Créer un portfolio

{{step1-click-main-menu}}

1. Cliquez sur **[!UICONTROL Portfolios]**.
1. Cliquez sur **[!UICONTROL Nouveau portfolio]**.
1. Remplacez **[!UICONTROL Portfolio sans titre]** par le nom que vous souhaitez donner au portfolio.

   Le nom peut contenir jusqu’à 255 caractères.

1. (Facultatif) Cliquez sur le nom sous **[!UICONTROL Personne gestionnaire de portfolio]** dans l’en-tête situé en haut de la page afin d’attribuer une autre personne responsable au portfolio.

   ![nom du gestionnaire Portfolio](assets/portfolio-manager-name-350x51.jpg)

   En tant que créateur ou créatrice du portfolio, vous êtes gestionnaire de portfolio par défaut.

1. Cliquez sur **[!UICONTROL Détails du portfolio]** dans le panneau de gauche.
1. Dans la zone **[!UICONTROL Vue d’ensemble]**, modifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td> <p>Saisissez une description du portfolio afin d’indiquer ce qui le distingue des autres. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
      <td> <p>Commencez à saisir le nom d’un utilisateur ou d’une utilisatrice que vous souhaitez indiquer en tant que personne gestionnaire de portfolio, puis sélectionnez-le lorsqu’il apparaît dans la liste. Il s’agit du même nom que la [!UICONTROL Portfolio Owner]. Il s’agit de la personne qui peut superviser le travail défini dans les projets du portfolio et approuver le business case.</p> <p>Important : lorsque vous désignez une personne comme [!UICONTROL Portfolio Manager], elle obtient automatiquement les autorisations [!UICONTROL Manage] du portfolio, des programmes et des projets du portfolio. </p> <p>Conseil : vous pouvez également mettre à jour la [!UICONTROL Portfolio Manager] dans l’en-tête en haut de la page.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Groupe </td> 
      <td> <p>Ajoutez le nom d’un groupe unique si le groupe détient le portfolio ou a la responsabilité de le terminer. </p> <p>Vous pouvez vous assurer que vous sélectionnez le groupe approprié en le survolant et en cliquant sur l’icône [!UICONTROL information] <img src="assets/info-icon.png"> qui s’affiche en regard de celui-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus et son équipe d’administration.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Cliquez dans la boîte de dialogue **[!UICONTROL Ajouter un formulaire personnalisé]** dans le coin supérieur droit de la page [!UICONTROL Détails du portfolio] pour sélectionner un formulaire personnalisé pour le portfolio et mettre à jour les champs personnalisés.

   >[!TIP]
   >
   >Vous devez avoir déjà créé des formulaires personnalisés de portfolio avant de pouvoir les joindre à des portfolios.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
1. (Facultatif) Cliquez sur **[!UICONTROL Programmes]** dans le panneau de gauche, puis **[!UICONTROL Ajouter des programmes]** pour ajouter des programmes au portfolio.

   Pour plus d’informations sur la création de programmes, consultez la section [Créer un programme](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. (Facultatif) Cliquez sur **[!UICONTROL Projets]** dans le panneau de gauche, puis **[!UICONTROL Ajouter des projets]** pour ajouter des projets au portfolio.

   Pour plus d’informations sur l’ajout de projets à un portfolio, consultez la section [Ajouter des projets à un portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Deactivate a portfolio</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this and moved it to their own article: delete-deactivate-portfolios)</p>
<p>When you deactivate a portfolio, you can still access it from the Portfolios area, but it no longer displays in the list of portfolios when users try to add it to a project.</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2">Click <strong>Portfolios</strong> .</li>
<li value="3"> <p>Click the name of the portfolio.</p> </li>
<li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon.png"> to the right of the portfolio name, then click <strong>Deactivate Portfolio</strong>.</li>
</ol>
<h2>Delete a portfolio</h2>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> <p>Click <strong>Portfolios</strong> .</p> </li>
<li value="3"> <p>Select the portfolio, then click the Delete icon <img src="assets/delete.png">.</p> </li>
<li value="4"> <p>In the box that appears, click <strong>Yes, Delete It</strong> to confirm.</p> </li>
</ol>
</div>
-->
