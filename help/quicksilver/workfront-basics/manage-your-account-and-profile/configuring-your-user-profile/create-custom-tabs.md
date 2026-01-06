---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Ajout d’un tableau de bord dans le panneau de gauche d’un objet ou d’une zone Workfront
description: Les informations affichées dans l’application web  [!DNL Workfront]  sont souvent affichées par défaut dans les sections du panneau de gauche. Chaque section contient des informations différentes sur une zone ou un objet  [!DNL Workfront] .
author: Becky and Lisa
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 72%

---

# Ajouter un tableau de bord dans le panneau de gauche d’un objet ou d’une zone Workfront

## Sections [!DNL Adobe Workfront]

Les informations affichées dans l’application web [!DNL Workfront] sont souvent affichées par défaut dans les sections du panneau de gauche. Chaque section contient des informations différentes sur une zone ou un objet [!DNL Workfront].

Pour plus d’informations sur les zones par défaut de [!DNL Workfront], voir l’article [À propos de la mise en page par d’ [!DNL Adobe Workfront] &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Outre les sections fournies avec [!DNL Workfront] par défaut, vous pouvez ajouter un tableau de bord sur lequel afficher les informations relatives à votre workflow. Vous ne pouvez pas ajouter de tableau de bord à toutes les zones et tous les objets.

Le tableau suivant répertorie toutes les zones et tous les objets [!DNL Workfront] qui contiennent des sections dans le panneau de gauche et ceux qui peuvent être personnalisés avec un tableau de bord :

| Zone ou objet **[!DNL Workfront]** | **Sections système par défaut** | **Tableaux de bord** |
|---|---|---|
| Zone [!UICONTROL Projets] | ✓ | ✓ |
| [!UICONTROL Équipe] | ✓ |    |
| Zone [!UICONTROL Demandes] | ✓ |    |
| Zone [!UICONTROL Feuilles de temps] | ✓ |    |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Programme] | ✓ | ✓ |
| [!UICONTROL Projet] | ✓ | ✓ |
| [!UICONTROL Tâche] | ✓ | ✓ |
| [!UICONTROL Problème] | ✓ | ✓ |
| [!UICONTROL Utilisateur ou utilisatice] | ✓ | ✓ |
| [!UICONTROL Document] | ✓ | ✓ |
| Zone [!UICONTROL Ressources] | ✓ | ✓ |

{style="table-layout:auto"}

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
   <p>Léger ou supérieur</p>
   <p>Révision ou supérieur</p></td>
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td><p>Accès d’affichage au type d’objet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter un tableau de bord dans le panneau de gauche d’un objet ou d’une zone [!DNL Workfront]

Avant de pouvoir ajouter un tableau de bord, vous devez le créer avec toutes les informations que vous souhaitez y afficher. Vous pouvez également créer une page externe.

Pour plus d’informations sur la création de tableaux de bord, voir l’article [Créer un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Pour plus d’informations sur la création de pages externes, voir l’article [Incorporer une page web externe dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Après avoir créé le tableau de bord ou la page externe, vous pouvez les ajouter au panneau de gauche.

1. Accédez à l’une des zones ou à l’un des objets [!DNL Workfront] où vous pouvez ajouter un tableau de bord dans le panneau de gauche.

   Pour plus d’informations sur les zones et les objets auxquels vous pouvez ajouter des tableaux de bord, voir [[!DNL Adobe Workfront] sections](#adobe-workfront-sections).

1. Cliquez sur **[!UICONTROL Ajouter un tableau de bord]** dans le panneau de gauche.
1. Saisissez le nom du tableau de bord dans le champ **[!UICONTROL Nom du lien rapide]**. Ceci est visible uniquement pour vous.
1. Commencez à saisir le nom d’un tableau de bord existant ou d’une page externe existante dans le champ **[!UICONTROL Choisir un tableau de bord]**, puis sélectionnez le tableau de bord lorsqu’il s’affiche dans la liste.
1. Cliquez sur **[!UICONTROL Ajouter]**.
1. (Facultatif) Faites glisser les sections dans l’ordre dans lequel vous souhaitez les afficher.

   La section supérieure est la section par défaut de la page.

   Les tableaux de bord que vous avez ajoutés ne sont disponibles que pour vous.

## Afficher les tableaux de bord dans le panneau de gauche des objets

Pour plus d’informations sur l’ajout d’un tableau de bord sous un objet, voir la section [[!UICONTROL Ajouter un tableau de bord] dans le panneau de gauche d’un objet ou d’une zone Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) dans cet article.

Lorsque vous ajoutez un tableau de bord au panneau de gauche d’un objet, l’objet agit comme un filtre pour le tableau de bord. Par exemple, si vous ajoutez un rapport de tâches à un tableau de bord et que vous ajoutez le tableau de bord à un projet, le tableau de bord affiche uniquement les tâches du projet que vous consultez.

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

Seul un administrateur système ou de groupe peut partager des tableaux de bord avec d’autres utilisateurs dans un modèle de mise en page. Pour plus d’informations sur la personnalisation du panneau de gauche avec un modèle de mise en page, voir [Personnaliser le panneau de gauche à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
