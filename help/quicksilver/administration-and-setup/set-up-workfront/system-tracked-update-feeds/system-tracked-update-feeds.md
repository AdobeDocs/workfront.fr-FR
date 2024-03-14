---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Mises à jour suivies par le système
description: Adobe Workfront capture l’activité qui se produit sur certains objets en consignant les informations d’état dans le rapport [!UICONTROL Mises à jour] zone.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: c50ff48bbc492199b39db17b8c445207209bb6a5
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Mises à jour suivies par le système

{{preview-and-fast-release}}

<!--remove new experience and legacy notes when we remove legacy in the UI - Jan 24???-->

[!DNL Adobe Workfront] capture l’activité qui se produit sur certains objets en consignant des informations d’état dans le rapport [!UICONTROL Mises à jour] zone.

La variable [!UICONTROL Mises à jour] comprend les types de mises à jour suivants :

* **Mises à jour de l’utilisateur :** saisie manuellement par les utilisateurs ; On parle également de commentaires, de réponses et de notes.

  Pour plus d’informations sur la configuration des mises à jour des utilisateurs, voir [Configuration des préférences pour les mises à jour des utilisateurs](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Mises à jour système :** Créé automatiquement par le système. Une mise à jour du système comprend une brève note décrivant le type de changement survenu dans l’élément.

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

* Voici les différences entre la nouvelle expérience et l’expérience de commentaire héritée :

   * Lors de l’utilisation de la nouvelle expérience de commentaire, les mises à jour de l’utilisateur s’affichent dans l’onglet Commentaires et les mises à jour du système s’affichent dans l’activité système. <span class="preview">et l’ensemble</span> onglets.

     Pour plus d’informations sur la nouvelle expérience de commentaire, voir [Nouvelle expérience de commentaire](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

   * <span class="preview">Lorsque vous utilisez la nouvelle expérience de commentaire, vous ne pouvez pas ajouter de commentaire à une mise à jour du système. Toutefois, toutes les réponses apportées aux enregistrements d’activité système dans l’expérience de commentaire héritée sont renseignées sur l’onglet Activité système en tant que lecture seule dans la nouvelle expérience de commentaire.</span>
   * Lors de l’utilisation de l’expérience de commentaire héritée, les mises à jour du système et de l’utilisateur s’affichent dans un flux continu.

   * Lors de l’utilisation de l’expérience de commentaire héritée, les utilisateurs peuvent afficher les mises à jour système par défaut ou choisir de ne pas les afficher. La désactivation des mises à jour du système n’est pas possible lors de l’utilisation de la nouvelle expérience de commentaire.

     Pour plus d’informations sur la désactivation de l’affichage des mises à jour système, voir la section [Activation ou désactivation des mises à jour système](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) dans l’article [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Workfront enregistre les mises à jour suivies par le système pour les objets suivants, mais il n’existe pas d’option pour les désactiver :

   * [!UICONTROL Portfolio]
   * [!UICONTROL Programme]
   * [!UICONTROL Itération]

* [!DNL Workfront] Les administrateurs peuvent définir le type de modifications dont le système doit effectuer le suivi dans la variable [!UICONTROL Mises à jour] zone. Tous les objets qui ont une propriété [!UICONTROL Mises à jour] zone également configurable [!UICONTROL update] flux. Les objets suivants ont une propriété [!UICONTROL Mises à jour] zone qui capture les flux de mise à jour trackés par le système, mais qui ne comporte pas de flux de mise à jour configurables :

   * [!UICONTROL Document]
   * [!UICONTROL Feuille de calcul]
   * [!UICONTROL Itération]
   * [!UICONTROL Objectif]


