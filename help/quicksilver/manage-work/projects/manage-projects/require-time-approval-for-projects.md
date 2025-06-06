---
product-area: projects
navigation-topic: manage-projects
title: Demander du temps pour l’approbation d’un projet
description: Demander du temps pour l’approbation d’un projet
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 79%

---

# Demander du temps pour l’approbation d’un projet

<!--audited: 08/2024-->

Vous pouvez configurer le projet pour que les heures consignées par rapport au projet soient approuvées par la personne propriétaire du projet. Lorsqu’elles sont configurées de cette manière, les heures doivent d’abord être approuvées par la personne propriétaire du projet avant de pouvoir être utilisées sur un enregistrement de facturation.\
Pour plus d’informations sur les enregistrements de facturation, voir l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>L’activation de cette option ne supprime pas la possibilité pour la personne approbatrice de feuille de temps d’approuver l’heure sur la feuille de temps. Si la personne propriétaire du projet n’approuve pas l’heure ou ne la rejette pas, une personne approbatrice de feuille de temps peut tout de même approuver l’heure sur une feuille de temps.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Pour demander du temps pour l’approbation du projet :</p>
   <ul><li>Nouveau : Standard</li>
   <li>Actuel : formule</li></ul>

<p>Pour approuver les heures consignées dans un projet :</p>
   <ul><li>Nouveau : Light ou supérieur</li>
   <li>Révision ou supérieur</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès Modification ou supérieur pour les projets</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures pour le projet</p>
  </tr> 
  <tr> 
   <td role="rowheader">Accès supplémentaire</td> 
   <td> <p>Pour approuver le temps passé sur un projet, vous devez respecter au moins l’une des conditions suivantes :</p> 
    <ul> 
     <li>Vous êtes la personne propriétaire du projet avec l’accès et les autorisations spécifiés ci-dessus. Dans ce cas, vous pouvez effectuer les opérations suivantes si l’une des conditions ci-dessous existe : 
      <ul>
       <li>Si vous disposez des autorisations de gestion sur le projet, vous pouvez approuver ou rejeter les heures consignées sur le projet par toute autre personne.</li>
       <li> Si vous disposez de l’accès Contribution ou Affichage au projet, vous pourrez approuver ou rejeter uniquement les heures consignées par vous ou par toute autre personne qui vous signale.<br></li>
      </ul></li> 
     <li>Vous disposez d’une licence Plan avec un accès administratif aux Feuilles de temps et heures. Dans ce cas :
      <ul>
       <li>Vous pouvez approuver ou rejeter toutes les heures sur les projets pour lesquels vous disposez au moins des autorisations d’affichage. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. Cliquez sur l’icône **Approuver** ![](assets/approve-hours-icon.png) en haut de la liste des heures.\
   Le statut des heures passe à **Approuvé**.\
   Si vous rejetez par la suite les heures approuvées, le statut des heures passe à **Non approuvé**.\
   Lorsque vous incluez les heures approuvées dans un enregistrement de facturation, le statut des heures passe à **Facturé et approuvé**. Les heures ajoutées à un enregistrement de facturation ne peuvent pas être supprimées. Pour plus d’informations sur la création d’enregistrements de facturation, voir l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

1. (Facultatif) Cliquez sur l’icône **Rejeter** ![](assets/reject-hours-icon.png) pour rejeter les entrées de temps dans le projet.\
   Le statut des heures passe à **Rejeté**.

   >[!NOTE]
   >
   >   Si les heures que vous sélectionnez sont incluses dans un enregistrement de facturation qui a été marqué comme Facturé ou Facturé et approuvé, les icônes Approuver et Rejeter ne s&#39;affichent pas. Vous ne pouvez approuver que les heures qui ne sont pas déjà facturées dans un enregistrement de facturation.

