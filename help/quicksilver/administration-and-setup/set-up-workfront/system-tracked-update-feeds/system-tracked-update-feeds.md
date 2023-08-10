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
source-git-commit: 207a8c8a642f3204a2d007789eb7ee8cd9379f1b
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 7%

---

# Mises à jour suivies par le système

[!DNL Adobe Workfront] capture l’activité qui se produit sur certains objets en consignant des informations d’état dans le rapport [!UICONTROL Mises à jour] zone.

La variable [!UICONTROL Mises à jour] comprend les types de mises à jour suivants :

* **Mises à jour de l’utilisateur :** saisie manuellement par les utilisateurs ; On parle également de commentaires, de réponses et de notes.

  Pour plus d’informations sur la configuration des mises à jour des utilisateurs, voir [Configuration des préférences pour les mises à jour des utilisateurs](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Mises à jour système :** Créé automatiquement par le système. Une mise à jour du système comprend une brève note décrivant le type de changement survenu dans l’élément.

  Pour plus d’informations sur les flux de mise à jour du système et leur activation, voir [Configuration des mises à jour du système](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Considérations sur les mises à jour suivies par le système

* Les mises à jour suivies par le système ne sont pas disponibles pour tous les objets disposant de la zone Mises à jour . La variable [!UICONTROL Mises à jour] est disponible pour les objets suivants :

   * [!UICONTROL Projet]
   * [!UICONTROL Tâche]
   * [!UICONTROL Problème]
   * [!UICONTROL Portfolio]
   * [!UICONTROL Programme]
   * [!UICONTROL Utilisateur]
   * [!UICONTROL Modèle]
   * [!UICONTROL Tâche de modèle]
   * [!UICONTROL Équipe]
   * [!UICONTROL Document]
   * [!UICONTROL Feuille de temps]
   * [!UICONTROL Histoire]

     Dans [!DNL Workfront], une histoire est une tâche.
   * [!UICONTROL Itération]
   * [!UICONTROL Objectif]

     Vous devez disposer d’une licence supplémentaire pour avoir accès à la variable [!UICONTROL Objectifs] zone. Pour plus d’informations, voir [Conditions requises pour utiliser les objectifs Workfront](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Carte] sur un panorama

     Pour plus d’informations sur les mises à jour des cartes, voir [Utilisation de cartes connectées sur les panoramas](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] ne suit aucune mise à jour système pour les objets suivants :

   * [!UICONTROL Équipe]
   * [!UICONTROL Modèle]
   * [!UICONTROL Tâche de modèle]
   * Ad hoc [!UICONTROL Carte]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Les utilisateurs peuvent afficher les mises à jour du système par défaut ou choisir de ne pas les afficher.

  Pour plus d’informations sur la désactivation de l’affichage des mises à jour système, voir la section [Activation ou désactivation des mises à jour système](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) dans l’article [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

  >[!NOTE]
  >
  >Nous sommes en train de reconcevoir l’expérience de commentaire et la [!UICONTROL Mises à jour] area dans [!DNL Workfront].
  >
  > Vous ne pouvez pas masquer les mises à jour système lors de l’utilisation de la nouvelle expérience de commentaire.
  > 
  >Pour plus d’informations sur la nouvelle expérience de commentaire, voir [Nouvelle expérience de commentaire](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

* Workfront enregistre les mises à jour suivies par le système pour les objets suivants, mais il n’existe pas d’option pour les désactiver :

   * [!UICONTROL Portfolio]
   * [!UICONTROL Programme]
   * [!UICONTROL Itération]

* [!DNL Workfront] Les administrateurs peuvent définir le type de modifications dont le système doit effectuer le suivi dans la variable [!UICONTROL Mises à jour] zone. Tous les objets qui ont une propriété [!UICONTROL Mises à jour] zone également configurable [!UICONTROL update] flux. Les objets suivants ont une propriété [!UICONTROL Mises à jour] zone qui capture les flux de mise à jour trackés par le système, mais qui ne comporte pas de flux de mise à jour configurables :

   * [!UICONTROL Document]
   * [!UICONTROL Feuille de temps]
   * [!UICONTROL Itération]
   * [!UICONTROL Objectif]


