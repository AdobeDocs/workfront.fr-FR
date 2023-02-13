---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mise à jour des priorités de l’initiative dans le planificateur de scénario
description: Il est important de donner la priorité aux initiatives parce que celles-ci reçoivent des rôles d'emploi et des ressources budgétaires du plan dans l'ordre où elles sont répertoriées dans le plan.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Mise à jour des priorités des initiatives dans [!DNL Scenario Planner]

Il est important de donner la priorité aux initiatives parce que celles-ci reçoivent des rôles d&#39;emploi et des ressources budgétaires du plan dans l&#39;ordre où elles sont répertoriées dans le plan.

Vous pouvez donner la priorité aux initiatives sur un plan que vous avez créé ou sur un plan que quelqu’un a partagé avec vous.

Pour plus d’informations sur la création de plans, voir [Créez et modifiez des plans dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Pour plus d’informations sur la création d’initiatives, voir [Créez et modifiez des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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
   <td> <p>Vous devez acheter une licence supplémentaire pour la variable [!DNL Adobe Workfront Scenario Planner] pour accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’obtention de [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser la variable [!DNL Scenario Planner]</a>. </p> </td> 
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

## Mettre à jour les priorités des initiatives

Lorsque vous modifiez la priorité des initiatives, vous modifiez l’ordre de leur liste dans le plan.

Nous vous recommandons de placer les initiatives plus urgentes en haut d&#39;un plan et les plus fluides - qui pourraient être prises à tout moment et uniquement si des ressources sont disponibles - au bas du plan.

>[!NOTE]
>
>[!DNL Workfront] alloue les ressources du plan aux initiatives dans l’ordre dans lequel elles sont répertoriées dans le plan.
>
>Par exemple, si le plan comporte 3 ingénieurs disponibles et les initiatives 1 et 2, chacun a besoin de 2 ingénieurs pour se terminer et qu’ils sont tous deux planifiés pour la même période, Workfront associe 2 ingénieurs à l’initiative 1 et un ingénieur disponible restant à l’initiative 2. Dans ce cas, l&#39;Initiative 2 montre qu&#39;il y a un conflit, parce qu&#39;il lui manque un ingénieur. Parfois, changer la priorité de vos initiatives est la seule façon d&#39;éviter les conflits sur un plan.

Pour mettre à jour la priorité de l’initiative :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png), puis cliquez sur [!UICONTROL Scénarios].

   Une liste des plans s’affiche.

1. Cliquez sur le nom d’un plan pour l’ouvrir, puis localisez les initiatives que vous souhaitez prioriser.
1. Cliquez sur la case à gauche d&#39;un ou plusieurs noms d&#39;initiatives et effectuez l&#39;une des opérations suivantes :

   * Cliquez sur la poignée située à gauche de l’un des noms des initiatives sélectionnées, puis faites-le glisser vers le haut ou le bas de la liste pour modifier la priorité de l’initiative.

      Workfront affiche le nombre d’initiatives sélectionnées.

      ![](assets/multi-select-initiative-number.png)

   * Cliquez sur le bouton **[!UICONTROL Définir la priorité]** au bas du plan, puis choisissez l’une des options suivantes :

      * **[!UICONTROL Haut]**: Déplace les initiatives sélectionnées en haut de la liste des initiatives. Les initiatives sélectionnées sont répertoriées en premier sur le plan.
      * **[!UICONTROL Bas]**: Déplace les initiatives sélectionnées au bas de la liste des initiatives. Les initiatives sélectionnées sont répertoriées en dernier sur le plan.
      * **[!UICONTROL Sélectionner un nombre]**: Déplace les initiatives sélectionnées après l’initiative que vous indiquez ici.

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] place immédiatement les initiatives sélectionnées à l’endroit où vous les indiquez et le nombre de toutes les initiatives est mis à jour en conséquence.


1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.
