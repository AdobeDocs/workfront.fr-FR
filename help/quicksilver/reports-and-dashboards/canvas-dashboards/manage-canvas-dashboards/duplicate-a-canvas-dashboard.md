---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Copie d’un tableau de bord de zone de travail
description: Vous pouvez copier un tableau de bord de zone de travail pour en créer une variante, telle qu’une copie spécifique à une audience, sans le recréer de zéro.
author: Courtney
feature: Reports and Dashboards
source-git-commit: b66f6931ee2fe83688fb8910861af6e958d1f74f
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 16%

---

# Copie d’un tableau de bord de zone de travail

{{highlighted-preview-article-level}}

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Il se peut que certaines parties de la fonction ne soient pas terminées ou ne fonctionnent pas comme prévu à cette étape. Veuillez soumettre tout commentaire concernant votre expérience en suivant les instructions de la section [Fournir un commentaire](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) de l’article de présentation de la version Beta des tableaux de bord de la zone de travail.<br>
>Si vous avez des commentaires concernant un bug ou un problème technique éventuel, envoyez un ticket à l’assistance Workfront. Pour plus d’informations, consultez la section [Contacter l’assistance clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Notez que cette version bêta n’est pas disponible sur les fournisseurs de cloud suivants :
>
>* Apporter votre propre clé pour Amazon Web Services
>* Azure
>* Google Cloud Platform

Vous pouvez copier un tableau de bord Zone de travail pour en créer une variante pour une autre audience, par exemple une copie au niveau du directeur d’un tableau de bord Exécutif, sans devoir le recréer de zéro.

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
<p>Standard </p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurations des niveaux d’accès</p></td> 
   <td><p>Modifier l’accès aux tableaux de bord ou en créer un</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td><p>Afficher l’accès au tableau de bord</p>
  </td> 
  </tr>
</tbody> 
</table>

Pour plus d’informations sur ce tableau, voir la section [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Conditions préalables

Vous devez créer un tableau de bord avant de pouvoir le dupliquer.

Pour plus d’informations, voir [Créer un tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Copier un tableau de bord

>[!NOTE]
>
>Les préférences de partage ne sont pas copiées dans le nouveau tableau de bord. Si un widget comporte une configuration **Exécuter en tant qu’utilisateur**, celle-ci n’est conservée sur la copie que si vous êtes l’utilisateur désigné ou un administrateur système.

Pour copier un tableau de bord :

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Sur la page **Tableaux de bord de la zone de travail**, ouvrez le tableau de bord à copier.

1. Dans le coin supérieur droit, sélectionnez l’icône **Plus** ![Plus](assets/more-icon.png), puis sélectionnez **Copier**.
   ![Option du menu Copier le tableau de bord](assets/duplicate-dashboard.png)

1. Dans la boîte de dialogue **Copier le tableau de bord**, saisissez un **Nom** pour le nouveau tableau de bord, qui correspond par défaut au nom du tableau de bord source suivi de « (Copier) ».

1. (Facultatif) Dans l’onglet **Détails du tableau de bord**, mettez à jour le **Description** ou **Devise** pour le nouveau tableau de bord.
   ![Copier le tableau de bord - Onglet Détails du tableau de bord](assets/duplicate-details.png)

1. (Facultatif) Cliquez sur l’onglet **Widgets**, puis désélectionnez les widgets que vous ne souhaitez pas inclure dans le tableau de bord en double.
   ![Copier le tableau de bord - Onglet Widgets](assets/copy-widgets.png)

1. (Facultatif) Cliquez sur l’onglet **Filtres et invites**, puis désactivez **Copier les filtres du tableau de bord** ou **Copier les invites du tableau de bord** pour les exclure du tableau de bord en double.
   ![Copier le tableau de bord - Onglet Filtres et invites](assets/copy-filters.png)

1. Cliquez sur **Copier le tableau de bord**.

Un message de confirmation s’affiche avec un lien vers le nouveau tableau de bord.
