---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Désactiver une équipe
description: Vous pouvez désactiver les équipes que vous n’utilisez plus tout en conservant les données historiques associées. Les administrateurs d’Adobe Workfront peuvent réactiver une équipe à tout moment à partir de la zone Équipes de la configuration.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 11%

---

# Désactiver une équipe

Vous pouvez désactiver les équipes que vous n’utilisez plus tout en conservant les données historiques associées. Les administrateurs de [!DNL Adobe Workfront] peuvent réactiver une équipe à tout moment à partir de la zone Équipes de la configuration. Si vous désactivez une équipe, celle-ci ne s’affiche plus dans les zones suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Champs de saisie anticipée dans les formulaires personnalisés</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Boîte de dialogue de partage pour les objets</p> </li> 
     <li> <p>[!UICONTROL User Profile]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Menu déroulant de sélection principal dans la zone [!UICONTROL Équipes]</p> </li> 
     <li> <p>Type de commande [!UICONTROL Affectations]</p> </li> 
     <li> <p>Boîte de dialogue du panorama [!UICONTROL Ajouter à Kanban] dans un projet</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Les équipes désactivées n’apparaissent pas lorsque vous recherchez une équipe, mais s’affichent toujours dans [!UICONTROL Home Team] et dans d’autres équipes si l’utilisateur a été affecté à l’équipe avant la désactivation.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir quel plan ou type de licence vous avez, contactez votre administrateur [!DNL Workfront].

## Désactiver une équipe

Tout travail assigné à l’équipe avant sa désactivation reste attribué. Il est recommandé de réaffecter le travail avant de désactiver l’équipe.

>[!TIP]
>
>Vous pouvez créer un rapport afin de filtrer les tâches ou les problèmes pour lesquels l’équipe désactivée est toujours affectée.

Lors de l’utilisation des files d’attente de demandes, si vous désactivez une équipe affectée en tant qu’équipe par défaut dans une règle de routage, l’équipe est conservée et les demandes sont toujours acheminées vers l’équipe désactivée. Nous vous recommandons de mettre à jour les règles de routage avec les équipes actives avant de désactiver l’équipe.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Equipes]**.
1. Cliquez sur l’icône **[!DNL Switch team]**, puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Modifier]**.

   ![](assets/edit-team-settings-350x205.png)

1. Décochez la case **[!UICONTROL Est actif]** .
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Limites connues

Les équipes désactivées s’affichent dans les zones suivantes :

* Le champ Propriétaire dans [!DNL Workfront Goals]. Cela nécessite une licence supplémentaire pour [!DNL Adobe Workfront Goals]. Pour plus d’informations, voir [Prise en main de [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
