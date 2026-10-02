---
user-type: administrator
product-area: system-administration;setup
title: Configurer la localisation personnalisée
description: La localisation personnalisée vous permet de définir des termes et expressions personnalisés dans différentes langues. Workfront affiche ensuite ces termes dans la langue définie dans les paramètres du navigateur.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: b077c95d8bb795fcd7c0983c78b7533cb8167270
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 18%
---
# Configurer la localisation personnalisée

{{highlighted-preview}}

La localisation personnalisée vous permet d’utiliser <span class="preview"> l’IA</span> pour définir des termes et des expressions personnalisés dans différentes langues. Workfront affiche ensuite ces termes dans la langue définie dans les paramètres Adobe Identity Management (IMS) de l’utilisateur.

Par exemple, le libellé « Public cible » peut être localisé sur le mot allemand « Zielgruppe ». Tout utilisateur dont la langue principale du navigateur est l’allemand voit le mot « Zielgruppe » comme libellé pour tout champ intitulé « Public cible » en anglais.

Vous pouvez configurer les traductions dans plusieurs langues. Les langues actuellement disponibles sont les suivantes :

* Chinois (traditionnel)
* Chinois (simplifié)
* Français
* Allemand
* Italien
* Japonais
* Coréen
* Portugais (Brésil)
* Espagnol

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Workflow Prime ou version ultérieure </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront pour configurer les traductions.</p>  </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant la définition de la localisation

Tenez compte des points suivants lors de la configuration de la localisation :

* Vous pouvez configurer un terme pour qu’il soit traduit dans plusieurs langues.
* La localisation s’applique aux libellés de champ personnalisés (y compris lorsqu’ils sont utilisés comme en-tête de colonne) et aux info-bulles.
* La localisation personnalisée peut s’appliquer aux messages générés à partir de règles métier, mais doit être activée dans la règle métier.

  Pour obtenir des instructions, voir [Activer la localisation dans une règle métier](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules) dans l’article Créer et modifier des règles métier.

## Configuration des traductions

Les traductions sont configurées dans la zone Configuration.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Dans la zone Configuration, cliquez sur **Localisation** dans le panneau de navigation de gauche.
1. Pour ajouter une nouvelle traduction, cliquez sur **Nouvelle ligne**.
1. Dans la colonne **Anglais**, saisissez le terme anglais qui doit être traduit.
1. Dans la colonne correspondant à la langue dans laquelle le terme doit être traduit, entrez le terme dans la langue cible.
1. (Facultatif) Pour traduire le mot dans d’autres langues, ajoutez la traduction dans la colonne de langue appropriée.
1. (Facultatif) Pour réorganiser les colonnes de langue, cliquez sur l’en-tête d’une colonne à déplacer et faites-la glisser à l’emplacement souhaité.
1. (Facultatif) Pour supprimer des traductions d’un terme, cochez la case en regard du terme, puis cliquez sur **Supprimer** dans la barre bleue en bas de la page.

<div class="preview">

## Localiser du texte personnalisé non traduit à l’aide de traductions IA

Vous pouvez utiliser l’IA pour localiser du texte personnalisé. Vous sélectionnez le terme et les langues, et pouvez approuver les traductions avant leur application.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Dans la zone Configuration, cliquez sur **Localisation** dans le panneau de navigation de gauche.
1. Dans la zone Localisation , sélectionnez l’onglet **Texte personnalisé non traduit**.

   Une liste de texte personnalisé non traduit s’affiche. Cela inclut du texte tel que des libellés de champ et des messages de règle personnalisés.

1. Sélectionnez un ou plusieurs termes à localiser.
1. Dans la barre bleue située en bas de l’écran, sélectionnez **Traduire avec l’IA**.

   La fenêtre Générer les traductions s&#39;ouvre.

1. Cliquez sur les langues dans lesquelles traduire le ou les termes. Pour sélectionner rapidement toutes les langues, cliquez sur **Tout sélectionner**.
1. (Facultatif) Pour fournir des conseils plus spécifiques pour la traduction, saisissez des instructions dans le champ « Instructions pour l’IA ».
1. Cliquez sur **Générer**.

   L’IA commence à générer des traductions.

   La fenêtre Vérifier les traductions s’ouvre.

1. (Facultatif) Pour ajuster des traductions ou ajouter votre propre traduction, cliquez dans le carré approprié du tableau, puis saisissez la traduction souhaitée.
1. Cliquer sur **Enregistrer**.

## Traduire un terme localisé dans d’autres langues

Vous pouvez traduire un terme précédemment localisé dans de nouvelles langues à l’aide de l’IA ou fournir votre propre traduction.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Dans la zone Configuration, cliquez sur **Localisation** dans le panneau de navigation de gauche.
1. Dans la zone Localisation , sélectionnez l’onglet **Traductions**.

   Une liste des termes précédemment traduits et de leurs traductions s’affiche.

1. (Facultatif) Pour modifier ou saisir directement une traduction, cliquez sur la zone appropriée dans le tableau et saisissez la traduction souhaitée.
1. Sélectionnez les termes pour lesquels vous souhaitez générer des traductions supplémentaires en cochant les cases en regard de ces termes.
1. Dans la barre bleue située en bas de la page, cliquez sur **Remplir avec l’IA**.


   La fenêtre Générer les traductions s&#39;ouvre.

1. Cliquez sur les langues dans lesquelles traduire le ou les termes. Pour sélectionner rapidement toutes les langues, cliquez sur **Tout sélectionner**.
1. (Facultatif) Pour fournir des conseils plus spécifiques pour la traduction, saisissez des instructions dans le champ « Instructions pour l’IA ».
1. Cliquez sur **Générer**.

   L’IA commence à générer des traductions.

   La fenêtre Vérifier les traductions s’ouvre.

1. (Facultatif) Pour ajuster des traductions ou ajouter votre propre traduction, cliquez dans le carré approprié du tableau, puis saisissez la traduction souhaitée.
1. Cliquer sur **Enregistrer**.
1. (Facultatif) Pour supprimer toutes les traductions d’un terme, cochez la case en regard du terme, puis cliquez sur **Supprimer** dans la barre bleue en bas de la page.


</div>
