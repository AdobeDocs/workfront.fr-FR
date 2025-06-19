---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurer les mises à jour système
description: Workfront génère des mises à jour système automatiques dans la zone [!UICONTROL Mises à jour] d’un objet pour enregistrer les modifications que les personnes effectuent sur l’objet. En tant qu’administrateur ou administratrice  [!DNL Workfront] , vous pouvez configurer quels champs d’objet et actions sont suivis par  [!DNL Workfront]  pour enregistrer les mises à jour du système.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f7cb314067d105d5534f4be356024aea8e8f9a28
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 50%

---

# Configurer les mises à jour du système

<!-- Audited: 6/2025 -->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div> -->

[!DNL Adobe Workfront] génère des mises à jour système automatiques dans la zone [!UICONTROL Mises à jour] d’un objet pour enregistrer les événements suivants :

* Modifications effectuées par les personnes dans un champ d’objet
* Actions effectuées par les personnes sur un objet

Ces mises à jour du système incluent les types d’informations suivants :

* Le changement qui a été apporté.
* Le nom de l’utilisateur ou l’utilisatrice qui a effectué la modification.
* La date et l’heure de la modification.

Pour plus d’informations sur les mises à jour du système, voir [Mises à jour suivies par le système](../system-tracked-update-feeds/system-tracked-update-feeds.md).

En tant qu’administrateur ou administratrice [!DNL Workfront], vous pouvez configurer quels champs d’objet et actions sont suivis par [!DNL Workfront] pour enregistrer les mises à jour du système.

Par exemple, vous pouvez avoir [!DNL Workfront] qui suit toutes les modifications apportées par les utilisateurs et utilisatrices aux noms des problèmes dans l’ensemble du système. Tout changement de nom de problème s’affiche alors comme une mise à jour système dans la zone [!UICONTROL Mises à jour] du problème.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   Ou
   <p>Actuelle : [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Déterminer les champs suivis par [!DNL Workfront] pour un type d’objet

Vous pouvez déterminer les informations suivies par [!DNL Workfront] lorsque les utilisateurs et utilisatrices modifient les informations associées à un certain type d’objet gràce à l’interface de [!DNL Workfront]. Pour ce faire, ajoutez ou supprimez les champs que vous souhaitez faire suivre par [!DNL Workfront] pour ce type d’objet.

>[!NOTE]
>
>* [!DNL Workfront] ne pouvez pas suivre et enregistrer les mises à jour des champs personnalisés calculés.
>* Vous pouvez personnaliser la mise à jour du système pour les projets, tâches, problèmes, portfolios, programmes, utilisateurs et utilisatrices. Vous ne pouvez pas personnaliser la mise à jour du système pour les modèles, les documents ou les feuilles de temps, mais [!DNL Workfront] enregistre les mises à jour du système pour ces objets.
>


### Ajouter les champs que vous souhaitez faire suivre par [!DNL Workfront] {#add-fields-you-want-workfront-to-track}

Vous pouvez ajouter les champs que vous souhaitez faire suivre par [!DNL Workfront] pour un type particulier d’objet grâce à l’interface de [!DNL Workfront]. Lorsque les utilisateurs changent d’informations dans ce champ, [!DNL Workfront] enregistre des informations sur la modification en tant que mise à jour du système dans la zone [!UICONTROL Mises à jour] de l’objet.

>[!NOTE]
>
>Vous pouvez effectuer le suivi de jusqu’à 300 champs intégrés et personnalisés dans les flux de mise à jour. Si vous suivez le nombre maximal de champs et que vous souhaitez suivre des champs supplémentaires qui ne sont pas affichés dans le sous-onglet [!UICONTROL Tous les champs], vous devez d’abord supprimer certains des champs suivis afin de suivre les nouveaux champs. Pour plus d’informations sur la suppression de champs des champs de mise à jour, voir [Supprimer les champs dont vous ne souhaitez pas le suivi](#remove-fields-you-don-t-want-tracked).

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Interface]**, puis **[!UICONTROL Mettre à jour les flux]**.
1. (Facultatif) Dans l’onglet **Champs suivis**, cliquez sur l’un des sous-onglets suivants, selon les types de champs que vous souhaitez suivre dans le flux de mise à jour :

   * **Champs intégrés** : affiche une liste de champs intégrés.
   * **Champs personnalisés** : affiche une liste de champs personnalisés. Vous devez créer les champs personnalisés avant qu’ils ne soient disponibles dans la liste.
   * **Tous les champs** : affiche une liste de champs intégrés et personnalisés.

1. Cliquez sur **[!UICONTROL Ajouter des champs]**, puis sélectionnez l’objet dont vous souhaitez effectuer le suivi dans la liste déroulante.

   La sélection manuelle des champs n’est pas disponible pour tous les objets qui possèdent une zone Mises à jour.

   Faites votre choix dans les champs des objets suivants :

   * Projet
   * Tâche
   * Problème
   * Portfolio
   * Programme
   * l’utilisateur ou de l’utilisatrice

   La zone **Ajouter des champs** s’ouvre pour chaque objet sélectionné.
1. Dans la zone **Ajouter des champs**, commencez à saisir un champ intégré (standard) ou un champ personnalisé pour l’objet, puis sélectionnez-le lorsqu’il apparaît dans la liste.

   >[!NOTE]
   >
   >Si [!DNL Workfront] effectue déjà le suivi du champ, vous ne pouvez pas l’ajouter une deuxième fois à partir de la liste.

1. Après avoir ajouté tous les champs [!DNL Workfront] suivre, cliquez sur **[!UICONTROL Ajouter des champs]**.
Les champs intégrés que vous avez ajoutés s’affichent sous le sous-onglet **[!UICONTROL Champs intégrés]** et les champs personnalisés s’affichent sous le sous-onglet **[!UICONTROL Champs personnalisés]**.
Le sous-onglet **[!UICONTROL Tous les champs]** affiche les champs intégrés et les champs personnalisés suivis par [!DNL Workfront].

<!-- replace the above when releasing to Preview: 

1. In the panel on the left, click **[!UICONTROL Interface]**, then **[!UICONTROL Update Feeds]**.
1. (Optional) In the <span class="preview">**Tracked fields** tab</span>, click one of the following subtabs, depending on which types of fields you want to track in the update feed:

   * <span class="preview">**Built-in fields**</span>: Displays a list of built-in fields.
   * <span class="preview">**Custom fields**</span>: Displays a list of custom fields. You must create the custom fields before they are available in the list. 
   * <span class="preview">**All fields**</span>: Displays a list of both built-in and custom fields. 

1. Click <span class="preview">**[!UICONTROL Add fields]**,</span> then select the object that you want to be tracked from the drop-down. 

   Manually selecting fields is not available for all the objects that have an Updates area.

   Select from fields for the following objects:

      * Project
      * Task
      * Issue
      * Portfolio
      * Program
      * User

   The <span class="preview">**Add fields** </span> box opens, for each object selected.
1. In the <span class="preview">**Add fields** </span> box, start typing either a built-in (standard) field or a custom field for the object, then select it when it appears in the list.

   >[!NOTE]
   >
   >If [!DNL Workfront] is already tracking the field, you can't add it a second time from the list.

1. After adding all the fields you want [!DNL Workfront] to track, <span class="preview"> click **[!UICONTROL Add]**.
   The built-in fields that you added show under the **[!UICONTROL Built-in fields]** subtab, and the custom fields show under the **[!UICONTROL Custom fields]** subtab.
   The **[!UICONTROL All fields]** subtab shows both the built-in and the custom fields that [!DNL Workfront] tracks.</span>

-->

### Supprimer les champs dont vous ne souhaitez pas le suivi {#remove-fields-you-don-t-want-tracked}

Vous pouvez supprimer des champs dont vous ne souhaitez pas que le système effectue le suivi pour un type d’objet particulier dans l’interface [!DNL Workfront].

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Interface]**, puis sur **[!UICONTROL Mettre à jour les flux]**.

1. Sous l’onglet **[!UICONTROL Champs suivis]**, sélectionnez le sous-onglet **[!UICONTROL Tous les champs]**. Les champs intégrés et personnalisés en cours de suivi s’affichent.

1. Sélectionnez le champ dont vous souhaitez arrêter le suivi, puis cliquez sur le bouton **[!UICONTROL Supprimer]**.


<!--replace above at Preview release with this:

1. On the <span class="preview">**[!UICONTROL Tracked fields]** tab</span>, select the **[!UICONTROL All fields]** subtab. Both the built-in and custom fields that are currently being tracked display.

1. Select the field you want to stop tracking, then click the <span class="preview">**[!UICONTROL Remove]** icon ![Remove icon](assets/remove-icon.png).</span>

-->

1. Dans la case **[!UICONTROL Supprimer le champ]** qui s’affiche, cliquez sur **[!UICONTROL Oui, supprimer]** pour confirmer.

   Toutes les mises à jour des champs précédemment suivis sont conservées dans la zone [!UICONTROL Mises à jour] où elles ont été enregistrées.

## Déterminer les actions suivies par [!DNL Workfront] pour un type d’objet

Vous pouvez demander [!DNL Workfront] suivi des actions que les utilisateurs effectuent sur les objets dans l’interface [!DNL Workfront].

Par exemple, vous pouvez demander [!DNL Workfront] enregistrer une mise à jour chaque fois qu’un utilisateur modifie une affectation en tâche ou en événement.

La modification s’affiche alors sous la forme d’une mise à jour du système dans la zone [!UICONTROL Mises à jour] de la tâche ou du problème.

Le tableau suivant décrit les actions que vous pouvez suivre sur les objets dans [!DNL Workfront] :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Action</strong> </th> 
   <th><strong>Objets</strong> </th> 
   <th><strong>Statut par défaut</strong> </th> 
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
   <td>L’enregistrement de facturation est créé ou supprimé.</td> 
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
   <td>Projets, tâches, problèmes</td> 
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
   <td>Projets, tâches, problèmes</td> 
   <td> <p>Activé</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour configurer les actions que vous souhaitez que [!DNL Workfront] suive, procédez comme suit :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Interface]**, puis sur **[!UICONTROL Mettre à jour les flux]**.

1. Cliquez sur l’onglet **[!UICONTROL Actions]**.

1. Cochez la case d’une action pour l’activer ou désélectionnez-la pour la désactiver.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Lorsque vous désactivez une action, toute mise à jour précédemment enregistrée la concernant est conservée dans la zone [!UICONTROL Mises à jour] où elle a été enregistrée. [!DNL Workfront] arrête d’enregistrer les nouvelles mises à jour de l’action désactivée.
