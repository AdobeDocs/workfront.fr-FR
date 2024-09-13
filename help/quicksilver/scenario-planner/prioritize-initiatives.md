---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mettre à jour les priorités de l’initiative dans le planificateur de scénarios
description: Il est important de hiérarchiser les initiatives parce que celles-ci reçoivent des fonctions et des ressources budgétaires d’un plan dans l’ordre où elles sont répertoriées dans celui-ci.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 90%

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
   <td> <p>[!DNL Adobe Workfront] formule*</p> </td> 
   <td> <ul></li>
   <li><p>Nouveau : Ultimate </p></li>
   <p>Le planificateur de scénario n’est pas disponible pour les nouveaux plans Workfront Select ou Workfront Prime. </p>
   <li><p>Actuel : [!UICONTROL Business] ou de niveau supérieur</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence*</p> </td> 
   <td> <p>Nouveau : Light ou supérieur</p> 
   <p>Actuel : [!UICONTROL Révision] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td>Produit* </td> 
   <td> <ul><li><p>Pour les nouveaux plans Workfront :</p><p> Adobe Workfront</li></p>
   <li><p>Pour les plans Workfront actuels : </p>
   <p>Adobe Workfront</p> <p>Planificateur de scénarios Adobe Workfront</p></li></ul>

<p>Pour plus d’informations, voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Niveau d’accès </td> 
   <td> <p>Accès [!UICONTROL Edit] à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, consultez <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Demander l’accès à un plan dans le [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès à la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

     ![](assets/multi-select-initiative-number.png)

   * Cliquez sur le bouton **[!UICONTROL Définir la priorité]** en bas du plan, puis choisissez l’une des options suivantes :

      * **[!UICONTROL En haut]** : déplace les initiatives sélectionnées en haut de la liste des initiatives. Les initiatives sélectionnées sont répertoriées en premier dans le plan.
      * **[!UICONTROL En bas]** : déplace les initiatives sélectionnées en bas de la liste des initiatives. Les initiatives sélectionnées sont répertoriées en dernier dans le plan.
      * **[!UICONTROL Sélectionner un nombre]** : déplace les initiatives sélectionnées après l’initiative que vous indiquez ici.

        ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] place immédiatement les initiatives sélectionnées à l’endroit où vous les indiquez et le nombre de toutes les initiatives est mis à jour en conséquence.

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.
