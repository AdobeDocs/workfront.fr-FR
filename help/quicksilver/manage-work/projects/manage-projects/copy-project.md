---
product-area: projects
navigation-topic: manage-projects
title: Copier un projet
description: Vous pouvez copier un projet plutôt que d’en créer un à partir de zéro. Vous ne pouvez copier qu’un seul projet à la fois. Vous ne pouvez pas copier des projets en bloc.
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 5%

---

# Copier un projet

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

Vous pouvez copier un projet plutôt que d’en créer un à partir de zéro. Vous ne pouvez copier qu’un seul projet à la fois. Vous ne pouvez pas copier des projets en bloc.

>[!IMPORTANT]
>
>Les éléments suivants ne sont jamais copiés d’un projet existant vers un nouveau :
>
>* Événements
>* Taux de facturation
>* Enregistrements de facturation
>* Notes
>* Heures
>* prédécesseurs sur plusieurs projets
>* Heures budgétées
>
>Les éléments suivants sont toujours copiés d’un projet existant vers un nouveau :
>
>* Tâches
>* Modèle
>* Risques
>* Informations sur la configuration de la file d’attente
>* Portfolio et programme
>* Carte de score
>* Informations par défaut sur la tâche (Processus d’approbation par défaut de la tâche, Forms personnalisé par défaut de la tâche)
>
> Les dates des tâches d’origine sur la copie des projets dans le nouveau projet. Vous devez modifier la date de début ou de fin du projet (en fonction de son mode de planification) pour mettre à jour les dates des tâches. Les contraintes de tâche peuvent vous empêcher de modifier les dates du projet.

## Exigences d’accès

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>Modifier l’accès aux projets avec la possibilité de créer <span>et Copier</span> projects</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorisations d’objet</strong> </p> </td> 
   <td> <p>Affichage des autorisations ou supérieures au projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Copier un seul projet

La copie d’un projet copie également certaines informations du projet d’origine vers le nouveau projet. Vous pouvez également spécifier les éléments qui ne doivent pas être copiés dans le nouveau projet au cours du processus de copie.

Pour copier un projet :

1. Accédez au projet à copier, puis cliquez sur le bouton **Plus** icon ![](assets/qs-more-menu.png) à droite du nom du projet

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Ou

   Accédez à une liste de projets ou à un rapport et sélectionnez un projet, puis cliquez sur le bouton **Plus** icon ![](assets/qs-more-menu.png) en haut de la liste.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Cliquez sur **Copier**.

1. Mettez à jour le nom du nouveau projet.

   Par défaut, le nouveau nom est **Copie de `<Original project name>`.**

   ![](assets/copy-project-box-nwe-350x276.png)

1. Sélectionnez la **État** pour le nouveau projet.

   Par défaut, la variable **État** correspond à celui du projet d’origine.

1. (Facultatif) Désélectionnez les éléments que vous ne souhaitez pas copier dans le nouveau projet. Le tableau suivant décrit ce qui se passe lorsque vous désélectionnez les éléments :


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sélectionner tout</td> 
      <td> <p>Sélectionne toutes les options et efface tous les champs et objets répertoriés dans le nouveau projet.</p> <p><b>CONSEIL</b>

   Désélection <strong>Tout sélectionner</strong> désélectionne tous les éléments. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Affectations</td> 
      <td>Supprime toutes les affectations de projet et de tâche</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progression</td> 
      <td>Supprime la progression de toutes les tâches et affiche la valeur Nouveau. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Données personnalisées</td> 
      <td> <p>Supprime les informations du formulaire personnalisé sur le projet, ainsi que les informations sur les formulaires personnalisés associés aux éléments suivants :</p> 
       <ul> 
        <li>Tâches</li> 
        <li>Frais</li> 
        <li> Documents</li> 
       </ul> <p><b>NOTE</b>

   Les formulaires personnalisés restent attachés aux tâches, dépenses, documents et projet, mais les informations contenues dans les champs personnalisés des formulaires ne sont pas copiées vers le nouveau projet. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td> <p>supprime tous les éléments de l’onglet documents, y compris les versions de documents, les documents liés et les dossiers.</p> <p>Par défaut, les BAT et les validations de document ne peuvent pas être copiés vers un autre projet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tous les prédécesseurs</td> 
      <td> <p>Supprime toutes les relations de prédécesseur entre les tâches du projet. </p> <p><b>CONSEIL</b>

   Les prédécesseurs sur plusieurs projets ne sont jamais transférés vers le nouveau projet, qu’il soit sélectionné ou non. </p> </td>
   </tr>

<tr> 
      <td role="rowheader">Heures budgétées</td> 
      <td> <p>Supprime les heures budgétées dans la zone Resource Planning de l’analyse de cas du projet copié.</p>

<b>NOTE</b>

Les heures budgétées à l’aide du planificateur de scénario ne sont jamais copiées vers le nouveau projet, car ce dernier n’est pas lié à une initiative dans le planificateur de scénario. Pour plus d’informations, voir <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">Budget des ressources dans l’analyse de cas à l’aide du planificateur de scénario</a>
</tr></td>
    <tr> 
      <td role="rowheader">Informations financières</td> 
      <td> <p>Supprime les informations dans les zones suivantes : </p> 
       <ul> 
        <li>Sous-onglet Finance du projet</li> 
        <li> Avantages prévus dans l’analyse de cas</li> 
        <li>Informations financières de toutes les tâches<br></li> 
       </ul> <p>Pour plus d’informations sur le sous-onglet Finance de projet, voir <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Gestion des informations dans la zone Finance du projet</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processus d'approbation</td> 
      <td>Supprime toutes les validations associées aux tâches ou au projet. </td> 
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
      <td> Supprime les autorisations pour tous les utilisateurs des tâches ou du projet.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Copier** pour créer une copie du projet.

   Cela crée un projet similaire au projet que vous avez copié.

   Vous pouvez commencer à apporter des modifications au nouveau projet copié, comme revoir les affectations de tâches ou ajuster les chronologies.
