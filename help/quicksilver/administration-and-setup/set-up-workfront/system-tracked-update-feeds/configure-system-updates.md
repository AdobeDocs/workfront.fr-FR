---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurer les mises à jour système
description: Workfront génère des mises à jour système automatiques dans la zone [!UICONTROL Mises à jour] d’un objet pour enregistrer les modifications que les utilisateurs effectuent sur l’objet. En tant qu'administrateur  [!DNL Workfront] , vous pouvez configurer les champs d'objet et les actions  [!DNL Workfront]  suivis pour enregistrer les mises à jour du système.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 19%

---

# Configurer les mises à jour système

[!DNL Adobe Workfront] génère des mises à jour système automatiques dans la zone [!UICONTROL Updates] d’un objet pour enregistrer les événements suivants :

* Modifications effectuées par les utilisateurs dans un champ d’objet
* Actions effectuées par les utilisateurs sur un objet

Ces mises à jour du système incluent les types d’informations suivants :

* Le changement qui a été apporté
* Nom de l’utilisateur qui a apporté la modification.
* Heure et date de la modification

Pour plus d’informations sur les mises à jour du système, voir [Mises à jour système trackées](../system-tracked-update-feeds/system-tracked-update-feeds.md).

En tant qu&#39;administrateur [!DNL Workfront], vous pouvez configurer les champs d&#39;objet et actions dont [!DNL Workfront] effectue le suivi pour enregistrer les mises à jour du système.

Par exemple, [!DNL Workfront] peut effectuer le suivi de toutes les modifications apportées par les utilisateurs aux noms des problèmes dans l’ensemble du système. Tout changement de nom de problème s’affiche alors comme une mise à jour système de la zone [!UICONTROL Updates] du problème.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Déterminer les champs dont [!DNL Workfront] effectue le suivi pour un type d’objet

Vous pouvez déterminer quelles informations [!DNL Workfront] suivent lorsque les utilisateurs modifient les informations associées à un certain type d’objet dans l’ensemble de l’interface [!DNL Workfront]. Pour ce faire, ajoutez ou supprimez les champs que [!DNL Workfront] doit suivre pour ce type d’objet.

>[!NOTE]
>
>* [!DNL Workfront] ne peut pas effectuer de suivi et enregistrer des mises à jour sur les champs personnalisés calculés.
>* Vous pouvez personnaliser la mise à jour du système pour les projets, tâches, problèmes, portefeuilles, programmes et utilisateurs. Vous ne pouvez pas personnaliser la mise à jour du système pour les modèles, les documents ou les feuilles de temps, mais [!DNL Workfront] enregistre les mises à jour du système pour ces objets.
>



* [Ajouter les champs dont vous souhaitez  [!DNL Workfront]  pour effectuer le suivi](#add-fields-you-want-workfront-to-track)
* [Supprimer les champs que vous ne souhaitez pas suivre](#remove-fields-that-you-don-t-want-tracked)

### Ajoutez les champs dont vous souhaitez effectuer le suivi [!DNL Workfront]. {#add-fields-you-want-workfront-to-track}

Vous pouvez ajouter des champs dont vous souhaitez [!DNL Workfront] le suivi pour un type particulier d’objet dans l’interface [!DNL Workfront]. Lorsque les utilisateurs changent d’informations dans ce champ, [!DNL Workfront] enregistre des informations sur la modification en tant que mise à jour du système dans la zone [!UICONTROL Mises à jour] de l’objet.

>[!NOTE]
>
>Vous pouvez effectuer le suivi de jusqu’à 300 champs intégrés et personnalisés dans les flux de mise à jour. Si vous effectuez le suivi du nombre maximal de champs et souhaitez effectuer le suivi de champs supplémentaires qui ne sont pas affichés dans le sous-onglet [!UICONTROL Tous les champs] , vous devez d’abord supprimer certains des champs suivis pour effectuer le suivi des nouveaux champs. Pour plus d’informations sur la suppression des champs des champs de mise à jour, voir [Suppression de champs que vous ne souhaitez pas suivre](#remove-fields-that-you-don-t-want-tracked).

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Mettre à jour les flux]**.

1. &#x200B; cliquez sur **[!UICONTROL Ajouter des champs]**, puis cliquez sur l’objet dont vous souhaitez effectuer le suivi.

1. Dans la zone &#x200B; **[!UICONTROL Mettre à jour les flux]** qui s’affiche, commencez à saisir un champ intégré (standard) ou personnalisé pour l’objet, puis cliquez pour le sélectionner lorsqu’il apparaît dans la liste.

   Si [!DNL Workfront] effectue déjà le suivi du champ, vous ne pouvez pas l’ajouter une seconde fois à partir de la liste.

1. Après avoir ajouté tous les champs dont vous souhaitez effectuer le suivi sur [!DNL Workfront], cliquez sur **[!UICONTROL Ajouter des champs]**.

   Les champs natifs que vous avez ajoutés s’affichent sous le sous-onglet **[!UICONTROL Champs natifs]** .

   Les champs personnalisés que vous avez ajoutés s’affichent sous le sous-onglet **[!UICONTROL Champs personnalisés]** .

   Le sous-onglet **[!UICONTROL Tous les champs]** affiche à la fois les champs intégrés et personnalisés qui font l’objet d’un suivi.

### Supprimer les champs que vous ne souhaitez pas suivre {#remove-fields-that-you-don-t-want-tracked}

Vous pouvez supprimer les champs que le système ne souhaite pas suivre pour un type particulier d’objet dans l’interface [!DNL Workfront].

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Mettre à jour les flux]**.

1. Dans l’onglet **[!UICONTROL Champs trackés]**, sélectionnez le sous-onglet **[!UICONTROL Tous les champs]** .

   Vous affichez ainsi les champs intégrés et personnalisés actuellement suivis.

1. Sélectionnez le champ dont vous souhaitez arrêter le suivi, puis cliquez sur **[!UICONTROL Supprimer]**.

1. Dans la zone **[!UICONTROL Supprimer le champ]** qui s’affiche, cliquez sur **[!UICONTROL Oui, le supprimer]** pour confirmer.

Toutes les mises à jour des champs précédemment suivis sont conservées dans la zone [!UICONTROL Mises à jour] où elles ont été enregistrées.

## Déterminer quelles actions [!DNL Workfront] effectuent le suivi d&#39;un type d&#39;objet

[!DNL Workfront] peut effectuer le suivi des actions suivantes que les utilisateurs peuvent effectuer sur les objets dans l’interface [!DNL Workfront].

Par exemple, [!DNL Workfront] peut enregistrer et mettre à jour chaque fois qu’un utilisateur modifie une affectation en une tâche ou un problème. La modification s’affiche ensuite comme une mise à jour du système dans la zone [!UICONTROL Mises à jour] pour la tâche ou le problème.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Action</strong> </th> 
   <th><strong>Objets</strong> </th> 
   <th><strong>État par défaut</strong> </th> 
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

Pour configurer les actions dont vous souhaitez [!DNL Workfront] effectuer le suivi :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Mettre à jour les flux]**.

1. Cliquez sur l’onglet **[!UICONTROL Actions]** .

1. Sélectionnez une action pour l’activer ou désélectionnez une action pour la désactiver.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

Lorsque vous désactivez une action, toute mise à jour précédemment enregistrée de cette action est conservée dans la zone [!UICONTROL Mises à jour] où elle a été enregistrée.
