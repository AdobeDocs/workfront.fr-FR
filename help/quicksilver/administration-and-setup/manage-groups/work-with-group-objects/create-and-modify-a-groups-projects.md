---
user-type: administrator
product-area: system-administration;user-management
keywords: groupe, projets
navigation-topic: work-with-a-groups-objects
title: Création et modification de projets d’un groupe
description: Lorsque vous visualisez un groupe que vous gérez dans la zone Groupes, vous pouvez créer, modifier, exporter, copier et supprimer les projets du groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: db90cf52-7c8f-4972-b67f-401657ba9b13
source-git-commit: 7eaff1c74cd880bde062e6fdf169c73d6eeb7f75
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 88%

---

# Créer et modifier les projets d’un groupe

Lorsque vous visualisez un groupe que vous gérez dans la zone Groupes, vous pouvez visualiser et travailler sur ses projets de la manière suivante :

* Créer un projet pour le groupe
* Modifier, exporter, copier ou supprimer un projet

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs et administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr>
   <td>Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr>
  <tr> 
   <td>Autorisations d’objet</td>
   <td> 
    <ul> 
     <li> <p>Le projet doit être associé au groupe ou à l’un de ses sous-groupes. </p> <p>Pour plus d’informations sur l’affectation d’un groupe à un projet, voir <a href="../../../manage-work/projects/manage-projects/understand-project-overview-area.md" class="MCXref xref">Gérer les informations dans la zone Vue d’ensemble du projet</a>.</p> </li> 
     <li> <p>En outre, vous devez avoir l’autorisation de modifier le projet, soit parce que vous l’avez créé, soit parce qu’il a été partagé avec vous.</p></li> 
    </ul>
    <p><b>NOTE</b> : lorsque vous créez un projet à partir de la page d’un groupe, le système assigne le projet à ce groupe. Cela diffère de la création d’un projet dans d’autres domaines de Workfront, où le système assigne le projet au groupe principal de la personne qui l’a créé (la personne propriétaire du projet).</p> </td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher, travailler et créer des projets pour votre groupe à partir de la zone Groupes

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel créer, afficher ou travailler sur des projets.
1. Dans le panneau de gauche, cliquez sur **Projets** ![Projets dans le menu principal](assets/projects-in-main-menu.png) pour afficher la liste des projets associés au groupe.

1. Effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Travailler avec un projet</p> </td> 
      <td> <p>Sélectionnez le projet, puis utilisez les boutons de la barre d’outils pour le modifier <img src="assets/edit-icon.png">, le partager <img src="assets/share-icon.png"> ou le supprimer <img src="assets/delete.png">.</p> <p>Pour plus d’informations sur ces activités, voir <a href="../../../manage-work/projects/manage-projects/manage-projects-overview.md" class="MCXref xref">Gérer les projets : index des articles</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Créer un projet pour le groupe</p> </td> 
      <td> 
       <ol> 
        <li value="1"> <p>Cliquez sur <strong>Nouveau projet</strong>, puis sélectionnez une option dans le menu déroulant pour indiquer comment vous voulez le créer. </p> <p>Pour plus d’informations, voir la section <a href="../../../manage-work/projects/create-projects/create-project.md#ways-to-create-projects" class="MCXref xref">Comment créer des projets</a> dans l’article <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Créer un projet</a>.</p> </li> 
        <li value="2">Saisissez un nom pour le projet et configurez-le, comme expliqué dans <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifier des projets</a>.</li> 
       </ol> <p> Les préférences de projet définies pour le groupe affectent tous les projets que vous créez dans la zone Groupes. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md" class="MCXref xref">Configurer les préférences d’un projet pour un groupe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exporter la liste des projets</td> 
      <td>Cliquez sur l’icône d’export <img src="assets/export.png"> dans la barre d’outils au-dessus de la liste.</td> 
     </tr> 
    </tbody> 
   </table>
