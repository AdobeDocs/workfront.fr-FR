---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configurer l’accès aux plans directeurs
description: En tant qu’administrateur ou administratrice système, vous pouvez autoriser les utilisateurs et utilisatrices à demander l’installation de plans directeurs en configurant une file d’attente de demandes pour stocker les demandes. Vous disposez d’un emplacement unique pour effectuer le suivi et la mise à jour des demandes.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 99%

---

# Configurer l’accès aux plans directeurs

Tous les utilisateurs et utilisatrices [!DNL Adobe Workfront] peuvent parcourir le catalogue de plans directeurs.

En tant qu’administrateur ou administratrice système, vous pouvez :

* Ajouter des [!UICONTROL Plans directeurs] au menu principal dans les modèles de disposition et attribuer le modèle de mise en page à des utilisateurs et utilisatrices ou à des groupes. Pour plus d’informations, voir [Personnaliser le [!UICONTROL menu principal] à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) et [Affecter des utilisateurs et utilisatrices à un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

  >[!NOTE]
  >
  >* Les utilisateurs et utilisatrices auxquels aucun modèle de mise en page n’est affecté verront l’icône [!UICONTROL Plans directeurs] dans le [!UICONTROL menu principal].
  >* Lorsque vous créez un modèle de mise en page, l’icône [!UICONTROL Plans directeurs] est incluse dans la liste [!UICONTROL Éléments actifs] du [!UICONTROL menu principal] par défaut.


* Autorisez les utilisateurs et utilisatrices à demander l’installation de plans directeurs en configurant une file d’attente de demandes pour stocker les demandes. Vous disposez d’un emplacement unique pour effectuer le suivi et la mise à jour des demandes. Pour plus d’informations, suivez la procédure ci-dessous.
* Installez des plans directeur. Pour plus d’informations, voir [Installer un plan directeur](../../administration-and-setup/blueprints/blueprints-install.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Vous devez être administrateur ou administratrice [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir la section [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables {#prerequisites}

* Vous devez utiliser une file d’attente de demandes existante pour stocker les demandes de plan directeur. Le projet doit être enregistré en tant que file d’attente des demandes et il doit avoir le statut [!UICONTROL Actuel].
* La file d’attente des demandes doit être publique. Dans les détails de la file d’attente des demandes, « [!UICONTROL Qui peut ajouter des demandes à cette file d’attente ?] » doit être défini sur **[!UICONTROL N’importe qui]**.

>[!TIP]
>
>Si vous souhaitez créer une file d’attente des demandes pour les demandes de plan directeur, vous devez la créer avant de configurer l’accès aux plans directeurs. Pour plus d’informations sur la création d’une file d’attente des demandes, voir [Créer une file d’attente des demandes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Sélectionner la file d’attente des demandes pour stocker les demandes de plan directeur

Avant que les utilisateurs et utilisatrices puissent vous demander de leur installer des plans directeurs, vous devez sélectionner une file d’attente pour ces demandes. Tant que la file d’attente des demandes n’est pas définie, les utilisateurs et utilisatrices peuvent uniquement parcourir le catalogue des plans directeurs.

{{step1-to-blueprints}}

1. Cliquez sur **[!UICONTROL Configurer les demandes de plan directeur]** en haut à droite de l’écran du catalogue.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. Dans la boîte de dialogue **[!UICONTROL Configurer les plans directeurs]**, commencez à saisir le nom d’une file d’attente des demandes active, puis sélectionnez-la lorsqu’elle apparaît dans les résultats de la recherche.

   >[!IMPORTANT]
   >
   >Seules les files d’attente des demandes publiques apparaissent dans cette liste. Pour rendre votre file d’attente des demandes publique, voir la section [Conditions préalables](#prerequisites) ci-dessus.

   La préférence de file d’attente des demandes est définie et les utilisateurs et utilisatrices peuvent désormais demander l’installation du plan directeur.

   ![Configurer une file d’attente des demandes](assets/Blueprints_access_setup_request_queue.png)

1. (Facultatif) Pour apporter des modifications à la file d’attente des demandes actuelle, cliquez sur **[!UICONTROL Modifier cette file d’attente des demandes]**.

   Le projet de file d’attente des demandes s’ouvre dans un nouvel onglet du navigateur et vous pouvez le mettre à jour si nécessaire.

1. (Facultatif) Si la file d’attente des demandes contient des groupes de sujets ou des rubriques de file d’attente, vous pouvez les sélectionner dans la liste.
1. Pour revenir au catalogue des plans directeurs, cliquez sur **[!UICONTROL Fermer]**.

>[!NOTE]
>
>Lorsque vous installez un plan directeur qui vous a été demandé, vous devez remplacer le statut du problème par **[!UICONTROL Fermé]** ou **[!UICONTROL Résolu]** dans la file d’attente des demandes afin que la personne qui a fait la demande soit informée. Pour plus d’informations sur l’installation d’un plan directeur, voir [Installer un plan directeur](../../administration-and-setup/blueprints/blueprints-install.md).
