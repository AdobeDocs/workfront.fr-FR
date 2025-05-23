---
content-type: reference
navigation-topic: search
title: Utiliser le numéro de référence des objets
description: Dans  [!DNL Adobe Workfront], les éléments sont identifiés sous la forme d’objets. Les objets correspondent à la base de données et sont utilisés pour corréler les données à un élément. Les numéros de référence sont utiles pour distinguer deux objets similaires (par exemple, des tâches portant le même nom). Vous pouvez rechercher des numéros de référence et les inclure dans les rapports.
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 100%

---

# Utiliser le numéro de référence des objets

Dans [!DNL Adobe Workfront], les éléments sont identifiés sous la forme d’objets. Les objets correspondent à la base de données et sont utilisés pour corréler les données à un élément.

Workfront affecte automatiquement un numéro de référence unique à chacun des objets suivants lors de sa création :

* Projets
* Tâches
* Problèmes
* Documents

Les numéros de référence sont utiles pour distinguer deux objets similaires (par exemple, des tâches portant le même nom). Vous pouvez rechercher des numéros de référence et les inclure dans les rapports.

>[!IMPORTANT]
>
>* [!DNL Workfront] affecte en continu des numéros de référence à l’ensemble des clientes et clients et à tous les objets. Par exemple, lorsque vous créez une tâche, [!DNL Workfront] peut lui affecter le numéro de référence 00005. Si une autre personne crée ensuite un projet, son projet peut recevoir le prochain numéro de référence disponible, par exemple 00006. Puis, si vous créez un problème, celui-ci peut recevoir le numéro de référence 00007, etc.
>* Vous ne pouvez pas contrôler la séquence des numéros de référence des objets de [!DNL Workfront]. La séquence est toujours contrôlée par notre base de données.
>



## Afficher le numéro de référence d’un objet

Les numéros de référence s’affichent par défaut pour les tâches et les problèmes. Vous pouvez également configurer facilement [!DNL Workfront] pour qu’il affiche les numéros de référence d’autres types d’objets.

* [Afficher les numéros de référence pour les tâches et les problèmes](#view-reference-numbers-for-tasks-and-issues)
* [Afficher les numéros de référence pour d’autres objets](#view-reference-numbers-for-other-objects)
* [Afficher les numéros de référence dans les rapports](#view-reference-numbers-in-reports)

### Afficher les numéros de référence pour les tâches et les problèmes

Les numéros de référence s’affichent par défaut lors de l’affichage d’une tâche ou d’un problème.  Pour afficher le numéro de référence, cliquez sur **[!UICONTROL Détails sur la tâche]** ou **[!UICONTROL Détails du problème]** dans le panneau de gauche, puis localisez la section **[!UICONTROL Informations de base]** dans la section Vue d’ensemble.

![Numéro de référence](assets/reference-number-nwe-350x184.png)

### Afficher les numéros de référence pour d’autres objets

Pour afficher les numéros de référence des objets, vous pouvez créer une vue personnalisée ou modifier une vue existante et ajouter le champ [!UICONTROL Numéro de référence] dans une colonne de la vue. Par exemple, vous pouvez modifier la vue [!UICONTROL Projets] pour afficher le numéro de référence de tous vos projets.

Pour plus d’informations sur la création ou la modification d’une vue, voir la section [Vue d’ensemble des vues dans  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Afficher les numéros de référence dans les rapports

Vous pouvez afficher le numéro de référence des objets dans les rapports en ajoutant la colonne [!UICONTROL Numéro de référence] au rapport.

Pour plus d’informations sur l’ajout d’une colonne à un rapport, voir la section [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Rechercher un objet par son numéro de référence

[!DNL Workfront] permet de rechercher un objet par son numéro de référence.

Saisissez le numéro de référence d’un objet dans le champ **[!UICONTROL Rechercher]**, puis appuyez sur **[!UICONTROL Entrée]**.

Pour plus d’informations sur la recherche dans Workfront, voir la section [Rechercher [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
