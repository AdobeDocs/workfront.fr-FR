---
title: Accorder l’accès aux utilisateurs
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès entre les utilisateurs et utilisatrices dans Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: 5113771baf269405e758307d11a392f95ee870fe
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 97%

---


# Accorder l’accès aux utilisateurs et utilisatrices

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès entre les utilisateurs et utilisatrices dans Workfront, comme expliqué dans la section [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurer l’accès aux utilisateurs et utilisatrices

Vous pouvez gérer les informations que les utilisateurs et utilisatrices peuvent afficher et modifier pour d’autres personnes à l’aide d’un niveau d’accès par défaut ou personnalisé que vous créez. Les utilisateurs et utilisatrices disposant des licences de plan et de travail par défaut peuvent afficher les coordonnées d’autres personnes. Les personnes suivantes peuvent créer et modifier d’autres utilisateurs et utilisatrices :

* Administrateur ou administratrice Workfront.

  Pour plus d’informations, voir [Accorder un accès administratif complet à un utilisateur ou une utilisatrice](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Personne disposant d’une licence de plan par défaut qui a également accès aux utilisateurs et utilisatrices, comme expliqué dans cet article.

  Les utilisateurs et utilisatrices qui sont limités à l’affichage des utilisateurs et utilisatrices de leur entreprise ou de l’entreprise principale ont accès à la modification uniquement des personnes qu’ils peuvent voir. Pour plus d’informations, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Personne disposant d’une licence de plan par défaut qui est également désignée comme responsable d’un autre utilisateur ou d’une autre utilisatrice.

  Les personnes qui se voient accorder l’accès en modification aux utilisateurs et utilisatrices de leur niveau d’accès peuvent gérer les personnes qui leur sont rattachées. Pour plus d’informations sur la gestion d’un utilisateur ou d’une utilisatrice, voir [Afficher l’organigramme](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* Une personne disposant d’une licence de plan par défaut qui a créé un utilisateur ou une utilisatrice peut le désactiver, le supprimer ou le modifier. Pour plus d’informations sur la création d’utilisateurs et d’utilisatrices, voir [Ajouter des utilisateurs et utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configurer l’accès des utilisateurs et utilisatrices à la modification des utilisateurs et utilisatrice à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d’accès, comme expliqué dans la section [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Pour modifier la capacité des utilisateurs et utilisatrices disposant d’une licence de plan ou de travail d’afficher les profils d’autres utilisateurs et utilisatrices :

   1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Vue** à droite d’**Utilisateurs et utilisatrices**.

   1. Désactivez **Afficher les informations sur les contacts**, puis cliquez sur le bouton X pour fermer la boîte de dialogue **Ajuster vos paramètres**.

1. Pour modifier la capacité des utilisateurs et utilisatrices disposant d’un accès sous licence de plan à modifier d’autres utilisateurs et utilisatrices, cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Modifier** à droite d’**Utilisateurs et utilisatrices**, puis sélectionnez les fonctionnalités à accorder :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Créer</strong> </td> 
      <td> <p>Permet aux utilisateurs et utilisatrices d’en créer d’autres.<br>Cette option est activée par défaut.</p> 
      &lt;!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Assurez-vous que cette modification est effectuée avant de déchiffrer ces deux notes. Le 29/03, le document spécifiant les besoins indique que cela dépend des résultats de l’enquête.</p>

       &lt;p>&lt;b>NOTE&lt;/b> : cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.&lt;/p>
     --> &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Supprimer</strong> </td> 
      <td> <p> Permet aux utilisateurs et utilisatrices de supprimer les utilisateurs et utilisatrices qu’ils ont eux-mêmes créés.<br>Cette option est activée par défaut.</p> <p><b>NOTE</b> : cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administration des utilisateurs et utilisatrices (tous)</strong> </td> 
      <td> <p>Permet d’effectuer les opérations suivantes pour n’importe quelle personne utilisant Workfront :</p> 
       <ul> 
        <li>Modifier, supprimer ou désactiver la personne</li> 
        <li>Se connecter en tant qu’utilisateur ou utilisatrice<p><b>REMARQUE</b> : vous ne pouvez pas vous connecter en tant qu’utilisateur administrateur système.</p></li> 
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
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si vous ne souhaitez pas accorder aux administrateurs et administratrices de groupes l’accès à l’ensemble des personnes membres des groupes qu’ils gèrent, désactivez les deux options d’administration des utilisateurs et utilisatrices ci-dessus. Les administrateurs et administratrices de groupes pourront toujours accéder aux personnes membres du groupe qu’ils ajoutent à Workfront ou qui leur rendent compte dans Workfront.

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans la section [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), par exemple [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

## Accès des utilisateurs et utilisatrices par type de licence

Pour plus d’informations sur ce que les utilisateurs et utilisatrices de chaque niveau d’accès peuvent faire avec les utilisateurs et utilisatrices, voir la section [Utilisateurs et utilisatrices](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
