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
ht-degree: 0%

---

# Configurer l’accès aux plans directeurs

Tous [!DNL Adobe Workfront] les utilisateurs peuvent parcourir le catalogue de plans directeurs.

En tant qu’administrateur système, vous pouvez :

* Ajouter [!UICONTROL Plans directeurs] au menu principal dans les modèles de mise en page et affectez le modèle de mise en page aux utilisateurs ou aux groupes. Pour plus d’informations, voir [Personnalisez le [!UICONTROL Menu Principal] utilisation d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) et [Affecter des utilisateurs à un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   >[!NOTE]
   >
   >* Les utilisateurs auxquels aucun modèle de mise en page n’est affecté verront le [!UICONTROL Plans directeurs] dans le [!UICONTROL Menu Principal].
   >* Lorsque vous créez un modèle de mise en page, la variable [!UICONTROL Plans directeurs] est incluse dans la variable [!UICONTROL Principaux éléments] pour la [!UICONTROL Menu Principal] par défaut.



* Activez l’accès pour que les utilisateurs puissent demander l’installation de plans directeurs en configurant une file d’attente de demandes pour stocker les demandes. Vous disposez là d’un emplacement unique pour effectuer le suivi et mettre à jour les requêtes. Pour plus d’informations, suivez la procédure ci-dessous.
* Installez les plans directeurs. Pour plus d’informations, voir [Installation d’un plan directeur](../../administration-and-setup/blueprints/blueprints-install.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] license</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Conditions préalables {#prerequisites}

* Vous devez utiliser une file d’attente de requêtes existante pour stocker les requêtes de plan directeur. Le projet doit être enregistré en tant que file d’attente des demandes et il doit se trouver dans [!UICONTROL Actuel] statut.
* La file d’attente des demandes doit être publique. Dans les détails de la file d’attente des demandes, &quot;[!UICONTROL Qui peut ajouter des requêtes à cette file d’attente ?]&quot; doit être défini sur **[!UICONTROL Personne]**.

>[!TIP]
>
>Si vous souhaitez créer une file d’attente de requêtes pour les demandes de plan directeur, vous devez la créer avant de configurer l’accès aux plans directeurs. Pour plus d’informations sur la création d’une file d’attente de requêtes, voir [Création d’une file d’attente de requête](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Sélectionnez la file d’attente des demandes pour stocker les demandes de plan directeur.

Avant que les utilisateurs puissent demander que vous installez des plans directeurs pour eux, vous devez sélectionner une file d’attente de requêtes pour ces demandes. Tant que la file d’attente des demandes n’est pas définie, les utilisateurs ne peuvent parcourir que le catalogue des plans directeurs.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Plans directeurs]**.
1. Cliquez sur **[!UICONTROL Configuration des requêtes de plan directeur]** en haut à droite de l’écran catalogue.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. Sur le **[!UICONTROL Configuration des plans directeurs]** , commencez à saisir le nom d’une principale file d’attente de requêtes, puis sélectionnez-la lorsqu’elle apparaît dans les résultats de la recherche.

   >[!IMPORTANT]
   >
   >Seules les files d’attente de demandes publiques apparaissent dans cette liste. Pour rendre votre file d’attente de requêtes publique, voir [Conditions préalables](#prerequisites) ci-dessus.

   La préférence de file d’attente des demandes est définie et les utilisateurs peuvent désormais demander l’installation du plan directeur.

   ![Configuration de la file d’attente des demandes](assets/Blueprints_access_setup_request_queue.png)

1. (Facultatif) Pour apporter des modifications à la file d’attente de requêtes réelle, cliquez sur **[!UICONTROL Modifier cette file d’attente de demandes]**.

   Le projet de file d’attente des demandes s’ouvre dans un nouvel onglet du navigateur et vous pouvez le mettre à jour si nécessaire.

1. (Facultatif) Si la file d’attente des requêtes contient des groupes de rubriques ou des rubriques de file d’attente, vous pouvez les sélectionner dans la liste.
1. Pour revenir au catalogue des plans directeurs, cliquez sur **[!UICONTROL Fermer]**.

>[!NOTE]
>
>Lorsque vous installez un plan directeur demandé, vous devez modifier l’état du problème en **[!UICONTROL Fermé]** ou **[!UICONTROL Résolu]** dans la file d’attente des demandes afin que le demandeur soit informé. Pour plus d’informations sur l’installation d’un plan directeur, voir [Installation d’un plan directeur](../../administration-and-setup/blueprints/blueprints-install.md).
