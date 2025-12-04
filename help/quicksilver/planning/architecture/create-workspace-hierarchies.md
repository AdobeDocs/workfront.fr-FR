---
title: Création de hiérarchies Workspace
description: En tant que gestionnaire d'espace de travail, vous pouvez créer plusieurs hiérarchies d'espaces de travail entre les types d'enregistrements dans Adobe Workfront Planning. Après avoir connecté des types d’enregistrements dans un espace de travail et créé une hiérarchie, les types d’enregistrements sont connectés les uns aux autres, un type d’enregistrement étant désigné comme parent et jusqu’à 6 autres types d’enregistrements étant configurés comme enfants.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: ff9371b639e7684a94c08b8cd6293b632fac9edf
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 12%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# Créer des hiérarchies d’espace de travail

En tant que gestionnaire d&#39;espace de travail, vous pouvez créer plusieurs hiérarchies d&#39;espaces de travail entre les types d&#39;enregistrements dans Adobe Workfront Planning.

Après avoir connecté des types d’enregistrements dans un espace de travail et créé une hiérarchie, les types d’enregistrements sont connectés les uns aux autres, un type d’enregistrement étant désigné comme parent et jusqu’à 6 autres types d’enregistrements étant configurés comme enfants. <!--asking Robert how many we can have in one hierarchy; I think 7 total but not sure-->

Les hiérarchies génèrent des chemins de navigation pour les types d’enregistrements et les <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> d’enregistrements qui s’affichent dans leurs en-têtes. Ainsi, les utilisateurs savent où ils se trouvent dans la hiérarchie à n’importe quelle étape de leur workflow.

Pour obtenir des informations générales sur les hiérarchies et les chemins de navigation, voir [&#x200B; Présentation des hiérarchies et des chemins de navigation &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).


## Conditions d’accès

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

+++ Développez pour afficher les exigences d’accès afin d’effectuer les étapes de cet article :  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Tout Workfront et tout package Planning</p></li>
Ou
<li><p>Tout workflow et tout package Planning</p></li></ul>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations d’un espace de travail</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une hiérarchie d’espace de travail
