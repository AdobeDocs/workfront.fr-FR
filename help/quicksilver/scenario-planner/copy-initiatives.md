---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copier des initiatives dans le planificateur de scénarios
description: Vous pouvez créer des initiatives en copiant des initiatives existantes. Vous pouvez copier des initiatives sur un plan que vous créez ou sur un plan que quelqu’un partage avec vous.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 14%

---

# Copiez les initiatives dans le [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Vous pouvez créer des initiatives en copiant des initiatives existantes. Vous pouvez copier des initiatives sur un plan que vous créez ou sur un plan que quelqu’un partage avec vous.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] forfait*</p> </td> 
   <td> <p>Actuel : [!UICONTROL Entreprise] ou version ultérieure</p>
   <p>Nouveau : Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence*</p> </td> 
   <td> <p>Nouveau : Léger ou supérieur</p> 
   <p>Actuel : [!UICONTROL Révision] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td>Produit* </td> 
   <td> 
   <p>Pour les plans Workfront actuels : </p>
   <p>Vous devez acheter une licence supplémentaire pour le [!DNL Adobe Workfront Scenario Planner] afin d’accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’accès et les autorisations pour [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser le [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Niveau d’accès </td> 
   <td> <p>Accès à l’accès à la fonction [!UICONTROL Modifier] [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Autorisations [!UICONTROL Gérer] pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Demander l’accès à un plan dans le [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès à la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

  Pour plus d’informations sur la création d’initiatives par import de projets, voir [Importer des projets dans des plans dans le  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Copie d’initiatives

{{step1-to-scenario-planner}}

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
