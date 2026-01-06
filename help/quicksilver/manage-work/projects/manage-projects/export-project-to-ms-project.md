---
product-area: projects
navigation-topic: manage-projects
title: Exportation d’un projet vers un projet Microsoft
description: Vous pouvez exporter des projets Adobe Workfront vers Microsoft Project.
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 73%

---

# Exporter un projet vers Microsoft Project

Vous pouvez exporter des projets Adobe Workfront vers Microsoft Project.

>[!IMPORTANT]
>
>* Tous les champs Workfront ne sont pas transférés dans le fichier Microsoft Project.\
>  Pour plus d’informations sur la compatibilité des champs entre Workfront et Microsoft Project, voir l’article [Mapper des champs Microsoft Project avec des projets Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).
>* Nous vous recommandons de limiter le nombre de fois où vous transférez des projets d’une application à une autre.
>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Léger ou supérieur</p>
   <p>Révision ou supérieur</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou supérieur aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Autorisations Afficher ou supérieures au projet</p></td> 
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Exporter un projet de Workfront vers Microsoft Project

Vous pouvez exporter un projet de Workfront à partir de la page du projet, d’une liste de projets ou d’un rapport.

1. Accédez au projet à exporter et cliquez sur l’icône **Plus** ![Menu Plus](assets/qs-more-menu.png) à droite du nom du projet

   ![Liste déroulante supplémentaire](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Ou

   Accédez à une liste ou à un rapport de projet et sélectionnez un projet, puis cliquez sur l’icône Plus ![menu Plus](assets/qs-more-menu.png) en haut de la liste.

   ![Menu Plus développé](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Cliquez sur **Exporter MS Project**.

   Le projet est téléchargé en tant que fichier XML sur votre ordinateur et il est prêt à être importé dans Microsoft Project.
