---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Prise en main des résultats et des activités dans les objectifs d’Adobe Workfront
description: Vous devez ajouter des résultats, des activités ou des objectifs alignés à un objectif pour pouvoir l’activer. Cela met à jour l’état de l’objectif de Brouillon à Principal et commence à enregistrer la progression de l’objectif.
author: Alina
feature: Workfront Goals
exl-id: 64fa0aef-cb92-465a-9b74-d863fc232fd1
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Prise en main des résultats et des activités dans les objectifs d’Adobe Workfront

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>Votre entreprise doit disposer des éléments suivants pour utiliser les fonctionnalités décrites dans cet article :
>
>* A Pro ou version ultérieure [Formule Adobe Workfront](https://www.workfront.com/plans).
>* Une licence Adobe Workfront Goals en plus d’une licence Workfront.
>
>  Contactez votre gestionnaire de compte Workfront pour en savoir plus sur une licence Workfront Goals.
>
>Pour plus d’informations sur l’accès aux objectifs de Workfront, voir [Conditions requises pour utiliser les objectifs Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


Lorsque vous créez un objectif, celui-ci a l’état Brouillon. Pour plus d’informations sur la création d’objectifs, voir [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Pour commencer à enregistrer la progression sur un objectif, vous devez l’activer. Pour activer votre objectif et définir son état sur Principal, vous devez d’abord y ajouter les éléments suivants :

* Résultat
* Une activité
* Un projet
* Un objectif aligné

Une fois au moins l’un de ces éléments ajouté, vous pouvez activer l’objectif. Vous devez mettre à jour les résultats et les activités des objectifs pour indiquer la progression par rapport à l’objectif.


>[!IMPORTANT]
>
> Un objectif ne peut pas comporter plus de 1 000 activités, résultats, projets ou objectifs alignés.</span>

Cet article donne un aperçu des activités et des résultats. Pour plus d’informations sur l’alignement des objectifs, voir [Alignement des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-alignment/goal-alignment.md). Pour plus d’informations sur la connexion des projets aux objectifs, voir [Ajout de projets aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

## Présentation des résultats

<!--
<p> This will have additional types in the future - add another section for types?)</p>
-->

Les résultats mesurent la progression de votre objectif ou le degré auquel vous êtes près d’y parvenir. En tant que propriétaire de l’objectif, vous pouvez également posséder le résultat. Un résultat à votre objectif peut également être attribué à un autre utilisateur.

Pour plus d’informations sur l’ajout de résultats aux objectifs, voir [Ajout de résultats aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).

Vous pouvez ajouter des résultats à vos propres objectifs ou objectifs appartenant à d’autres entités de votre entreprise.

Tenez compte des points suivants lorsque vous utilisez les résultats :

* Ils répondent à la question : &quot;Comment saurai-je quand mon objectif sera atteint ?&quot;
* Il s’agit d’indicateurs de mesure. Vous pouvez sélectionner l’une des options suivantes pour indiquer la progression de votre résultat :

   <!--
  this might change (jira, Salesforce, etc))
  -->

   * Devise
   * Nombre
   * Pourcentage

Pour plus d’informations sur les résultats, consultez la liste des similitudes entre les résultats et les activités dans la section . [Similarités entre les résultats, les activités et les projets](#similarities-between-results-activities-and-projects) dans cet article.

## Présentation des activités

<!--
This will have additional types in the future - add another section for types?
-->

Les activités, comme les résultats, sont spécifiques et mesurables, et incluent généralement un indicateur de pourcentage complet. En tant que propriétaire de l’objectif, vous pouvez également posséder les activités associées à l’objectif. Une activité sur votre objectif peut également être affectée à un autre utilisateur.

Pour plus d’informations sur l’ajout d’activités à des objectifs, voir [Ajout d’activités aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

Tenez compte des points suivants lorsque vous associez des activités à vos objectifs :

* Ils répondent à la question : &quot;Qu&#39;est-ce que j&#39;atteindrai quand l&#39;objectif sera atteint ?&quot;
* Les activités sont des entrées personnalisées qui peuvent être considérées comme plus complètes ou incomplètes. Elles doivent être mises à jour manuellement pour indiquer le pourcentage de l’activité qui a été terminée jusqu’à présent.

<!--
* You can associate the following activities with goals:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Manual progress bar </td> 
     <td> <p>Custom entries that can be thought of more in terms of complete or incomplete. They must be manually updated.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><p>Project</p></td> 
     <td> <p>Existing projects that you have at least permissions to View and are not in a status of Dead. They are updated automatically, based on the progress of their work items. </p> <p>The projects must exist before associating them with the goal. You can associate a project with multiple goals. For information about adding projects to goals, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</p>
     <p><span class="preview">In the Preview environment, projects are separate progress indicators, independent from activities. Adding projects to a goal in the Preview environment is different from adding activities. For more information, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</span></p>
      </td> 
    </tr> 
   </tbody> 
  </table>
-->
<!--drafted for goal redesign: For THE PRODUCTION RELEASE: remove the projects in this article altogether.-->

Pour plus d’informations sur les résultats et les activités, consultez la liste des similitudes entre les résultats et les activités dans la section . [Similarités entre les résultats, les activités et les projets](#similarities-between-results-activities-and-projects) dans cet article.

## Similarités entre les résultats, les activités et les projets {#similarities-between-results-activities-and-projects}

Les résultats, les activités et les projets sont des indicateurs de progression des objectifs.

Il existe des différences dans la manière dont vous gérez les projets par rapport à la manière dont vous gérez les résultats et les activités. Pour plus d’informations sur l’ajout de projets à des objectifs, voir [Ajout d’activités aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md). Pour plus d’informations sur les projets liés aux objectifs, voir [Ajout de projets aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

Outre les résultats, les activités et les projets, vous pouvez associer des objectifs enfants à un objectif. Les objectifs pour les enfants sont également un type d’indicateur de progression pour un objectif. Pour plus d’informations, voir [Alignement des objectifs en les connectant aux objectifs Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md). La progression des indicateurs de progression de l&#39;objectif pour enfants détermine également la progression de l&#39;objectif parent.

Le tableau suivant affiche les similitudes et les différences entre les résultats, les activités et les projets, comme indicateurs d’objectif :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b><p>Fonctionnalité</p></b></td> 
   <td><b><p>Résultats</p></b></td> 
   <td><b><p>Activités</p></b></td> 
   <td> <p><strong>Projets</strong> </p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td><span style="font-weight: normal;">Vous pouvez personnaliser le nom de l’objet dans l’interface de Workfront</span> </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Vous pouvez les ajouter aux objectifs passés.</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Vous pouvez associer plusieurs résultats, activités ou projets avec le même objectif. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Vous pouvez associer l’un d’eux à plusieurs objectifs.</td> 
   <td> </td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Leur progression est prise en compte dans le calcul de la progression de l'objectif. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Ils doivent être mis à jour manuellement dans les objectifs Workfront</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Elles doivent se terminer à la date de fin de l’objectif.</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ils ne peuvent être affectés qu’à un utilisateur, et non à une équipe, à un groupe ou à une entreprise. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Elles sont spécifiques et mesurables et comprennent généralement des nombres définis qui indiquent leur progression. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Elles offrent une plage de valeurs entre les valeurs de début et de fin qui illustre la distance à laquelle vous êtes parvenu. La proximité avec la valeur de fin calcule une valeur de progression pour votre objectif. </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
 </tbody> 
</table>
