---
title: Afficher tous les rapports qui utilisent un champ ou un widget personnalisé spécifique
description: Vous pouvez ajouter une vue personnalisée dans la zone Forms personnalisée qui indique les rapports qui utilisent un champ ou un widget personnalisé spécifique. Cela s’avère utile lorsque vous devez modifier ou supprimer le champ ou le widget, car il peut déjà être implémenté dans un ou plusieurs rapports. Il est important d’évaluer si ces rapports devront être ajustés pour continuer à fonctionner correctement.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: c1bc2832d1c52885e737056172e7aec93a951e6c
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 9%

---

# Afficher tous les rapports qui utilisent un champ ou un widget personnalisé spécifique

Vous pouvez ajouter une vue personnalisée dans la zone Forms personnalisée qui indique les rapports qui utilisent un champ ou un widget personnalisé spécifique. Cela s’avère utile lorsque vous devez modifier ou supprimer le champ ou le widget, car il peut déjà être implémenté dans un ou plusieurs rapports. Il est important d’évaluer si ces rapports devront être ajustés pour continuer à fonctionner correctement.

Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Concevoir un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Forfait Adobe Workfront</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouvelle : standard</p>
   <p>ou</p>
   <p>Actuelle : formule</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Liste des rapports qui utilisent un champ ou un widget personnalisé spécifique

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Cliquez sur **Champs** pour afficher un rapport répertoriant tous les champs et widgets personnalisés de votre instance Workfront.

1. Cliquez sur le menu **Afficher** , puis recherchez les vues personnalisées de la liste qui incluent la colonne **Rapports** (qui n’est pas une colonne par défaut sur cet onglet).

   La colonne Rapports vous permet de voir les rapports qui utilisent chaque champ et widget personnalisés ajouté à un formulaire personnalisé de votre système. Il est possible qu’une personne ait déjà créé une vue qui inclut la colonne **Rapports**.

1. Si vous ne voyez pas de vue qui inclut la colonne **Reports**, créez une vue qui l’inclut :

   1. Cliquez sur le menu **Afficher**, puis sur **Nouvelle vue**.

   1. Sur la page **Nouvelle vue** qui s’affiche, dans la zone située dans le coin supérieur gauche, remplacez **Nouvelle vue de paramètre** par un nom descriptif pour la vue, tel que *Champs et widgets*.

   1. Cliquez sur **Ajouter la colonne** près du coin inférieur droit.
   1. Dans la zone **Afficher dans cette colonne** qui s’affiche près du coin supérieur gauche, commencez à saisir *report*, puis sélectionnez **Reports** lorsqu’il apparaît dans la liste sous la zone.

   1. (Conditionnel) Si vous souhaitez déplacer la colonne **Rapports** que vous venez d’ajouter à une autre position horizontale, faites glisser son en-tête dans la zone **Aperçu de la colonne** au bas de la page.

   1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.

1. Cliquez sur le menu déroulant **Afficher** , puis sélectionnez le nom de la vue personnalisée que vous venez de créer.
1. Dans la colonne **Nom**, recherchez le champ personnalisé ou le widget que vous prévoyez de modifier ou de supprimer, puis examinez la colonne **Rapports** sur cette ligne pour voir quels rapports l’utilisent, le cas échéant.

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
   > 1. Près du coin supérieur gauche, cliquez sur **Nouveau rapport**, puis sur **Paramètre** dans la liste qui s’affiche.
   > 1. Cliquez sur **Ajouter la colonne** près du coin inférieur droit.
   > 1. Dans la zone **Afficher dans cette colonne** qui s’affiche près du coin supérieur gauche, commencez à saisir *report*, puis sélectionnez **Reports** lorsqu’il apparaît dans la liste sous la zone.
   > 1. (Conditionnel) Si vous souhaitez déplacer la colonne **Rapports** que vous venez d’ajouter à une autre position horizontale, faites glisser son en-tête dans la zone **Aperçu de la colonne** au bas de la page.
   > 1. Cliquez sur **Terminé**, puis sur **Enregistrer+Fermer**.
   > 1. Saisissez un nom explicite pour le rapport, tel que *Champs et widgets*.
