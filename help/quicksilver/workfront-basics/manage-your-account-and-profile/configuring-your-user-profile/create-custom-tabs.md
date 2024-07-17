---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Créer des sections personnalisées
description: Par défaut, les informations affichées dans l’application web  [!DNL Workfront] s’affichent souvent dans les sections du panneau de gauche. Chaque section contient des informations différentes sur une zone ou un objet  [!DNL Workfront] .
author: Nolan
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 1079f85651ec691280e2cccefaa6e48e0b9d89f8
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 9%

---

# Créer des sections personnalisées

## [!DNL Adobe Workfront] sections

Par défaut, les informations affichées dans l’application web [!DNL Workfront] s’affichent souvent dans les sections du panneau de gauche. Chaque section contient des informations différentes sur une zone ou un objet [!DNL Workfront].\
Pour plus d’informations sur les zones par défaut de [!DNL Workfront], consultez l’article [À propos de la  [!DNL Adobe Workfront] mise en page par défaut](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Outre les sections fournies avec [!DNL Workfront] par défaut, vous pouvez ajouter un tableau de bord sur lequel afficher les informations relatives à votre workflow. Vous ne pouvez pas ajouter de tableau de bord à toutes les zones et tous les objets.

Le tableau suivant répertorie toutes les zones et tous les objets [!DNL Workfront] qui contiennent des sections dans le panneau de gauche et lesquels d’entre eux peuvent être personnalisés :

| **[!DNL Workfront]zone ou objet** | **Sections système par défaut** | **Sections personnalisées** |
|---|---|---|
| Zone [!UICONTROL Projets] | ✓ | ✓ |
| [!UICONTROL Équipe] | ✓ |   |
| Zone [!UICONTROL Demandes] | ✓ |   |
| [!UICONTROL Zone de feuilles de calcul ] | ✓ |   |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Programme] | ✓ | ✓ |
| [!UICONTROL Projet] | ✓ | ✓ |
| [!UICONTROL Tâche] | ✓ |  ✓ |
| [!UICONTROL Problème] |  ✓ |  ✓ |
| [!UICONTROL Utilisateur ou utilisatrice] |  ✓ |  ✓ |
| [!UICONTROL Document] |  ✓ |  ✓ |

{style="table-layout:auto"}

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td>[!UICONTROL Reviewer] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td>Afficher l’accès au type d’objet</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir quel plan ou type de licence vous avez, contactez votre administrateur [!DNL Workfront].

## Ajouter un tableau de bord dans le panneau de gauche d’un objet ou d’une zone [!DNL Workfront]

Avant de pouvoir ajouter un tableau de bord, vous devez le créer avec toutes les informations que vous souhaitez y afficher. Vous pouvez également créer une page externe.\
Pour plus d’informations sur la création de tableaux de bord, consultez l’article [Création d’un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Pour plus d’informations sur la création de pages externes, consultez l’article [Incorporation d’une page web externe dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Après avoir créé le tableau de bord ou la page externe, vous pouvez les ajouter au panneau de gauche.

1. Accédez à l’une des zones ou à l’un des objets [!DNL Workfront] où vous pouvez ajouter une section personnalisée dans le panneau de gauche.\
   Ou
1. Accédez à un objet où vous pouvez ajouter un [!UICONTROL tableau de bord] dans le panneau de gauche.\
   Pour plus d’informations sur les zones et les objets auxquels vous pouvez ajouter des sections personnalisées, voir [[!DNL Adobe Workfront] sections](#adobe-workfront-sections).
1. Cliquez sur **[!UICONTROL Ajouter un tableau de bord]** dans le panneau de gauche.
1. Saisissez un nom pour le tableau de bord dans le champ **[!UICONTROL Nom du lien rapide]**. Ceci est visible uniquement pour vous.
1. Commencez à saisir le nom d’un tableau de bord existant ou d’une page externe dans le champ **[!UICONTROL Choisir un tableau de bord]** , puis sélectionnez le tableau de bord lorsqu’il s’affiche dans la liste.
1. Cliquez sur **[!UICONTROL Ajouter]**.
1. (Facultatif) Faites glisser les sections dans l’ordre dans lequel vous souhaitez les afficher.

   La section supérieure est la section par défaut de la page.

   Les sections que vous avez créées pour des objets individuels s’affichent lorsque vous accédez à tous les objets du même type et que vous n’y avez accès que.

## Afficher les tableaux de bord dans le panneau de gauche des objets

Pour plus d’informations sur l’ajout d’un tableau de bord sous un objet, reportez-vous à la section [[!UICONTROL Ajout d’un tableau de bord] dans le panneau de gauche d’un objet ou d’une zone Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) de cet article.

Lorsque vous ajoutez un tableau de bord à une section personnalisée sous un objet, celui-ci sert de filtre pour le tableau de bord. Par exemple, si vous ajoutez un rapport de tâche sur un tableau de bord à un projet, la section personnalisée qui contient le tableau de bord du projet affiche uniquement les tâches du projet que vous affichez.

Les objets suivants sont filtrés pour l’objet sous lequel ils s’affichent, si cet objet est supérieur à leur hiérarchie :

* Projet
* Tâche
* Problème
* Processus d&#39;approbation
* Note
* Document

Pour plus d’informations sur la hiérarchie et l’interdépendance des objets, reportez-vous à la section [Interdépendance et hiérarchie des objets](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) de l’article [Comprendre les objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personnalisation du panneau de gauche dans un modèle de mise en page

Lorsque vous ajoutez des tableaux de bord à votre instance [!DNL Workfront], ils ne sont visibles que par vous.

Vous pouvez personnaliser les sections de [!DNL Workfront] et partager la nouvelle mise en page avec plusieurs utilisateurs dans un modèle de mise en page. Seul un administrateur système ou de groupe peut les partager avec d’autres utilisateurs dans un modèle de mise en page. Pour plus d’informations sur la personnalisation du panneau de gauche avec un modèle de mise en page, voir [Personnalisation du panneau de gauche à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
