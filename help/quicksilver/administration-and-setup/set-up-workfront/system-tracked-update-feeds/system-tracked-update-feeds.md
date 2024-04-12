---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Mises à jour suivies par le système
description: Adobe Workfront capture l’activité qui se produit sur certains objets en consignant les informations d’état dans le rapport [!UICONTROL Mises à jour] zone.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Mises à jour suivies par le système

<!-- Audited: April, 2024-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>-->

[!DNL Adobe Workfront] capture l’activité qui se produit sur certains objets en consignant des informations d’état dans le rapport [!UICONTROL Mises à jour] .

Pour plus d’informations sur la section Mises à jour, voir [Présentation de la section Mises à jour](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

La variable [!UICONTROL Mises à jour] comprend les types de mises à jour suivants :

* **Mises à jour de l’utilisateur :** saisie manuellement par les utilisateurs ; On parle également de commentaires, de réponses et de notes. Les mises à jour des utilisateurs s’affichent dans les onglets Commentaires et Tous de la section Mises à jour d’un objet.

  Pour plus d’informations sur la configuration des mises à jour des utilisateurs, voir [Configuration des préférences pour les mises à jour des utilisateurs](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Mises à jour système :** Créé automatiquement par le système. Une mise à jour du système comprend une brève note décrivant le type de changement survenu dans l’élément. Les mises à jour système s’affichent dans l’activité système et dans les onglets Toutes de la section Mises à jour d’un objet.

  Pour plus d’informations sur les flux de mise à jour du système et leur activation, voir [Configuration des mises à jour du système](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Considérations sur les mises à jour suivies par le système

Les mises à jour suivies par le système ne sont pas disponibles pour tous les objets disposant de la zone Mises à jour .

* La variable [!UICONTROL Mises à jour] est disponible pour les objets suivants :

   * [!UICONTROL Projet]
   * [!UICONTROL Tâche]
   * [!UICONTROL Problème]
   * [!UICONTROL Portfolio]
   * [!UICONTROL Programme]
   * [!UICONTROL Utilisateur]
   * [!UICONTROL Modèle]
   * [!UICONTROL Tâche du modèle]
   * [!UICONTROL Équipe]
   * [!UICONTROL Document]
   * [!UICONTROL Feuille de calcul]
   * [!UICONTROL Histoire]

     Dans [!DNL Workfront], une histoire est une tâche.
   * [!UICONTROL Itération]
   * [!UICONTROL Objectif]

     Vous devez disposer d’une licence supplémentaire pour avoir accès à la variable [!UICONTROL Objectifs] zone. Pour plus d’informations, voir [Conditions requises pour utiliser les objectifs Workfront](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Carte] sur un panorama

     Pour plus d’informations sur les mises à jour des cartes, voir [Utilisation de cartes connectées sur les panoramas](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] ne suit pas les mises à jour système pour les objets suivants :

   * [!UICONTROL Équipe]
   * [!UICONTROL Modèle]
   * [!UICONTROL Tâche du modèle]
   * Ad hoc [!UICONTROL Carte]
   * [!UICONTROL Itérations]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Les mises à jour des utilisateurs s’affichent dans l’onglet Commentaires et les mises à jour système s’affichent dans l’activité système et dans les onglets Tous .

  Pour obtenir la liste des objets ne disposant pas des onglets Activité système ou Tous, voir [Mise à jour de la section - Aperçu](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)

* Vous ne pouvez pas ajouter de réponse à une mise à jour du système. Toutefois, toutes les réponses apportées aux enregistrements d’activité du système dans l’expérience de commentaire héritée avant le 11 avril 2024 sont renseignées en lecture seule dans l’onglet Activité du système.

<!--
* The following are differences between the new and the legacy commenting experience: 

   * When using the new commenting experience, user updates display in the Comments tab and system updates display in the System Activity <span class="preview">and the All</span> tabs.  

      For more information about the new commenting experience, see [New commenting experience](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

      <span class="preview">For a list of objects that do not have the System Activity or the All tabs, see [Update section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)</span>

   * <span class="preview">When using the new commenting experience, you cannot add a comment to a system update. However, any replies made to system activity records in the legacy commenting experience are populated on the System Activity tab as read-only in the new commenting experience.</span>
   * When using the legacy commenting experience, the system and user updates display in one continuous feed. 

   * When using the legacy commenting experience, users can view system updates by default or they can choose to not display them. Disabling system updates is not possible when using the new commenting experience. 

      For information about disabling the display of system updates, see the section [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) in the article [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).  

   * <span class="preview">The legacy commenting experience has been disabled in the Preview environment. For more information, see [Second Quarter 2024 Update stream and notification enhancements](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md).</span>
-->

* [!DNL Workfront] Les administrateurs peuvent définir le type de modifications dont le système doit effectuer le suivi dans la variable [!UICONTROL Mises à jour] zone. Tous les objets qui ont une propriété [!UICONTROL Mises à jour] zone également configurable [!UICONTROL update] flux. Les objets suivants ont une propriété [!UICONTROL Mises à jour] zone qui capture les flux de mise à jour trackés par le système, mais qui ne comporte pas de flux de mise à jour configurables :

   * [!UICONTROL Document]
   * [!UICONTROL Feuille de calcul]
   * [!UICONTROL Itération]
   * [!UICONTROL Objectif]


