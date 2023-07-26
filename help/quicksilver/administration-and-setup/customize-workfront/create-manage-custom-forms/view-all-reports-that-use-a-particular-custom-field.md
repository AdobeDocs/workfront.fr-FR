---
title: Afficher tous les rapports qui utilisent un champ ou un widget personnalisé spécifique
description: Vous pouvez ajouter une vue personnalisée dans la zone Forms personnalisée qui indique les rapports qui utilisent un champ ou un widget personnalisé spécifique. Cela s’avère utile lorsque vous devez modifier ou supprimer le champ ou le widget, car il peut déjà être implémenté dans un ou plusieurs rapports. Il est important d’évaluer si ces rapports devront être ajustés pour continuer à fonctionner correctement.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Afficher tous les rapports qui utilisent un champ ou un widget personnalisé spécifique

Vous pouvez ajouter une vue personnalisée dans la zone Forms personnalisée qui indique les rapports qui utilisent un champ ou un widget personnalisé spécifique. Cela s’avère utile lorsque vous devez modifier ou supprimer le champ ou le widget, car il peut déjà être implémenté dans un ou plusieurs rapports. Il est important d’évaluer si ces rapports devront être ajustés pour continuer à fonctionner correctement.

Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Ajouter un champ personnalisé à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) et [Ajout ou modification d’un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Pour plus d’informations sur la manière dont les administrateurs de Workfront accordent cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur Workfront.

## Liste des rapports qui utilisent un champ ou un widget personnalisé spécifique

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Forms personnalisée**.
1. Ouvrez le **Champs** pour afficher un rapport répertoriant tous les champs et widgets personnalisés de votre instance Workfront.

   ![](assets/fields-tab.png)

1. Cliquez sur le bouton **Affichage** dans le menu déroulant de l’en-tête en haut de la liste, puis recherchez les vues personnalisées de la liste qui incluent la variable **Rapports** (qui n’est pas une colonne par défaut sur cet onglet).

   La colonne Rapports vous permet de voir les rapports qui utilisent chaque champ et widget personnalisés ajouté à un formulaire personnalisé de votre système. Il est possible qu’une personne ait déjà créé une vue qui inclut la variable **Rapports** colonne .

1. Si vous ne voyez pas d’affichage qui inclut la variable **Rapports** , créez une vue qui l’inclut :

   1. Cliquez sur le bouton **Affichage** , puis cliquez sur **Nouvelle vue**.

   1. Sur le **Nouvelle vue** dans la zone située dans le coin supérieur gauche, remplacez **Nouvelle vue des paramètres** avec un nom descriptif pour la vue, tel que *Champs et widgets*.

   1. Cliquez sur **Ajouter une colonne** près du coin inférieur droit.
   1. Dans le **Afficher dans cette colonne** qui s’affiche près du coin supérieur gauche, commencez à saisir du texte *rapport*, puis sélectionnez **Rapports** lorsqu’il apparaît dans la liste sous la zone.

   1. (Conditionnel) Si vous souhaitez déplacer la variable **Rapports** que vous venez d’ajouter à une autre position horizontale, faites glisser son en-tête dans la **Aperçu des colonnes** au bas de la page.

   1. Cliquez sur **Terminé**, puis cliquez sur **Enregistrer la vue**.

1. Cliquez sur le bouton **Affichage** , puis sélectionnez le nom de la vue personnalisée que vous venez de créer.
1. Dans le **Nom** , recherchez le champ personnalisé ou le widget que vous prévoyez de modifier ou de supprimer, puis examinez le **Rapports** sur cette ligne pour identifier les rapports qui l’utilisent, le cas échéant.

   Pour trouver les informations de cette colonne, Workfront recherche les champs personnalisés et les widgets dans tous les filtres de rapport, vues et regroupements.

   Si un signe plus s’affiche, vous pouvez cliquer sur cette ligne de texte pour afficher une zone répertoriant tous les rapports supplémentaires qui utilisent le champ ou le widget.

   >[!NOTE]
   >
   >Le temps de chargement initial de cet outil peut prendre de 10 secondes à 2,5 minutes, selon la quantité de données de votre système.

   >[!TIP]
   >
   >Si vous n’avez pas le temps d’examiner les rapports qui utilisent le champ ou le widget personnalisé, vous pouvez cliquer sur Exporter pour créer un fichier qui les répertorie. Vous pouvez partager ce fichier avec toute personne propriétaire d’un rapport qui utilise le champ ou le widget et discuter des changements qui doivent se produire, de l’impact que cela peut avoir sur le rapport et des mesures à prendre pour s’assurer que le rapport continue à fonctionner correctement.
   >
   >Cette vue est également disponible dans un rapport Paramètre :
   >      
   > 1. Dans le menu principal, cliquez sur **Rapports**.
   > 1. Dans le coin supérieur gauche, cliquez sur **Nouveau rapport**, puis cliquez sur **Paramètre** dans la liste qui s’affiche.
   > 1. Cliquez sur **Ajouter une colonne** près du coin inférieur droit.
   > 1. Dans le **Afficher dans cette colonne** qui s’affiche près du coin supérieur gauche, commencez à saisir du texte *rapport*, puis sélectionnez **Rapports** lorsqu’il apparaît dans la liste sous la zone.
   > 1. (Conditionnel) Si vous souhaitez déplacer la variable **Rapports** que vous venez d’ajouter à une autre position horizontale, faites glisser son en-tête dans la **Aperçu des colonnes** au bas de la page.
   > 1. Cliquez sur **Terminé**, puis cliquez sur **Enregistrer + Fermer**.
   > 1. Saisissez un nom explicite pour le rapport, tel que *Champs et widgets*.
