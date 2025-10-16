---
title: Afficher tous les rapports qui utilisent un champ personnalisé ou un widget particulier
description: Vous pouvez ajouter une vue personnalisée dans la zone des formulaires personnalisés qui montre quels rapports utilisent un champ personnalisé ou un widget particulier. Cette opération est utile lorsque vous devez modifier ou supprimer le champ ou le widget, car il peut déjà être implémenté dans un ou plusieurs rapports. Il est important d’évaluer si ces rapports doivent être modifiés pour continuer à fonctionner correctement.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 96%

---

# Afficher tous les rapports qui utilisent un champ personnalisé ou un widget particulier

Vous pouvez ajouter une vue personnalisée dans la zone des formulaires personnalisés qui montre quels rapports utilisent un champ personnalisé ou un widget particulier. Cette opération est utile lorsque vous devez modifier ou supprimer le champ ou le widget, car il peut déjà être implémenté dans un ou plusieurs rapports. Il est important d’évaluer si ces rapports doivent être modifiés pour continuer à fonctionner correctement.

Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Répertorier les rapports qui utilisent un champ personnalisé ou un widget particulier

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Cliquez sur **Champs** pour afficher un rapport répertoriant tous les champs personnalisés et les widgets de votre instance Workfront.

1. Cliquez sur le menu **Vue**, puis recherchez dans la liste les vues personnalisées qui incluent la colonne **Rapports** (qui n’est pas une colonne par défaut dans cet onglet).

   La colonne des rapports vous permet de voir quels rapports utilisent chaque champ personnalisé et chaque widget ajoutés à un formulaire personnalisé dans votre système. Une autre personne peut avoir déjà créé une vue qui inclut la colonne **Rapports**.

1. Si vous ne voyez pas une vue qui inclut la colonne **Rapports**, créez une vue qui l’inclut :

   1. Cliquez sur le menu **Vue**, puis sur **Nouvelle vue**.

   1. Sur la page **Nouvelle vue** qui s’affiche, remplacez **Nouveau paramètre de vue** par un nom descriptif de la vue, tel que *Champs et widgets*.

   1. Cliquez sur **Ajouter une colonne** dans le coin inférieur droit.
   1. Dans la zone **Afficher dans cette colonne** qui s’affiche dans le coin supérieur gauche, commencez à saisir *rapport*, puis sélectionnez **Rapports** lorsqu’il apparaît dans la liste.

   1. (Le cas échéant) Si vous souhaitez déplacer la colonne **Rapports** que vous venez d’ajouter vers une autre position horizontale, faites glisser son en-tête dans la zone de **prévisualisation de la colonne** au bas de la page.

   1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.

1. Cliquez sur le menu déroulant **Vue**, puis sélectionnez le nom de la vue personnalisée que vous venez de créer.
1. Dans la colonne **Nom**, recherchez le champ personnalisé ou le widget que vous souhaitez modifier ou supprimer, puis consultez la colonne **Rapports** de cette ligne pour voir quels rapports l’utilisent, le cas échéant.

   Pour trouver les informations de cette colonne, Workfront recherche les champs personnalisés et les widgets dans tous les filtres, vues et regroupements de rapports.

   Si vous voyez un signe plus, vous pouvez cliquer sur cette ligne de texte pour afficher une zone listant tous les rapports supplémentaires qui utilisent le champ ou le widget.

   >[!NOTE]
   >
   >Le temps de chargement initial de cet outil peut durer de 10 secondes à 2,5 minutes, en fonction de la quantité de données contenues dans votre système.

   >[!TIP]
   >
   >Si vous n’avez pas le temps d’étudier les rapports qui utilisent le champ personnalisé ou le widget, vous pouvez cliquer sur « Exporter » pour créer un fichier qui les répertorie. Vous pouvez partager ce fichier avec toute personne propriétaire d’un rapport utilisant le champ ou le widget et discuter de la modification à apporter, de l’impact qu’elle pourrait avoir sur le rapport et de ce qu’il faut faire pour s’assurer que le rapport continue à fonctionner correctement.
   >
   >Cette vue est également disponible dans un rapport de paramètres :
   >      
   > 1. Dans le menu principal, cliquez sur **Rapports**.
   > 1. Dans le coin supérieur gauche, cliquez sur **Nouveau rapport**, puis sur **Paramètres** dans la liste qui s’affiche.
   > 1. Cliquez sur **Ajouter une colonne** dans le coin inférieur droit.
   > 1. Dans la zone **Afficher dans cette colonne** qui s’affiche dans le coin supérieur gauche, commencez à saisir *rapport*, puis sélectionnez **Rapports** lorsqu’il apparaît dans la liste.
   > 1. (Le cas échéant) Si vous souhaitez déplacer la colonne **Rapports** que vous venez d’ajouter vers une autre position horizontale, faites glisser son en-tête dans la zone de **prévisualisation de la colonne** au bas de la page.
   > 1. Cliquez sur **Terminé**, puis sur **Enregistrer et fermer**.
   > 1. Saisissez un nom descriptif pour le rapport, tel que *Champs et widgets*.
