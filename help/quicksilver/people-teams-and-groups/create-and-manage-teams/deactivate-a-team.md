---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Désactivation d’une équipe
description: Vous pouvez désactiver les équipes que vous n’utilisez plus tout en conservant les données historiques associées. Les administrateurs d’Adobe Workfront peuvent réactiver une équipe à tout moment à partir de la zone Équipes de la configuration.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Désactivation d’une équipe

Vous pouvez désactiver les équipes que vous n’utilisez plus tout en conservant les données historiques associées. [!DNL Adobe Workfront] Les administrateurs peuvent réactiver une équipe à tout moment à partir de la zone Équipes de la configuration. Si vous désactivez une équipe, celle-ci ne s’affiche plus dans les zones suivantes :

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

Les équipes désactivées n’apparaissent pas lorsque vous recherchez une équipe, mais s’affichent toujours dans [!UICONTROL Équipe Accueil] et Autres équipes si l’utilisateur a été affecté à l’équipe avant la désactivation.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan ou le type de licence dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Désactivation d’une équipe

Tout travail assigné à l’équipe avant sa désactivation reste attribué. Il est recommandé de réaffecter le travail avant de désactiver l’équipe.

>[!TIP]
>
>Vous pouvez créer un rapport afin de filtrer les tâches ou les problèmes pour lesquels l’équipe désactivée est toujours affectée.

Lors de l’utilisation des files d’attente de demandes, si vous désactivez une équipe affectée en tant qu’équipe par défaut dans une règle de routage, l’équipe est conservée et les demandes sont toujours acheminées vers l’équipe désactivée. Nous vous recommandons de mettre à jour les règles de routage avec les principales équipes avant de désactiver l’équipe.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Équipes]**.
1. Cliquez sur le bouton **[!DNL Switch team]** , puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.

   ![](assets/edit-team-settings-350x205.png)

1. Effacez la variable **[!UICONTROL Est Principal]** .
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Limites connues

Les équipes désactivées s’affichent dans les zones suivantes :

* Le champ Propriétaire dans [!DNL Workfront Goals]. Cela nécessite une licence supplémentaire pour [!DNL Adobe Workfront Goals]. Pour plus d’informations, voir [Prise en main d’ [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
