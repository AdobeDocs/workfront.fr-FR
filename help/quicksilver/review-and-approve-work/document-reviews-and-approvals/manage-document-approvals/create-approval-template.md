---
product-area: documents
navigation-topic: approvals
title: Créer un modèle de workflow d’approbation pour les documents
description: Vous pouvez créer des modèles d’approbation afin d’optimiser votre processus d’approbation.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
source-git-commit: 6d6ac026bb2aa10ba3e678fb7e0f32dc95d0405f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 47%

---

# Créer un modèle de workflow d’approbation pour les documents

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

Dans la zone Configuration de Workfront , les utilisateurs disposant d’une licence Standard peuvent créer des modèles d’approbation réutilisables. Une fois créés, les modèles d’approbation peuvent être appliqués aux ressources dans la zone Documents d’un projet, d’une tâche ou d’un problème.

>[!IMPORTANT]
>
>Le contenu de cet article fait référence à la fonctionnalité d’approbation de document mise à jour, disponible uniquement pour des comptes spécifiques. Pour plus d’informations sur les processus d’approbation standard, reportez-vous aux articles répertoriés dans la section [Approbations de travail](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

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
   <td> <p>Standard</p> 
   <p>Plan</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++




## Création d’un modèle d’approbation dans votre environnement de production

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Révision et approbation** > **Modèles d’approbation**.
1. Cliquez sur **Nouveau modèle** sur le côté droit de la page.
1. Indiquez les informations suivantes :

   | Nom de modèle | Commencez à saisir un nom pour ce modèle. |
   |----------------------------|---|
   | **(Facultatif) Délai** | Saisissez le délai en jours. La date limite de validation est calculée à partir de ce champ une fois le modèle appliqué à une ressource. |
   | **Ajouter des personnes approbatrices ou des personnes réviseuses** | Commencez à saisir le nom des personnes ou des équipes, puis désigner-les comme réviseuses ou approbatrices. |

1. Cliquer sur **Enregistrer**.



<div class="preview">

## Création d’un modèle d’approbation dans votre environnement de prévisualisation

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Révision et approbation** > **Modèles d’approbation**.
1. Cliquez sur **Nouveau modèle** sur le côté droit de la page.

1. Renseignez les détails suivants :

   <table>
     <tr>
   <td><strong>Nom de modèle</strong></td>
   <td>Ajoutez un nom de modèle. </td>
   </tr>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Ajoutez un nom d’étape. Vous pouvez remplacer le nom par un nom plus explicite, tel que <em> Révision initiale </em> ou <em> Approbation finale </em>.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des noms ou des adresses e-mail</strong></td>
   <td>Commencez à saisir le nom d’un utilisateur ou d’une équipe à ajouter en tant qu’approbateur ou réviseur. Si vous avez uniquement des réviseurs, ils seront avertis et auront la possibilité de terminer la révision, mais aucune décision ne sera requise ou prise.</td>
   </tr>
   <tr>
   <td><strong>Une décision requise (facultatif)</strong></td>
   <td>La première personne qui prend une décision termine l’étape.</td>
   </tr>
   <tr>
   <td><strong>Jours ouvrés jusqu’à échéance</strong></td>
   <td>Sélectionnez le nombre de jours ouvrables restant avant que l'approbation ne soit due après l'activation d'une étape.</td>
   </tr>
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres étapes si nécessaire.

   >[!NOTE]
   >
   >Si vous ajoutez plusieurs étapes, le workflow d’approbation se poursuit dans l’ordre dans lequel elles sont répertoriées. Lorsque toutes les décisions requises sont prises, l’étape suivante commence et l’étape précédente est verrouillée.

   ![&#x200B; Détails du document &#x200B;](assets/new-stage.png)

1. Cliquez sur **Enregistrer**.

Une fois le modèle créé, il peut être appliqué aux documents de la zone Documents d’un projet, d’une tâche ou d’un événement pour lancer le processus formel de révision et d’approbation dans Workfront.

</div>


<!-- Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)-->
