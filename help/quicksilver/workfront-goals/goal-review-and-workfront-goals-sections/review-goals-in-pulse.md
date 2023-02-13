---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Révision des objectifs dans la section Pulse des objectifs d’Adobe Workfront
description: Vous pouvez afficher tous les objectifs de votre entreprise, quel que soit le propriétaire. Pour plus d’informations sur la création d’objectifs, voir Création d’objectifs dans les objectifs Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 33873797-183d-4efc-9099-26eb907ca799
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 1%

---

# Révision des objectifs dans la section Pulse des objectifs d’Adobe Workfront

>[!IMPORTANT]
> 
>Les fonctionnalités décrites dans cet article ont été supprimées de Workfront, à compter de la version 23.1.\
>Cet article sera également supprimé peu de temps après la version 23.1, début 2023. Pour l’instant, nous vous recommandons de mettre à jour les signets en conséquence.


Vous pouvez afficher tous les objectifs de votre entreprise, quel que soit le propriétaire. Pour plus d’informations sur la création d’objectifs, voir [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Vous pouvez utiliser la section Pulse des objectifs d’Adobe Workfront en tant qu’outil de collaboration, dans lequel vous pouvez passer en revue et participer à un flux de mises à jour des objectifs actuels qui vous appartiennent, à vos équipes, à vos groupes ou à votre organisation, et vous assurer que les objectifs restent à jour. Les objectifs de Workfront regroupent les mises à jour, commentaires et historique de progression par objectif dans la section Pulse.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les actions décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td> <p>Pour accéder aux fonctionnalités décrites dans cet article, vous devez acheter une licence supplémentaire pour les objectifs d’Adobe Workfront. </p> <p>Pour plus d’informations, voir <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Conditions requises pour utiliser les objectifs Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Affichage ou accès supérieur aux objectifs</p> <p>Note:  <p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir :</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Accorder l’accès aux objectifs Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> 
    <div> 
     <p>Affichage ou autorisations supérieures sur les objectifs</p> 
     <p>Pour plus d’informations sur le partage des objectifs, voir <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partage d’un objectif dans les objectifs Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

## Gestion des mises à jour et des commentaires d’objectif dans la section Pulse 

>[!TIP]
>
>Seuls les objectifs qui ont été archivés au moins une fois s’affichent dans la section Pulse .

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) > **Objectifs** dans le coin supérieur droit de votre écran.

   La zone Objectifs de Workfront s’ouvre alors.

   Tous les objectifs s’affichent par défaut.

1. Cliquez sur **Pulse** dans le panneau de gauche.

   <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: see the numbering in the procedure)
      </MadCap:conditionalText>
      -->

   Une liste d’objectifs s’affiche. La liste contient les colonnes suivantes avec des informations sur chaque objectif :

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Objectifs</td> 
         <td>Nom de l’objectif.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Propriétaire</td> 
         <td>Nom du propriétaire de l’objectif.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Période</td> 
         <td>Période pour laquelle l’objectif est planifié.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Progression</td> 
         <td>Indicateur de progression de l’objectif, généralement une valeur en pourcentage.</td> 
      </tr> 
      <tr> 
         <td role="rowheader"> <p>État (icône d’alignement incluse)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
         <td> <p>L’état de l’objectif qui peut être l’un des suivants :</p> 
         <ul> 
         <li>Actif</li> 
         <li>Brouillon</li> 
         <li>Inactif</li> 
         <li>Fermé</li> 
         </ul> <p>L’icône d’alignement s’affiche sur les objectifs alignés sur d’autres objectifs. Pour plus d’informations sur l’alignement des objectifs, voir <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Alignement des objectifs en les connectant aux objectifs Adobe Workfront</a>.</p>

   <p>La colonne État inclut également les mises à jour incrémentielles effectuées pour chaque résultat ou activité avec chaque archivage sur l’objectif.</p>

   Par exemple, si l’objectif comporte une activité de barre de progression manuelle et que vous archivez l’objectif et mettez à jour l’activité à 50 %, la colonne État affiche 50 % pour l’activité de cet objectif. Par la suite, vous pourrez mettre à jour la même activité à 60 %. Dans ce cas, une nouvelle ligne s’affiche sous le même objectif pour la même activité pour 10 %, car vous venez d’ajouter 10 % à la progression de l’activité.
   </td>
   </tr> 
      </tbody> 
      </table>

1. (Facultatif) Sélectionnez le type d’informations à afficher en mettant à jour les filtres dans le coin supérieur droit de la section Pulse .

   La liste Pulse affiche les objectifs et leur historique mis à jour correspondant aux critères de votre filtre sélectionné.

   Pour plus d’informations sur les objectifs de filtrage, voir [Filtrage des informations dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Cliquez sur la flèche pointant vers la droite située à gauche du nom de l’objectif pour développer un objectif et afficher des informations supplémentaires sur les mises à jour de chaque objectif.

   Les informations suivantes s’affichent dans la section Pulse sous chaque objectif :

   * Noms et propriétaires des résultats. Pour plus d’informations sur les résultats, voir [Ajout de résultats aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * Noms d’activité et propriétaires. Pour plus d’informations sur les activités, voir [Ajout d’activités aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * Barres de progression des résultats et des activités et états de progression. Pour plus d’informations sur la façon dont les objectifs de Workfront calculent la progression des objectifs, voir [Présentation de la progression et de la condition des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/calculate-goal-progress.md).

1. Cliquez sur **Ajouter un commentaire** pour ajouter un commentaire pour l’objectif, puis cliquez sur **Post**. Le commentaire est visible dans la zone Archivage, ainsi que dans l’onglet Mises à jour du panneau Détails de l’objectif . Nous vous recommandons d’utiliser la section Pulse pour commenter les objectifs qui n’ont pas été mis à jour depuis un certain temps et de demander au propriétaire de l’objectif de les mettre à jour.

1. (Facultatif) Cliquez sur **Afficher toutes les mises à jour** pour afficher toutes les mises à jour d’objectif. L’onglet Mises à jour s’ouvre alors dans le panneau Détails de l’objectif à droite.
1. Cliquez sur le nom d’un objectif pour ouvrir la **Détails de l’objectif** sur la droite et passez en revue plus d’informations sur l’objectif et gérez-le, ainsi que ses résultats et activités. Pour plus d’informations sur la révision des objectifs individuels, voir [Mise à jour des objectifs dans la section Détails de l’objectif dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Facultatif et conditionnel) Cliquez sur **l&#39;icône d&#39;alignement** ![](assets/align-icon.png) pour ouvrir l’objectif dans la section Alignement de l’objectif , si l’objectif est aligné sur d’autres objectifs.

1. (Facultatif) Développez la variable **Objectifs par page** et sélectionnez l’une des options suivantes pour afficher d’autres objectifs :

   * 20. Il s’agit de la sélection par défaut.
   * 50
   * 100


