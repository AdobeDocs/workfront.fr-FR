---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mettre à jour les priorités des initiatives dans le planificateur de scénarios
description: Il est important de hiérarchiser les initiatives parce que celles-ci reçoivent des fonctions et des ressources budgétaires d’un plan dans l’ordre où elles sont répertoriées dans celui-ci.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 88%

---

# Mettre à jour les priorités de l’initiative dans le [!DNL Scenario Planner]

Il est important de hiérarchiser les initiatives parce que celles-ci reçoivent des fonctions et des ressources budgétaires d’un plan dans l’ordre où elles sont répertoriées dans celui-ci.

Vous pouvez donner la priorité aux initiatives d’un plan que vous avez créé ou d’un plan qu’une personne a partagé avec vous.

Pour plus d’informations sur la création de plans, voir [Créer et modifier des plans dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Pour plus d’informations sur la création d’initiatives, voir [Créer et modifier des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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

Pour plus d’informations sur l’accès au planificateur de scénarios, voir [ Accès nécessaire pour utiliser le  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Documentation sur les exigences d’accès à Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--<table style="table-layout:auto"> 
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

## Mettre à jour les priorités des initiatives

Lorsque vous modifiez la priorité des initiatives, vous modifiez l’ordre dans lequel elles sont répertoriées dans un plan.

Nous vous recommandons de placer les initiatives plus urgentes en haut d’un plan et les plus fluides (qui pourraient être prises à tout moment et uniquement si des ressources sont disponibles) en bas du plan.

>[!NOTE]
>
>[!DNL Workfront] alloue les ressources du plan aux initiatives dans l’ordre dans lequel elles sont répertoriées dans le plan.
>
>Par exemple, si le plan comporte 3 personnes disponibles chargées de l’ingénierie et que les initiatives 1 et 2 ont chacune besoin de 2 personnes pour se terminer et qu’elles sont toutes les deux planifiées pour la même période, Workfront associe 2 personnes à l’initiative 1 tandis qu’une troisième reste disponible pour l’initiative 2. Dans ce cas, l’Initiative 2 montre qu’il y a un conflit, parce qu’il lui manque une personne chargée de l’ingénierie. Parfois, changer la priorité de vos initiatives est la seule façon d’éviter les conflits dans un plan.

Pour mettre à jour la priorité de l’initiative, procédez comme suit :

{{step1-to-scenario-planner}}

Une liste des plans s’affiche.

1. Cliquez sur le nom d’un plan pour l’ouvrir, puis localisez les initiatives pour lesquelles vous souhaitez définir une priorité.
1. Cliquez sur la case à gauche d’un ou de plusieurs noms d’initiatives et effectuez l’une des opérations suivantes :

   * Cliquez sur la poignée située à gauche de l’un des noms des initiatives sélectionnées, puis faites-le glisser vers le haut ou le bas de la liste pour modifier la priorité de l’initiative.

     Workfront affiche le nombre d’initiatives sélectionnées.

     ![Numéro d’initiative à sélection multiple](assets/multi-select-initiative-number.png)

   * Cliquez sur le bouton **[!UICONTROL Définir la priorité]** en bas du plan, puis choisissez l’une des options suivantes :

      * **[!UICONTROL En haut]** : déplace les initiatives sélectionnées en haut de la liste des initiatives. Les initiatives sélectionnées sont répertoriées en premier dans le plan.
      * **[!UICONTROL En bas]** : déplace les initiatives sélectionnées en bas de la liste des initiatives. Les initiatives sélectionnées sont répertoriées en dernier dans le plan.
      * **[!UICONTROL Sélectionner un nombre]** : déplace les initiatives sélectionnées après l’initiative que vous indiquez ici.

        ![Hiérarchiser les initiatives](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] place immédiatement les initiatives sélectionnées à l’endroit où vous les indiquez et le nombre de toutes les initiatives est mis à jour en conséquence.

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.
