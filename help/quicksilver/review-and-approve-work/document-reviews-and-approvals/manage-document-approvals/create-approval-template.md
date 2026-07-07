---
product-area: documents
navigation-topic: approvals
title: Créer un modèle de workflow d’approbation pour les documents
description: Vous pouvez créer des modèles d’approbation afin d’optimiser votre processus d’approbation.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jsEcIKopi-lJOSXQitDnufu3j0AmkWkPmCXtCR0V6nk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5e9318366f0dff85591a5d5a752920027f5c9b0e
workflow-type: tm+mt
source-wordcount: 895
ht-degree: 15%

---

# Créer un modèle de workflow d’approbation pour les documents

{{highlighted-preview}}

Dans la zone Configuration de Workfront , les utilisateurs disposant d’une licence Standard peuvent créer des modèles d’approbation réutilisables. Une fois créés, les modèles d’approbation peuvent être appliqués aux ressources de la zone Documents d’un objet.
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
   <td><p>Tout package Workfront pour gérer les approbations à l’aide du stockage Workfront hérité</p>
<p>Tout package de workflow pour gérer les validations à l’aide de l’espace de stockage dans le cloud Adobe</p> </td> 
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

## Création d’un modèle d’approbation en production

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

Une fois le modèle créé, il peut être appliqué aux documents dans la zone Documents d’un objet pour lancer le processus de révision et d’approbation formel dans Workfront.

<div class="preview">

## Création d’un modèle de validation dans la Prévisualisation

La boîte de dialogue Modèle d’approbation s’ouvre toujours en mode avancé. Il n’existe pas de mode de base pour les modèles. Vous pouvez configurer jusqu’à 30 chemins parallèles dans un modèle, pour un total de 100 étapes. Chaque chemin s’exécute indépendamment et peut contenir une ou plusieurs étapes séquentielles.

Pour créer un modèle de validation :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Révision et approbation** > **Modèles d’approbation**.

1. Cliquez sur **Nouveau modèle** sur le côté droit de la page.

1. Ajoutez un **Nom du modèle**.

1. Renseignez les détails de l’étape 1 du chemin 1 :

   <table>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Les étapes sont nommées <em>Étape 1</em>, <em>Étape 2</em>, etc. par défaut. Renommez l’étape en quelque chose de plus explicite, comme <em> Révision initiale </em> ou <em> Approbation finale </em>.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des noms ou des adresses e-mail (facultatif)</strong></td>
   <td>Commencez à saisir le nom d’un utilisateur ou d’une équipe à ajouter en tant qu’approbateur ou réviseur. Les participants sont facultatifs dans les modèles. Vous pouvez les ajouter lorsque le modèle est appliqué à un document.<p>Remarque : un réviseur ou un approbateur ne peut être affecté qu’à une seule étape ouverte à la fois sur la même ressource. Si plusieurs étapes parallèles sont ouvertes simultanément, la même personne ne peut pas être ajoutée à plusieurs d’entre elles.</p></td>
   </tr>
   <tr>
   <td><strong>Une seule décision requise (facultatif)</strong></td>
   <td>La première personne qui prend une décision termine l’étape.</td>
   </tr>
   <tr>
   <td><strong>Jours ouvrables jusqu'à la date d'échéance (facultatif)</strong></td>
   <td>Choisissez le nombre de jours ouvrés nécessaires à l'exécution de l'étape après son ouverture. La première étape de chaque chemin prend également en charge une date d’échéance absolue. Chaque étape suivante du chemin prend uniquement en charge une date d’échéance relative.</td>
   </tr>
   <tr>
   <td><strong>Ajouter un message personnalisé (facultatif)</strong></td>
   <td>Saisissez un message dans la zone de texte <strong>Ajouter un message personnalisé</strong>. Lorsque le modèle est appliqué à un document, le message s’affiche dans la notification électronique d’approbation et dans l’onglet Approbations de Workfront.<p>Lorsque vous ajoutez une deuxième étape, l’option <strong>Afficher ce message sur toutes les étapes</strong> est sélectionnée par défaut. Laissez-la sélectionnée pour utiliser le même message à chaque étape. Pour utiliser un message différent pour chaque étape, désélectionnez <strong>Afficher ce message sur toutes les étapes</strong>, puis saisissez le message spécifique à l’étape dans la zone de texte <strong>Ajouter un message personnalisé</strong> de chaque étape.</p></td>
   </tr>
   </table>

   ![ajouter une étape](assets/add-stage.png)

1. (Facultatif) Cliquez sur **Ajouter une étape** pour ajouter une autre étape au chemin d’accès. Les étapes d’un chemin s’exécutent de manière séquentielle dans l’ordre dans lequel elles sont répertoriées. Lorsque toutes les décisions requises d’une étape sont prises, l’étape suivante de ce chemin commence et l’étape précédente est verrouillée. Vous pouvez réorganiser les étapes d’un chemin, mais vous ne pouvez pas déplacer une étape d’un chemin à un autre. Chaque chemin peut avoir un nombre différent d’étapes.

1. (Facultatif) Sous **Chemins parallèles**, cliquez sur **Ajouter un chemin** pour ajouter un autre chemin. Le nouveau chemin commence par une étape vide et devient le chemin sélectionné. Les chemins ne peuvent pas être réorganisés.

   ![ajouter des chemins parallèles](assets/add-path.png)

1. (Facultatif) Pour renommer un chemin d’accès, pointez sur le libellé du chemin d’accès, cliquez sur l’icône en forme de crayon, puis saisissez un nouveau nom. Pour supprimer un chemin d’accès, passez le curseur sur le libellé du chemin et cliquez sur l’icône de corbeille. **Le chemin 1** ne peut pas être supprimé et les autres chemins ne peuvent être supprimés que si aucune étape du chemin n’est verrouillée ou terminée.

1. (Facultatif) Pour effacer tous les chemins et toutes les étapes et recommencer, cliquez sur **Réinitialiser** dans le coin supérieur droit.

1. Cliquez sur **Enregistrer**.

Une fois le modèle créé, il peut être appliqué aux documents dans la zone Documents d’un objet pour lancer le processus de révision et d’approbation formel dans Workfront.

</div>



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
