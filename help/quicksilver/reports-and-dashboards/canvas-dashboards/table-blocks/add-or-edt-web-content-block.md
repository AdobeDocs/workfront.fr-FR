---
title: Ajouter ou modifier un bloc de contenu web dans la zone de travail de reporting
description: Les blocs de contenu web permettent d'afficher dans votre rapport les informations provenant de sites web externes.
hidefromtoc: true
hide: true
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 7%

---

# Ajouter ou modifier un bloc de contenu web dans la zone de travail de reporting

Les blocs de contenu web permettent d&#39;afficher dans votre rapport les informations provenant de sites web externes.

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta du canevas de création de rapports. Pour plus d’informations, reportez-vous à la section [Présentation du canevas de rapports bêta : présentation](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Ajouter ou modifier un bloc de contenu web

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Création de rapports**.
1. Cliquez sur **Nouveau rapport**.

   Ou

   Accédez à un rapport existant, cliquez sur l&#39;icône **Plus** ![](assets/more-icon-27x15.png) dans l&#39;en-tête du rapport, puis cliquez sur **Modifier**.

1. Sur le côté droit de l’écran, sous **Ajouter un bloc**, vous pouvez effectuer l’une des opérations suivantes :

   Faites glisser l’icône **Contenu web** sur la zone de travail directement vers l’emplacement souhaité.

   Ou

   Double-cliquez sur l&#39;icône **Contenu web** pour ajouter un bloc en haut de la zone de travail.

   >[!TIP]
   >
   >Vous pouvez modifier la taille du bloc une fois qu’il a été placé en faisant glisser ses poignées d’angle.

1. Cliquez sur **Contenu web sans titre** dans l’en-tête du bloc, puis tapez le titre du bloc.
1. Cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) dans l’en-tête du bloc.

   ![](assets/web-content-block-header-350x76.png)

1. Dans le panneau **Paramètres** qui s’ouvre, saisissez l’URL complète de la page que vous souhaitez afficher (y compris &quot;https://&quot;) dans le champ **URL** .

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

1. (Facultatif) Cliquez sur le bouton d’activation/désactivation **Pass Parameters** (Transférer des paramètres) pour ouvrir une liste de paramètres de transmission disponibles.

   >[!WARNING]
   >
   >Les paramètres de transfert sont actuellement désactivés.

1. Cliquez sur **Intégrer l&#39;URL** pour enregistrer vos sélections et revenir à votre rapport.
