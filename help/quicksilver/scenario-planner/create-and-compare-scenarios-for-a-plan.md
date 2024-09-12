---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Créer et comparer des scénarios de plan dans le planificateur de scénarios
description: Lorsque vous planifiez la stratégie à long terme de votre entreprise, il y a de nombreuses informations dont vous ne disposez pas ou auxquelles vous ne pensez pas au début. Il faut du temps et de l’expérience pour arriver à une stratégie finale que vos parties prenantes peuvent accepter. La réalisation d’une analyse d’hypothèses afin de créer plusieurs scénarios pour votre plan peut vous aider à prévoir et évaluer précisément les circonstances potentielles et, en fin de compte, à élaborer le meilleur plan possible.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 93%

---

# Créer et comparer des scénarios de plan dans le [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Lorsque vous planifiez la stratégie à long terme de votre entreprise, il y a de nombreuses informations dont vous ne disposez pas ou auxquelles vous ne pensez pas au début. Il faut du temps et de l’expérience pour arriver à une stratégie finale que vos parties prenantes peuvent accepter. La réalisation d’une analyse d’hypothèses afin de créer plusieurs scénarios pour votre plan peut vous aider à prévoir et évaluer précisément les circonstances potentielles et, en fin de compte, à élaborer le meilleur plan possible.

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
   <p>Le planificateur de scénario n’est pas disponible pour le nouveau plan Workfront Select ou Workfront. </p>
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

## Créer des scénarios

Un scénario est une copie d’un plan. Vous pouvez créer autant de scénarios que nécessaire. Cependant, nous vous recommandons de limiter le nombre de scénarios afin de pouvoir facilement les comparer.

{{step1-to-scenario-planner}}

1. Créez un plan ou cliquez sur le nom d&#39;un plan existant.

   Pour plus d’informations sur la création de plans, voir [Créer et modifier des plans dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Le premier plan que vous créez est automatiquement enregistré comme « [!UICONTROL Scénario initial] ».

1. Cliquez sur la flèche pointant vers le bas en regard d’un scénario existant, puis cliquez sur l’icône **[!UICONTROL Copier]**.

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   Un nouveau scénario est ainsi créé avec les mêmes informations que le scénario copié. Il est automatiquement nommé « [!UICONTROL Scénario 2] » si c’est le deuxième scénario de votre plan, « [!UICONTROL Scénario 3] » s’il s’agit du troisième, etc. Vous ne pouvez pas renommer vos scénarios. Le nombre de copies que vous pouvez effectuer n’est pas limité.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. Mettez à jour votre nouveau scénario de l’une des manières suivantes :

   * Créer, mettre à jour ou supprimer des initiatives

     >[!TIP]
     >
     >Lorsque vous supprimez une initiative dans un scénario, elle n’est supprimée que du scénario sélectionné, et non de tous les scénarios.

     Pour plus d’informations sur la création d’initiatives, voir [Créer et modifier des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Mettre à jour les priorités de vos initiatives
   * Ajuster les informations sur les personnes ou les budgets
   * Réviser et ajuster les conflits d’initiative dans votre scénario

     Pour plus d’informations sur la résolution des conflits, voir [Résoudre les conflits d’initiative dans le  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.

## Comparer les scénarios

Après avoir créé vos scénarios, vous pouvez les comparer afin de trouver le meilleur pour votre entreprise.

1. Accédez au plan pour lequel vous souhaitez comparer des scénarios.
1. Cliquez sur **[!UICONTROL Comparer les scénarios]**. La page de comparaison des scénarios s’affiche.

   Tous les scénarios existants pour le plan s’affichent côte à côte, au format carte. Le scénario initial est toujours répertorié en premier et il est statique.

   ![](assets/scenario-cards-overlapping-350x166.png)

1. (Facultatif) Faites défiler l’écran vers la droite pour afficher toutes les cartes de scénario.

   Les informations suivantes s’affichent sur une carte de scénario :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nom du scénario</td> 
      <td> <p>Nom généré automatiquement par Workfront, qui ne peut pas être modifié. Par exemple, « [!UICONTROL Initial scenario] », « [!UICONTROL Scenario 2] », etc. </p> </td> 
     </tr> 
     <tr> 
      <td>Description du scénario</td> 
      <td>Entrée manuelle dans laquelle vous pouvez décrire les détails du scénario. </td> 
     </tr> 
     <tr> 
      <td>Fonctions disponibles</td> 
      <td>Nombre de fonctions disponibles dans le budget de la formule pour la durée de la formule. </td> 
     </tr> 
     <tr> 
      <td>Fonctions requises</td> 
      <td>Nombre de fonctions requises, en fonction de vos initiatives. </td> 
     </tr> 
     <tr> 
      <td>Budget</td> 
      <td>Budget total défini pour la formule dans ce scénario. Pour plus d’informations budgétaires à propos des formules, voir la section <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Vue d’ensemble des formules dans [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Coûts</td> 
      <td>Les coûts associés aux initiatives dans le scénario. Pour plus d’informations sur les coûts, voir la section <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Vue d’ensemble des initiatives dans [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Utilisation</td> 
      <td>Pourcentage d’[!UICONTROL Budget Utilization] pour la formule dans ce scénario. Pour plus d’informations sur le pourcentage d’[!UICONTROL Budget Utilization], voir la section <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Vue d’ensemble des formules dans [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Valeur nette</td> 
      <td>La [!UICONTROL Net Value] de la formule dans ce scénario. Pour plus d’informations sur la [!UICONTROL Net Value] d’une formule, voir la section <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Vue d’ensemble des formules dans [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Initiatives</td> 
      <td>Nombre d’initiatives pour la formule dans ce scénario.</td> 
     </tr> 
     <tr> 
      <td>Conflit</td> 
      <td>Nombre d’initiatives qui montrent n’importe quel type de conflit dans la formule pour ce scénario. Pour plus d’informations sur les conflits d’initiatives, voir la section <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">Résoudre les conflits d’initiative dans [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Lorsque les informations diffèrent entre le scénario initial et les scénarios supplémentaires, une flèche vers le haut ou vers le bas s’affiche en regard de la valeur modifiée pour indiquer une augmentation ou une diminution de cette valeur par rapport au scénario initial.
   >
   >
   >![](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >Par exemple, le budget, le nombre de fonctions et le nombre d’initiatives peuvent changer d’un scénario à l’autre.

1. Cliquez sur le nom d’un scénario pour y accéder et y apporter des modifications.

   Pour plus d’informations, voir la section [Créer des scénarios](#create-scenarios) dans cet article.

1. Cliquez sur **[!UICONTROL Ajouter une description]** pour ajouter une description relative au scénario.

   Ou

   Cliquez sur le champ de description pour le mettre à jour, puis cliquez n’importe où à l’écran pour enregistrer vos modifications.

1. (Facultatif) Cliquez sur le menu **[!UICONTROL Plus]** ![](assets/more-icon.png) pour **[!UICONTROL Copier]** ou **[!UICONTROL Supprimer]** le scénario.

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   Lorsque vous copiez un scénario, il apparaît automatiquement sur la page de carte et est renommé selon ce modèle : « [!UICONTROL Scénario] `<next number in order>` ».

1. (Le cas échéant) Si vous avez cliqué sur **[!UICONTROL Supprimer]**, cliquez sur **[!UICONTROL Oui, supprimer]** pour confirmer.

   Les scénarios supprimés ne peuvent pas être récupérés.

   Pour plus d’informations sur la suppression des scénarios, voir la section [Supprimer des formules dans  [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Cliquez sur **[!UICONTROL Enregistrer la formule]** pour enregistrer vos scénarios et votre formule.
