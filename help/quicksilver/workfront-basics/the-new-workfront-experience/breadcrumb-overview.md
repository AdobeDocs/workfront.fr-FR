---
content-type: overview
title: Vue d’ensemble des chemins de navigation
description: Les chemins de navigation affichent la hiérarchie de navigation complète pour tous les types d’objets.
feature: Get Started with Workfront
exl-id: c4103f8e-4c3f-4d4d-a0eb-628c60735ab7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/VryLEVTqJFgAxlm-al5y0hqxVQ71zFPi8YG1oAlox8k
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 8771d66f6b7ecae9ac439456822889d4fe438649
workflow-type: tm+mt
source-wordcount: 334
ht-degree: 87%

---

# Vue d’ensemble des chemins de navigation

Les chemins de navigation affichent la hiérarchie de navigation complète pour tous les types d’objets. Chaque objet du chemin de navigation comporte un libellé qui affiche le type d’objet. La page sur laquelle vous vous trouvez actuellement s’affiche à la fois dans l’en-tête de la page et à la fin du chemin de navigation en italique. Dans l’exemple ci-dessous, il s’agit de la tâche « [!UICONTROL Partager avec l’équipe de marque] ».

![Chemin de navigation réduit](assets/collapsed-breadcrumb-2026.png)

Lorsqu’il y a trop d’objets dans le chemin de navigation ou que la largeur d’écran empêche l’affichage de la hiérarchie de navigation complète, le chemin réduit certains chemins de navigation et regroupe ces objets au début du chemin de navigation. Le projet et la page d’objet active sont toujours visibles dans le chemin de chemin de navigation.

Par exemple, « 3 autres » dans l’image ci-dessus indique que 3 objets ne s’affichent pas. Ces éléments peuvent se trouver au-dessus du niveau du projet ou entre le projet et la page actuelle.

Cliquer sur « [!UICONTROL Plus] » vous permet de développer la hiérarchie complète. Vous pouvez cliquer sur « [!UICONTROL Moins] » pour réduire à nouveau le chemin de navigation.

![Chemin de navigation réduit](assets/expanded-breadcrumb-2026.png)

Vous pouvez également utiliser les touches suivantes pour parcourir les chemins de navigation :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Onglet</strong> </td> 
   <td> <p>Accédez à chaque élément dans le chemin de navigation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Entrée</strong> </td> 
   <td> <p>Développez un chemin de navigation réduit, réduisez un chemin de chemin de navigation développé, puis ouvrez une nouvelle page sur un lien d’objet.</p> </td> 
  </tr> 
 </tbody> 
</table>



<!--
drafted: this is no longer possible, since we removed Campaigns, but it might come back as part of Maestro: 

## Multi-object breadcrumbs

>[!NOTE]
>
>The information in this article is available only in the Preview environment when you participate in the [!UICONTROL Campaigns] beta program. The functionality described here might not be fully available yet. For more information about current available features and how to enroll, see [Campaigns beta].

Some objects can belong to multiple parent objects. For example, a project can belong to multiple campaigns. In this case, all the campaigns that the project belongs to display in the breadcrumb.

The multi-object listing in the breadcrumb (for example, the campaigns) displays the number of parent objects which expands into a list to display all the campaigns that the project is associated with. For more information, see [Add objects to a campaign](../../manage-work/campaigns/add-objects-to-a-campaign.md).


![Project with multiple campaigns in the breadcrumb](assets/project-with-multiple-campaigns-in-breadcrumb.png)

-->

## Accéder à un objet parent à partir des chemins de navigation

Pour plus d’informations sur les objets parent dans [!DNL Workfront], voir [Comprendre les objets dans  [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Le cas échéant) Si vous ne voyez pas l’objet auquel vous souhaitez accéder dans un chemin de navigation réduit, cliquez sur **[!UICONTROL Plus]**, puis localisez l’objet.

   >[!NOTE]
   >
   >Si vous ne disposez pas d’une autorisation d’accès à un objet, celui-ci n’est pas visible dans les chemins de navigation.

1. Cliquez sur un objet du chemin de navigation pour y accéder.

   La page d’objet s’ouvre.

   Si vous vous intéressez à un projet connecté à un objet dans Workfront Planning (une campagne, par exemple), vous pouvez basculer entre les deux types d’objets Planning et Workfront à partir du chemin de navigation. Pour plus d’informations, voir [&#x200B; Présentation de la hiérarchie et du chemin de navigation &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).
