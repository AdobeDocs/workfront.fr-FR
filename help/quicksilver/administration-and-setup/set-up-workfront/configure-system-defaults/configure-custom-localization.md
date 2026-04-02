---
user-type: administrator
product-area: system-administration;setup
title: Configurer la localisation personnalisée
description: La localisation personnalisée vous permet de définir des termes et expressions personnalisés dans différentes langues. Workfront affiche ensuite ces termes dans la langue définie dans les paramètres du navigateur.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 18211a3529b612a6fcdcedf7820aecfe38cb3b6f
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 19%

---

# Configurer la localisation personnalisée

La localisation personnalisée vous permet de définir des termes et expressions personnalisés dans différentes langues. Workfront affiche ensuite ces termes dans la langue définie dans les paramètres Adobe Identity Management (IMS) de l’utilisateur. Si l’utilisateur ou l’utilisatrice n’utilise pas Adobe IMS, les termes s’affichent dans la langue définie dans les paramètres du navigateur de l’utilisateur ou de l’utilisatrice.

Par exemple, vous pouvez définir le libellé « Public cible » à traduire par le mot allemand « Zielgruppe ». Tout utilisateur dont la langue principale du navigateur est l’allemand voit le mot « Zielgruppe » comme libellé pour tout champ intitulé « Public cible » en anglais.

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
1. Pour traduire le mot dans d’autres langues, ajoutez la traduction dans la colonne de langue appropriée.
1. Pour réorganiser les colonnes de langue, cliquez sur l’en-tête d’une colonne à déplacer et faites-la glisser à l’emplacement souhaité.
