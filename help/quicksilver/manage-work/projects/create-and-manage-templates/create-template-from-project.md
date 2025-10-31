---
product-area: templates
navigation-topic: templates-navigation-topic
title: Créer un modèle à partir d’un projet
description: Vous pouvez créer des modèles lorsque vous enregistrez un projet existant en tant que modèle.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 60%

---

# Créer un modèle à partir d’un projet

<!--Audited: 10/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

Vous pouvez créer des modèles lorsque vous enregistrez un projet existant en tant que modèle.

Après avoir enregistré un projet existant en tant que modèle, vous pouvez utiliser le nouveau modèle pour créer des projets. Cela simplifie et accélère le processus de création du projet.

>[!NOTE]
>
>Lors de l’enregistrement d’un projet en tant que modèle, les dates réelles des tâches et du projet ne sont pas enregistrées pour le modèle.
>
>Un modèle et ses tâches n’ont pas de dates réelles, mais plutôt une indication du jour (à partir duquel le futur projet pourrait démarrer) où une tâche pourrait démarrer et du jour où la tâche doit s’achever. Lors de l’utilisation de modèles pour créer les futurs projets, les projets recevront des dates réelles. Pour plus d’informations, voir [Créer un projet](../create-projects/create-project.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux modèles</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou de niveau supérieur sur un projet </p> <p>Lorsque vous créez un modèle, vous obtenez l’autorisation Gérer.</p></td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you create it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Créer un modèle à partir d’un projet

1. Accédez au projet que vous souhaitez enregistrer en tant que modèle.
1. Cliquez sur le menu **Plus** ![icône Plus](assets/more-icon.png), puis sur **Enregistrer en tant que modèle**.
1. Indiquez les informations suivantes pour le modèle :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom de modèle</td> 
      <td>Attribuez un nom au modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Fournissez une description du modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est active</td> 
      <td> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Oui</strong> : d’autres utilisateurs et utilisatrices peuvent trouver le modèle et le joindre à des projets.</p> </li> 
        <li><strong>Non</strong> : les autres utilisateurs et utilisatrices ne peuvent pas trouver le modèle et ne peuvent pas le joindre aux projets.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Formulaires personnalisés** dans le panneau de gauche.
1. Cliquez sur le champ **Ajouter un formulaire personnalisé** et commencez à saisir le nom d’un projet personnalisé pour ou sélectionnez-en un dans la liste.

   Si des formulaires personnalisés sont déjà associés au projet, toutes les informations contenues dans les champs existants de ces formulaires personnalisés s’affichent dans les formulaires.

   Vous pouvez inclure jusqu’à 10 formulaires personnalisés sur un seul modèle.

1. Pointez sur le nom d’un formulaire, puis cliquez pour le faire glisser et le déposer à un nouvel emplacement.

   ![Enregistrer le projet en tant que modèle prêt à l’emploi](assets/save-project-as-template-top-of-the-form.png)

1. Cliquez sur **Options** dans le panneau de gauche, puis sélectionnez les champs ou les éléments à transférer au modèle.

   Tous les éléments sont cochés par défaut. Les éléments désélectionnés ne sont pas transférés vers le modèle.

   ![Options Enregistrer en tant que modèle ](assets/save-project-as-template-options-area.png)

1. Cliquez sur **Exclure** dans le panneau de gauche, puis sélectionnez les tâches à exclure du projet.

   ![Enregistrer en tant que modèle à exclure](assets/save-project-as-template-exclude-area.png)

1. Cliquez sur **Terminer et enregistrer le modèle**.

   Votre modèle apparaît désormais dans la liste des modèles disponibles. Les utilisateurs peuvent joindre le nouveau modèle à un projet existant ou l’utiliser pour créer un projet.


