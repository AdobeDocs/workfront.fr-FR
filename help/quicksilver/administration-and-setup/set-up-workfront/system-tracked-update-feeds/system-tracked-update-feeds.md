---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Mises à jour suivies par le système
description: Adobe Workfront capture l’activité qui se produit sur certains objets en consignant les informations d’état dans le rapport [!UICONTROL Mises à jour] zone.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 5%

---

# Mises à jour suivies par le système

[!DNL Adobe Workfront] capture l’activité qui se produit sur certains objets en consignant des informations d’état dans le rapport [!UICONTROL Mises à jour] zone.

Le [!UICONTROL Mises à jour] comprend les types de mises à jour suivants :

* **Mises à jour utilisateur :** saisie manuellement par les utilisateurs ; On parle également de commentaires, de réponses et de notes.

   ![](assets/updates-qs-350x125.png)

* **Mises à jour système :** Créé automatiquement par le système. Une mise à jour du système comprend une brève note décrivant le type de changement survenu dans l’élément.

   <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

Les objets suivants peuvent avoir des mises à jour :

* Projet
* Tâche
* Problème
* Portfolio
* Programme
* Utilisateur
* Modèles
* Tâches de modèle
* Documents
* Feuilles de temps

Votre [!DNL Workfront] détermine si les mises à jour système s’affichent par défaut dans la variable [!UICONTROL Mises à jour] de la zone d’objets. [!DNL Workfront] utilisateurs avec un [!UICONTROL Plan] les mises à jour système de la licence sont affichées dans la variable [!UICONTROL Mises à jour] par défaut. Cependant, les utilisateurs peuvent filtrer les mises à jour du système, comme décrit dans la section [[!UICONTROL Activer] ou désactiver les mises à jour système](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) dans [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Toutes les autres [!DNL Workfront] les licences filtrent les mises à jour du système par défaut.

[!DNL Workfront] Les administrateurs peuvent définir le type de modifications dont le système doit effectuer le suivi dans la variable [!UICONTROL Mises à jour] zone. Tous les objets ne sont pas configurables. [!UICONTROL update] flux d’état. Les objets suivants ont une propriété [!UICONTROL Mises à jour] zone qui capture les flux de mise à jour trackés par le système, mais qui ne comporte pas de flux d’état de mise à jour configurables :

* Modèles
* Tâches de modèle
* Documents
* Feuilles de temps

Pour plus d’informations sur les flux de mise à jour du système et leur activation, voir [Configuration des mises à jour du système](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md). Pour plus d’informations sur la configuration des mises à jour des utilisateurs, voir [Configuration des préférences pour les mises à jour des utilisateurs](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
