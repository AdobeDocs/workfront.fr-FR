---
title: Affectation d’utilisateurs à un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: En tant qu’administrateur d’Adobe Workfront, vous pouvez affecter un modèle de mise en page que vous avez créé à tout utilisateur, rôle de tâche, équipe ou groupe qui doit l’utiliser.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 13%

---

# Affecter des utilisateurs à un modèle de mise en page

Vous pouvez affecter un modèle de mise en page que vous avez créé à tout utilisateur, rôle de tâche, équipe ou groupe qui doit l’utiliser.

Pour les utilisateurs auxquels aucun modèle de mise en page n’est affecté, la mise en page par défaut est utilisée. Pour en savoir plus sur la mise en page par défaut, voir [À propos de la mise en page Adobe Workfront par défaut](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Les utilisateurs peuvent également s’attribuer un modèle de mise en page, comme décrit dans la section Modifier les zones Mes demandes de travail et de travail avec des modèles de mise en page.

Vous pouvez attribuer plusieurs modèles de mise en page différents au même nom. Pour plus d’informations sur le modèle de mise en page en vigueur pour un utilisateur, un rôle, un groupe ou une équipe, voir la [priorité d’affectation de modèle de mise en page](#layout-template-assignment-priority) plus loin dans cet article.

Pour plus d’informations sur les modèles de mise en page, voir [Modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Pour plus d’informations sur les modèles de disposition pour les groupes, voir [Créer et modifier des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.
Pour les exécuter pour un groupe, vous devez être responsable de ce groupe.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas accès, demandez à votre équipe d’administration Workfront si des restrictions supplémentaires sont définies pour votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Attribuer un modèle de mise en page aux utilisateurs

1. Commencez à travailler sur un modèle de disposition, comme décrit dans la section [Créer et gérer des modèles de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >Lorsque le modèle de mise en page vous convient, nous vous recommandons de le tester, comme décrit dans la section [Test d&#39;un nouveau modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Cliquez sur **Attribuer ceci à** dans la section supérieure de la page.
1. Dans la zone qui s’affiche, cliquez sur **Ajouter un utilisateur, un rôle de tâche, une équipe ou un groupe**, commencez à saisir le nom d’un utilisateur, d’un rôle de tâche, d’une équipe ou d’un groupe, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   Les noms récemment ajoutés s’affichent avec un arrière-plan bleu. Cela s’avère utile lorsque vous modifiez un modèle de mise en page existant, car vous pouvez distinguer les noms que vous venez d’ajouter de ceux qui étaient déjà dans la liste.

   Une icône Infos ![](assets/info-icon.png) s’affiche à droite du nom de tout utilisateur, rôle de tâche, équipe ou groupe déjà affecté à un autre modèle de mise en page. Vous pouvez placer le pointeur de la souris sur l’icône pour afficher le nom de ce modèle de mise en page et décider si vous souhaitez remplacer l’affectation existante.

1. Répétez les deux étapes précédentes pour affecter le modèle de mise en page à d’autres utilisateurs, rôles de tâche, équipes ou groupes, si nécessaire.

   Vous pouvez affecter jusqu’à 100 utilisateurs à la fois.

1. Cliquez sur **Terminé**, puis sur **Enregistrer** dans le coin inférieur gauche.

   Cette étape complète le processus de création et d’attribution d’un modèle de mise en page.

## Priorité d’attribution du modèle de mise en page {#layout-template-assignment-priority}

Vous et d’autres administrateurs Workfront pouvez affecter plusieurs modèles de mise en page différents à un même utilisateur de quatre manières différentes :

* À l’utilisateur individuel
* Pour un rôle de tâche particulier de l’utilisateur
* Pour une certaine équipe, l’utilisateur est activé
* Pour un certain groupe dans lequel se trouve l’utilisateur

Cependant, un seul modèle de mise en page est visible à tout moment par l’utilisateur. Le modèle visible est déterminé par la hiérarchie de priorité suivante :

* **Utilisateur individuel** : le modèle de mise en page attribué à la personne en tant qu’utilisateur individuel remplace tous les autres. Vous pouvez remplacer une affectation précédente effectuée pour un utilisateur individuel en effectuant une nouvelle affectation ; la plus récente est prioritaire.
* **Rôle de tâche de Principal** : si la personne ne se voit pas attribuer un modèle de mise en page en tant qu’utilisateur unique, elle voit le modèle affecté pour son rôle de tâche principale.

  Seul le modèle de mise en page affecté au rôle de tâche principal d’un utilisateur est visible par l’utilisateur. Les modèles affectés à des rôles de tâche secondaires détenus par l’utilisateur ne sont pas visibles.

* **Équipe Accueil** : si la personne ne se voit pas attribuer un modèle de mise en page en tant qu’utilisateur individuel ou en tant qu’utilisateur avec un rôle de tâche principal, elle voit le modèle affecté à son équipe d’accueil.

  Seul le modèle affecté à l’équipe d’accueil d’un utilisateur est visible par l’utilisateur. Les modèles attribués à d’autres équipes dans lesquelles un utilisateur est membre ne sont pas visibles.

* **Groupe d’accueil** : si la personne ne se voit pas attribuer un modèle de mise en page en tant qu’utilisateur individuel, en tant qu’utilisateur avec un rôle de tâche principal ou en tant que membre d’une équipe d’accueil, elle voit le modèle affecté à son groupe d’accueil.

  Seul le modèle affecté au groupe Accueil d’un utilisateur est visible par l’utilisateur. Les modèles affectés à l’un de leurs autres groupes ne sont pas visibles.

## Un grand nombre d’utilisateurs affectés à un modèle de mise en page

Si vous modifiez un modèle de mise en page qui est attribué à plus de 2 000 utilisateurs et que vous y apportez des modifications, seuls les 2 000 premiers utilisateurs seront conservés dans le modèle de mise en page et les modifications que vous avez apportées seront visibles. Le modèle de mise en page est supprimé de tous les autres.

Si vous avez plus de 2 000 utilisateurs à affecter à un modèle de mise en page, nous vous recommandons d’effectuer l’une des opérations suivantes :

* Organisez les utilisateurs en groupes ou en équipes et affectez le modèle de mise en page à ces groupes ou équipes. Pour plus d’informations, voir [Création d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) et [Création et gestion d’équipes](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Affectez des rôles de tâche aux utilisateurs et affectez le modèle de mise en page à leur rôle de tâche principal. Pour plus d’informations, voir [Création et gestion des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
