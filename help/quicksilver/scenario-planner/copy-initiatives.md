---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copier des initiatives dans le planificateur de scénarios
description: Vous pouvez créer des initiatives en copiant des initiatives existantes. Vous pouvez copier des initiatives sur un plan que vous créez ou sur un plan que quelqu’un partage avec vous.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 88%

---

# Copier des initiatives dans [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Vous pouvez créer des initiatives en copiant des initiatives existantes. Vous pouvez copier des initiatives sur un plan que vous créez ou sur un plan que quelqu’un partage avec vous.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] paquet</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTE</b></p>
<p>Contactez votre représentant Workfront si vous disposez d’un autre package Workfront.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence</p> </td> 
   <td> <p>[!UICONTROL Light] ou version ultérieure</p> 
   <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
    <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès [!UICONTROL Edit] à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour un plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur l’accès au planificateur de scénarios, voir [&#x200B; Accès nécessaire pour utiliser le  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Documentation sur les exigences d’accès à Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Copier des initiatives

Tenez compte des éléments suivants lorsque vous copiez des initiatives :

* Copier une initiative place la copie sur le même plan que l’initiative originale.
* Copier une initiative permet de copier et d’ajouter les informations suivantes de l’initiative originale à la nouvelle initiative :

   * [!UICONTROL Durée]
   * [!UICONTROL Fonctions]
   * [!UICONTROL Personnes] et [!UICONTROL Coûts fixes]
   * [!UICONTROL Bénéfice prévu]

* Copier une initiative peut modifier les informations suivantes pour le plan, si ces informations existent dans l’initiative originale :

   * Nombre requis de fonctions
   * [!UICONTROL Coûts]
   * [!UICONTROL Utilisation du plan]
   * Utilisation de la fonction
   * [!UICONTROL Valeur nette]

* Copier une initiative qui a été créée par l’import d’un projet ou qui a été publiée au moins une fois dans un projet a les implications suivantes :

   * Cette opération ne duplique pas le projet associé à l’initiative.
   * Elle ne connecte pas l’initiative copiée au projet.
   * Pour les projets qui ont été publiés au moins une fois, elle ne modifie pas la section du [!DNL Scenario Planner] sur le projet.

  Pour plus d’informations sur la publication d’initiatives dans des projets, consultez la section [Mettre à jour ou créer des projets en publiant des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

  Pour plus d’informations sur la création d’initiatives par l’import de projets, voir [Importer des projets dans des plans dans le  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Copier des initiatives

{{step1-to-scenario-planner}}

Une liste des plans s’affiche.

1. Cliquez sur le nom d’un plan pour l’ouvrir, puis localisez les initiatives que vous souhaitez copier.
1. Sélectionnez la case à gauche de l’initiative ou des initiatives que vous souhaitez copier, puis cliquez sur **[!UICONTROL Copier]** dans le menu qui apparaît au bas du plan.

   ![Copier l’initiative](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] copie immédiatement les initiatives et les place sous la dernière initiative sélectionnée.

   Le nom de l’initiative copiée est *[!UICONTROL Copie de]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Selon l’endroit où vous insérez les nouvelles initiatives, le nombre d’initiatives existantes peut changer.

1. Mettez à jour le nom de l’initiative copiée.

   >[!TIP]
   >
   >Nous vous recommandons de toujours mettre à jour le nom de l’initiative afin d’éviter toute confusion au cas où vous voudriez la copier à nouveau.

1. (Facultatif) Mettez à jour la priorité des initiatives nouvellement créées.

   Pour plus d’informations sur la hiérarchisation des initiatives, consultez la section [Mettre à jour les priorités des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.
