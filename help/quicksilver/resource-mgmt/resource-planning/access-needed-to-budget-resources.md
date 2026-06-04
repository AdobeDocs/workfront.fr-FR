---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Accès aux ressources de budget nécessaire dans Workfront
description: Vous pouvez afficher et gérer des informations sur la planification des ressources pour les projets auxquels vous avez accès lorsque vous disposez de certains paramètres de niveau d’accès et des autorisations pour vos tâches, utilisateurs et utilisatrices, fonctions et équipes.
author: Lisa
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
TQID: https://experienceleague.adobe.com/X0g8M77au0kHvFSt6q-v0TOc9Lh3VxaHtUngvg-uoUk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 62%

---

# Accès aux ressources de budget nécessaire dans Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

Lorsque votre entreprise a acheté une licence Adobe Workfront qui inclut la planification des ressources, vous pouvez afficher les informations de budget des ressources pour les projets que vous pouvez afficher. Vous pouvez afficher les informations de budget dans le planificateur de ressources.

Pour plus d’informations sur les conditions préalables requises pour utiliser les outils de budgétisation dans Workfront, voir [Commencer avec la planification des ressources](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Pour budgéter les ressources, gérer les pools de ressources et afficher les informations sur les coûts dans les outils de planification des ressources, votre société et vous devez disposer des droits d&#39;accès suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> 
    <ul> 
     <li> <p>Modifier l’accès à la gestion des ressources dans votre niveau d’accès qui inclut :</p> 
      <ul> 
       <li> <p>L’accès pour modifier les priorités du projet et les heures budgétées. </p> </li> 
       <li> <p>Accès à la gestion des pools de ressources, si vous devez gérer des pools de ressources.</p> </li> 
      </ul> <p>Pour plus d’informations sur le niveau d’accès à la gestion des ressources, reportez-vous à l’article <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Accorder l’accès à la gestion des ressources</a>.</p> </li> 
     <li> <p>Modifiez l’accès aux projets et aux personnes. </p> </li> 
     <li> <p> Modifier l'accès aux données financières dans votre niveau d'accès qui inclut l'accès à l'option Afficher ou Modifier les taux de coûts et à l'option Afficher ou Modifier les finances générales, si vous devez afficher ou gérer des informations par coût.</p> <p>Pour plus d’informations sur le niveau d’accès aux données financières, consultez l’article <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Accorder l’accès aux données financières</a>.</p> </li> 
    </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérez les autorisations sur le projet qui incluent les autorisations Modifier les taux de coûts et Modifier les finances générales.</p> <p>Pour plus d’informations sur les autorisations de projet, voir l’article <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Partager un projet dans Adobe Workfront</a>.</p> <p>Pour plus d’informations sur les autorisations financières d’un projet, reportez-vous à l’article <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Partager les autorisations financières sur un objet</a></a>.</p>

<p><b>REMARQUE :</b> lors de l'établissement du budget des ressources dans la vue Rôle, si vous disposez de moins que Gérer les autorisations pour au moins un projet répertorié sous le rôle, vous ne pouvez pas budgéter les heures, l'équivalent temps complet ou le coût pour le rôle. Vous pouvez budgéter uniquement les projets pour lesquels vous disposez des autorisations de gestion.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
