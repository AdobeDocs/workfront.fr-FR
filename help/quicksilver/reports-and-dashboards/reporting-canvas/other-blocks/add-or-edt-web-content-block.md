---
product-area: reporting
navigation-topic: other-blocks
title: Ajouter ou modifier un bloc de contenu web dans le canevas de création de rapports
description: Les blocs de contenu web permettent d'afficher dans votre rapport les informations provenant de sites web externes.
author: Nolan
feature: Reports and Dashboards
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Ajouter ou modifier un bloc de contenu web dans le canevas de création de rapports

Les blocs de contenu web permettent d&#39;afficher dans votre rapport les informations provenant de sites web externes.

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta du canevas de création de rapports. Pour plus d’informations, voir [Version bêta du canevas de création de rapports : présentation](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Ajouter ou modifier un bloc de contenu web

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Reporting**.
1. Cliquez sur **Nouveau rapport**.

   Ou

   Accédez à un rapport existant, puis cliquez sur le bouton **Plus** icon ![](assets/more-icon-27x15.png) dans l’en-tête du rapport, puis cliquez sur **Modifier**.

1. Dans la partie droite de l’écran, sous **Ajouter un bloc**, soit :

   Faites glisser le **Contenu web** sur la zone de travail, directement à l’emplacement souhaité.

   Ou

   Double-cliquez sur le **Contenu web** pour ajouter un bloc en haut de la zone de travail.

   >[!TIP]
   >
   >Vous pouvez modifier la taille du bloc une fois qu’il a été placé en faisant glisser ses poignées d’angle.

1. Cliquez sur **Contenu web sans titre** dans l’en-tête de bloc, saisissez le titre du bloc.
1. Cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png) dans l’en-tête block.

   ![](assets/web-content-block-header-350x76.png)

1. Dans le **Paramètres** qui s’ouvre, saisissez l’URL complète de la page que vous souhaitez afficher (y compris &quot;https://&quot;) dans le **URL** champ .

   >[!NOTE]
   >
   >Actuellement, seuls les sites de certains domaines peuvent être affichés. Les domaines qui peuvent actuellement être utilisés sont les suivants :
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com

   Un avertissement s’affiche sous l’URL saisie s’il n’est pas possible de l’incorporer. Ces avertissements sont les suivants :

   | Nom de l’avertissement | Motif |
   |---|---|
   | URL non valide | L’URL saisie ne renvoie pas de site valide. |
   | Restrictions du site du fournisseur | Le site que vous essayez d’incorporer n’est pas autorisé. |

   {style="table-layout:auto"}

1. (Facultatif) Cliquez sur le **Transmission des paramètres** pour ouvrir une liste de paramètres de transmission disponibles.

   >[!WARNING]
   >
   >Les paramètres de transfert sont actuellement désactivés.

1. Cliquez sur **Incorporer l’URL** pour enregistrer vos sélections et revenir à votre rapport.
