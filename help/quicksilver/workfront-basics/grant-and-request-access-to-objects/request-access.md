---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Demande d’accès aux objets
description: La visibilité des objets dans Adobe Workfront dépend de l’accès à ce type d’objet et de vos autorisations sur un objet particulier.
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 968f17721477a4a4c545a553d24de1855388d585
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 95%

---

# Demander l’accès aux objets

La visibilité des objets dans Adobe Workfront dépend de l’accès à ce type d’objet et de vos autorisations sur un objet particulier.

>[!NOTE]
>
>Cet article décrit comment vous pouvez demander des autorisations pour tous les objets, à l’exception des éléments suivants :
>
>* Plan du planificateur de scénarios dans le planificateur de scénarios Adobe Workfront. Pour plus d’informations, voir [Demande d’accès à un plan dans le planificateur de scénario](../../scenario-planner/request-access-to-plan.md). Cette fonction nécessite une licence supplémentaire.
>
>* Vues et espaces de travail dans la planification Workfront. Pour plus d’informations, voir [Présentation des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). Cette fonction nécessite une licence supplémentaire.


Votre équipe d’administration Workfront configure votre accès à un type d’objet dans votre niveau d’accès. Pour plus d’informations, voir [Fonctionnement des niveaux d’accès et des autorisations](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Si vous avez besoin d’autorisations pour des objets spécifiques dans Workfront, vous pouvez demander l’accès à ces objets. Plutôt que d’envoyer un e-mail à l’équipe d’administration Workfront ou à la personne propriétaire de l’objet pour expliquer vos besoins, vous pouvez demander un accès ou des autorisations supplémentaires dans Workfront.

Vous pouvez demander un accès initial aux objets si une personne partage avec vous un lien vers l’objet ou vous pouvez demander un accès supplémentaire aux objets que vous pouvez au moins afficher.

Par exemple, vous disposez peut-être des autorisations d’affichage pour un projet, mais vous devez y ajouter des tâches. Dans ce cas, vous pouvez demander des autorisations de contribution au projet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Pour partager des objets, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard</p> 
   <p>Actuellement : Travail ou licence supérieure</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou de niveau supérieur aux objets pour lesquels vous demandez des autorisations.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Présentation des règles de partage standard

Les règles de partage standard suivantes prennent effet automatiquement, car elles sont configurées en tant qu’options par défaut dans votre système Workfront.

* Les utilisateurs et utilisatrices affectés à une tâche ou à un problème disposent d’un accès en contribution.
* Les personnes gestionnaires de projet, de portfolio et de programme disposent de l’accès en gestion sur leurs objets.
* Les utilisateurs et utilisatrices inclus dans une conversation disposent d’un accès en affichage sur l’objet sur lequel la conversation se produit.
* Les utilisateurs et utilisatrices affectés en tant qu’approbateurs et approbatrices disposent d’un accès en affichage sur l’objet en attente d’approbation.
* Lors du partage d’un tableau de bord, tous les rapports de ce dernier sont également partagés avec le même accès pour les mêmes utilisateurs et utilisatrices.
* Les personnes propriétaires d’objets ne peuvent pas étendre l’accès à un objet au-delà de leur accès à cet objet, comme défini par l’équipe d’administration.

## Demander l&#39;accès

Vous pouvez demander un accès initial aux objets auxquels vous n’avez actuellement pas accès ou demander un accès supplémentaire aux objets auxquels vous n’avez qu’un accès limité.

* [Demander un accès initial](#request-initial-access)
* [Demander un accès supplémentaire](#request-additional-access)

### Demander un accès initial  {#request-initial-access}

Si vous n’avez pas encore accès à un objet et que vous accédez à cet objet à partir d’un lien, un écran s’affiche pour vous informer que vous n’avez pas accès à l’affichage des informations.

Pour demander l’accès initial à un objet, procédez comme suit :

1. Cliquez sur **Demander l’accès**.\
   La boîte de dialogue **Demander l’accès** s’affiche.

1. (Le cas échéant) Si plusieurs personnes disposent de l’accès approprié pour vous accorder un accès supplémentaire, une flèche déroulante s’affiche en regard du nom de la personne.
1. Sélectionnez dans la liste déroulante la personne qui doit recevoir votre demande d’accès.\
   Seuls 10 utilisateurs et utilisatrices sont affichés dans la liste déroulante. La liste est triée par ordre alphabétique.\
   Pour plus d’informations sur l’ordre des utilisateurs et utilisatrices répertoriés dans ce menu déroulant, voir [Hiérarchie des menus déroulants « Demander l’accès » et « Demander davantage d’accès »](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Dans la liste déroulante, sélectionnez le type d’accès que vous demandez.
1. (Facultatif) Dans le champ **P.S.**, rédigez une note à l’attention de l’utilisateur ou de l’utilisatrice sur les raisons pour lesquelles vous avez besoin d’un accès supplémentaire.

   ![](assets/request-access-dialog-350x314.png)

Si vous ne disposez pas des droits de niveau d’accès à un objet et que vous tentez d’y accéder à partir d’un lien, un écran s’affiche pour vous informer de contacter l’administrateur ou administratrice Workfront.

Par exemple, si vous ne disposez pas d’un accès au portfolio, mais que vous recevez un lien vers un portfolio, le message suivant s’affiche :\
![](assets/permission-request-initial2-350x96.png)

### Demander un accès supplémentaire {#request-additional-access}

Pour demander un accès supplémentaire à un objet auquel vous avez déjà un accès limité :

1. Accédez à l’objet pour lequel vous souhaitez demander un accès supplémentaire.

1. Cliquez sur le menu **Plus** à droite du nom du projet, puis cliquez sur **Demander plus d’accès**.

   ![](assets/request-access-in-project-350x201.png)

1. (Le cas échéant) Si plusieurs personnes disposent de l’accès approprié pour vous accorder un accès supplémentaire, une flèche déroulante s’affiche en regard du nom de la personne.
1. Sélectionnez dans la liste déroulante la personne qui doit recevoir votre demande d’accès.\
   Seuls 10 utilisateurs et utilisatrices sont affichés dans la liste déroulante. La liste est triée par ordre alphabétique.\
   Pour plus d’informations sur l’ordre des utilisateurs et utilisatrices répertoriés dans ce menu déroulant, voir [Hiérarchie des menus déroulants « Demander l’accès » et « Demander plus d’accès »](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Dans la liste déroulante, sélectionnez le niveau d’accès que vous demandez.
1. (Facultatif) Dans le champ **P.S.**, indiquez une note expliquant pourquoi vous avez besoin d’un accès supplémentaire.
1. Cliquez sur **Demander l’accès**.\
   ![](assets/request-access-dialog-350x314.png)

## Hiérarchie des menus déroulants « Demander l’accès » et « Demander plus d’accès » {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Comprendre la hiérarchie des utilisateurs et utilisatrices répertoriés dans les menus déroulants Demander l’accès et Demander plus d’accès](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [Comprendre la personne propriétaire d’un objet](#understand-the-owner-of-an-object)

### Comprendre la hiérarchie des utilisateurs et utilisatrices répertoriés dans les menus déroulants Demander l’accès et Demander plus d’accès {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Lors du remplissage des listes « Demander l’accès » ou « Demander plus d’accès » sur des objets, Workfront sélectionne une liste de maximum dix personnes qui remplissent différents rôles dans le partage de l’objet comme décrit ci-dessous. Ces personnes peuvent accorder l’accès à l’objet à la personne qui le demande.\
La liste qui en résulte est alors triée par nom dans l’ordre alphabétique croissant.\
Workfront affiche jusqu’à 10 personnes dans les listes « Demander l’accès » et « Demander plus d’accès ».

L’ordre des utilisateurs et utilisatrices dans les menus déroulants « Demander l’accès » ou « Demander plus d’accès » est dicté par les règles suivantes :

* La première personne de la liste est la « personne propriétaire » de l’objet, comme décrit dans la section [Comprendre la personne propriétaire d’un objet](#understand-the-owner-of-an-object).
* Ensuite, la liste est remplie avec les personnes avec lesquelles l’objet est partagé individuellement. Elles sont répertoriés par ordre alphabétique.
* La liste est ensuite complétée par des utilisateurs et utilisatrices qui obtiennent l’accès requis en partageant avec leurs équipes, groupes ou entreprises. Elles sont répertoriés par ordre alphabétique.
* Si la liste est vide, les administrateurs et administratrices Workfront sont ajoutés afin qu’il y ait toujours quelqu’un à qui demander l’accès. Elles sont répertoriés par ordre alphabétique.
* Chacune des personnes de la liste doit disposer de l’accès requis à l’objet et de l’accès requis pour partager l’objet.

### Comprendre la personne propriétaire d’un objet {#understand-the-owner-of-an-object}

La personne propriétaire d’un objet est définie comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objet</strong> </th> 
   <th><strong>Définition de la personne propriétaire de l’objet</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projets</td> 
   <td>La personne propriétaire est celle qui est propriétaire du projet ou, si elle est manquante ou si elle ne dispose pas de l’accès nécessaire, la personne propriétaire du portfolio parent. <p>Il se peut qu’elle ne soit pas la même personne que le créateur ou la créatrice du projet. </p></td> 
  </tr> 
  <tr> 
   <td>Tâches</td> 
   <td>La personne propriétaire est la personne cessionnaire principale ou, si elle est manquante ou qu’elle ne dispose pas de l’accès nécessaire, la personne propriétaire du projet sur lequel réside la tâche, comme défini ci-dessus. <p>Il se peut qu’elle ne soit pas la même personne que le créateur ou la créatrice de la tâche. </p></td> 
  </tr> 
  <tr> 
   <td>Problèmes</td> 
   <td> <p>La personne propriétaire est le contact principal du problème ou, s’il est manquant ou s’il ne dispose pas d’un accès nécessaire, la personne propriétaire du projet sur lequel réside le problème, comme défini ci-dessus. </p> <p>Il peut ne pas être la même personne que le créateur ou la créatrice du problème. </p> </td> 
  </tr> 
  <tr> 
   <td>Portefeuilles</td> 
   <td>La personne propriétaire est celle qui est propriétaire du portfolio. <p>Il se peut qu’elle ne soit pas la même personne que le créateur ou la créatrice du portfolio. </p></td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>La personne propriétaire est celle propriétaire du document (l’utilisateur ou utilisatrice qui a chargé le document) ou, si elle est manquante ou si elle ne dispose pas d’un accès nécessaire, la personne propriétaire de l’objet sur lequel réside le document.</td> 
  </tr> 
  <tr> 
   <td>Rapports et tableaux de bord</td> 
   <td>La personne propriétaire est celle qui a créé le rapport ou le tableau de bord. </td> 
  </tr> 
  <tr> 
   <td>Calendriers</td> 
   <td>La personne propriétaire est celle qui a créé le calendrier. Par défaut, un calendrier est affecté à toutes les personnes. Chaque personne est considérée comme propriétaire de ce calendrier. </td> 
  </tr> 
  <tr> 
   <td>Filtres, vues et regroupements</td> 
   <td>La personne propriétaire d’un filtre, d’une vue ou d’un regroupement est celle qui en est à l’origine. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Plans</span> </td> 
   <td> <p><span>La personne propriétaire est celle qui a créé le plan.</span> </p> <p>Cette fonction nécessite une licence supplémentaire. </p> <p><span>Pour plus d’informations sur le planificateur de scénarios Workfront, voir</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Vue d’ensemble du planificateur de scénarios</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Objectifs</td> 
   <td> <p>La personne propriétaire est celle désignée comme propriétaire. Il se peut que ce ne soit pas la même personne que celle ayant créé l’objectif. </p> <p>Cette fonction nécessite une licence supplémentaire. </p> <p>Pour plus d’informations sur les objectifs de Workfront, voir <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">vue d’ensemble des Objectifs Adobe Workfront</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


