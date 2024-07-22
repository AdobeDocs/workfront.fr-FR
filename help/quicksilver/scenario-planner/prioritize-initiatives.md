---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mettre à jour des priorités d’initiative dans le planificateur de scénarios
description: Il est important de donner la priorité aux initiatives parce que celles-ci reçoivent des rôles d'emploi et des ressources budgétaires du plan dans l'ordre où elles sont répertoriées dans le plan.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 12%

---

# Mettez à jour les priorités des initiatives dans le [!DNL Scenario Planner]

Il est important de donner la priorité aux initiatives parce que celles-ci reçoivent des rôles d&#39;emploi et des ressources budgétaires du plan dans l&#39;ordre où elles sont répertoriées dans le plan.

Vous pouvez donner la priorité aux initiatives sur un plan que vous avez créé ou sur un plan que quelqu’un a partagé avec vous.

Pour plus d’informations sur la création de plans, voir [Création et modification de plans dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Pour plus d’informations sur la création d’initiatives, consultez la section [Créer et modifier des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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

## Mettre à jour les priorités des initiatives

Lorsque vous modifiez la priorité des initiatives, vous modifiez l’ordre de leur liste dans le plan.

Nous vous recommandons de placer les initiatives plus urgentes en haut d&#39;un plan et les plus fluides - qui pourraient être prises à tout moment et uniquement si des ressources sont disponibles - au bas du plan.

>[!NOTE]
>
>[!DNL Workfront] alloue des ressources de plan aux initiatives dans l’ordre dans lequel elles sont répertoriées dans le plan.
>
>Par exemple, si le plan comporte 3 ingénieurs disponibles et les initiatives 1 et 2, chacun a besoin de 2 ingénieurs pour se terminer et qu’ils sont tous deux planifiés pour la même période, Workfront associe 2 ingénieurs à l’initiative 1 et un ingénieur disponible restant à l’initiative 2. Dans ce cas, l&#39;Initiative 2 montre qu&#39;il y a un conflit, parce qu&#39;il lui manque un ingénieur. Parfois, changer la priorité de vos initiatives est la seule façon d&#39;éviter les conflits sur un plan.

Pour mettre à jour la priorité de l’initiative :

{{step1-to-scenario-planner}}

Une liste des plans s’affiche.

1. Cliquez sur le nom d’un plan pour l’ouvrir, puis localisez les initiatives que vous souhaitez prioriser.
1. Cliquez sur la case à gauche d&#39;un ou plusieurs noms d&#39;initiatives et effectuez l&#39;une des opérations suivantes :

   * Cliquez sur la poignée située à gauche de l’un des noms des initiatives sélectionnées, puis faites-le glisser vers le haut ou le bas de la liste pour modifier la priorité de l’initiative.

     Workfront affiche le nombre d’initiatives sélectionnées.

     ![](assets/multi-select-initiative-number.png)

   * Cliquez sur la zone **[!UICONTROL Prioriser]** au bas du plan, puis choisissez l’une des options suivantes :

      * **[!UICONTROL Top]** : déplace les initiatives sélectionnées en haut de la liste des initiatives. Les initiatives sélectionnées sont répertoriées en premier sur le plan.
      * **[!UICONTROL Bas]** : déplace les initiatives sélectionnées au bas de la liste des initiatives. Les initiatives sélectionnées sont répertoriées en dernier sur le plan.
      * **[!UICONTROL Sélectionner un nombre]** : déplace les initiatives sélectionnées après l’initiative que vous indiquez ici.

        ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] place immédiatement les initiatives sélectionnées à l’endroit où vous indiquez et le nombre de toutes les initiatives est mis à jour en conséquence.

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.
