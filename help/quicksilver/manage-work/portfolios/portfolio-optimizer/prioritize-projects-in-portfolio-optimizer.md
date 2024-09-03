---
title: Hiérarchiser des projets dans l’Optimisateur de portfolio
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: Vous pouvez hiérarchiser vos projets dans l’Optimisateur de portfolio afin de définir l’ordre dans lequel ils doivent être terminés.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 100%

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

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>[!UICONTROL Business] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en [!UICONTROL Edit] aux projets et aux portfolios</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre administrateur ou administratrice [!DNL Workfront] si des restrictions supplémentaires ont été définies dans votre niveau d’accès. Pour plus d’informations sur la manière dont l’administration [!DNL Workfront] peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour le portfolio</p> <p>Autorisation Contribuer ou supérieure pour les projets</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Modifier la priorité des projets dans l’[!UICONTROL Optimisateur de portfolio]

1. Cliquez sur l’icône **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **[!UICONTROL Portfolios]**.
1. (Facultatif) Sélectionnez le filtre approprié dans le menu déroulant **[!UICONTROL Filtrer]** pour afficher la liste appropriée de portfolios.
1. Cliquez sur le nom d’un portfolio pour l’ouvrir.
1. Cliquez sur **[!UICONTROL Optimisation de portfolio]** dans le panneau de gauche.
1. Dans la zone [!UICONTROL optimisation de projet], modifiez la priorité de vos projets en les faisant glisser par ordre de priorité, puis en les déposant à la position souhaitée sur l’affichage.

   ![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   Cliquez sur **[!UICONTROL Définir la priorité]** dans la zone d’optimisation de projet une fois que vous avez terminé de réorganiser vos projets. Les projets reçoivent un nouveau numéro en fonction du nouvel ordre.

1. Cliquez sur **[!UICONTROL Enregistrer]** pour enregistrer la nouvelle priorité des projets dans l’[!UICONTROL Optimisateur de portfolio]. La priorité est répertoriée sous la forme d’un nombre dans la colonne de nombres **#**.

   >[!TIP]
   >
   >Cela ne modifie pas nécessairement l’ordre des projets dans l’[!UICONTROL Optimisateur de portfolio], car la liste des projets peut être triée selon une colonne autre que la colonne **#**. Cliquez sur l’en-tête de colonne **#** pour trier la liste par priorité de projet.

   Vous pouvez voir la priorité du projet telle qu’elle apparaît dans l’[!UICONTROL Optimisateur de portfolio] dans le planificateur de ressources, en activant le paramètre **[!UICONTROL Afficher les priorités de portfolio]** dans le planificateur de ressources.

   Pour plus d’informations sur la hiérarchisation des projets dans le [!UICONTROL Planificateur de ressources], voir l’article [Hiérarchiser des projets dans le [!UICONTROL Planificateur de ressources]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).
