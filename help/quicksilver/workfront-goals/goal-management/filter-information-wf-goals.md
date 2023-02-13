---
product-previous: workfront-goals
navigation-topic: goal-management
title: Filtrage des informations dans les objectifs Adobe Workfront
description: Vous pouvez afficher les objectifs que vous ou toute autre personne avez ajoutés dans les objectifs Adobe Workfront. Pour plus d’informations sur la création d’objectifs, voir Création d’objectifs dans les objectifs Adobe Workfront. Lorsque vous affichez des objectifs, vous pouvez filtrer les informations dans les objectifs de Workfront afin de n’afficher que les objectifs qui vous semblent importants.
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 2%

---

# Filtrage des informations dans les objectifs Adobe Workfront

Vous pouvez afficher les objectifs que vous ou toute autre personne avez ajoutés dans les objectifs Adobe Workfront. Pour plus d’informations sur la création d’objectifs, voir [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md). Lorsque vous affichez des objectifs, vous pouvez filtrer les informations dans les objectifs de Workfront afin de n’afficher que les objectifs qui vous semblent importants.

## Exigences d’accès

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>
-->

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
   <td> <p>Affichage ou accès supérieur aux objectifs</p> <p><b>NOTE</b>

<p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir :</p> 
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

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

## Présentation des filtres dans les objectifs Workfront

>[!NOTE]
>
>Pour identifier et vous concentrer efficacement sur les objectifs appropriés, nous vous recommandons d’utiliser des filtres dans les objectifs de Workfront. Vous pouvez ainsi afficher les informations correctes avant de commencer à gérer les objectifs importants pour vous. Par défaut, les objectifs de Workfront affichent tous les objectifs du système.

Vous pouvez localiser et filtrer les objectifs dans les sections suivantes de la zone Objectifs de Workfront :

* Liste d’objectifs
* Graphiques
* Alignement des objectifs

Pour plus d’informations sur les sections de la zone Objectifs , voir [Présentation des sections Objectifs d’Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>Vous pouvez configurer des filtres pour une section et ils restent persistants lors du passage à une autre section des objectifs de Workfront.

Tenez compte des points suivants lorsque vous utilisez des filtres dans les objectifs Workfront :

* Vous pouvez créer et appliquer un filtre sans l’enregistrer, ou enregistrer un filtre pour le réutiliser ultérieurement.

   Les scénarios suivants existent :

   * Lorsque vous enregistrez un filtre, il devient le filtre par défaut pour vous chaque fois que vous vous connectez aux objectifs Workfront.
   * Lorsque vous appliquez un filtre sans l’enregistrer, vous pouvez revenir aux listes d’origine en actualisant votre page.

* Vous pouvez uniquement afficher et appliquer les filtres que vous avez créés. Les filtres créés par d’autres utilisateurs s’affichent uniquement pour ces utilisateurs.
* Vous ne pouvez pas partager les filtres que vous avez créés avec d’autres utilisateurs.

## Application d’un filtre rapide dans les objectifs Workfront

Vous pouvez utiliser un filtre rapide dans une liste d’objectifs pour vous aider à localiser uniquement les éléments importants pour vous. Vous ne pouvez pas enregistrer les filtres rapides qui ne sont pas persistants. Workfront efface les résultats d’un filtre rapide lors de l’actualisation de la page.

Pour plus d’informations, voir [Appliquer le filtre rapide à une liste](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## Création et application d’un filtre dans les objectifs Workfront

Le processus de création de filtres est le même pour toute section des objectifs de Workfront.

Vous pouvez créer un filtre à partir de zéro ou modifier l’un des filtres intégrés.

1. Accédez aux objectifs de Workfront.

   Pour plus d’informations sur l’accès aux objectifs de Workfront, voir [Accès et ouverture d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   Par défaut, la section Liste des objectifs s’affiche.

1. Cliquez sur **Filtrer** dans le coin supérieur droit de la liste.

   ![](assets/filter-icon-and-label.png)

   Par défaut, Workfront applique la variable **Tous** qui affiche tous les objectifs de votre système.

   >[!TIP]
   >
   >Vous ne pouvez pas modifier ni supprimer le filtre Toutes .

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur l’un des filtres prédéfinis suivants pour afficher uniquement les objectifs pour les propriétaires suivants :

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>Tout</td> 
        <td> <p>Tous les objectifs de votre système, indépendamment de qui les a créés, quelle que soit la période pour lesquels ils ont été créés ou de qui est le propriétaire. Il s’agit du filtre par défaut et vous ne pouvez pas le modifier. </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>Personnel</td> 
        <td>Les objectifs pour lesquels vous êtes le propriétaire.</td> 
       </tr> 
       <tr> 
        <td>Mes équipes</td> 
        <td> <p>Les objectifs pour lesquels l’une de vos équipes est sélectionnée en tant que propriétaire. </p> <p><b>CONSEIL</b>

      Aucun objectif ne s’affiche lorsque vous n’êtes affecté à aucune équipe. </p> </td>
      </tr> 
       <tr> 
        <td>Mes groupes</td> 
        <td>Les objectifs pour lesquels l’un de vos groupes est sélectionné en tant que propriétaire. </td> 
       </tr> 
       <tr> 
        <td>Entreprise</td> 
        <td> <p>Objectifs associés à votre organisation. </p> <p><b>CONSEIL</b>
        <p>Dans les objectifs Adobe Workfront, le filtre Société affiche les objectifs pour lesquels votre entreprise est sélectionnée en tant que propriétaire. </p> <p>Vous ne pouvez pas rechercher des sociétés utilisant ce champ. Seule votre organisation propriétaire de votre instance Workfront est sélectionnée par défaut. </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * Passez la souris sur le nom d’un filtre, puis cliquez sur l’icône **Modifier** icon ![](assets/edit-icon.png) en regard de son nom pour le personnaliser et ajouter des noms spécifiques d’utilisateurs, d’équipes, de groupes ou du nom de votre organisation, puis sélectionnez-le lorsqu’ils apparaissent dans la liste.

   * Cliquez sur **Nouveau filtre** pour créer un nouveau filtre, sélectionnez parmi les options suivantes pour personnaliser le nouveau filtre :

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
        <td> <p>Sélectionnez un état dans le menu déroulant à partir des options suivantes :</p> 
         <ul> 
          <li> <p>Actif</p> </li> 
          <li> <p>Brouillon</p> </li> 
          <li> <p>Inactif</p> </li> 
          <li> <p>Fermé</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Progression</td> 
        <td> <p>Sélectionnez une progression dans le menu déroulant parmi les options suivantes : </p> 
         <ul> 
          <li> <p>En difficulté</p> </li> 
          <li> <p>En danger</p> </li> 
          <li> <p>Dans les temps</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Propriétaire</td> 
        <td> <p>Commencez à saisir le nom d’un propriétaire, puis sélectionnez-le lorsqu’il apparaît dans la liste. </p> <p>Vous pouvez saisir les noms des utilisateurs, des équipes, des groupes ou le nom de votre organisation ou sélectionner des options prédéfinies. </p> <p>Les options de filtre prédéfinies suivantes se rapportent toujours à l’utilisateur actuellement connecté : </p> 
         <ul> 
          <li> <p><strong>Me</strong>: Affiche les objectifs dont vous êtes le propriétaire.</p> </li> 
          <li> <p><strong>Mon équipe d’accueil</strong> et <strong>Toutes mes équipes</strong>: Affiche les objectifs pour lesquels votre équipe d’accueil ou l’une de vos équipes est désignée comme propriétaire. </p> <p>Conseil : Aucun objectif ne s’affiche lorsque vous n’êtes affecté à aucune équipe. </p> </li> 
          <li> <p><strong>Mon groupe d’accueil</strong> et <strong>Tous mes groupes</strong>: Affiche les objectifs pour lesquels votre groupe d’accueil ou l’un de vos groupes est désigné comme propriétaire.</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. (Facultatif) Cliquez sur **Réinitialiser** dans le coin inférieur droit de la zone de filtrage pour effacer tous les champs que vous avez sélectionnés et commencer à créer le filtre à partir de zéro.
1. (Facultatif) Cliquez sur **Appliquer** pour appliquer le filtre sans enregistrer.

   Le filtre s’affiche dans la variable **Non enregistré** du créateur de filtres en tant que **Nouveau filtre**.

   Vous ne pouvez pas renommer un filtre non enregistré.

   Les filtres non enregistrés sont supprimés de la zone Objectifs la prochaine fois que vous vous déconnectez de Workfront et que vous vous reconnectez.

   >[!TIP]
   >
   >Vous ne pouvez avoir qu’un seul nouveau filtre non enregistré à la fois.

1. Cliquez sur **Enregistrer** pour enregistrer le filtre afin de l’utiliser ultérieurement, ajoutez un nom pour le filtre dans la variable **Ajouter un nom de filtre** champ et clic **Terminé**.

   Le filtre est ainsi enregistré dans la variable **Enregistré** du créateur de filtres. Vous pouvez utiliser ce filtre à l’avenir.

   Le dernier filtre enregistré et appliqué s’affiche par défaut lors de la prochaine connexion à Workfront.

1. (Facultatif) Cliquez sur le **flèche pointant vers la gauche** en regard de **Nouveau filtre** pour quitter le créateur de filtres et revenir à la liste des filtres.
1. (Facultatif) Pointez sur le nom d’un filtre personnalisé, puis cliquez sur le bouton **Plus** , puis cliquez sur **Supprimer**, puis **Supprimer**. Cela supprime le filtre et vous ne pouvez pas le récupérer.

   >[!TIP]
   >
   >Vous ne pouvez supprimer aucun des filtres prédéfinis.

1. Cliquez sur le bouton **Icône X** dans le coin supérieur droit du créateur de filtres pour fermer le créateur de filtres.

   Le nom du filtre actuellement appliqué s’affiche à droite de l’icône Filtrer, dans le coin supérieur droit de la liste des objectifs.

   La liste des objectifs est filtrée selon vos critères de filtrage.

1. (Facultatif et conditionnel) Lors de l’affichage des objectifs dans la section Alignement de l’objectif , cliquez sur **Montrez-les** si vous souhaitez afficher les objectifs filtrés.

   ![](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   Le nom du filtre est indiqué en jaune pour indiquer qu’il est ignoré.

   ![](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. (Facultatif et conditionnel) Cliquez sur **Réappliquer le filtre** pour appliquer le filtre et omettre les éléments affichés à l&#39;étape précédente.


