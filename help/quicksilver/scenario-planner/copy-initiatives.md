---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copier des initiatives dans le planificateur de scénarios
description: Vous pouvez créer des initiatives en copiant des initiatives existantes. Vous pouvez copier des initiatives sur un plan que vous créez ou sur un plan que quelqu’un partage avec vous.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 21%

---

# Copiez les initiatives dans le [!DNL Scenario Planner]

Vous pouvez créer des initiatives en copiant des initiatives existantes. Vous pouvez copier des initiatives sur un plan que vous créez ou sur un plan que quelqu’un partage avec vous.

## Conditions d’accès

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] ou niveau supérieur</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produit</b> </td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour le [!DNL Adobe Workfront Scenario Planner] afin d’accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’obtention du [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser le [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Accès à [!UICONTROL Modifier] ou supérieur à la variable [!DNL Scenario Planner]</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont l’équipe d’administration [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorisations d’objets</strong> </p> </td> 
   <td> <p>Autorisations [!UICONTROL Gérer] pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Demander l’accès à un plan dans le [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Copie d’initiatives

Tenez compte des points suivants lors de la copie d’initiatives :

* La copie d’une initiative place la copie sur le même plan que l’initiative initiale.
* La copie d&#39;une initiative copie et ajoute les informations suivantes de l&#39;initiative originale à la nouvelle initiative :

   * [!UICONTROL Durée]
   * [!UICONTROL Fonctions]
   * [!UICONTROL Personnes] et [!UICONTROL Coûts fixes]
   * [!UICONTROL Bénéfice prévu]

* La copie d&#39;une initiative peut modifier les informations suivantes pour le plan, si l&#39;information existe sur l&#39;initiative initiale :

   * Nombre requis de rôles de tâche
   * [!UICONTROL Coûts]
   * [!UICONTROL  Utilisation du plan ]
   * Utilisation des rôles de tâche
   * [!UICONTROL Valeur réseau]

* La copie d’une initiative qui a été créée par un import de projet ou qui a été publiée sur un projet au moins une fois a les implications suivantes :

   * Il ne duplique pas le projet associé à l’initiative.
   * Il ne connecte pas l’initiative copiée au projet.
   * Il ne modifie pas la section [!DNL Scenario Planner] du projet, pour les projets qui ont été publiés au moins une fois.

  Pour plus d’informations sur la publication d’initiatives dans des projets, voir [Mise à jour ou création de projets en publiant des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

  Pour plus d’informations sur la création d’initiatives par l’importation de projets, voir [Importation de projets dans des plans dans  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## Copie d’initiatives

1. Cliquez sur l&#39;icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png), puis sur [!UICONTROL Scénarios].

   Une liste des plans s’affiche.

1. Cliquez sur le nom d’un plan pour l’ouvrir, puis localisez les initiatives que vous souhaitez copier.
1. Sélectionnez la zone située à gauche de l’initiative ou des initiatives que vous souhaitez copier, puis cliquez sur **[!UICONTROL Copier]** dans le menu qui s’affiche au bas du plan.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] copie immédiatement les initiatives et les place sous la dernière initiative sélectionnée.

   Le nom de l’initiative copiée est *[!UICONTROL Copie de]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Selon l’emplacement où vous insérez les nouvelles initiatives, le nombre d’initiatives existantes peut changer.

1. Mettez à jour le nom de l’initiative copiée.

   >[!TIP]
   >
   >Nous vous recommandons de toujours mettre à jour le nom de l’initiative afin d’éviter toute confusion si vous souhaitez les copier à nouveau.

1. (Facultatif) Mettez à jour la priorité de vos nouvelles initiatives.

   Pour plus d’informations sur la hiérarchisation des initiatives, voir [Mise à jour des priorités des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.
