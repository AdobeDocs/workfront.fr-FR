---
title: Ajouter ou modifier un bloc de contenu web dans la zone de travail de reporting
description: Les blocs de contenu web vous permettent d’afficher des informations provenant de sites web externes directement dans votre rapport.
hidefromtoc: true
hide: true
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 84%

---

# Ajouter ou modifier un bloc de contenu web dans la zone de travail de reporting

Les blocs de contenu web vous permettent d’afficher des informations provenant de sites web externes directement dans votre rapport.

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta de la zone de travail de reporting. Pour plus d’informations, voir [Version bêta de la zone de travail de reporting : vue d’ensemble](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Ajouter ou modifier un bloc de contenu web

1. Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Reporting**.
1. Cliquez sur **Nouveau rapport**.

   Ou

   Dans un rapport existant, cliquez sur l’icône **Plus** ![Plus](assets/more-icon-27x15.png) dans l’en-tête du rapport, puis sur **Modifier**.

1. Sur le côté droit de l’écran, sous **Ajouter un bloc**, effectuez l’une des actions suivantes :

   Faites glisser l’icône **Contenu web** sur la zone de travail directement à l’endroit souhaité.

   Ou

   Double-cliquez sur l’icône **Contenu web** pour ajouter un bloc en haut de la zone de travail.

   >[!TIP]
   >
   >Vous pouvez modifier la taille du bloc une fois qu’il est placé en faisant glisser ses poignées d’angle.

1. Cliquez sur **Contenu web sans titre** dans l’en-tête du bloc, puis saisissez un titre pour le bloc.
1. Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) dans l’en-tête du bloc.

   ![Icône Modifier dans l’en-tête du bloc](assets/web-content-block-header-350x76.png)

1. Dans le panneau **Paramètres** qui s’ouvre, saisissez l’URL complète de la page que vous souhaitez afficher (y compris « https:// ») dans le champ **URL**.

   >[!NOTE]
   >
   >Actuellement, seuls les sites de certains domaines peuvent être affichés. Les domaines qui peuvent actuellement être utilisés sont les suivants :
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com

   Un avertissement s’affiche sous l’URL saisie si elle ne peut pas être intégrée. Ces avertissements comprennent les éléments suivants :

   | Nom de l’avertissement | Raison |
   |---|---|
   | URL non valide | L’URL saisie ne renvoie pas un site valide. |
   | Restrictions concernant le site du fournisseur | Le site que vous essayez d’intégrer n’est pas autorisé. |

   {style="table-layout:auto"}

1. (Facultatif) Cliquez sur le bouton **Paramètres de passage** pour ouvrir une liste des paramètres de passage disponibles.

   >[!WARNING]
   >
   >Les paramètres de passage sont actuellement désactivés.

1. Cliquez sur **Intégrer l’URL** pour enregistrer vos sélections et revenir à votre rapport.
