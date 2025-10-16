---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Accès nécessaire pour gérer les ressources dans l’équilibreur de charge de travail
description: Si vous ne disposez pas de l’accès ou des autorisations nécessaires, il se peut que vous ne puissiez pas afficher ou gérer vos affectations de travail dans l’équilibreur de charge de travail.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 67%

---

# Accès nécessaire pour gérer les ressources dans l’équilibreur de charge de travail

{{preview-fast-release-general}}

Si vous ne disposez pas de l’accès ou des autorisations nécessaires, il se peut que vous ne puissiez pas afficher ou gérer vos affectations de travail dans l’équilibreur de charge de travail.

Vous devez disposer d’un accès permettant d’afficher les utilisateurs et utilisatrices dont vous souhaitez consulter ou gérer la charge de travail dans l’équilibreur de charge de travail. En outre, vous devez disposer du bon niveau d’accès et des autorisations adaptées sur les projets auxquels le travail est associé.

<!--## Adobe Workfront package needed to use the Workload Balancer for different areas

The following table illustrates the connection between the Workfront plan your company has and where in the system you can use the Workload Balancer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><p><b>Workfront Plan (Current)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr> 
  <tr> 
   <td>Team or higher </td> 
   <td>Workload Balancer for a team or a project</td> 
  </tr> 
  <tr> 
   <td>Pro or higher</td> 
   <td>Workload Balancer for multiple projects, at the system level</td> 
  </tr> 
  <tr> 
   <td><p><b>Workfront Plan (New)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr>
  <tr> 
   <td>Any </td> 
   <td>Access the Workload Balancer anywhere in Workfront</td> 
  </tr> 
 </tbody> 
</table>

For information about the Workfront plans, see [Our Plans](https://business.adobe.com/fr/products/workfront/pricing.html).

For information about where you can locate the Workload Balancer in Workfront, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).-->

## Accès nécessaire pour visualiser l’équilibreur de charge de travail

Vous devez disposer de l’accès suivant pour visualiser l’équilibreur de charge de travail :

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
       <p>Plan, pour afficher l’équilibreur de charge de travail dans la zone Ressource ; Travail, pour afficher l’équilibreur de charge de travail d’une équipe ou d’un projet</p></td>
  </tr>  
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou supérieur à la gestion des ressources</p> <p>Pour plus d’informations sur le niveau d’accès à la gestion des ressources, reportez-vous à l’article <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md">Accorder l’accès à la gestion des ressources</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td> <p>Vous devez disposer des autorisations d'affichage pour le projet dont vous souhaitez afficher les affectations. </p> <p>Pour plus d’informations sur les autorisations de projet, voir l’article <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">Partager un projet dans Adobe Workfront</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<span class="preview">Tous les utilisateurs ont accès à l’équilibreur de charge de travail sur leurs propres profils. Ce n’est pas limité par la licence ou le niveau d’accès. Notez que l’équilibreur de charge de travail sur un profil utilisateur est en lecture seule et que les affectations et les allocations ne peuvent pas être modifiées.</span>

## Accès nécessaire pour gérer les affectations dans l’équilibreur de charge de travail

Vous devez disposer des accès suivants pour gérer l’équilibreur de charge de travail :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td>
  </tr>
  <tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Planification, pour gérer les affectations dans l’équilibreur de charge de travail dans la zone Ressource ; Travail, pour gérer les affectations dans l’équilibreur de charge de travail d’une équipe ou d’un projet</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td>
   <td> <p>Modifier l’accès à la gestion des ressources</p>
     <p>Pour plus d’informations sur le niveau d’accès à la gestion des ressources, voir l’article <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" >Accorder l’accès à la gestion des ressources</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td> <p> Autorisations de contribution ou supérieures relatives au projet dont vous voulez gérer les affectations, ce qui inclut les permissions d’attribuer des affectations. </p> <p>Pour plus d’informations sur les autorisations de projet, voir l’article <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">Partager un projet dans Adobe Workfront</a>.</p></td>
  </tr> 
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->
