---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurer les mises à jour du système
description: Workfront génère des mises à jour système automatiques dans la zone [!UICONTROL Mises à jour] d’un objet pour enregistrer les modifications que les personnes effectuent sur l’objet. En tant qu’administrateur ou administratrice  [!DNL Workfront] , vous pouvez configurer quels champs d’objet et actions sont suivis par  [!DNL Workfront]  pour enregistrer les mises à jour du système.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 100%

---

# Configurer les mises à jour du système

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

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être administrateur ou administratrice de [!DNL Workfront].</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice de [!DNL Workfront] s’il ou elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Déterminer les champs suivis par [!DNL Workfront] pour un type d’objet

Vous pouvez déterminer les informations suivies par [!DNL Workfront] lorsque les utilisateurs et utilisatrices modifient les informations associées à un certain type d’objet gràce à l’interface de [!DNL Workfront]. Pour ce faire, ajoutez ou supprimez les champs que vous souhaitez faire suivre par [!DNL Workfront] pour ce type d’objet.

>[!NOTE]
>
>* [!DNL Workfront] ne peut pas effectuer de suivi et enregistrer des mises à jour sur les champs personnalisés calculés.
>* Vous pouvez personnaliser la mise à jour du système pour les projets, tâches, problèmes, portfolios, programmes, utilisateurs et utilisatrices. Vous ne pouvez pas personnaliser la mise à jour du système pour les modèles, documents ou feuilles de temps, mais [!DNL Workfront] effectue des mises à jour du système d’enregistrement pour ces objets.
>



* [Ajouter les champs que vous souhaitez faire suivre par  [!DNL Workfront] ](#add-fields-you-want-workfront-to-track)
* [Supprimer les champs que vous ne souhaitez pas suivre](#remove-fields-that-you-don-t-want-tracked)

### Ajouter les champs que vous souhaitez faire suivre par [!DNL Workfront] {#add-fields-you-want-workfront-to-track}

Vous pouvez ajouter les champs que vous souhaitez faire suivre par [!DNL Workfront] pour un type particulier d’objet grâce à l’interface de [!DNL Workfront]. Lorsque les utilisateurs changent d’informations dans ce champ, [!DNL Workfront] enregistre des informations sur la modification en tant que mise à jour du système dans la zone [!UICONTROL Mises à jour] de l’objet.

>[!NOTE]
>
>Vous pouvez effectuer le suivi de jusqu’à 300 champs intégrés et personnalisés dans les flux de mise à jour. Si vous effectuez le suivi du nombre maximal de champs et souhaitez effectuer le suivi de champs supplémentaires qui ne sont pas affichés dans le sous-onglet [!UICONTROL Tous les champs], vous devez d&#39;abord supprimer certains des champs suivis pour effectuer le suivi des nouveaux champs. Pour plus d’informations sur la suppression de champs des champs de mise à jour, voir [Supprimer les champs que vous ne souhaitez pas suivre](#remove-fields-that-you-don-t-want-tracked).

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Flux de mises à jour]**.

1. Cliquez sur **[!UICONTROL Ajouter des champs]**, puis cliquez sur l’objet dont vous souhaitez effectuer le suivi.

1. Dans la boîte **[!UICONTROL Flux de mises à jour]** qui s’affiche, commencez à saisir un champ intégré (standard) ou personnalisé pour l’objet, puis cliquez pour le sélectionner lorsqu’il apparaît dans la liste.

   Si [!DNL Workfront] effectue déjà le suivi du champ, vous ne pouvez pas l’ajouter une seconde fois à partir de la liste.

1. Après avoir ajouté tous les champs que vous souhaitez faire suivre par [!DNL Workfront], cliquez sur **[!UICONTROL Ajouter des champs]**.

   Les champs intégrés que vous avez ajoutés s’affichent dans le sous-onglet **[!UICONTROL Champs intégrés]**.

   Les champs personnalisés que vous avez ajoutés s’affichent dans le sous-onglet **[!UICONTROL Champs personnalisés]**.

   Le sous-onglet **[!UICONTROL Tous les champs]** affiche à la fois les champs intégrés et personnalisés qui font l’objet d’un suivi.

### Supprimer les champs que vous ne souhaitez pas suivre {#remove-fields-that-you-don-t-want-tracked}

Vous pouvez supprimer les champs que vous ne voulez pas faire suivre par le système pour un type particulier d’objet grâce à l’interface de [!DNL Workfront].

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Mettre à jour les flux]**.

1. Sur l’onglet **[!UICONTROL Champs suivis]**, sélectionnez le sous-onglet **[!UICONTROL Tous les champs]**.

   Vous affichez ainsi les champs intégrés et personnalisés actuellement suivis.

1. Sélectionnez le champ dont vous souhaitez arrêter le suivi, puis cliquez sur **[!UICONTROL Supprimer]**.

1. Dans la case **[!UICONTROL Supprimer le champ]** qui s’affiche, cliquez sur **[!UICONTROL Oui, supprimer]** pour confirmer.

Toutes les mises à jour des champs précédemment suivis sont conservées dans la zone [!UICONTROL Mises à jour] où elles ont été enregistrées.

## Déterminer les actions suivies par [!DNL Workfront] pour un type d’objet

Vous pouvez demander à [!DNL Workfront] de suivre les actions suivantes que les personnes peuvent effectuer sur les objets dans l’ensemble de l’interface [!DNL Workfront].

Par exemple, vous pouvez demander à [!DNL Workfront] d’enregistrer une mise à jour chaque fois qu’une personne modifie une affectation sur une tâche ou un problème. La modification s’affiche alors sous la forme d’une mise à jour du système dans la zone [!UICONTROL Mises à jour] de la tâche ou du problème.

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

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Interface]** > **[!UICONTROL Mettre à jour les flux]**.

1. Cliquez sur l’onglet **[!UICONTROL Actions]**.

1. Sélectionnez une action pour l’activer ou désélectionnez une action pour la désactiver.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

Lorsque vous désactivez une action, toute mise à jour précédemment enregistrée relative à cette action est conservée dans la zone [!UICONTROL Mises à jour] ou elle a été enregistrée.
