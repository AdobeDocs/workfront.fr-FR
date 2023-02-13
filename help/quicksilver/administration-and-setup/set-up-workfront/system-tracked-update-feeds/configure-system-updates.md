---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configuration des mises à jour du système
description: Workfront génère des mises à jour système automatiques dans le [!UICONTROL Mises à jour] pour enregistrer les modifications que les utilisateurs effectuent sur l’objet. Comme [!DNL Workfront] administrateur, vous pouvez configurer les champs d’objet et les actions [!DNL Workfront] effectue un suivi pour enregistrer les mises à jour du système.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 7%

---

# Configuration des mises à jour du système

[!DNL Adobe Workfront] génère des mises à jour système automatiques dans le [!UICONTROL Mises à jour] pour enregistrer les événements suivants :

* Modifications effectuées par les utilisateurs dans un champ d’objet
* Actions effectuées par les utilisateurs sur un objet

Ces mises à jour du système incluent les modifications apportées, le nom de l’utilisateur qui a apporté la modification, ainsi que l’heure et la date du changement.

Comme [!DNL Workfront] administrateur, vous pouvez configurer les champs d’objet et les actions [!DNL Workfront] effectue un suivi pour enregistrer les mises à jour du système.

Par exemple, vous pouvez avoir [!DNL Workfront] effectuez le suivi de toutes les modifications apportées par les utilisateurs aux noms des problèmes dans l’ensemble du système. Tout changement de nom de problème s’affiche alors comme une mise à jour système du problème [!UICONTROL Mises à jour] zone.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Déterminer les champs [!DNL Workfront] trace un type d’objet

Vous pouvez déterminer les informations [!DNL Workfront] effectue le suivi lorsque les utilisateurs modifient les informations associées à un certain type d’objet dans l’ensemble du [!DNL Workfront] . Pour ce faire, ajoutez ou supprimez les champs de votre choix. [!DNL Workfront] pour effectuer le suivi de ce type d’objet.

>[!NOTE]
>
>* [!DNL Workfront] ne peut pas effectuer de suivi et enregistrer des mises à jour sur les champs personnalisés calculés.
>* Vous pouvez personnaliser la mise à jour du système pour les projets, les tâches, les problèmes, les portefeuilles, les programmes et les utilisateurs. Vous ne pouvez pas personnaliser la mise à jour du système pour les modèles, les documents ou les feuilles de temps, mais [!DNL Workfront] effectue des mises à jour du système d’enregistrement pour ces objets.
>




* [Ajouter les champs de votre choix [!DNL Workfront] pour effectuer le suivi](#add-fields-you-want-workfront-to-track)
* [Supprimer les champs que vous ne souhaitez pas suivre](#remove-fields-that-you-don-t-want-tracked)

### Ajouter les champs de votre choix [!DNL Workfront] pour effectuer le suivi {#add-fields-you-want-workfront-to-track}

Vous pouvez ajouter les champs de votre choix. [!DNL Workfront] pour effectuer le suivi d’un type particulier d’objet dans l’ensemble de la variable [!DNL Workfront] . Lorsque les utilisateurs changent d’informations dans ce champ, [!DNL Workfront] enregistre des informations sur la modification en tant que mise à jour du système dans la variable [!UICONTROL Mises à jour] zone de l’objet.

>[!NOTE]
>
>Vous pouvez effectuer le suivi de 300 champs intégrés et personnalisés dans les flux de mise à jour. Si vous effectuez le suivi du nombre maximal de champs et souhaitez effectuer le suivi de champs supplémentaires qui ne sont pas affichés dans la variable [!UICONTROL Tous les champs] Sous-onglet, vous devez d&#39;abord supprimer certains des champs suivis pour effectuer le suivi des nouveaux champs. Pour plus d’informations sur la suppression de champs des champs de mise à jour, voir [Supprimer les champs que vous ne souhaitez pas suivre](#remove-fields-that-you-don-t-want-tracked).

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Mise à jour de flux]**.

1. &#x200B; Clics **[!UICONTROL Ajouter des champs]**, puis cliquez sur l’objet dont vous souhaitez effectuer le suivi.

1. Dans le &#x200B; **[!UICONTROL Mise à jour de flux]** qui s’affiche, commencez à saisir un champ intégré (standard) ou personnalisé pour l’objet, puis cliquez pour le sélectionner lorsqu’il apparaît dans la liste.

   If [!DNL Workfront] effectue déjà le suivi du champ, vous ne pouvez pas l’ajouter une seconde fois à partir de la liste.

1. Après avoir ajouté tous les champs de votre choix [!DNL Workfront] pour effectuer le suivi, cliquez sur **[!UICONTROL Ajouter des champs]**.

   Les champs intégrés que vous avez ajoutés s’affichent sous le **[!UICONTROL Champs intégrés]** sous-onglet.

   Les champs personnalisés que vous avez ajoutés s’affichent sous **[!UICONTROL Champs personnalisés]** sous-onglet.

   Le **[!UICONTROL Tous les champs]** Le sous-onglet affiche à la fois les champs intégrés et personnalisés qui font l’objet d’un suivi.

### Supprimer les champs que vous ne souhaitez pas suivre {#remove-fields-that-you-don-t-want-tracked}

Vous pouvez supprimer les champs que le système ne souhaite pas suivre pour un type particulier d’objet dans l’ensemble de la variable [!DNL Workfront] .

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Mise à jour de flux]**.

1. Sur le **[!UICONTROL Champs suivis]** , sélectionnez la variable **[!UICONTROL Tous les champs]** sous-onglet.

   Vous affichez ainsi les champs intégrés et personnalisés actuellement suivis.

1. Sélectionnez le champ dont vous souhaitez arrêter le suivi, puis cliquez sur **[!UICONTROL Supprimer]**.

1. Dans le **[!UICONTROL Supprimer le champ]** s’affiche, cliquez sur **[!UICONTROL Oui, Supprimer]** pour confirmer.

Toutes les mises à jour des champs précédemment trackés sont conservées dans la variable [!UICONTROL Mises à jour] zone où elles ont été enregistrées.

## Déterminer les actions [!DNL Workfront] trace un type d’objet

Vous pouvez [!DNL Workfront] effectuer le suivi des actions suivantes que les utilisateurs peuvent effectuer sur les objets dans l’ensemble de la variable [!DNL Workfront] .

Par exemple, vous pouvez avoir [!DNL Workfront] enregistrer une mise à jour chaque fois qu’un utilisateur modifie une affectation en une tâche ou un problème ; La modification s’affiche alors sous la forme d’une mise à jour du système dans la variable [!UICONTROL Mises à jour] zone de la tâche ou du problème.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Action</strong> </th> 
   <th><strong>Objets</strong> </th> 
   <th><strong>Statut principal</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>L'affectation est modifiée</td> 
   <td>Tâches, événements</td> 
   <td> <p>Activé</p> </td> 
  </tr> 
  <tr> 
   <td>La base est supprimée</td> 
   <td>Projets</td> 
   <td> <p>Désactivé</p> </td> 
  </tr> 
  <tr> 
   <td>L’enregistrement de facturation est créé ou supprimé</td> 
   <td>Projets</td> 
   <td> <p>Activé</p> </td> 
  </tr> 
  <tr> 
   <td>Le document est créé ou supprimé</td> 
   <td>Projets, tâches, événements, portefeuilles, programmes</td> 
   <td> <p>Activé</p> </td> 
  </tr> 
  <tr> 
   <td>La dépense est créée ou supprimée</td> 
   <td>Projets, tâches, événements, portefeuilles, programmes</td> 
   <td> <p>Activé</p> </td> 
  </tr> 
  <tr> 
   <td>Le temps est enregistré ou supprimé</td> 
   <td>Projets, tâches, événements</td> 
   <td> <p>Activé</p> </td> 
  </tr> 
  <tr> 
   <td>L'événement est supprimé</td> 
   <td>Projets</td> 
   <td> <p>Activé</p> </td> 
  </tr> 
  <tr> 
   <td>La tâche est supprimée</td> 
   <td>Projets</td> 
   <td> <p>Activé</p> </td> 
  </tr> 
  <tr> 
   <td>L'accès d'un utilisateur est modifié</td> 
   <td>Projets, tâches, événements, documents, portefeuilles, programmes</td> 
   <td> <p>Activé</p> </td> 
  </tr> 
  <tr> 
   <td>Sujet du commentaire sur l'abonnement</td> 
   <td>Projets, tâches, événements</td> 
   <td> <p>Activé</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour configurer les actions que vous souhaitez [!DNL Workfront] pour effectuer le suivi :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Mise à jour de flux]**.

1. Cliquez sur le bouton **[!UICONTROL Actions]** .

1. Sélectionnez une action pour l’activer ou désélectionnez une action pour la désactiver.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

Lorsque vous désactivez une action, toute mise à jour précédemment enregistrée relative à cette action est conservée dans la variable [!UICONTROL Mises à jour] zone d’enregistrement.
