---
title: Accorder l’accès aux documents
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux documents dans Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 14%

---

# Accorder l’accès aux documents

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux documents, comme expliqué dans la [présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Cet accès s’applique également aux dossiers de documents.

Pour plus d’informations sur l’utilisation de niveaux d’accès personnalisés pour gérer l’accès des utilisateurs à d’autres types d’objets dans Workfront, voir [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Conditions d’accès

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
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.&gt;.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurer l’accès des utilisateurs aux documents à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d&#39;accès, comme expliqué dans la section [Créer ou modifier des niveaux d&#39;accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite de Documents, puis sélectionnez les fonctionnalités que vous souhaitez accorder sous **Ajuster vos paramètres**.

   ![document_access.png](assets/document-access.png)

   Vous pouvez permettre aux utilisateurs d’effectuer les opérations suivantes sur les projets, tâches et problèmes auxquels ils ont accès :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Créer</td> 
      <td>Télécharger des documents.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer</td> 
      <td> <p>Supprimez les documents téléchargés.</p> <p>L’option <b>Créer</b> est activée automatiquement lorsque cette option est activée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partager</td> 
      <td>Partagez des documents avec des utilisateurs, des rôles de tâche et des équipes spécifiques.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partager les documents publiquement</td> 
      <td>Partagez des documents avec des utilisateurs externes (sans licence Workfront).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partager sur le système</td> 
      <td> <p>Mettez les documents à la disposition de tous dans votre instance Workfront.</p> <p>Tout le monde dans le système peut voir un document partagé de cette manière si :</p> 
       <ul> 
        <li> <p>Vous leur envoyez un lien vers la page Documents où il est téléchargé.</p> </li> 
        <li> <p>Ils la recherchent dans Workfront</p> </li> 
       </ul> <p>L’option <b>Partager</b> est automatiquement activée lorsque cette option est activée.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Lorsque vous configurez un paramètre de niveau d’accès pour un certain type d’objet, cette configuration n’affecte pas l’accès des utilisateurs aux objets de rang inférieur. Par exemple, vous pouvez empêcher les utilisateurs de supprimer des projets de niveau d’accès, mais cela ne les empêche pas de supprimer des documents, qui sont de rang inférieur à des projets. Pour plus d’informations sur la hiérarchie des objets, reportez-vous à la section [Interdépendance et hiérarchie des objets](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) de l’article [Comprendre les objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Facultatif) Pour restreindre les autorisations héritées pour les documents provenant d’objets de rang supérieur, cliquez sur **Définir des restrictions supplémentaires**, puis sélectionnez **Ne jamais hériter de l’accès aux documents des projets, tâches, problèmes, etc**.
1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, passez à l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tels que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’affecter à un utilisateur. Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accès aux documents par type de licence

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec les documents, reportez-vous à la section [Documents](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) de l’article [Fonctionnalité disponible pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accès aux documents partagés

Après avoir téléchargé un document vers Workfront, vous pouvez le partager avec d’autres utilisateurs en leur accordant des autorisations, comme expliqué dans la section [Partager un document](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

Lorsque vous partagez un objet avec un autre utilisateur, les droits du destinataire le concernant sont déterminés par une combinaison de deux éléments :

* Autorisations que vous accordez à votre destinataire pour l’objet
* Paramètres du niveau d&#39;accès du destinataire pour le type d&#39;objet
