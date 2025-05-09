---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Créer une carte de score
description: Une carte de performance permet de mesurer l’adéquation d’un projet avec les critères précédemment établis d’un portfolio. Une carte de performance reflète souvent la mission, les valeurs et les objectifs stratégiques d’une organisation. Les gestionnaires de portfolios définissent généralement les questions et les réponses de la carte de performance afin de s’assurer qu’elles sont significatives et utiles lors de la hiérarchisation et de la sélection des projets. Un administrateur ou une administratrice  [!DNL Adobe Workfront]  élabore les cartes de performance sur la base des recommandations des gestionnaires de portfolios.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 83%

---

# Créer une carte de performance

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Une carte de performance permet de mesurer l’adéquation d’un projet avec les critères précédemment établis d’un portfolio. Une carte de performance reflète souvent la mission, les valeurs et les objectifs stratégiques d’une organisation.

Les gestionnaires de portfolios définissent généralement les questions et les réponses de la carte de performance afin de s’assurer qu’elles sont significatives et utiles lors de la hiérarchisation et de la sélection des projets. Un administrateur ou une administratrice [!DNL Adobe Workfront] élabore les cartes de performance sur la base des recommandations des gestionnaires de portfolios.

Les questions et les réponses choisies pour une carte de performance doivent être quantifiables afin de fournir une valeur d’alignement pour comparer différents projets.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des droits d&#39;accès suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Nouveau : [!UICONTROL Prime] ou supérieur</p>
   <p>Actuel : [!UICONTROL Business] ou de niveau supérieur</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   <p>Actuelle : [!UICONTROL Plan]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une carte de performance

Vous pouvez créer une carte de performance à partir de zéro ou en copier une existante.

Pour créer une carte de performance à partir de zéro :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Cartes de performance]**, puis sur **[!UICONTROL Nouvelle carte de performance]**. La boîte **Nouvelle carte de performance** s’ouvre.

   <!--add screen shot at unshim-->

1. Indiquez un **[!UICONTROL nom de carte de performance]** et une **[!UICONTROL description]**.

   Le nom s’affiche lorsque vous associez la carte de performance au projet. La description s’affiche à côté du nom de la carte de performance dans la liste des cartes de performance.

1. Cliquez sur le menu déroulant **[!UICONTROL Ajouter une question]** pour ouvrir la section [!UICONTROL Question de carte de performance], puis indiquez les informations suivantes pour votre question :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Question]</td> 
      <td>Saisissez la question que vous souhaitez inclure dans la carte de performance.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>Inscrivez le maximum de points possibles pour cette question.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Negative Points]</td> 
      <td>Sélectionnez cette option pour indiquer que [!DNL Workfront] doit être soustrait du total des points possibles. Les scores négatifs ne peuvent pas être ajoutés au nombre maximum de points possibles d’une carte de performance.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Display Type]</td> 
      <td>Sélectionnez <strong>[!UICONTROL Value(0-100)]</strong> si vous souhaitez afficher un champ numérique dans la carte de performance où les utilisateurs et utilisatrices peuvent spécifier une valeur comprise entre 0 et 100.<p>Vous pouvez également sélectionner <strong>[!UICONTROL Drop Down]</strong> ou <strong>[!UICONTROL Radio Buttons]</strong> pour créer une réponse que les utilisateurs et utilisatrices peuvent spécifier à l’aide de ce contrôle. Cliquez sur <strong>[!UICONTROL Add Answer]</strong>, puis saisissez la <strong>[!UICONTROL Value]</strong> en points de pourcentage pour cette réponse, au cas où elle serait satisfaite. Si vous choisissez 100 %, le nombre de points attribués à cette question est entièrement atteint. Si vous souhaitez indiquer que cette réponse ne représente qu’une partie du total des points attribués à cette question, sélectionnez un pourcentage inférieur. Par exemple, si votre question est évaluée à 10 points et que vous souhaitez que cette réponse rapporte 5 de ces points, choisissez 50 % pour votre valeur.</p>
      <p>Sélectionnez <strong>[!UICONTROL Default]</strong> si vous souhaitez indiquer que cette réponse est celle par défaut.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Ajouter une question]** pour ajouter d’autres questions et réponses à votre carte de performance, en suivant les mêmes étapes.

   >[!NOTE]
   >
   >Vous pouvez réorganiser les questions dans votre carte de performance en faisant glisser les questions dans le bon ordre.

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé de saisir toutes les informations.

   La carte de performance est ainsi créée et les responsables de projet peuvent désormais l’annexer au business case de leur projet.

## Copier une carte de performance existante

Vous pouvez créer une carte de performance en copiant et en modifiant une carte existante.

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Cartes de performance]** dans le panneau de gauche.
1. Sélectionnez une carte de performance dans la liste, puis cliquez sur l’icône **Copier** ![Copier la carte de performance](assets/copy-scorecard-icon.png) en haut de la liste des cartes de performance.
La boîte de dialogue **Copier la carte de performance** s’ouvre.

   <!--add screen shot at unshim-->
1. Indiquez les informations suivantes :

   * **Carte de performance** : saisissez le nom de la carte de performance.  Par défaut, le nom est automatiquement mis à jour selon le format suivant :

     `Original scorecard name (Copy)`
   * **Description** : saisissez des informations supplémentaires sur la carte de performance.
1. Cliquer sur **Enregistrer**.

## Appliquer une carte de performance à un projet

Une personne ayant les permissions de [!UICONTROL gestion] sur un projet peut appliquer une carte de performance à un projet, après que la carte de performance a été créée par l’administrateur ou administratrice [!DNL Workfront].

Une carte de performance est ajoutée à un projet dans le cadre de la création d’un business case pour le projet. Pour plus d’informations sur l’ajout d’une carte de performance à un projet, voir [Appliquer une carte de performance à un projet et générer un score d’alignement](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Pour plus d’informations sur les autorisations relatives aux projets, voir [Partager un projet dans  [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).


