---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Accès nécessaire à la gestion des ressources dans l’équilibreur de charge de travail
description: Si vous ne disposez pas de l’accès ou des autorisations nécessaires, il se peut que vous ne puissiez pas afficher ou gérer vos affectations de travail dans l’équilibreur de charge de travail.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 80%

---

# Accès nécessaire pour gérer les ressources dans l’équilibreur de charge de travail

Si vous ne disposez pas de l’accès ou des autorisations nécessaires, il se peut que vous ne puissiez pas afficher ou gérer vos affectations de travail dans l’équilibreur de charge de travail.

Vous devez disposer d’un accès permettant d’afficher les utilisateurs et utilisatrices dont vous souhaitez consulter ou gérer la charge de travail dans l’équilibreur de charge de travail. En outre, vous devez disposer du bon niveau d’accès et des autorisations adaptées sur les projets auxquels le travail est associé.

## Le plan Adobe Workfront a nécessité l’utilisation de l’équilibreur de charge pour différentes zones.

Le tableau suivant illustre le lien entre le plan Workfront de votre entreprise et l’endroit du système où vous pouvez utiliser l’équilibreur de charge de travail :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Formule Workfront (actuelle)</b></p></td> 
   <td> <p><b>Zones d’accès à l’équilibreur de charge de travail</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Équipe ou supérieure </td> 
   <td>Équilibreur de charge de travail pour une équipe ou un projet</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro ou niveau supérieur</td> 
   <td>Équilibreur de charge de travail pour plusieurs projets, au niveau du système</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p><b>Formule Workfront (nouveau)</b></p></td> 
   <td> <p><b>Zones d’accès à l’équilibreur de charge de travail</b></p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Tous </td> 
   <td>Accès à l’équilibreur de charge de travail n’importe où dans Workfront</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur les plans Workfront, voir la section [Nos plans](https://www.workfront.com/plans?lang=fr).

Pour plus d’informations sur l’emplacement possible de l’équilibreur de charge de travail dans Workfront, voir la section [Localiser l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Accès nécessaire pour visualiser l’équilibreur de charge de travail

Vous devez disposer de l’accès suivant pour visualiser l’équilibreur de charge de travail :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : prévoyez d’afficher l’équilibreur de charge de travail dans la zone Ressource ;</br>
       Travail, pour afficher l’équilibreur de charge de travail d’une équipe ou d’un projet</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Affichage ou accès supérieur à la gestion des ressources</p> <p>Pour plus d’informations sur le niveau d’accès à la gestion des ressources, reportez-vous à l’article <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Accorder l’accès à la gestion des ressources</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Vous devez disposer des autorisations d’affichage sur le projet dont vous souhaitez afficher les affectations. </p> <p>Pour plus d’informations sur les autorisations de projet, voir l’article <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Partager un projet dans Adobe Workfront</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Accès nécessaire pour gérer les affectations dans l’équilibreur de charge de travail

Vous devez disposer des accès suivants pour gérer l’équilibreur de charge de travail :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : planifiez la gestion des affectations dans l’équilibreur de charge de travail dans la zone Ressource ;</br>
       Utilisation, pour gérer les affectations dans l’équilibreur de charge de travail d’une équipe ou d’un projet</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès à la gestion des ressources</p> 
     <p>Pour plus d’informations sur le niveau d’accès à la gestion des ressources, voir l’article <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Accorder l’accès à la gestion des ressources</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Autorisations de contribution ou supérieures relatives au projet dont vous voulez gérer les affectations, ce qui inclut les permissions d’attribuer des affectations. </p> <p>Pour plus d’informations sur les autorisations de projet, voir l’article <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Partager un projet dans Adobe Workfront</a>.</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->