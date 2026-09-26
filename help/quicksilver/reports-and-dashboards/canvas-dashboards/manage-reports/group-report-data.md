---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Regrouper les données de rapport dans un tableau de bord Zone de travail
description: Organisez les résultats des rapports en groupes. Le regroupement fonctionne différemment selon le type de rapport.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 14%
---
# Regrouper les données de rapport dans un tableau de bord Zone de travail

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Il se peut que certaines parties de la fonction ne soient pas terminées ou ne fonctionnent pas comme prévu à cette étape. Veuillez soumettre tout commentaire concernant votre expérience en suivant les instructions de la section [Fournir un commentaire](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) de l’article de présentation de la version Beta des tableaux de bord de la zone de travail.<br>
>Si vous avez des commentaires concernant un bug ou un problème technique éventuel, envoyez un ticket à l’assistance Workfront. Pour plus d’informations, consultez la section [Contacter l’assistance clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Notez que cette version bêta n’est pas disponible sur les fournisseurs de cloud suivants :
>
>* Apporter votre propre clé pour Amazon Web Services
>* Azure
>* Google Cloud Platform

Le regroupement organise les résultats de votre rapport de sorte que les enregistrements associés apparaissent ensemble. Le fonctionnement du regroupement dépend du type de rapport. Par conséquent, cet article comporte une section distincte pour chacun.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tous </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td> 
<p>Standard</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurations des niveaux d’accès</p></td> 
   <td><p>Accès en modification aux rapports, aux tableaux de bord et aux calendriers</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td><p>Gestion des autorisations relatives au tableau de bord</p>
  </td> 
  </tr>
</tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Conditions préalables

Vous devez disposer d’un rapport sur un tableau de bord, ou être en train d’en créer un, avant de pouvoir regrouper ses données. Pour plus d’informations, voir [Créer un tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Regrouper les lignes dans un rapport tabulaire

Dans un rapport tabulaire, le regroupement organise les lignes du rapport lui-même.

1. Dans la boîte de dialogue **Configurer**, cliquez sur l’icône **Paramètres du groupe** dans le panneau de gauche.

1. Cliquez sur **Ajouter un regroupement**, puis sélectionnez le champ selon lequel vous souhaitez effectuer un regroupement. Le regroupement s’affiche dans l’aperçu de droite.

1. (Facultatif) Répétez cette opération pour ajouter d’autres regroupements.

## Configurer des regroupements d’analyse dans des rapports graphiques et d’indicateurs clés de performance

Dans les rapports de graphiques et d’indicateurs de performance clés, vous ne regroupez pas la visualisation principale. Au lieu de cela, vous configurez la manière dont le tableau d’exploration est regroupé lorsqu’une visionneuse explore une valeur.

1. Dans la boîte de dialogue **Configurer**, cliquez sur l’icône **Paramètres du groupe d’analyse** dans le panneau de gauche.

1. Cliquez sur **Ajouter un regroupement**, puis sélectionnez le champ par lequel vous souhaitez regrouper le tableau d&#39;analyse.

## Configuration des segments dans un rapport de tableau croisé dynamique

Les rapports de tableau croisé dynamique n&#39;utilisent pas les regroupements. Au lieu de cela, vous définissez jusqu’à deux segments, qui sont les catégories par lesquelles les mesures du pivot sont regroupées et totalisées.

1. Dans la boîte de dialogue **Configurer**, cliquez sur l’icône **Segments** dans le panneau de gauche.

1. Cliquez sur **Ajouter un segment**, puis sélectionnez le champ de votre choix. Le segment s’affiche sous forme de colonne dans l’aperçu.

1. (Facultatif) Répétez l’opération pour ajouter un second segment. Vous pouvez ajouter deux segments maximum.

## Affichage de données groupées dans un tableau de bord

Les visionneuses de rapports peuvent développer, réduire et trier les données regroupées. Pour plus d’informations, voir [Affichage des rapports avec des données groupées](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md#view-reports-with-grouped-data) dans [Utilisation des tableaux de bord de la zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).
