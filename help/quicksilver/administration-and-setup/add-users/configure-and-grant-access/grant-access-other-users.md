---
title: Octroi de l’accès aux utilisateurs
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès entre les utilisateurs et utilisatrices dans Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: f895803007a8f606169589bc4b17c19711c9e3f8
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 61%

---


# Accorder l’accès aux utilisateurs et utilisatrices

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès entre les utilisateurs et utilisatrices dans Workfront, comme expliqué dans la section [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer l’accès aux utilisateurs et utilisatrices

Vous pouvez gérer les informations que les utilisateurs et utilisatrices peuvent afficher et modifier pour d’autres personnes à l’aide d’un niveau d’accès par défaut ou personnalisé que vous créez. Les utilisateurs disposant des licences Standard, Plan et Travail par défaut peuvent consulter les coordonnées d&#39;autres utilisateurs. Les personnes suivantes peuvent créer et modifier d’autres utilisateurs et utilisatrices :

* Administrateur ou administratrice Workfront.

  Pour plus d’informations, voir [Accorder un accès administratif complet à un utilisateur ou une utilisatrice](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Un utilisateur disposant d’une licence Standard ou Plan par défaut qui a également accès aux utilisateurs, comme expliqué dans cet article.

  Les utilisateurs et utilisatrices qui sont limités à l’affichage des utilisateurs et utilisatrices de leur entreprise ou de l’entreprise principale ont accès à la modification uniquement des personnes qu’ils peuvent voir. Pour plus d’informations, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Utilisateur disposant d’une licence Standard ou Plan par défaut et désigné comme responsable d’un autre utilisateur.

  Les personnes qui se voient accorder l’accès en modification aux utilisateurs et utilisatrices de leur niveau d’accès peuvent gérer les personnes qui leur sont rattachées. Pour plus d’informations sur la gestion d’un utilisateur ou d’une utilisatrice, voir [Afficher l’organigramme](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* Un utilisateur disposant d’une licence Standard ou Plan par défaut qui a créé un utilisateur peut désactiver, supprimer ou modifier l’utilisateur qu’il a créé. Pour plus d’informations sur la création d’utilisateurs et d’utilisatrices, voir [Ajouter des utilisateurs et utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configurer l’accès des utilisateurs et utilisatrices à la modification des utilisateurs et utilisatrice à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou à modifier le niveau d’accès, comme expliqué dans [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Pour permettre aux utilisateurs disposant d&#39;une licence Standard, Plan ou Travail d&#39;afficher des informations concernant d&#39;autres utilisateurs, cliquez sur l&#39;icône en forme d&#39;engrenage ![icône en forme d&#39;engrenage](assets/gear-icon-settings.png) sur le bouton **Affichage** situé à droite de **Utilisateurs**, puis sélectionnez les options d&#39;affichage que vous souhaitez accorder dans la zone **Ajuster vos paramètres** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Afficher les taux de facturation</strong> </td> 
      <td> Permet aux utilisateurs d’afficher les taux de facturation sur les profils utilisateur.</td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Afficher les coordonnées</strong> </td> 
      <td> Permet aux utilisateurs d’afficher les pages de détails des utilisateurs des autres utilisateurs.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Afficher les taux de coûts</strong> </td> 
      <td> Permet aux utilisateurs d’afficher les taux de coûts sur les profils utilisateur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Afficher finances générales</strong> </td> 
      <td> Permet aux utilisateurs d'afficher les champs Finances généraux (non liés aux taux de facturation ou de coûts) sur les profils d'utilisateurs.</td>
     </tr> 
    </tbody> 
   </table>

   ![Ajuster les paramètres utilisateur de la vue](assets/fine-tune-view-users.png)

1. Pour permettre aux utilisateurs disposant d&#39;un accès de licence Standard ou Plan de modifier d&#39;autres utilisateurs, cliquez sur l&#39;icône d&#39;engrenage ![icône d&#39;engrenage](assets/gear-icon-settings.png) sur le bouton **Modifier** situé à droite de **Utilisateurs**, puis sélectionnez les options de modification que vous souhaitez accorder dans la zone **Ajuster vos paramètres** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Créer</strong> </td> 
      <td> <p>Permet aux utilisateurs et utilisatrices d’en créer d’autres.<br>Cette option est activée par défaut.</p> 
     <p><b>NOTE</b> : cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.</p>
        </td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Supprimer</strong> </td> 
      <td> <p> Permet aux utilisateurs et utilisatrices de supprimer les utilisateurs et utilisatrices qu’ils ont eux-mêmes créés.<br>Cette option est activée par défaut.</p> <p><b>NOTE</b> : cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modifier les taux de facturation</strong> </td> 
      <td> Permet aux utilisateurs de modifier les taux de facturation sur les profils utilisateur.</td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modifier les taux de coûts</strong> </td> 
      <td> Permet aux utilisateurs de modifier les taux de coût sur les profils utilisateur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modifier finances générales</strong> </td> 
      <td> Permet aux utilisateurs de modifier les champs Finances généraux (sans rapport avec les taux de facturation ou de coûts) des profils d'utilisateurs.</td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administration des utilisateurs et utilisatrices (tous)</strong> </td> 
      <td> <p>Permet d’effectuer les opérations suivantes pour n’importe quelle personne utilisant Workfront :</p> 
       <ul> 
        <li>Modifier, supprimer ou désactiver la personne</li> 
        <li>Se connecter en tant qu’utilisateur ou utilisatrice<p><b>REMARQUE </b> : vous ne pouvez pas vous connecter en tant qu'utilisateur administrateur système.</p></li> 
        <li>Réinitialiser le mot de passe de l’utilisateur ou de l’utilisatrice</li> 
       </ul> <p>Cette option est désactivée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administration des utilisateurs et utilisatrices (utilisateurs et utilisatrices de groupe)</strong> </td> 
      <td> <p>Permet d’effectuer les opérations suivantes pour toute personne d’un groupe administré : 
        <ul>
         <li><p>Modifier, supprimer ou désactiver la personne</p></li>
         <li>Se connecter en tant qu’utilisateur ou utilisatrice</li>
         <li><p>Réinitialiser le mot de passe de l’utilisateur ou de l’utilisatrice</p><p><b>NOTE</b> : un administrateur ou une administratrice de groupes ne peut pas se connecter en tant qu’administrateur ou administratrice Workfront, ni réinitialiser son mot de passe.</p></li>
        </ul><p>Cette option est désactivée par défaut.</p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Afficher les taux de facturation</strong> </td> 
      <td> Permet aux utilisateurs d’afficher les taux de facturation sur les profils utilisateur.</td>  
     </tr>
     <tr> 
      <td role="rowheader"><strong>Afficher les taux de coûts</strong> </td> 
      <td> Permet aux utilisateurs d’afficher les taux de coûts sur les profils utilisateur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Afficher finances générales</strong> </td> 
      <td> Permet aux utilisateurs d'afficher les champs Finances généraux (non liés aux taux de facturation ou de coûts) sur les profils d'utilisateurs.</td>
     </tr>
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si vous ne souhaitez pas accorder aux administrateurs et administratrices de groupes l’accès à l’ensemble des personnes membres des groupes qu’ils gèrent, désactivez les deux options d’administration des utilisateurs et utilisatrices ci-dessus. Les administrateurs et administratrices de groupes pourront toujours accéder aux personnes membres du groupe qu’ils ajoutent à Workfront ou qui leur rendent compte dans Workfront.

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans la section [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), par exemple [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

## Accès des utilisateurs et utilisatrices par type de licence

Pour plus d’informations sur ce que les utilisateurs et utilisatrices de chaque niveau d’accès peuvent faire avec les utilisateurs et utilisatrices, voir la section [Utilisateurs et utilisatrices](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
