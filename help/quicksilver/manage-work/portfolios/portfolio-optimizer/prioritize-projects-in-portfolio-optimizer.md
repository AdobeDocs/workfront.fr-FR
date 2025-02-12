---
title: Hiérarchiser des projets dans l’Optimisateur de portfolio
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: Vous pouvez hiérarchiser vos projets dans l’Optimisateur de portfolio afin de définir l’ordre dans lequel ils doivent être terminés.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 91%

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

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard</p>
   <p>Actuel : formule</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en [!UICONTROL Edit] aux projets et aux portfolios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour le portfolio</p> <p>Autorisation Contribuer ou supérieure pour les projets</p> 
   <p>Vous devez disposer d’autorisations de niveau Gérer pour tous les projets de la liste pour pouvoir utiliser <b>Définir la priorité du projet</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises pour la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier la priorité des projets dans l’[!UICONTROL Optimisateur de portfolio]

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **[!UICONTROL Portfolios]**.
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
