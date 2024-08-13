---
title: Accorder l’accès aux utilisateurs
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur à d’autres utilisateurs dans Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 15%

---


# Accorder l’accès aux utilisateurs et utilisatrices

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur à d’autres utilisateurs dans Workfront, comme expliqué dans la [présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configuration de l’accès des utilisateurs

Vous pouvez gérer les informations que les utilisateurs peuvent afficher et modifier pour d’autres utilisateurs à l’aide d’un niveau d’accès par défaut ou personnalisé que vous créez. Les utilisateurs disposant des licences de plan et de travail par défaut peuvent afficher les coordonnées d’autres utilisateurs. L’un des utilisateurs suivants peut créer et modifier d’autres utilisateurs :

* Un administrateur Workfront.

  Pour plus d’informations, voir [Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Un utilisateur disposant d’une licence Plan par défaut qui a également accès aux utilisateurs, comme expliqué dans cet article.

  Les utilisateurs qui sont limités pour afficher uniquement les utilisateurs de leur entreprise ou de la principale entreprise ont accès à la modification uniquement des utilisateurs qu’ils peuvent voir. Pour plus d’informations, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Un utilisateur disposant d’une licence Plan par défaut qui est également désigné comme responsable d’un autre utilisateur.

  Les utilisateurs qui se voient accorder l’accès Modifier aux utilisateurs de leur niveau d’accès peuvent gérer les utilisateurs qui leur signalent des informations. Pour plus d&#39;informations sur la gestion d&#39;un utilisateur, voir [Affichage de l&#39;organigramme](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* Un utilisateur disposant d’une licence Plan par défaut qui a créé un utilisateur peut désactiver, supprimer ou modifier l’utilisateur qu’il a créé. Pour plus d&#39;informations sur la création de nouveaux utilisateurs, voir [Ajout d&#39;utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configurer l’accès des utilisateurs à la modification des utilisateurs à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d&#39;accès, comme expliqué dans la section [Créer ou modifier des niveaux d&#39;accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Pour modifier la capacité des utilisateurs disposant d’une licence Plan ou Travail d’afficher les profils d’autres utilisateurs :

   1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** à droite de **Utilisateurs**.

   1. Désactivez **Afficher les informations de contact**, puis cliquez sur le X pour fermer la zone **Affiner vos paramètres**.

1. Pour modifier la capacité des utilisateurs disposant d’un accès sous licence Plan à modifier d’autres utilisateurs, cliquez sur l’icône en forme d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Modifier** à droite de **Utilisateurs**, puis sélectionnez les fonctionnalités que vous souhaitez accorder :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Créer</strong> </td> 
      <td> <p>Permet aux utilisateurs de créer des utilisateurs.<br>Cette option est activée par défaut.</p> 
      &lt;!—
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Assurez-vous que cette modification est effectuée avant de déchiffrer ces deux notes. Le 3/29, le req doc dit que cela dépend des résultats de l'enquête.</p>

       &lt;p>&lt;b>REMARQUE&lt;/b> : cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.&lt;/p>
       —> &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Supprimer</strong> </td> 
      <td> <p> Permet aux utilisateurs de supprimer les utilisateurs qu’ils ont eux-mêmes créés.<br>Cette option est activée par défaut.</p> <p><b>REMARQUE</b> : cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrateur utilisateur (tous les utilisateurs)</strong> </td> 
      <td> <p>Permet aux utilisateurs d’effectuer les opérations suivantes pour n’importe quel utilisateur de Workfront :</p> 
       <ul> 
        <li>Modifier, supprimer ou désactiver l’utilisateur</li> 
        <li>Connexion en tant qu’utilisateur</li> 
        <li>Réinitialisation du mot de passe de l’utilisateur</li> 
       </ul> <p>Cette option est désactivée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrateur utilisateur (utilisateurs de groupe)</strong> </td> 
      <td> <p>Permet aux utilisateurs d’effectuer les opérations suivantes pour tout utilisateur d’un groupe qu’ils administrent : 
        <ul>
         <li><p>Modifier, supprimer ou désactiver l’utilisateur</p></li>
         <li>Connexion en tant qu’utilisateur</li>
         <li><p>Réinitialisation du mot de passe de l’utilisateur</p><p><b>REMARQUE</b> : un administrateur de groupe ne peut pas se connecter en tant qu’administrateur ou réinitialiser le mot de passe d’un administrateur Workfront.</p></li>
        </ul><p>Cette option est désactivée par défaut.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si vous ne souhaitez pas accorder aux administrateurs de groupe l’accès à tous les membres des groupes qu’ils gèrent, désactivez les deux options d’administration des utilisateurs ci-dessus. Les administrateurs de groupe pourront toujours accéder aux membres du groupe qu’ils ajoutent à Workfront ou qui leur signalent dans Workfront.

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, passez à l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tels que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

## Accès des utilisateurs par type de licence

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec les utilisateurs, reportez-vous à la section [Users](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) de l’article [Fonctionnalité disponible pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
