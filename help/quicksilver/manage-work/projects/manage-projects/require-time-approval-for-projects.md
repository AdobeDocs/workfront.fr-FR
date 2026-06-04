---
product-area: projects
navigation-topic: manage-projects
title: L’approbation d’un projet demande du temps
description: Vous pouvez configurer le projet pour que les heures consignées par rapport au projet soient approuvées par la personne propriétaire du projet. Lorsqu’elles sont configurées de cette manière, les heures doivent d’abord être approuvées par la personne propriétaire du projet avant de pouvoir être utilisées sur un enregistrement de facturation.
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Ux3CyN-AC7EKD74-GKadkODI3rCBcIIcQIH26LKCA-Y
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 774
ht-degree: 77%

---

# Demander du temps pour l’approbation d’un projet

<!--audited: 08/2024-->

Vous pouvez configurer le projet pour que les heures consignées par rapport au projet soient approuvées par la personne propriétaire du projet. Lorsqu’elles sont configurées de cette manière, les heures doivent d’abord être approuvées par la personne propriétaire du projet avant de pouvoir être utilisées sur un enregistrement de facturation.\
Pour plus d’informations sur les enregistrements de facturation, voir l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>L’activation de cette option ne supprime pas la possibilité pour la personne approbatrice de feuille de temps d’approuver l’heure sur la feuille de temps. Si la personne propriétaire du projet n’approuve pas l’heure ou ne la rejette pas, une personne approbatrice de feuille de temps peut tout de même approuver l’heure sur une feuille de temps.

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
   <td> <p>Pour demander du temps pour l’approbation du projet :</p>
   <ul><li><p>Standard</p></li>
   <li><p>Plan</p></li></ul>

<p>Pour approuver les heures consignées dans un projet :</p>
   <ul><li><p>Léger ou supérieur</p></li>
   <li><p>Révision ou supérieur</p></li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures pour le projet</p>
  </tr> 
  <tr> 
   <td role="rowheader">Accès supplémentaire</td> 
   <td> <p>Pour approuver le temps passé sur un projet, vous devez respecter au moins l’une des conditions suivantes :</p> 
    <ul> 
     <li>Vous êtes le propriétaire du projet avec l'accès et les autorisations spécifiés ci-dessus. Dans ce cas, vous pouvez effectuer les opérations suivantes si l’une des conditions ci-dessous existe : 
      <ul>
       <li>Si vous disposez des autorisations de gestion sur le projet, vous pouvez approuver ou rejeter les heures consignées sur le projet par toute autre personne.</li>
       <li> Si vous disposez de l’accès Contribution ou Affichage au projet, vous pourrez approuver ou rejeter uniquement les heures consignées par vous ou par toute autre personne qui vous signale.<br></li>
      </ul></li> 
     <li>Vous disposez d’une licence Standard ou Plan avec un accès administratif aux Feuilles de temps et heures. Dans ce cas :
      <ul>
       <li>Vous pouvez approuver ou rejeter toutes les heures sur les projets pour lesquels vous disposez au moins des autorisations d’affichage. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

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
   <td> <p>To require time to be approved on the project:</p>
   <ul><li>New: Standard</li>
   <li>Current: Plan</li></ul>
   
   <p>To approve hours logged on a project:</p>
   <ul><li>New: Light or higher</li>
   <li>Review or higher</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects or higher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher</p>
  </tr> 
  <tr> 
   <td role="rowheader">Additional access</td> 
   <td> <p>You must meet at least one of the following conditions to approve time on a project:</p> 
    <ul> 
     <li>You are the Project Owner with the access and permissions specified above. In this case, you can do the following if one of the conditions below exists: 
      <ul>
       <li>If you have Manage permissions on the project, you can approve or reject hours logged on the project by any other user.</li>
       <li> If you have Contribute or View access to the project you will be able to approve or reject only the hours logged by you or any other user that reports you.<br></li>
      </ul></li> 
     <li>You have a Plan license with administrative access to Timesheets &amp; Hours. In this case:
      <ul>
       <li>You can approve or reject any hours on the projects you have at least permissions to View. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Demander du temps pour l’approbation d’un projet

Pour exiger que la personne responsable du projet approuve les heures passées sur le projet :

1. Accédez au projet pour lequel vous souhaitez demander une approbation pour des heures.
1. Cliquez sur l’icône **Plus** ![Plus](assets/more-icon.png) à droite du nom du projet, puis cliquez sur **Modifier**.\
   La boîte de dialogue Modifier le projet s’affiche.

1. Dans la section **Paramètres du projet**, sélectionnez **Demander l’approbation d’heures pour ce projet**.
1. Cliquer sur **Enregistrer**.\
   Désormais, lorsque des heures sont consignées et approuvées, elles sont verrouillées et ne peuvent plus être modifiées par l’utilisateur qui les a saisies dans le projet ou la feuille de temps. Seule une personne de l’administration Workfront peut ajuster les heures consignées.

## Approuver et refuser des heures pour un projet

En tant que responsable de projet, vous pouvez approuver ou rejeter les heures enregistrées pour les tâches, les problèmes ou le projet.

L’approbation des heures au niveau du projet n’a aucun impact sur la feuille de temps des personnes qui ont consigné les heures. Par exemple, les heures du projet peuvent être approuvées par la personne responsable de projet, mais la feuille de temps doit encore être approuvée par le ou la responsable de la personne ou par la personne approbatrice de la feuille de temps.

Si vous configurez un projet pour que ses heures consignées soient approuvées, la personne responsable de projet doit approuver les heures afin qu’elles puissent être incluses dans un enregistrement de facturation pour le projet. Pour plus d’informations sur la création d’enregistrements de facturation, consultez l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

Pour approuver ou rejeter des heures sur un projet :

1. Accédez au projet.
1. Cliquez sur la zone **Heures** dans le panneau de gauche.

1. Les heures consignées pour les problèmes, les tâches et le projet s’affichent et doivent avoir le statut **Envoyé**.\
   Cliquez sur la zone située à gauche des entrées d’heures pour sélectionner les heures à approuver.

1. Cliquez sur l’icône **Approuver** ![Icône Approuver](assets/approve-hours-icon.png) en haut de la liste des heures.\
   Le statut des heures passe à **Approuvé**.\
   Si vous rejetez par la suite les heures approuvées, le statut des heures passe à **Non approuvé**.\
   Lorsque vous incluez les heures approuvées dans un enregistrement de facturation, le statut des heures passe à **Facturé et approuvé**. Les heures ajoutées à un enregistrement de facturation ne peuvent pas être supprimées. Pour plus d’informations sur la création d’enregistrements de facturation, voir l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

1. (Facultatif) Cliquez sur **Icône Rejeter** ![Icône Rejeter les heures](assets/reject-hours-icon.png) pour rejeter les entrées de temps dans le projet.\
   Le statut des heures passe à **Rejeté**.

   >[!NOTE]
   >
   >   Si les heures que vous sélectionnez sont incluses dans un enregistrement de facturation qui a été marqué comme Facturé ou Facturé et approuvé, les icônes Approuver et Rejeter ne s&#39;affichent pas. Vous ne pouvez approuver que les heures qui ne sont pas déjà facturées dans un enregistrement de facturation.

