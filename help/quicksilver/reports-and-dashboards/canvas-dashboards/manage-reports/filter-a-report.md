---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filtrer un rapport dans un tableau de bord Zone de travail
description: Ajoutez ou modifiez un filtre sur un rapport pour contrôler les données affichées dans un tableau de bord Zone de travail.
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
source-wordcount: '434'
ht-degree: 19%
---
# Filtrer un rapport dans un tableau de bord Zone de travail

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Il se peut que certaines parties de la fonction ne soient pas terminées ou ne fonctionnent pas comme prévu à cette étape. Veuillez soumettre tout commentaire concernant votre expérience en suivant les instructions de la section [Fournir un commentaire](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) de l’article de présentation de la version Beta des tableaux de bord de la zone de travail.<br>
>Si vous avez des commentaires concernant un bug ou un problème technique éventuel, envoyez un ticket à l’assistance Workfront. Pour plus d’informations, consultez la section [Contacter l’assistance clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Notez que cette version bêta n’est pas disponible sur les fournisseurs de cloud suivants :
>
>* Apporter votre propre clé pour Amazon Web Services
>* Azure
>* Google Cloud Platform

Vous pouvez filtrer un rapport pour contrôler les données qui s’affichent, à la fois pendant et après la création du rapport. Les options de filtrage et le comportement sont identiques dans les deux cas.

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

Vous devez disposer d’un rapport sur un tableau de bord, ou être en train d’en créer un, avant de pouvoir le filtrer. Pour plus d’informations, voir [Créer un tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Ajout ou modification d’un filtre de rapport

Pour ajouter ou modifier un filtre sur un rapport :

1. Ouvrez le panneau de filtrage du rapport :

   * Si vous créez un rapport, cliquez sur l’icône **Filtrer** dans le panneau de gauche de la boîte de dialogue **Configurer**.
   * Si vous modifiez un rapport existant, cliquez sur l’icône **Plus** dans le coin supérieur droit, sélectionnez **Modifier**, puis cliquez sur le panneau **Filtres** dans la boîte de dialogue **Configurer**.

1. Cliquez sur **Modifier le filtre**.

1. Cliquez sur **Ajouter une condition** puis définissez la condition :

   * Cliquez sur **Choisir un champ**, puis sélectionnez le champ selon lequel vous souhaitez appliquer un filtre.
   * Sélectionnez le modificateur qui définit le type de condition auquel le champ doit répondre.
   * Saisissez ou sélectionnez la valeur à évaluer, si le modificateur en a besoin.

   ![&#x200B; Ajouter une condition &#x200B;](assets/add-condition.png)

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres conditions.

1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

>[!NOTE]
>
>Pour obtenir la liste complète des champs, des opérateurs, des caractères génériques et des règles de filtrage spéciales, voir [Référence de filtre de rapport pour les tableaux de bord de la zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md).

1. Cliquer sur **Enregistrer**.
