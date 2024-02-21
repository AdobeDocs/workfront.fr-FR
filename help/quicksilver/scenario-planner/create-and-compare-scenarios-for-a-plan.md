---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Créer et comparer des scénarios de plan dans le planificateur de scénarios
description: Lorsque vous planifiez la stratégie à long terme de votre entreprise, il y a de nombreuses informations dont vous ne disposez pas ou auxquelles vous ne pensez pas au début. Il faut du temps et de l’expérience pour arriver à une stratégie finale que vos parties prenantes peuvent accepter. La réalisation d’une analyse "et si" afin de créer plusieurs scénarios pour votre plan peut vous aider à prévoir et évaluer précisément les circonstances potentielles et, en fin de compte, à élaborer le meilleur plan possible.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 296de69a1c444659c60bcf767bdacdd9e6e36830
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 1%

---

# Créez et comparez des scénarios de plan dans la section [!DNL Scenario Planner]

Lorsque vous planifiez la stratégie à long terme de votre entreprise, il y a de nombreuses informations dont vous ne disposez pas ou auxquelles vous ne pensez pas au début. Il faut du temps et de l’expérience pour arriver à une stratégie finale que vos parties prenantes peuvent accepter. La réalisation d’une analyse &quot;et si&quot; afin de créer plusieurs scénarios pour votre plan peut vous aider à prévoir et évaluer précisément les circonstances potentielles et, en fin de compte, à élaborer le meilleur plan possible.

## Exigences d’accès

Vous devez disposer des éléments suivants :

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
   <td> <p>Modifiez l’accès ou au-delà de la fonction [!DNL Scenario Planner]</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorisations d’objet</strong> </p> </td> 
   <td> <p>Autorisations [!UICONTROL Gérer] pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Demandez l’accès à un plan dans la [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Création de scénarios

Un scénario est une copie d’un plan. Vous pouvez créer autant de scénarios que nécessaire. Cependant, nous vous recommandons de limiter le nombre de scénarios afin de pouvoir facilement les comparer.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png), puis cliquez sur [!UICONTROL Scénarios].

1. Créez un plan.

   Pour plus d’informations sur la création de plans, voir [Créez et modifiez des plans dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Le premier plan que vous créez est automatiquement enregistré comme &quot;&quot;[!UICONTROL Scénario initial].&quot;

1. Cliquez sur la flèche pointant vers le bas en regard d’un scénario existant, puis cliquez sur le bouton **[!UICONTROL Copier]** Icône

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   Un nouveau scénario est ainsi créé avec les mêmes informations que le scénario copié. Il est automatiquement nommé &quot;[!UICONTROL Scénario 2]&quot; si c&#39;est le deuxième scénario de votre plan, &quot;[!UICONTROL Scénario 3]&quot; s’il s’agit du troisième, etc. Vous ne pouvez pas renommer vos scénarios. Le nombre de copies que vous pouvez effectuer n’est pas limité.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. Mettez à jour votre nouveau scénario de l’une des manières suivantes :

   * Créer, mettre à jour ou supprimer des initiatives

     >[!TIP]
     >
     >Lorsque vous supprimez une initiative dans un scénario, elle n’est supprimée que du scénario sélectionné, et non de tous les scénarios.

     Pour plus d’informations sur la création d’initiatives, voir [Créez et modifiez des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Mettre à jour les priorités de vos initiatives
   * Ajuster les informations sur les personnes ou les budgets
   * Réviser et ajuster les conflits d’initiative dans votre scénario

     Pour plus d’informations sur la résolution des conflits, voir [Résoudre les conflits d’initiative dans les [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.

## Comparer les scénarios

Après avoir créé vos scénarios, vous pouvez les comparer afin d’en trouver le meilleur pour votre entreprise.

1. Accédez au plan pour lequel vous souhaitez comparer des scénarios.
1. Cliquez sur **[!UICONTROL Comparaison de scénarios]**. La page de comparaison des scénarios s’affiche.

   Tous les scénarios existants pour le plan s’affichent côte à côte. Le scénario initial est toujours répertorié en premier et il est statique.

   ![](assets/scenario-cards-overlapping-350x166.png)

1. (Facultatif) Faites défiler l’écran vers la droite pour afficher toutes les cartes de scénario.

   Les informations suivantes s’affichent sur une carte de scénario :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nom du scénario</td> 
      <td> <p>Un nom généré automatiquement par Workfront et ne peut pas être modifié. Par exemple, "[!UICONTROL Scénario initial]", "[!UICONTROL Scénario 2]", etc. </p> </td> 
     </tr> 
     <tr> 
      <td>Description du scénario</td> 
      <td>Entrée manuelle où vous pouvez décrire les détails du scénario. </td> 
     </tr> 
     <tr> 
      <td>Rôles de tâche disponibles</td> 
      <td>Nombre de rôles d’emploi disponibles dans le budget du plan pour la durée du plan. </td> 
     </tr> 
     <tr> 
      <td>Fonctions requises</td> 
      <td>Nombre de rôles d’emploi requis, en fonction de vos initiatives. </td> 
     </tr> 
     <tr> 
      <td>Budget</td> 
      <td>Le budget total défini pour le plan dans ce scénario. Pour plus d’informations sur le budget, voir <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Présentation des plans dans [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Coûts</td> 
      <td>Les coûts associés aux initiatives dans le scénario. Pour plus d’informations sur les coûts, voir <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Aperçu des initiatives dans la section [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Utilisation</td> 
      <td>Pourcentage d’[!UICONTROL utilisation du budget] pour le plan dans ce scénario. Pour plus d’informations sur le pourcentage d’[!UICONTROL utilisation du budget], voir <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Présentation des plans dans [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Valeur nette</td> 
      <td>La [!UICONTROL Valeur nette] du plan dans ce scénario. Pour plus d’informations sur la [!UICONTROL Valeur nette] d’un plan, voir <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Présentation des plans dans [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Initiatives</td> 
      <td>Nombre d’initiatives pour le plan dans ce scénario.</td> 
     </tr> 
     <tr> 
      <td>Conflit</td> 
      <td>Le nombre d’initiatives qui montrent tout type de conflit dans le plan pour ce scénario. Pour plus d’informations sur les conflits d’initiatives, voir <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">Résoudre les conflits d’initiative dans les [!DNL Scenario Planner]</a>. </td> 
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
   >Par exemple, le budget, le nombre de rôles d’emploi et le nombre d’initiatives peuvent changer d’un scénario à l’autre.

1. Cliquez sur le nom d&#39;un scénario pour y accéder et y apporter des modifications.

   Pour plus d’informations, voir [Création de scénarios](#create-scenarios) dans cet article.

1. Cliquez sur **[!UICONTROL Ajouter une description]** pour ajouter une description pour le scénario

   Ou

   Cliquez sur le champ de description pour le mettre à jour, puis cliquez n’importe où à l’écran pour enregistrer vos modifications.

1. (Facultatif) Cliquez sur le **[!UICONTROL Plus]** menu ![](assets/more-icon.png) to **[!UICONTROL Copier]** ou **[!UICONTROL Supprimer]** le scénario.

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   Lorsque vous copiez un scénario, il apparaît automatiquement sur la page de carte et est renommé selon ce modèle : &quot;[!UICONTROL Scénario] `<next number in order>`.&quot;

1. (Conditionnel) Si vous avez cliqué sur **[!UICONTROL Supprimer]**, cliquez sur **[!UICONTROL Oui, supprimez-le.]** pour confirmer.

   Les scénarios supprimés ne peuvent pas être récupérés.

   Pour plus d’informations sur la suppression de scénarios, voir [Suppression de plans dans la [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos scénarios et votre plan.
