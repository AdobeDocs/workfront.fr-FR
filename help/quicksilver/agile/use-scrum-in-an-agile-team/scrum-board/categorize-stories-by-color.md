---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Catégorisation des articles par couleur sur le panorama
description: L’association des couleurs par défaut des articles du panorama de défilement varie selon que le panorama se trouve sur une itération ou sur un projet.
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 12%

---

# Classez les articles par couleur sur le panorama [!UICONTROL Scrum]

## Modification de l’association des couleurs par défaut des articles

L’association des couleurs par défaut des articles varie selon que le panorama se trouve sur une itération ou sur un projet :

* **[!UICONTROL Itération]** : lors d’une itération, les mosaïques des tableaux de bord sont codées par couleur en fonction du projet auquel l’article est associé. (Chaque projet se voit attribuer arbitrairement une couleur sur le tableau de bord.) Vous pouvez modifier ce comportement par défaut pour chaque équipe agile. Les couleurs pour les articles agiles d’une itération peuvent être liées au projet (par défaut), à la priorité de l’article, au propriétaire ou à la forme libre. Pour plus d’informations, voir [Configuration de l’utilisation des indicateurs de couleur pour les articles sur le tableau de bord agile](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) dans l’article [Configurer le graphique](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL Projet]** : sur un projet, toutes les sous-tâches correspondent à la couleur de la tâche parente, de sorte que les couleurs de tous les articles d’un couloir donné soient les mêmes. Les couleurs sont attribuées de manière aléatoire aux tâches lorsqu’elles sont créées si la tâche ne comporte aucune sous-tâche ou n’a pas de tâche parent. Vous pouvez modifier ce comportement par défaut en modifiant la vue agile. Les couleurs des articles agiles sur un projet peuvent être liées à l’article parent (par défaut), à la priorité de l’article, au propriétaire ou à la forme libre. Pour plus d’informations, voir [Création ou personnalisation d’une [!UICONTROL vue Agile]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) dans [Présentation des vues dans [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p> 
   ou
   <p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Changer la couleur des histoires lors de l’utilisation de forme libre

Si les paramètres de l’équipe agile ont été configurés de sorte que l’option [!UICONTROL Associer la couleur de la carte à] soit définie sur [!UICONTROL Formulaire libre], les utilisateurs peuvent modifier manuellement la couleur des mosaïques d’articles. Cela peut s’avérer utile pour communiquer d’autres types d’informations importantes pour l’équipe ou l’organisation :

{{step1-to-team}}

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]** pour choisir une itération spécifique ou **[!UICONTROL Itération actuelle]**.
1. Pointez sur la bannière de couleur en haut de la mosaïque de l’article.

   ![](assets/agile-story-color1-nwe-350x140.png)

1. Cliquez sur **[!UICONTROL Changer de couleur]**, puis sélectionnez la couleur de votre choix.

   ![](assets/agile-story-color2-nwe-350x138.png)
