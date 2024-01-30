---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Création d’une Fiche d’évaluation
description: Une fiche d’évaluation mesure si un projet s’aligne sur les critères précédemment établis d’un portefeuille. Une fiche d’évaluation reflète souvent la mission, les valeurs et les objectifs stratégiques d’une organisation. Les gestionnaires de Portfolios définissent généralement les questions et les réponses de la fiche d’évaluation afin de s’assurer qu’elles sont pertinentes et utiles lors de la définition des priorités et de la sélection du projet. Un [!DNL Adobe Workfront] L’administrateur crée les fiches d’évaluation en fonction des recommandations des gestionnaires de portefeuille.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Création d’une Fiche d’évaluation

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Une fiche d’évaluation mesure si un projet s’aligne sur les critères précédemment établis d’un portefeuille. Une fiche d&#39;évaluation reflète souvent la mission, les valeurs et les objectifs stratégiques d&#39;une organisation.

Les gestionnaires de Portfolios définissent généralement les questions et réponses de la fiche d’évaluation afin de s’assurer qu’elles sont significatives et utiles lors de la définition des priorités et de la sélection du projet. Un [!DNL Adobe Workfront] L’administrateur crée les fiches d’évaluation en fonction des recommandations des gestionnaires de portefeuille.

Les questions et réponses choisies pour une fiche d’évaluation doivent être quantifiables afin de fournir une valeur d’alignement pour comparer différents projets.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Actuel : [!UICONTROL Entreprise] ou version ultérieure</p> 
   Ou
   <p>Nouveau : [!UICONTROL Prime] ou version ultérieure</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>Actuel : formule [!UICONTROL]</p>
   Ou
   <p>Nouveau : [!UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

## Création d’une Fiche d’évaluation

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Fiches d’évaluation]**, puis cliquez sur **[!UICONTROL Nouvelle Fiche d’évaluation]** pour lancer le créateur de Fiche d’évaluation et créer une Fiche d’évaluation.

1. Spécifiez un **[!UICONTROL Nom de la Fiche d’évaluation]** et un **[!UICONTROL Description]**.

   Le nom s’affiche lorsque vous associez la fiche d’évaluation au projet. La description s’affiche en regard du nom de la fiche d’évaluation dans la liste de la fiche d’évaluation.

1. Cliquez sur le bouton **[!UICONTROL Ajouter une question]** pour ouvrir le [!UICONTROL question de la fiche d’évaluation] , puis indiquez les informations suivantes pour votre question :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Question]</td> 
      <td>Saisissez la question que vous souhaitez inclure dans la fiche d’évaluation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>Saisissez le nombre maximal de points possibles pour cette question.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points négatifs]</td> 
      <td>Sélectionnez cette option pour indiquer que [!DNL Workfront] doit soustraire au total des points possibles. Il n’est pas possible d’ajouter des scores négatifs au maximum possible d’une fiche d’évaluation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Display Type]</td> 
      <td>Sélectionner <strong>[!UICONTROL Value(0-100)]</strong> si vous souhaitez afficher un champ numérique dans la fiche d’évaluation où les utilisateurs peuvent spécifier une valeur comprise entre 0 et 100.<p>Ou, sélectionnez <strong>[!UICONTROL Liste déroulante]</strong> ou <strong>[!UICONTROL Boutons radio]</strong> pour créer une réponse, les utilisateurs peuvent spécifier à l'aide de ce contrôle. Cliquez sur <strong>[!UICONTROL Ajouter une réponse]</strong>, puis saisissez la variable <strong>[!UICONTROL Value]</strong> en points de pourcentage pour cette réponse, au cas où elle serait remplie. Si vous choisissez 100 %, le nombre de points attribués à cette question est entièrement atteint. Si vous souhaitez indiquer que cette réponse ne porte qu'une partie du montant total de points attribués à cette question, sélectionnez une valeur en pourcentage plus faible. Par exemple, si votre question est évaluée à 10 points et que vous souhaitez que cette réponse porte 5 de ces points, choisissez 50 % pour votre valeur.</p>
      <p>Sélectionner <strong>[!UICONTROL Par Défaut]</strong> si vous souhaitez indiquer que cette réponse est la réponse par défaut.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Ajouter une question]** pour ajouter d’autres questions et réponses à votre fiche d’évaluation, procédez comme suit.

   >[!NOTE]
   >
   >Vous pouvez réorganiser les questions de votre fiche d’évaluation en les faisant glisser et en les déposant dans le bon ordre.

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé de saisir toutes les informations.

   Cela crée la Fiche d’évaluation et les chefs de projet peuvent désormais la joindre à leur analyse de projet.

## Application d’une fiche d’évaluation à un projet

Un utilisateur avec [!UICONTROL gérer] les autorisations d’un projet peuvent appliquer une fiche d’évaluation à un projet, une fois la fiche d’évaluation créée par la fonction [!DNL Workfront] administrateur.

Une fiche d’évaluation est ajoutée à un projet dans le cadre de la création d’un dossier commercial pour le projet. Pour plus d’informations sur l’ajout d’une fiche d’évaluation à un projet, voir [Application d’une fiche d’évaluation à un projet et génération d’une note d’alignement](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Pour plus d’informations sur les autorisations de projet, voir [Partager un projet dans [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
