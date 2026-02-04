---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Utiliser des champs de devise dans les tableaux de bord de la zone de travail
description: Vous pouvez utiliser les champs de devise dans un tableau de bord Zone de travail.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 3e4ab2dfc66efd262c0c2ad30a9c62758084f8ce
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 10%

---


# Utiliser des champs de devise dans les tableaux de bord de la zone de travail

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Il se peut que certaines parties de la fonction ne soient pas terminées ou ne fonctionnent pas comme prévu à cette étape. Veuillez soumettre tout commentaire concernant votre expérience en suivant les instructions de la section [Fournir un commentaire](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) de l’article de présentation de la version Beta des tableaux de bord de la zone de travail.<br>
>Si vous avez des commentaires concernant un bug ou un problème technique éventuel, envoyez un ticket à l’assistance Workfront. Pour plus d’informations, voir [Contacter le service clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Notez que cette version bêta n’est pas disponible sur les fournisseurs de cloud suivants :
>
>* Apporter votre propre clé pour Amazon Web Services
>* Azure
>* Google Cloud Platform

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
   <p>Afficher l'accès aux données financières</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td><p>Gestion des autorisations relatives au tableau de bord</p>
  </td> 
  </tr> 
</tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Conditions préalables

1. Plusieurs types de devise doivent être configurés dans votre instance Workfront pour utiliser la fonctionnalité décrite dans cet article. Pour plus d&#39;informations, voir [Configurer des taux de change](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   >[!IMPORTANT]
   >
   >La fonctionnalité décrite dans cet article s’applique uniquement aux champs de devise native. La prise en charge des champs de devise personnalisés sera bientôt disponible.


## Définir une devise par défaut pour un tableau de bord de zone de travail

Lors de la création d’un tableau de bord Zone de travail, vous pouvez définir une devise par défaut pour le tableau de bord. Cette devise sera utilisée pour afficher tous les champs de devise native dans les rapports sur le tableau de bord, sauf si le champ de devise est verrouillé au niveau du rapport.

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Cliquez sur **Nouveau tableau de bord** dans le coin supérieur droit.

1. Dans la zone **Créer un tableau de bord** :

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nom</strong></td>
      <td><p>Saisissez un nom pour votre tableau de bord. Nous vous recommandons d’utiliser uniquement des caractères UTF-8 pour éviter des problèmes de compatibilité.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Description (facultative)</strong></td>
      <td>Saisissez une description de votre tableau de bord.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Devise</strong></td>
      <td>Choisissez le type de devise par défaut pour le tableau de bord. <br>
      <br>Les utilisateurs peuvent basculer entre différents types de devise lors du filtrage du tableau de bord.</td>
     </tr>
    </tbody>
   </table>


## Basculer entre les devises sur un tableau de bord Zone de travail

Vous pouvez basculer entre différents types de devise au niveau du tableau de bord. Les rapports qui contiennent des champs de devise seront mis à jour pour refléter le type de devise sélectionné.

Les champs de devise peuvent être verrouillés au niveau du rapport. Si un champ de devise est verrouillé, le type de devise de ce rapport ne change pas lorsque vous modifiez le type de devise du tableau de bord.

Pour modifier le type de devise du tableau de bord :

1. Cliquez sur le menu déroulant Devise dans le coin supérieur droit de la page des détails du tableau de bord.
1. Sélectionnez le type de devise souhaité dans la liste.

   ![liste déroulante modifier la devise](assets/filter-by-currency.png)


## Limites

Le tableau suivant décrit les limites lorsque les devises sont définies dans la zone Taux de change de la Configuration.

<table> 
<tr>
<td></td>
<td>Les utilisateurs peuvent</td>
<td>Les utilisateurs ne peuvent pas</td>
</tr>
<tr> 
<td>La devise unique est définie.</td>
<td>
<ul>
<li>Utiliser des champs de devise native dans les rapports de tableau, d’indicateur de performance clé et de graphique en zone de travail</li>
<li>Utiliser des champs de devise personnalisés dans les rapports de graphique en zone de travail, d’ICP et de graphique</li>
</ul>
</td>
<td>
<ul>
<li>Attribuer une devise par défaut au tableau de bord (à la création ou lors de la modification du tableau de bord)</li>
<li>Afficher et utiliser le bouton (bascule) de devise au niveau du tableau de bord</li>
<li>Verrouiller une devise spécifique pour l’affichage dans un graphique en canevas, un KPI ou un rapport tabulaire</li>
<li>Utilisez les champs de devise Planning dans un graphique en canevas, un KPI et des rapports tabulaires.</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>Plusieurs devises sont définies</td>
<td>
<ul>
  <li>Utiliser des champs de devise native dans les rapports de tableau, d’indicateur de performance clé et de graphique en zone de travail</li>
  <li>Définir une devise par défaut pour le tableau de bord (à la création ou lors de la modification du tableau de bord)</li>
  <li>Afficher et utiliser le bouton (bascule) de devise au niveau du tableau de bord</li>
  <li>Verrouillez une devise spécifique pour l’affichage dans un graphique de zone de travail, un KPI ou un rapport de tableau pour ignorer la préférence de basculement de devise du tableau de bord</li>
</ul>
</td>
<td><ul>
  <li>Utiliser des champs de devise de données personnalisés dans les rapports de tableau, de graphique à zones de travail et d’ICP</li>
  <li>Utilisez les champs de devise Planning dans un graphique en canevas, un KPI et des rapports tabulaires.</li>
</ul>
</td>
</tr></table>





