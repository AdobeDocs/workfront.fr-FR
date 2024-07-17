---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configurer l’accès aux plans directeurs
description: En tant qu’administrateur système, vous pouvez autoriser les utilisateurs à demander l’installation de plans directeurs en configurant une file d’attente de demandes pour stocker les demandes. Vous disposez là d’un emplacement unique pour effectuer le suivi et mettre à jour les requêtes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 6%

---

# Configurer l’accès aux plans directeurs

Tous les utilisateurs de [!DNL Adobe Workfront] peuvent parcourir le catalogue de plans directeurs.

En tant qu’administrateur système, vous pouvez :

* Ajoutez des [!UICONTROL plans directeurs] au menu principal dans les modèles de mise en page et affectez le modèle de mise en page aux utilisateurs ou aux groupes. Pour plus d’informations, voir [Personnaliser le [!UICONTROL menu principal] à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) et [Affecter des utilisateurs à un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

  >[!NOTE]
  >
  >* Les utilisateurs qui n’ont pas de modèle de mise en page qui leur est attribué verront l’icône [!UICONTROL Blueprints] dans le [!UICONTROL menu principal].
  >* Lorsque vous créez un modèle de mise en page, l’icône [!UICONTROL Blueprints] est incluse par défaut dans la liste [!UICONTROL Éléments actifs] du [!UICONTROL menu principal].


* Activez l’accès pour que les utilisateurs puissent demander l’installation de plans directeurs en configurant une file d’attente de demandes pour stocker les demandes. Vous disposez là d’un emplacement unique pour effectuer le suivi et mettre à jour les requêtes. Pour plus d’informations, suivez la procédure ci-dessous.
* Installez les plans directeurs. Pour plus d’informations, voir [Installation d’un plan directeur](../../administration-and-setup/blueprints/blueprints-install.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe de la licence [!DNL Workfront]</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Conditions préalables {#prerequisites}

* Vous devez utiliser une file d’attente de requêtes existante pour stocker les requêtes de plan directeur. Le projet doit être enregistré en tant que file d’attente des demandes et il doit être à l’état [!UICONTROL Actuel].
* La file d’attente des demandes doit être publique. Dans les détails de la file d’attente des requêtes, &quot;[!UICONTROL Qui peut ajouter des requêtes à cette file d’attente ?]&quot; doit être défini sur **[!UICONTROL Anyone]**.

>[!TIP]
>
>Si vous souhaitez créer une file d’attente de requêtes pour les demandes de plan directeur, vous devez la créer avant de configurer l’accès aux plans directeurs. Pour plus d’informations sur la création d’une file d’attente de requêtes, voir [Création d’une file d’attente de requêtes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Sélectionnez la file d’attente des demandes pour stocker les demandes de plan directeur.

Avant que les utilisateurs puissent demander que vous installez des plans directeurs pour eux, vous devez sélectionner une file d’attente de requêtes pour ces demandes. Tant que la file d’attente des demandes n’est pas définie, les utilisateurs ne peuvent parcourir que le catalogue des plans directeurs.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Blueprints]**.
1. Cliquez sur **[!UICONTROL Configurer les requêtes de plan directeur]** en haut à droite de l’écran du catalogue.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. Dans la boîte de dialogue **[!UICONTROL Configurer les plans directeurs]**, commencez à saisir le nom d’une file d’attente de requêtes active, puis sélectionnez-la lorsqu’elle apparaît dans les résultats de la recherche.

   >[!IMPORTANT]
   >
   >Seules les files d’attente de demandes publiques apparaissent dans cette liste. Pour rendre votre file d’attente de demandes publique, reportez-vous à la section [Conditions préalables](#prerequisites) ci-dessus.

   La préférence de file d’attente des demandes est définie et les utilisateurs peuvent désormais demander l’installation du plan directeur.

   ![Configurer la file d’attente des demandes](assets/Blueprints_access_setup_request_queue.png)

1. (Facultatif) Pour apporter des modifications à la file d’attente de requêtes réelle, cliquez sur **[!UICONTROL Modifier cette file d’attente de requêtes]**.

   Le projet de file d’attente des demandes s’ouvre dans un nouvel onglet du navigateur et vous pouvez le mettre à jour si nécessaire.

1. (Facultatif) Si la file d’attente des requêtes contient des groupes de rubriques ou des rubriques de file d’attente, vous pouvez les sélectionner dans la liste.
1. Pour revenir au catalogue des plans directeurs, cliquez sur **[!UICONTROL Fermer]**.

>[!NOTE]
>
>Lorsque vous installez un plan directeur demandé, vous devez définir l’état du problème sur **[!UICONTROL Fermé]** ou **[!UICONTROL Résolu]** dans la file d’attente des demandes afin que le demandeur soit informé. Pour plus d’informations sur l’installation d’un plan directeur, voir [Installation d’un plan directeur](../../administration-and-setup/blueprints/blueprints-install.md).
