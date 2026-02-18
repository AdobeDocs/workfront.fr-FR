---
product-area: projects
navigation-topic: manage-projects
title: Copier un projet
description: Vous pouvez copier un projet plutôt que d’en créer un à partir de zéro. Vous pouvez copier un seul projet à la fois. Vous ne pouvez pas copier des projets en bloc.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 93db334537b5ec12dc0c77d51f8b2d83d8348f3d
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 59%

---

# Copier un projet

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

<!-- Audited: 5/2025 -->

Vous pouvez copier un projet à partir d’un projet existant plutôt que d’en créer un à partir de zéro, ce qui vous permet de gagner du temps.

Veuillez noter que vous ne pouvez pas copier des projets en bloc.

>[!IMPORTANT]
>
>Les éléments suivants ne sont jamais copiés d’un projet existant vers un nouveau :
>
>* Problèmes
>* Taux de facturation
>* Enregistrements de facturation
>* Notes
>* Heures
>* Projets transversaux antérieurs
>* Heures budgétées
>
>Les éléments suivants sont toujours copiés d’un projet existant vers un nouveau :
>
>* Tâches
>* Modèle
>* Risques
>* Informations sur la configuration de la file d’attente
>* Portfolio et programme
>* Carte de score
>* Informations par défaut sur la tâche (processus d’approbation par défaut de la tâche, formulaires personnalisés par défaut de la tâche)
>
> Les dates des tâches du projet d&#39;origine seront copiées dans le nouveau projet. Vous devez modifier la date de Début ou d&#39;Achèvement du projet (selon son Mode de planification) pour mettre à jour les dates des tâches. Les contraintes de tâche peuvent vous empêcher de modifier les dates du projet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.
Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Package Adobe Workfront</p> </td>  
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront</p> </td> 
   <td> <p>Standard</p> 
   <p>Plan</p>
      </td> 
  </tr> 
     <td>Configurations des niveaux d’accès </td> 
   <td> <p>Modifier l’accès aux projets avec la possibilité de Créer et de copier des projets</p> </td> 
  </tr>

<td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Accès en affichage ou accès supérieur au projet</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td> <p>New: Standard </p> 
   <p>Or</p>
   <p>Current: Plan </p>
   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configurations </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>View permissions or higher to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Considérations

* Le traitement est limité à 5 minutes lors de la copie d’un projet. Si le projet est associé à un grand nombre de documents et qu’il ne parvient pas à les copier, vous devrez peut-être supprimer certains des documents et réessayer.

## Copier un seul projet

La copie d’un projet copie également certaines informations du projet d’origine vers le nouveau projet. Vous pouvez également indiquer les éléments qui ne doivent pas être copiés dans le nouveau projet au cours du processus de copie.

Pour copier un projet :

{{step1-to-projects}}

1. Sélectionnez le projet à copier dans la liste des projets, puis cliquez sur l’icône **Plus** ![menu Plus](assets/more-icon.png) à droite du nom du projet.

   Ou

   Accédez à une liste ou à un rapport de projet et sélectionnez un projet, puis cliquez sur l’icône **Plus** ![Menu Plus](assets/more-icon.png) en haut de la liste.

1. Dans le menu déroulant **Plus**, cliquez sur **Copier**. La boîte de dialogue **Copie du [Nom du projet]** s’affiche.

1. (Facultatif) Mettez à jour le **nom du projet**. Par défaut, le nouveau nom est **Copie de [Nom original du projet]**.

   ![Zone Copier le projet](assets/copy-of-project-box.png)

1. Sélectionnez un **Statut**. Par défaut, le statut du projet d’origine est sélectionné.

1. (Facultatif) Désélectionnez les éléments que vous ne souhaitez pas copier dans le nouveau projet. Le tableau suivant décrit ce qui se passe lorsque vous désélectionnez les éléments :


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sélectionner tout</td> 
      <td> <p>Sélectionne toutes les options et efface tous les champs et objets répertoriés dans le nouveau projet. </p>

   <p> Désélectionner cette option désélectionne tous les éléments. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Affectations</td> 
      <td>Supprime toutes les affectations de projet et de tâche.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progression</td> 
      <td>Supprime la progression de toutes les tâches en les affichant comme étant Nouvelle. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Données personnalisées</td> 
      <td> <p>Supprime les informations du formulaire personnalisé sur le projet, ainsi que les informations sur les formulaires personnalisés associés aux éléments suivants :</p> 
       <ul> 
        <li>Tâches</li> 
        <li>Frais</li> 
        <li> Documents</li> 
       </ul> 
      <p>Les formulaires personnalisés restent joints aux tâches, dépenses, documents et projets, mais les informations contenues dans les champs personnalisés du formulaire ne sont pas copiées dans le nouveau projet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td> <p>Supprime tous les éléments de l’onglet Documents, y compris les versions de documents, les documents liés et les dossiers.</p> <p>Par défaut, les épreuves et les approbations de document ne peuvent pas être copiées vers un autre projet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toutes les tâches antérieures</td> 
      <td> <p>Supprime toutes les relations de tâche antérieure entre les tâches du projet. </p> <p>

   Les projets transversaux antérieurs ne sont jamais transférés vers le nouveau projet, que cela soit sélectionné ou non. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Heures budgétées</td> 
      <td> <p>Supprime les heures budgétées dans la zone Planification des ressources du business case du projet copié.</p> 
    <p>
   Les heures budgétées à l’aide du planificateur de scénarios ne sont jamais copiées vers le nouveau projet, car ce dernier n’est pas lié à une initiative dans le planificateur de scénarios. Pour plus d’informations, voir <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Budgétiser des ressources dans le business case à l’aide du planificateur de scénarios</a>.</p>
   </tr></td>
    <tr> 
      <td role="rowheader">Informations financières</td> 
      <td> <p>Supprime les informations dans les zones suivantes : </p> 
       <ul> 
        <li>Sous-onglet Finances du projet</li> 
        <li> Bénéfice prévu dans le business case</li> 
        <li>Informations financières de toutes les tâches<br></li> 
       </ul> <p>Pour plus d’informations sur le sous-onglet Finances du projet, voir <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref"> Gérer les informations dans la zone Finances du projet </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processus d’approbation</td> 
      <td>Supprime toutes les approbations associées aux tâches ou au projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td> Supprime les notifications de rappel associées aux tâches ou au projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td>Supprime les dépenses associées aux tâches ou au projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autorisations</td> 
      <td> Supprime les autorisations pour toutes les personnes des tâches ou du projet.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Copier le projet**. Le projet copié est créé.
