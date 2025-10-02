---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Créer des sections personnalisées
description: Les informations affichées dans l’application web  [!DNL Workfront]  sont souvent affichées par défaut dans les sections du panneau de gauche. Chaque section contient des informations différentes sur une zone ou un objet  [!DNL Workfront] .
author: Becky
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: ccaf637601c53e5d92dd3357fb07e84b5fd69166
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 99%

---

# Créer des sections personnalisées

## Sections [!DNL Adobe Workfront]

Les informations affichées dans l’application web [!DNL Workfront] sont souvent affichées par défaut dans les sections du panneau de gauche. Chaque section contient des informations différentes sur une zone ou un objet [!DNL Workfront].\
Pour plus d’informations sur les zones par défaut de [!DNL Workfront], voir l’article [À propos de la mise en page par d’ [!DNL Adobe Workfront] &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Outre les sections fournies avec [!DNL Workfront] par défaut, vous pouvez ajouter un tableau de bord sur lequel afficher les informations relatives à votre workflow. Vous ne pouvez pas ajouter de tableau de bord à toutes les zones et tous les objets.

Le tableau suivant répertorie toutes les zones et tous les objets [!DNL Workfront] qui contiennent des sections dans le panneau de gauche et lesquels peuvent être personnalisés :

| Zone ou objet **[!DNL Workfront]** | **Sections système par défaut** | **Sections personnalisées** |
|---|---|---|
| Zone [!UICONTROL Projets] | ✓ | ✓ |
| [!UICONTROL Équipe] | ✓ |   |
| Zone [!UICONTROL Demandes] | ✓ |   |
| Zone [!UICONTROL Feuilles de temps] | ✓ |   |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Programme] | ✓ | ✓ |
| [!UICONTROL Projet] | ✓ | ✓ |
| [!UICONTROL Tâche] | ✓ |  ✓ |
| [!UICONTROL Problème] |  ✓ |  ✓ |
| [!UICONTROL Utilisateur ou utilisatrice] |  ✓ |  ✓ |
| [!UICONTROL Document] |  ✓ |  ✓ |
| Zone [!UICONTROL Ressources] | ✓ | ✓ |

{style="table-layout:auto"}

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td>[!UICONTROL Reviewer] ou supérieur</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Accès d’affichage au type d’objet</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan ou le type de licence dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Ajouter un tableau de bord dans le panneau de gauche d’un objet ou d’une zone [!DNL Workfront]

Avant de pouvoir ajouter un tableau de bord, vous devez le créer avec toutes les informations que vous souhaitez y afficher. Vous pouvez également créer une page externe.\
Pour plus d’informations sur la création de tableaux de bord, voir l’article [Créer un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Pour plus d’informations sur la création de pages externes, voir l’article [Incorporer une page web externe dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Après avoir créé le tableau de bord ou la page externe, vous pouvez les ajouter au panneau de gauche.

1. Accédez à l’une des zones ou l’un des objets [!DNL Workfront] dans lesquels vous pouvez ajouter une section personnalisée dans le panneau de gauche.\
   Ou
1. Accédez à un objet où vous pouvez ajouter un [!UICONTROL tableau de bord] dans le panneau de gauche.\
   Pour plus d’informations sur les zones et les objets auxquels vous pouvez ajouter des sections personnalisées, voir [[!DNL Adobe Workfront] Sections](#adobe-workfront-sections).
1. Cliquez sur **[!UICONTROL Ajouter un tableau de bord]** dans le panneau de gauche.
1. Saisissez le nom du tableau de bord dans le champ **[!UICONTROL Nom du lien rapide]**. Ceci est visible uniquement pour vous.
1. Commencez à saisir le nom d’un tableau de bord existant ou d’une page externe existante dans le champ **[!UICONTROL Choisir un tableau de bord]**, puis sélectionnez le tableau de bord lorsqu’il s’affiche dans la liste.
1. Cliquez sur **[!UICONTROL Ajouter]**.
1. (Facultatif) Faites glisser les sections dans l’ordre dans lequel vous souhaitez les afficher.

   La section supérieure est la section par défaut de la page.

   Les sections que vous avez créées pour des objets individuels s’affichent lorsque vous accédez à tous les objets du même type et sont seulement disponibles pour vous.

## Afficher les tableaux de bord dans le panneau de gauche des objets

Pour plus d’informations sur l’ajout d’un tableau de bord sous un objet, voir la section [[!UICONTROL Ajouter un tableau de bord] dans le panneau de gauche d’un objet ou d’une zone Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) dans cet article.

Lorsque vous ajoutez un tableau de bord à une section personnalisée sous un objet, celui-ci sert de filtre pour le tableau de bord. Par exemple, si vous ajoutez un rapport de tâche sur un tableau de bord et que vous ajoutez ce tableau de bord à un projet, la section personnalisée qui contient le tableau de bord du projet affiche uniquement les tâches du projet que vous voyez.

Les objets suivants sont filtrés pour l’objet sous lequel ils s’affichent, si cet objet est supérieur à leur hiérarchie :

* Projet
* Tâche
* Problème
* Processus d’approbation
* Note
* Document

Pour plus d’informations sur la hiérarchie et l’interdépendance des objets, voir la section [Interdépendance et hiérarchie des objets](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) dans l’article [Présentation des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personnaliser le panneau de gauche dans un modèle de mise en page

Lorsque vous ajoutez des tableaux de bord à votre instance [!DNL Workfront], ils ne sont visibles que par vous.

Vous pouvez personnaliser les sections dans [!DNL Workfront] et partager la nouvelle mise en page avec plusieurs personnes dans un modèle de mise en page. Seul un administrateur ou une administratrice système ou de groupe peut les partager avec d’autres personnes dans un modèle de mise en page. Pour plus d’informations sur la personnalisation du panneau de gauche avec un modèle de mise en page, voir [Personnaliser le panneau de gauche à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
