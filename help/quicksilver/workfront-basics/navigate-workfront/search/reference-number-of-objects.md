---
content-type: reference
navigation-topic: search
title: Utilisation du numéro de référence des objets
description: Dans [!DNL Adobe Workfront], les éléments sont identifiés comme des objets. Les objets correspondent à la base de données et sont utilisés pour corréler les données avec un élément. Les numéros de référence sont utiles pour distinguer deux objets similaires (par exemple, des tâches portant le même nom). Vous pouvez rechercher des numéros de référence et les inclure dans les rapports.
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Utilisation du numéro de référence des objets

Dans [!DNL Adobe Workfront], les éléments sont identifiés comme des objets. Les objets correspondent à la base de données et sont utilisés pour corréler les données avec un élément.

Workfront attribue automatiquement à chacun des objets suivants un numéro de référence unique lors de la création de l’objet :

* Projets
* Tâches
* Événements
* Documents

Les numéros de référence sont utiles pour distinguer deux objets similaires (par exemple, des tâches portant le même nom). Vous pouvez rechercher des numéros de référence et les inclure dans les rapports.

>[!IMPORTANT]
>
>* [!DNL Workfront] affecte en continu des numéros de référence à tous les clients et à tous les objets. Par exemple, lorsque vous créez une tâche, [!DNL Workfront] peut lui attribuer un numéro de référence 00005. Si un autre client crée un projet, son projet peut recevoir le prochain numéro de référence disponible, par exemple 0006. Si vous créez ensuite un problème, celui-ci peut recevoir le numéro de référence 00007, etc.
>* Vous ne pouvez pas contrôler la séquence de numéros de référence d’un objet dans [!DNL Workfront]. La séquence est toujours contrôlée par notre base de données.
>




## Affichage du numéro de référence d’un objet

Les numéros de référence s’affichent par défaut pour les tâches et les problèmes. Vous pouvez également configurer facilement [!DNL Workfront] pour afficher les numéros de référence d’autres types d’objets.

* [Affichage des numéros de référence pour les tâches et les problèmes](#view-reference-numbers-for-tasks-and-issues)
* [Affichage des numéros de référence d’autres objets](#view-reference-numbers-for-other-objects)
* [Affichage des numéros de référence dans les rapports](#view-reference-numbers-in-reports)

### Affichage des numéros de référence pour les tâches et les problèmes

Les numéros de référence s’affichent par défaut lors de l’affichage d’une tâche ou d’un problème.  Pour afficher le numéro de référence, cliquez sur **[!UICONTROL Détails de la tâche]** ou **[!UICONTROL Détails du problème]** dans le panneau de gauche, puis localisez la variable **[!UICONTROL Informations de base]** dans la section Aperçu.

![](assets/reference-number-nwe-350x184.png)

### Affichage des numéros de référence d’autres objets

Pour afficher les numéros de référence des objets, vous pouvez créer une vue personnalisée ou modifier une vue existante et ajouter le [!UICONTROL Numéro de référence] à une colonne dans la vue. Par exemple, vous pouvez modifier la variable [!UICONTROL Projets] pour afficher le numéro de référence de tous vos projets.

Pour plus d’informations sur la création ou la modification d’une vue, voir [Présentation des vues dans [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Affichage des numéros de référence dans les rapports

Vous pouvez afficher le numéro de référence des objets dans les rapports en ajoutant la variable [!UICONTROL Numéro de référence] au rapport.

Pour plus d’informations sur l’ajout d’une colonne à un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Recherche d’un objet par numéro de référence

[!DNL Workfront] permet de rechercher un objet par numéro de référence.

Saisissez le numéro de référence d’un objet dans la variable **[!UICONTROL Rechercher]** champ, puis appuyez sur **[!UICONTROL Entrée]**.

Pour plus d’informations sur la recherche dans Workfront, voir [Rechercher [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
