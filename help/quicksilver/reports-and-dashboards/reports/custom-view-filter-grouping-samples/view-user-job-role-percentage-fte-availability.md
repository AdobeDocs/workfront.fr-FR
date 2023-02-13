---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : Pourcentage du rôle de l’utilisateur par rapport à la disponibilité de l’éditeur de texte enrichi"
description: Vous pouvez ajouter une colonne à l’affichage d’une liste d’utilisateurs pour afficher la liste des rôles de tâche auxquels l’utilisateur est associé, ainsi que le pourcentage de disponibilité de l’éditeur de texte enrichi pour chaque rôle de tâche, tel que défini dans le profil utilisateur.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Afficher : Pourcentage du rôle de l’utilisateur par rapport à la disponibilité de l’éditeur de texte enrichi

Vous pouvez ajouter une colonne à l’affichage d’une liste d’utilisateurs pour afficher la liste des rôles de tâche auxquels l’utilisateur est associé, ainsi que le pourcentage de disponibilité de l’éditeur de texte enrichi pour chaque rôle de tâche, tel que défini dans le profil utilisateur.

Pour plus d’informations sur la définition du pourcentage de disponibilité de l’éditeur de texte enrichi pour les utilisateurs, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_avialbility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Affichage du pourcentage du rôle de tâche de l’utilisateur pour la disponibilité de l’éditeur de texte enrichi

1. Accédez à une liste d’utilisateurs.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Dans le **Aperçu des colonnes** zone, cliquez sur **Ajouter une colonne**.

1. Cliquez sur l’en-tête de la nouvelle colonne, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :

   <pre>displayname=Roles (pourcentage de temps)<br>listsepariter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. Cliquez sur **Enregistrer**, puis **Enregistrer la vue**.

1. (Facultatif) Attribuez un nom à votre vue, puis cliquez sur **Enregistrer la vue**.
