---
title: Hiérarchiser des projets dans l’Optimisateur de portfolio
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: Vous pouvez hiérarchiser vos projets dans l’Optimisateur de portfolio afin de définir l’ordre dans lequel ils doivent être terminés.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: 714e6e09f1429f0382c36d17d3f2aca95edcfbc6
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 93%

---

# Hiérarchiser des projets dans [!UICONTROL l’Optimisateur de portfolio]

Vous pouvez hiérarchiser vos projets dans [!UICONTROL l’Optimisateur de portfolio] afin de définir l’ordre dans lequel ils doivent être terminés.

Tenez compte des points suivants lorsque vous utilisez [!UICONTROL l’Optimisateur de portfolio] :

* Les projets situés en haut dans [!UICONTROL l’Optimisateur de portfolio] sont considérés comme plus importants que ceux du bas. Vous devez terminer les projets par ordre de priorité dans [!UICONTROL l’Optimisateur de portfolio] pour que le Portfolio soit optimisé.
* La priorité des projets dans [!UICONTROL l’Optimisateur de portfolio] n’est pas liée au champ [!UICONTROL Priorité] situé dans l’onglet [!UICONTROL Détails du projet] d’un projet.

  Le champ [!UICONTROL Priorité] dans l’onglet [!UICONTROL Détails du projet] est un indicateur visuel que vous spécifiez manuellement pour déterminer l’importance d’un projet.

* La priorité des projets dans l’Optimisateur de portfolio est visible dans le [!DNL Resource Planner], s’il est activé dans ce dernier. Dans le [!DNL Resource Planner], les projets reçoivent les ressources suivant l’ordre de leur priorité issue du [!UICONTROL Planificateur de ressources], et non la [!UICONTROL Priorité du portfolio].

  Pour plus d’informations sur la hiérarchisation des projets dans le [!UICONTROL Planificateur de ressources], voir l’article [Hiérarchiser des projets dans le [!UICONTROL Planificateur de ressources]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* La zone **[!UICONTROL Hiérarchisation des projets]** de l’[!UICONTROL Optimisateur de portfolio] affiche les projets dans l’ordre des [!UICONTROL Dates de début planifiées] et de la [!UICONTROL Valeur nette], par défaut.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquet</td> 
   <td> <p>Workfront Prime ou version ultérieure</p>
      <p>Workflow Prime ou version ultérieure</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès de [!UICONTROL Edit] aux [!UICONTROL Portfolios] et aux [!UICONTROL Projects]</p>  </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour le portfolio</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises pour la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## Modifier la priorité des projets dans l’[!UICONTROL Optimisateur de portfolio]

{{step1-to-portfolios}}

1. (Facultatif) Sélectionnez le filtre approprié dans le menu déroulant **[!UICONTROL Filtrer]** pour afficher la liste appropriée de portfolios.
1. Cliquez sur le nom d’un portfolio pour l’ouvrir.
1. Cliquez sur **[!UICONTROL Optimisation de portfolio]** dans le panneau de gauche.
1. Dans la zone [!UICONTROL optimisation de projet], modifiez la priorité de vos projets en les faisant glisser par ordre de priorité, puis en les déposant à la position souhaitée sur l’affichage.

   ![Portfolio optimizer avec projets](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   Cliquez sur **[!UICONTROL Définir la priorité]** dans la zone d’optimisation de projet une fois que vous avez terminé de réorganiser vos projets. Les projets reçoivent un nouveau numéro en fonction du nouvel ordre.

1. Cliquez sur **[!UICONTROL Enregistrer]** pour enregistrer la nouvelle priorité des projets dans l’[!UICONTROL Optimisateur de portfolio]. La priorité est répertoriée sous la forme d’un nombre dans la colonne de nombres **#**.

   >[!TIP]
   >
   >Cela ne modifie pas nécessairement l’ordre des projets dans l’[!UICONTROL Optimisateur de portfolio], car la liste des projets peut être triée selon une colonne autre que la colonne **#**. Cliquez sur l’en-tête de colonne **#** pour trier la liste par priorité de projet.

   Vous pouvez voir la priorité du projet telle qu’elle apparaît dans l’[!UICONTROL Optimisateur de portfolio] dans le planificateur de ressources, en activant le paramètre **[!UICONTROL Afficher les priorités de portfolio]** dans le planificateur de ressources.

   Pour plus d’informations sur la hiérarchisation des projets dans le [!UICONTROL Planificateur de ressources], voir l’article [Hiérarchiser des projets dans le [!UICONTROL Planificateur de ressources]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).
