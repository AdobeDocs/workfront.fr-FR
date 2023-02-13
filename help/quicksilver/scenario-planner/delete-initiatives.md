---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Suppression d’initiatives dans le planificateur de scénarios
description: Vous pouvez supprimer des initiatives sur un plan que vous avez créé ou sur un plan que quelqu’un a partagé avec vous. Vous ne pouvez pas récupérer les initiatives que vous avez supprimées.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# Supprimer des initiatives dans le [!DNL Scenario Planner]

Vous pouvez supprimer des initiatives sur un plan que vous avez créé ou sur un plan que quelqu’un a partagé avec vous. Vous ne pouvez pas récupérer les initiatives que vous avez supprimées.

## Exigences d’accès

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produit</b> </td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour la variable [!DNL Adobe Workfront Scenario Planner] pour accéder aux fonctionnalités décrites dans cet article. </p> <p>Pour plus d’informations sur l’obtention de [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire à l’utilisation du [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>Accès à [!UICONTROL Modifier] ou supérieur à la variable [!DNL Scenario Planner]</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorisations d’objet</strong> </p> </td> 
   <td> <p>Autorisations [!UICONTROL Gérer] pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Demandez l’accès à un plan dans la [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Suppression d’initiatives

Tenez compte des points suivants lors de la suppression d’initiatives :

* La suppression d’une initiative supprime du plan le nombre requis de rôles d’emploi et les informations de coûts associées à l’initiative.
* La suppression d’une initiative créée par l’importation d’un projet ne supprime pas le projet associé à l’initiative.
* La suppression d’une initiative qui a été publiée sur un projet au moins une fois entraîne les résultats suivants :

   * L’initiative est supprimée du scénario, mais la variable [!DNL Scenario Planner] reste dans la zone [!UICONTROL Détails du projet] .
   * Si l’initiative que vous supprimez est la seule initiative publiée sur le scénario, l’indicateur que le plan a été publié est également supprimé.

      Pour plus d’informations sur la publication d’initiatives dans des projets, voir [Mettez à jour ou créez des projets en publiant des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

      Pour plus d’informations sur la création d’initiatives par importation de projets, voir [Importation de projets dans des plans dans [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

Vous pouvez supprimer une initiative à la fois ou supprimer plusieurs initiatives en bloc.

* [Supprimer une initiative](#delete-one-initiative)
* [Supprimer des initiatives en bloc](#delete-initiatives-in-bulk)

### Supprimer une initiative {#delete-one-initiative}

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png), puis cliquez sur [!UICONTROL Scénarios].

   Une liste des plans s’affiche.

1. Cliquez sur le nom d’un plan pour l’ouvrir, puis localisez l’initiative que vous souhaitez supprimer.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur le bouton **[!UICONTROL Plus de menu]** ![](assets/more-menu.png) à droite du nom de l’initiative, puis cliquez sur **[!UICONTROL Supprimer]** > **[!UICONTROL Oui, supprimez-le.]**.

   * Sélectionnez la zone située à gauche de l’initiative, puis cliquez sur **[!UICONTROL Supprimer]** dans le menu flottant qui s’affiche au bas du plan, puis cliquez sur **[!UICONTROL Oui, supprimez-le.]**.

   L&#39;initiative, son rôle et ses informations sur les coûts sont supprimés du plan.

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.

### Supprimer des initiatives en bloc {#delete-initiatives-in-bulk}

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png), puis cliquez sur [!UICONTROL Scénarios].

   Une liste des plans s’affiche.

1. Cliquez sur le nom d’un plan pour l’ouvrir, puis localisez l’initiative que vous souhaitez supprimer.
1. Cochez les cases situées à gauche des initiatives que vous souhaitez supprimer, puis cliquez sur **[!UICONTROL Supprimer]** dans le menu qui s’affiche au bas du plan, puis cliquez sur **[!UICONTROL Oui, supprimez-les.]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Les initiatives, leur rôle professionnel et leurs informations sur les coûts sont supprimés du plan.

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.
