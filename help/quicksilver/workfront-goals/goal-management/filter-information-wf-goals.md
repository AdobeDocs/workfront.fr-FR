---
product-previous: workfront-goals
navigation-topic: goal-management
title: Filtrer les informations dans les objectifs Adobe Workfront
description: Vous pouvez afficher les objectifs que vous ou toute autre personne avez ajoutés dans Objectifs Adobe Workfront. Pour plus d’informations sur la création d’objectifs, voir Créer des objectifs dans Objectifs Adobe Workfront. Lorsque vous affichez des objectifs, vous pouvez filtrer les informations dans les Objectifs Workfront afin de n’afficher que les objectifs qui vous semblent importants.
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 89%

---

# Filtrer des informations dans Objectifs Adobe Workfront

<!--Audited for P&P only: 4/2025-->

Vous pouvez afficher les objectifs que vous ou toute autre personne avez ajoutés dans Objectifs Adobe Workfront. Pour plus d’informations sur la création d’objectifs, voir [Créer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md). Lorsque vous affichez des objectifs, vous pouvez filtrer les informations dans les Objectifs Workfront afin de n’afficher que les objectifs qui vous semblent importants.

## Conditions d’accès

>[!NOTE]
>
>Votre entreprise peut choisir de continuer à utiliser les objectifs Adobe Workfront si elle a déjà acheté ce package par le passé. Pour plus de détails, contactez votre représentant de compte.
>
>Adobe Workfront Goals ne peut plus être acheté.

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Package Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licence Adobe Workfront</td>
 <td>
 <p>Contributeur ou version ultérieure</p>
<p>Requête ou supérieure</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuration du niveau d’accès</td>
 <td> <p>Modifier l’accès aux Objectifs</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <div>
  <p>Autorisations d’affichage ou supérieures pour les objectifs.</p>
  <p>Gérez les autorisations relatives aux objectifs pour les modifier.</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Un modèle de mise en page comprenant la zone Objectifs du menu principal doit être affecté à tous les utilisateurs, y compris les administrateurs système. </p>  
</td>
  </tr>
</tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
   <p> New product requirement: Workfront</p>
  <p>Or</p>
   <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Vue d’ensemble des filtres dans les Objectifs Workfront

>[!NOTE]
>
>Pour identifier et vous concentrer efficacement sur les objectifs appropriés, nous vous recommandons d’utiliser des filtres dans les Objectifs Workfront. Vous pouvez ainsi afficher les informations correctes avant de commencer à gérer les objectifs importants pour vous. Par défaut, les Objectifs Workfront affichent tous les objectifs du système.

Vous pouvez localiser et filtrer les objectifs dans différentes sections de la zone Objectifs dans Workfront :

* Liste d’objectifs
* Graphiques
* Alignement des objectifs

Pour plus d’informations sur les sections de la zone Objectifs, voir [Vue d’ensemble des sections d’Objectifs Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>Vous pouvez configurer des filtres pour une section et ils restent persistants lors du passage à une autre section des Objectifs Workfront.

Tenez compte des points suivants lorsque vous utilisez des filtres dans les Objectifs Workfront :

* Vous pouvez créer et appliquer un filtre sans l’enregistrer, ou enregistrer un filtre pour le réutiliser ultérieurement.

  Les scénarios suivants sont possibles :

   * Lorsque vous enregistrez un filtre, il devient votre filtre par défaut chaque fois que vous vous connectez aux Objectifs Workfront.
   * Lorsque vous appliquez un filtre sans l’enregistrer, vous pouvez revenir aux listes d’origine en actualisant votre page.

* Vous pouvez uniquement afficher et appliquer les filtres que vous avez créés. Les filtres créés par d’autres personnes s’affichent uniquement pour ces personnes.
* Vous ne pouvez pas partager les filtres que vous avez créés avec d’autres personnes.

## Appliquer un filtre rapide dans Objectifs Workfront

Pour localiser rapidement les éléments qui vous intéressent dans une liste d’objectifs, vous pouvez utiliser un filtre rapide. Vous ne pouvez pas enregistrer les filtres rapides et ils ne sont pas persistants. Lors de l’actualisation d’une page, Workfront supprime les résultats d’un filtre rapide.

Pour plus d’informations, consultez la section [Appliquer un filtre rapide à une liste](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## Créer et appliquer un filtre dans Objectifs Workfront

Pour toutes les sections des Objectifs Workfront, le processus de création de filtres est le même.

Vous pouvez créer un filtre à partir de zéro ou modifier l’un des filtres intégrés.

1. Accédez aux Objectifs Workfront.

   Pour plus d’informations sur l’accès aux Objectifs Workfront, consultez la section [Accéder et ouvrir des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   Par défaut, la section « Liste des objectifs » s’affiche.

1. Cliquez sur **Filtre** dans le coin supérieur droit de la liste.

   ![Icône de filtre](assets/filter-icon-and-label.png)

   Par défaut, Workfront applique le filtre **Tous** qui affiche tous les objectifs de votre système.

   >[!TIP]
   >
   >Le filtre « Tous » ne peut ni être modifié ni être supprimé.

1. Utilisez l’une des méthodes suivantes :

   * Pour afficher uniquement les objectifs pour les personnes propriétaires suivantes, cliquez sur l’un de ces filtres prédéfinis :

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>Tout</td> 
        <td> <p>Tous les objectifs de votre système, indépendamment des personnes qui les ont créés, de la période à laquelle ils se rapportent ou des personnes propriétaires. Il s’agit du filtre par défaut et vous ne pouvez pas le modifier. </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>Personnel</td> 
        <td>Objectifs dont vous êtes propriétaire.</td> 
       </tr> 
       <tr> 
        <td>Mes équipes</td> 
        <td> <p>Objectifs dont l’entité propriétaire est l’une de vos équipes. </p> <p><b>CONSEIL</b>

     Si aucune équipe ne vous est affectée, aucun objectif ne s’affichera. </p> </td>
     </tr> 
       <tr> 
        <td>Mes groupes</td> 
        <td>Objectifs dont l’entité propriétaire est l’un de vos groupes. </td> 
       </tr> 
       <tr> 
        <td>Entreprise</td> 
        <td> <p>Objectifs associés à votre entreprise. </p> <p><b>CONSEIL</b>
        <p>Le filtre « Entreprise » des Objectifs Adobe Workfront affiche les objectifs dont l’entité propriétaire est votre entreprise. </p> <p>Ce champ ne permet pas de rechercher des entreprises. Par défaut, seule votre entreprise, propriétaire de votre instance Workfront, est sélectionnée. </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * Pointez sur le nom d’un filtre, puis cliquez sur l’icône **Modifier** ![icône Modifier](assets/edit-icon.png) en regard de son nom pour le personnaliser et ajouter des noms spécifiques d’utilisateurs, d’équipes, de groupes ou le nom de votre organisation, puis sélectionnez-le lorsqu’il apparaît dans la liste.

   * Pour créer un filtre, cliquez sur **Nouveau filtre** et choisissez parmi les options suivantes pour le personnaliser :

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Période</td> 
        <td>Sélectionnez une période dans le menu déroulant. Vous pouvez sélectionner plusieurs périodes. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Statut</td> 
        <td> <p>Sélectionnez un statut dans le menu déroulant à partir des options suivantes :</p> 
         <ul> 
          <li> <p>Actif</p> </li> 
          <li> <p>Brouillon</p> </li> 
          <li> <p>Inactif</p> </li> 
          <li> <p>Fermé</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Progression</td> 
        <td> <p>Sélectionnez un statut de progression dans le menu déroulant parmi les options suivantes : </p> 
         <ul> 
          <li> <p>En difficulté</p> </li> 
          <li> <p>En danger</p> </li> 
          <li> <p>En bonne voie</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Propriétaire</td> 
        <td> <p>Commencez à saisir le nom d’une personne propriétaire, puis sélectionnez-le lorsqu’il apparaît dans la liste. </p> <p>Vous pouvez saisir les noms des utilisateurs et utilisatrices, des équipes, des groupes ou le nom de votre organisation ou sélectionner des options prédéfinies. </p> <p>Les options de filtre prédéfinies suivantes se rapportent toujours à la personne actuellement connectée : </p> 
         <ul> 
          <li> <p><strong>Moi</strong> : affiche les objectifs dont vous êtes propriétaire.</p> </li> 
          <li> <p><strong>Mon équipe interne</strong> et <strong>Toutes mes équipes</strong> : affichent les objectifs pour lesquels votre équipe interne ou l’une de vos équipes est désignée comme propriétaire. </p> <p>Conseil : aucun objectif ne s’affiche lorsqu’aucune équipe ne vous est affectée. </p> </li> 
          <li> <p><strong>Mon groupe interne</strong> et <strong>Tous mes groupes</strong> : affichent les objectifs pour lesquels votre groupe interne ou l’un de vos groupes est désigné comme propriétaire.</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. (Facultatif) Cliquez sur **Réinitialiser** dans le coin inférieur droit de la zone de filtrage pour effacer tous les champs que vous avez sélectionnés et commencer à créer le filtre à partir de zéro.
1. (Facultatif) Cliquez sur **Appliquer** pour appliquer le filtre sans enregistrer.

   Le filtre s’affiche dans la zone **Non enregistré** du créateur de filtres en tant que **Nouveau filtre**.

   Vous ne pouvez pas renommer un filtre non enregistré.

   Les filtres non enregistrés sont supprimés de la zone Objectifs la prochaine fois que vous vous déconnectez de Workfront et que vous vous reconnectez.

   >[!TIP]
   >
   >Vous ne pouvez avoir qu’un seul nouveau filtre non enregistré à la fois.

1. Cliquez sur **Enregistrer** pour enregistrer le filtre afin de l’utiliser ultérieurement, puis ajoutez un nom pour le filtre dans le champ **Ajouter un nom de filtre** et cliquez sur **Terminé**.

   Cela enregistre le filtre dans la section **Enregistré** du créateur de filtres. Vous pouvez utiliser ce filtre à l’avenir.

   Le dernier filtre enregistré et appliqué s’affiche par défaut lors de la prochaine connexion à Workfront.

1. (Facultatif) Cliquez sur la **flèche pointant vers la gauche** en regard de **Nouveau filtre** pour quitter le créateur de filtres et revenir à la liste des filtres.
1. (Facultatif) Pointez sur le nom d’un filtre personnalisé, cliquez sur le menu **Plus**, puis cliquez sur **Supprimer**, puis sur **Supprimer**. Cela supprime le filtre et vous ne pouvez pas le récupérer.

   >[!TIP]
   >
   >Vous ne pouvez supprimer aucun des filtres prédéfinis.

1. Cliquez sur l’**icône X** dans le coin supérieur droit du créateur de filtres pour fermer le créateur de filtres.

   Le nom du filtre actuellement appliqué s’affiche à droite de l’icône Filtrer, dans le coin supérieur droit de la liste des objectifs.

   La liste des objectifs est filtrée selon vos critères de filtre.

1. (Facultatif et le cas échéant) Lors de l’affichage des objectifs dans la section Alignement des objectifs, cliquez sur **Afficher** si vous souhaitez afficher les objectifs filtrés.

   ![Afficher le lien sur les éléments filtrés](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   Le nom du filtre est indiqué en jaune pour indiquer qu’il est ignoré.

   ![Contour jaune du filtre](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. (Facultatif et le cas échéant) Cliquez sur **Réappliquer le filtre** pour appliquer le filtre et omettre les éléments affichés à l’étape précédente.


