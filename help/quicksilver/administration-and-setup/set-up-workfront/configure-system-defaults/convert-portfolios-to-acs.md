---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Conversion de portefeuilles hérités en espace de stockage Adobe
description: Convertissez les anciens portfolios de stockage Workfront en stockage cloud Adobe à partir de la zone Préférences de stockage dans les Préférences système.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 9d28f52ace4d443bdffc475baf79d482152d4157
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 11%

---

# Conversion de portefeuilles hérités en espace de stockage Adobe

En tant qu’administrateur Workfront, vous pouvez convertir des portfolios de stockage Workfront existants en stockage dans le cloud Adobe à partir de la zone Préférences de stockage dans les Préférences système. Une fois un portfolio converti, il se comporte comme n’importe quel autre portfolio de stockage dans le cloud Adobe.

Pour plus d’informations sur le comportement des portfolios convertis et sur la manière dont leurs objets enfants sont affectés, voir [Portabilité des objets](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability) dans [Déplacer vers Workfront sur l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>N’importe quel package de workflow</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur ou une administratrice Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Avant la conversion d’un portfolio

Avant de convertir un ancien portefeuille de stockage Workfront, tenez compte des points suivants :

* La conversion affecte uniquement le portefeuille lui-même. Les projets et programmes enfants qui utilisent le stockage Workfront hérité restent sur le stockage hérité.
  >[!NOTE]
  >
  >Un programme hérité enfant est automatiquement converti en espace de stockage Adobe uniquement lorsqu’un utilisateur y ajoute manuellement un projet d’espace de stockage Adobe.
* Les documents et les dossiers de documents du portfolio restent sur l’ancien stockage Workfront après la conversion.
* Après la conversion, vous ne pouvez pas ajouter les projets de stockage Workfront hérités au portefeuille.

## Conversion de portefeuilles hérités en espace de stockage Adobe

Pour convertir un ou plusieurs portfolios de stockage Workfront hérités en stockage dans le cloud Adobe :

{{step-1-to-setup}}

1. Sélectionnez **Système** dans le volet de navigation de gauche, puis sélectionnez **Préférences**.

1. Faites défiler l’écran jusqu’à la section **Préférences de stockage**.

1. Dans le champ **Sélectionner les portfolios à convertir en espace de stockage Adobe**, sélectionnez un ou plusieurs portfolios de stockage Workfront hérités.

1. Cliquer sur **Enregistrer**.

   Un message de confirmation s’affiche, décrivant ce qui se produit lorsqu’un portfolio est converti :

   * Vous ne pouvez plus déplacer les projets de stockage Workfront hérités vers le portefeuille.
   * Tous les nouveaux projets créés dans le portefeuille utilisent l’espace de stockage dans le cloud d’Adobe.
   * Frame.io est la visionneuse de documents dans les projets de stockage dans le cloud Adobe du portfolio.
   * Les projets enfants qui utilisent le stockage Workfront hérité restent sur le stockage hérité.
   * Les programmes enfants restent sur l’ancien stockage.

1. Cliquez sur **Convertir** pour confirmer.

   Les portfolios sélectionnés sont convertis en espace de stockage dans le cloud Adobe.
