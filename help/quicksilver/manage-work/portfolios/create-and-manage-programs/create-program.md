---
product-area: programs
navigation-topic: create and manage programs
title: Créer un programme
description: Un programme représente un ensemble de projets qui partagent une stratégie, un objectif ou un objectif commun qui transcende les limites du projet. Les programmes ne peuvent pas exister en dehors d'un portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 11%

---

# Créer un programme

<!-- Audited: 1/2024 -->

Un programme représente un ensemble de projets qui partagent une stratégie, un objectif ou un objectif commun qui transcende les limites du projet. Les programmes ne peuvent pas exister en dehors d&#39;un portfolio.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>

<td> <p>Nouveau : Tous</p><p>Ou</p><p>Actuel : [!UICONTROL Entreprise] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard] </p><p>Ou </p><p>Actuelle : [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès à [!UICONTROL Modifier] Portfolio et programmes </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations [!UICONTROL Gérer] pour le portfolio</p> <p>Une fois que vous avez créé un programme, vous disposez par défaut des autorisations [!UICONTROL Gérer].</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un programme

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche.

1. Effectuez l’une des opérations suivantes.

   * Créez un programme à partir de la zone [!UICONTROL Programmes] :

      1. Cliquez sur **[!UICONTROL Programmes]** dans le menu principal.
      1. Cliquez sur **[!UICONTROL Nouveau programme]**.
      1. Dans la zone qui s’affiche, saisissez le nom d’un Portfolio existant dans le champ **[!UICONTROL Select Portfolio]** .
      1. Saisissez le nom du nouveau programme dans le champ **[!UICONTROL Nom]** .
      1. Cliquer sur **[!UICONTROL Enregistrer]**.
   * Créez un programme à partir de la zone [!UICONTROL Portfolios] :

      1. Cliquez sur **[!UICONTROL Portfolios]** dans le [!UICONTROL menu principal], puis ouvrez un portfolio.
      1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Programmes]**.
      1. Cliquez sur le menu déroulant **[!UICONTROL Nouveau programme]** , puis sur **[!UICONTROL Nouveau programme]**.


1. (Conditionnel) Si vous avez créé le programme à partir d’un portfolio, indiquez le nom du programme dans le champ **[!UICONTROL Programme sans titre]**.

   Le nom peut contenir jusqu’à 255 caractères.

1. (Facultatif) Cliquez sur **[!UICONTROL Gestionnaire de programmes]** dans l’en-tête du programme pour le mettre à jour.

   >[!TIP]
   >
   >En tant que créateur du programme, vous êtes défini comme responsable du programme par défaut.

1. Cliquez sur **[!UICONTROL Détails du programme]** dans le panneau de gauche.
1. Double-cliquez sur un champ pour mettre à jour les informations dans la zone **[!UICONTROL Overview]**.

Vous pouvez indiquer les informations suivantes :

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>champ</th> 
      <th>Description</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td> <p>Spécifiez une description pour le programme.</p> <p>La description s'affiche sur la landing page du programme.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Program Manager]</td> 
      <td> <p>Commencez à saisir le nom de l’utilisateur que vous souhaitez utiliser comme responsable de programme, puis cliquez sur son nom lorsqu’il apparaît dans la liste déroulante. Il s’agit du même nom que le [!UICONTROL Propriétaire du programme]. </p> <p>Conseil : Vous pouvez également mettre à jour le Gestionnaire de programmes dans l’en-tête du programme. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Group] </td> 
      <td> <p>Ajoutez le nom d’un seul groupe si le groupe est responsable du programme ou s’il est responsable de l’exécuter. </p> <p>Vous pouvez vous assurer de sélectionner le groupe approprié en pointant dessus et en cliquant sur l’icône [!UICONTROL information] <img src="assets/info-icon.png"> qui s’affiche en regard. Cette option permet d’afficher une infobulle contenant des informations sur le groupe, telles que la hiérarchie des groupes qui le précèdent et ses administrateurs et administratrices.</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif et conditionnel) Cliquez dans la zone **[!UICONTROL Ajouter un formulaire personnalisé]** pour sélectionner un formulaire personnalisé pour le portfolio et mettre à jour les champs personnalisés.

   >[!TIP]
   >
   >Vous devez avoir des formulaires personnalisés de programme déjà créés avant de pouvoir les joindre à des programmes.

1. (Facultatif et conditionnel) Si vous ajoutez un formulaire personnalisé, cliquez sur un champ du formulaire personnalisé pour mettre à jour les informations dans ce champ.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
1. Cliquez sur **[!UICONTROL Projets]** dans le panneau de gauche, puis sur **[!UICONTROL Ajouter des projets]** pour ajouter des projets au programme.

   Pour plus d’informations sur l’ajout de projets à des programmes, voir [Ajout d’un projet à un programme](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
1. (Facultatif) Cliquez sur le **[!UICONTROL menu Plus]** ![](assets/more-icon.png) en regard du nom du programme et cliquez sur **[!UICONTROL Désactiver le programme]**.

   Lorsque vous désactivez un programme, celui-ci ne s’affiche plus dans la liste des programmes lorsque les utilisateurs tentent de l’ajouter à un projet. Vous pouvez toujours accéder au programme à partir de la zone [!UICONTROL Programmes].

## Aperçu de l’en-tête du programme

Vous trouverez des informations sur le programme dans son en-tête.

Les informations suivantes s’affichent dans l’en-tête d’un programme :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Informations sur l’en-tête</td> 
   <td> <strong>Notes</strong> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Chemin de navigation avec le nom du portfolio</td> 
   <td>Vous pouvez accéder au portfolio auquel le programme appartient à partir de l’en-tête du programme. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nom du programme</td> 
   <td>Vous pouvez modifier le nom du programme dans l’en-tête .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nom du type d’objet et état d’activation</td> 
   <td>Le mot "Programme" s’affiche avec une icône orange lorsque vous affichez un programme. Le mot "[!UICONTROL Désactivé]" s’affiche en regard de celui-ci et la composition est grise si le programme n’est pas marqué comme [!UICONTROL actif]. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">La zone d’actions du programme </td> 
   <td> <p>Cliquez sur l’une des options suivantes pour accéder à d’autres informations ou options de modification du programme :</p> 
    <ul> 
     <li>L’icône en forme d’étoile pour ajouter le programme à votre liste de Favoris</li> 
     <li> <p>Le menu [!UICONTROL Plus] <img src="assets/qs-more-menu.png"> pour effectuer l’une des opérations suivantes : </p> 
      <ul> 
       <li>Modifier le programme</li> 
       <li>Désactivez-le. Lorsqu’un programme est désactivé, vous ne pouvez plus l’associer aux projets au niveau du projet. </li> 
       <li> <p>Supprimez-le. La suppression du programme ne supprime pas les projets du programme. Il supprime l’association des projets au programme. </p> </li> 
       <li>Partager avec d’autres</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pourcentage terminé]</td> 
   <td> <p>Vous ne pouvez pas modifier le [!UICONTROL Pourcentage terminé] du programme dans l’en-tête . Ces informations sont mises à jour à partir des projets du programme. Par défaut, le pourcentage de fin du programme correspond à la moyenne des valeurs de pourcentage de fin des projets dans un état [!UICONTROL Actuel] ou [!UICONTROL Approuvé] appartenant au programme.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Manager]</td> 
   <td> <p>Vous pouvez modifier le Gestionnaire de programmes dans l’en-tête . Il s’agit du même nom que le [!UICONTROL Propriétaire du programme]. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date d’achèvement prévue]</td> 
   <td>Vous ne pouvez pas modifier la date de fin planifiée du programme dans l’en-tête. Ces informations sont mises à jour à partir des projets du programme. La date d’achèvement prévue du dernier projet du programme devient la date d’achèvement prévu du programme.  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Condition des projets actifs]</td> 
   <td>Il s’agit d’un calcul du pourcentage de projets pour lesquels la [!UICONTROL Condition] est définie sur [!UICONTROL Sur Target], [!UICONTROL À risque] ou [!UICONTROL À risque]. Les projets représentés ici sont des projets dont le statut est [!UICONTROL Actuel] et [!UICONTROL Approuvé]. </td> 
  </tr> 
 </tbody> 
</table>

## Déplacer un programme

Vous pouvez ajouter des programmes existants à un portfolio. Comme les programmes ne peuvent pas exister dans deux portefeuilles différents, l’ajout d’un programme existant le déplace définitivement d’un portefeuille à un autre.

Pour plus d’informations, voir [Ajout d’un programme existant à un portfolio](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
