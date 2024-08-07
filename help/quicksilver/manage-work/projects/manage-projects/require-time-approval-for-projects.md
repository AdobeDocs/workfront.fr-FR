---
product-area: projects
navigation-topic: manage-projects
title: Demander du temps pour l’approbation d’un projet
description: Demander du temps pour l’approbation d’un projet
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 16%

---

# Demander du temps pour l’approbation d’un projet

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

Vous pouvez configurer le projet pour que les heures consignées par rapport au projet soient approuvées par le propriétaire du projet. Lorsqu’elles sont configurées de cette manière, les heures doivent d’abord être approuvées par le propriétaire du projet avant de pouvoir être utilisées sur un enregistrement de facturation.\
Pour plus d’informations sur les enregistrements de facturation, consultez l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>L’activation de cette option ne supprime pas la possibilité pour l’approbateur de feuille de temps d’approuver l’heure sur la feuille de temps. Si le propriétaire du projet n’approuve pas l’heure ou ne la rejette pas, un approbateur de feuille de temps peut tout de même approuver l’heure sur une feuille de temps.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Prévoyez le temps nécessaire à l’approbation du projet.</p>
   <p>Passez en revue ou au-delà pour approuver les heures de connexion à un projet.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès à Projets ou version ultérieure</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations pour le projet ou version ultérieure</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accès supplémentaire</td> 
   <td> <p>Pour approuver le temps passé sur un projet, vous devez respecter au moins l’une des conditions suivantes :</p> 
    <ul> 
     <li>Vous êtes le propriétaire du projet avec l’accès et les autorisations spécifiés ci-dessus. Dans ce cas, vous pouvez effectuer les opérations suivantes si l’une des conditions ci-dessous existe : 
      <ul>
       <li>Si vous disposez des autorisations de gestion sur le projet, vous pouvez approuver ou rejeter les heures de connexion au projet par tout autre utilisateur.</li>
       <li> Si vous disposez d’un accès Contribute ou Afficher au projet, vous pourrez approuver ou rejeter uniquement les heures enregistrées par vous ou par tout autre utilisateur qui vous signale.<br></li>
      </ul></li> 
     <li>Vous disposez d’une licence Plan avec un accès administratif aux Fiches horaires et heures. Dans ce cas :
      <ul>
       <li>Vous pouvez approuver ou rejeter toutes les heures sur les projets que vous disposez au moins des autorisations nécessaires pour les afficher. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Demander du temps pour l’approbation d’un projet

Pour exiger l’approbation du chef de projet pendant des heures, procédez comme suit :

1. Accédez au projet pour lequel vous souhaitez demander une approbation pendant des heures.
1. Cliquez sur l&#39;icône **Plus** ![](assets/more-icon.png) à droite du nom du projet, puis cliquez sur **Modifier**.\
   La boîte de dialogue Modifier le projet s’affiche.

1. Dans la section **Paramètres du projet**, sélectionnez **Exiger du temps pour l&#39;approbation de ce projet**.
1. Cliquer sur **Enregistrer**.\
   Désormais, lorsque l’heure est enregistrée et approuvée, ces heures sont verrouillées et ne peuvent pas être modifiées par l’utilisateur qui les a entrées sur le projet ou la feuille de temps. Seul un administrateur Workfront peut ajuster la durée d’enregistrement.

## Approbation et rejet de la durée d’un projet

En tant que chef de projet, vous pouvez approuver ou rejeter les heures enregistrées pour les tâches, les problèmes ou le projet.

La validation des heures au niveau du projet n’a aucun impact sur la feuille de temps des utilisateurs qui ont consigné les heures. Par exemple, les heures du projet peuvent être approuvées par le chef de projet, mais la feuille de temps doit encore être approuvée par le responsable de l’utilisateur ou l’approbateur de la feuille de temps. 

Si vous configurez un projet pour qu’il soit approuvé aux heures consignées, le chef de projet doit approuver les heures afin qu’elles puissent être incluses dans un enregistrement de facturation pour le projet. Pour plus d’informations sur la création d’enregistrements de facturation, consultez l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

Pour approuver ou rejeter des heures sur un projet :

1. Accédez au projet.
1. Cliquez sur la zone **Hours** dans le panneau de gauche. Elle peut se trouver sous la zone **Afficher plus**.

1. Les heures consignées pour les problèmes, les tâches et le projet s’affichent et doivent avoir le statut **Envoyé**.\
   Cliquez sur la zone située à gauche des entrées d’heure pour sélectionner les heures à valider.

1. Cliquez sur **Approve**.\
   L’état des heures passe à **Approuvé**.\
   Si vous rejetez par la suite les heures approuvées, l’état des heures passe à **Non approuvé**.\
   Lorsque vous incluez les heures approuvées dans un enregistrement de facturation, l’état des heures passe à **Facturé et Approuvé**. Les heures ajoutées à un enregistrement de facturation ne peuvent pas être supprimées. Pour plus d’informations sur la création d’enregistrements de facturation, consultez l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Facultatif) Cliquez sur **Rejeter** pour rejeter les entrées d’heure sur le projet.\
   L’état des heures passe à **Refusé**.
