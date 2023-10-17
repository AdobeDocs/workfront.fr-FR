---
product-area: projects
navigation-topic: manage-tasks
title: Copier et dupliquer des tâches
description: Vous pouvez copier une tâche d’un projet vers un autre projet ou dupliquer une tâche au sein du même projet.
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 5db9a4869e1321bd268e80f786d157fbb41c0656
workflow-type: tm+mt
source-wordcount: '1727'
ht-degree: 1%

---

# Copier et dupliquer des tâches

Vous pouvez copier une tâche d’un projet vers un autre projet ou dupliquer une tâche au sein du même projet.

Vous pouvez copier ou dupliquer une ou plusieurs tâches ou tâches parentes à la fois.

## Exigences d’accès

<!-- drafted for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>Contribute or higher permissions to the project</p> 
   <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou plus élevé </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour une tâche </p> <p>Attribuer ou des autorisations supérieures au projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Observations relatives à la copie de tâches

Tenez compte des points suivants lors de la copie d’une tâche :

* Lorsque vous copiez une tâche d’un projet vers un autre, les dates de la tâche peuvent être recalculées. Le nouveau calcul prendra en compte le planning utilisé par le nouveau projet, ainsi que les informations de planification de projet.
* Les formulaires personnalisés sont copiés avec la tâche. Les informations contenues dans les champs personnalisés ne sont transférées aux tâches copiées que lorsque vous choisissez de copier les données personnalisées lors de la copie de la tâche.
* Vous avez la possibilité de choisir de copier certains éléments associés à la tâche dans la tâche copiée au cours du processus de copie. Cependant, par défaut, les objets suivants ne sont pas transférés vers la tâche copiée :
   * Problèmes
   * Heures consignées
   * Commentaires des utilisateurs <!--not sure about this, enable only if requested by users and verified by Product: System activity comments transfer to the new task if they relate to information that you specifically select to be copied. For example, if you select to copy Expenses to the new task, system comments that identify adding expenses to the task will transfer to the copied task. -->
* Par défaut, les éléments suivants sont déplacés vers la tâche copiée :

   * Les jalons sont transférés à la tâche copiée et supprimés de la tâche d’origine.
   * Transférer les sous-tâches vers la nouvelle tâche.

* Vous pouvez copier une tâche à la fois ou copier plusieurs tâches à la fois lorsque vous modifiez des tâches dans une liste.

## Copier des tâches dans une liste {#copy-tasks-in-a-list}

1. Accédez au projet contenant la ou les tâches à copier.

   Ou

   Accédez à un rapport de tâche.

1. (Conditionnel) Cliquez sur **Tâche** dans le panneau de gauche, si vous avez ouvert le projet qui contient les tâches.
1. Cliquez sur le bouton **Mode Plan** icon ![](assets/qs-list-mode-or-save-mode-icon-small.png), et assurez-vous que la variable **Enregistrement automatique** est activée.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Vous ne pouvez copier des tâches dans une liste que lors de l’enregistrement automatique des modifications. Pour plus d’informations sur l’enregistrement des options lors de la modification de tâches, voir [Editer les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Sélectionnez la ou les tâches à copier, puis effectuez l’une des opérations suivantes :

   * Cliquez sur le bouton **Plus de menu** en haut de la liste des tâches, puis cliquez sur **Copier vers**.
   * Cliquez avec le bouton droit sur les tâches sélectionnées, puis cliquez sur **Copier vers**.
   * Lorsque vous sélectionnez une tâche, cliquez sur le bouton **Plus** menu ![](assets/more-icon-task-list.png) en regard du nom de la tâche dans la liste, puis cliquez sur **Copier vers**.

   ![](assets/copy-task-in-list-nwe-350x131.png)

1. Poursuivez la copie de la tâche, comme décrit dans la section . [Copier une tâche au niveau de la tâche](#copy-a-task-at-the-task-level) à partir de l’étape 4.

   <!--
      (NOTE: is this still accurate?!)
   -->

## Copier une tâche au niveau de la tâche {#copy-a-task-at-the-task-level}

Outre la copie de tâches dans une liste de tâches, vous pouvez également copier une tâche une fois que vous l’avez ouverte.

1. Recherchez une tâche dans votre système Workfront en la recherchant.
1. Cliquez sur le nom de la tâche pour l’ouvrir.
1. Cliquez sur le bouton **Plus** menu déroulant ![](assets/qs-more-menu.png) en regard du nom de la tâche, puis cliquez sur **Copier** **to**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   La zone Copier la tâche s’affiche.

1. (Facultatif) Mettez à jour la variable **Task Name**.

   >[!TIP]
   >
   >Ce champ est grisé et ne peut pas être modifié lorsque vous sélectionnez plusieurs tâches dans une liste. Vous pouvez placer le pointeur de la souris sur le champ Nom de la tâche pour afficher la liste de toutes les tâches sélectionnées.
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. Saisissez le nom du **Projet de destination** où vous souhaitez copier la tâche dans le **Sélectionner le projet de destination** champ .

   >[!TIP]
   >
   >* Le nom du projet est sensible à la casse.
   >* Vous pouvez également commencer à saisir le numéro de référence ou saisir l’ID du projet. Cela peut vous aider à distinguer les projets portant des noms identiques.
   >* Seuls 100 projets s’affichent dans la liste.

   Le nom actuel du projet s’affiche par défaut. Si vous souhaitez copier la tâche dans le même projet, laissez ce champ inchangé.

1. (Conditionnel) Cliquez sur **accès aux demandes** pour demander l’accès au projet, si vous n’avez pas accès au projet sélectionné.
1. (Conditionnel) Continuez à copier la tâche vers le projet de destination sélectionné sans demander l’accès si vous avez accès à l’une des tâches du projet de destination.

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Des messages similaires s’affichent si le projet sélectionné est en attente d’approbation, terminé ou mort, lorsque l’administrateur de Workfront empêche l’ajout de tâches à ces projets. Pour plus d’informations, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Cliquez sur **Options** dans le panneau de gauche, désélectionnez les attributs de tâche que vous ne souhaitez pas copier avec la tâche. Toutes les options sont sélectionnées par défaut.

   >[!TIP]
   >
   >Sélection puis désélection **Tout sélectionner** désélectionne toutes les options.

   Désélectionnez les options suivantes pour ne pas les transférer vers la tâche copiée. Le tableau suivant décrit ce qui se produit lorsque les options sont désélectionnées :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Contrainte</td> 
      <td> <p>La contrainte de tâche est définie sur Dès que possible ou Aussi tard que possible en fonction du paramètre Mode de planification du projet.</p> <p> Lorsque cette option est sélectionnée, la contrainte actuelle de la tâche est transférée à la tâche copiée. </p> <p>Remarque : lorsque vous déplacez ou copiez une tâche avec des contraintes de date spécifiques à un autre projet et que les dates de contrainte de la tâche ne sont pas conformes aux dates du nouveau projet, la contrainte de tâche passe à Dès que possible ou Aussi Tard que possible ou les dates de début planifié ou de fin planifiée des projets sont ajustées. Certains exemples de contraintes spécifiques à une date sont : Doit démarrer le, Doit se terminer le, Ne pas démarrer plus tôt que, Ne pas démarrer plus tard que, etc. Pour plus d’informations sur les contraintes de tâche et sur la manière dont les contraintes de tâche ou les dates de projet peuvent être affectées, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Présentation de la contrainte de tâche</a> et recherchez une contrainte spécifique.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Affectations</td> 
      <td> <p>Toutes les affectations sont supprimées de la tâche. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processus d'approbation</td> 
      <td>Tous les processus de validation sont supprimés de la tâche.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progression</td> 
      <td>L’état de la tâche est Nouveau. Sinon, la tâche copiée conserve l’état de la tâche existante.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informations financières</td> 
      <td>Les informations financières de la tâche sont supprimées.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tous les prédécesseurs</td> 
      <td> <p>Cela signifie que les dépendances ne seront pas transférées aux tâches copiées. </p> <p>Lorsque cette option est sélectionnée, les prédécesseurs du groupe de tâches copiées sont conservés, d’autres sont supprimés.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td> <p>Les documents joints à la tâche ne sont pas transférés vers la tâche copiée. Cela inclut les versions, les bons à tirer et les documents liés.</p> <p>Cela ne comprend pas les approbations de documents. Les validations de document ne peuvent jamais être copiées lorsqu’une tâche est copiée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td>Les rappels de tâche ne sont pas transférés vers la tâche copiée. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td>Les dépenses enregistrées sur la tâche ne sont pas transférées vers la tâche copiée. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autorisations</td> 
      <td>Workfront supprime les noms de toutes les entités qui s'affichent dans la liste Partage de la tâche. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Données personnalisées</td> 
      <td> <p>Les valeurs des champs personnalisés sont effacées et les formulaires personnalisés sont transférés vers la tâche copiée. </p> <p>Lorsque cette option est sélectionnée, les formulaires et les valeurs des champs personnalisés sont transférés à la tâche copiée. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Cliquez sur **Sélectionner le parent** dans le panneau de gauche, sélectionnez la tâche dans le projet de destination que vous souhaitez devenir le parent de la tâche copiée.

   >[!TIP]
   >
   >Lorsque vous choisissez de copier plusieurs tâches dans une liste, toutes les tâches sélectionnées deviennent les enfants du parent sélectionné.

   Sélectionnez un parent en effectuant l’une des opérations suivantes :

   * Dans la liste des tâches, sélectionnez l’un des parents du plan de projet.
   * Cliquez sur l’icône de recherche ![Icône Rechercher](assets/search-icon.png) et recherchez une tâche parente par nom.

   La tâche s’affiche dans la liste.

   ![Sélectionner une tâche parente lors du déplacement d’une tâche avec une fonctionnalité de recherche ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Sélectionnez le bouton radio du parent une fois que vous l’avez trouvé.

   Si vous ne sélectionnez pas de tâche parent, les tâches sont copiées en tant que tâches principales plutôt que sous-tâches et elles sont placées à la fin de la liste des tâches sur le projet de destination.

1. Cliquez sur **Copier la tâche**

   Ou

   Cliquez sur **Copie de tâches** lorsque vous sélectionnez plusieurs tâches dans une liste.
Les tâches copiées se trouvent désormais sur le projet spécifié et sont soit des sous-tâches à la tâche parent sélectionnée, soit les dernières tâches du projet.

## Duplication de tâches

Vous pouvez rapidement dupliquer une tâche dans une liste de tâches, si vous avez besoin d’une tâche identique sur le même projet.

* [Considérations relatives à la duplication de tâches](#considerations-for-duplicating-tasks)
* [Duplication de tâches](#duplicate-tasks)

### Considérations relatives à la duplication de tâches {#considerations-for-duplicating-tasks}

* Vous ne pouvez dupliquer une tâche dans une liste de tâches que lorsque la liste est triée par numéro de tâche.
* La nouvelle tâche porte le même nom que la tâche d’origine.
* Vous ne pouvez pas sélectionner les informations qui sont dupliquées vers la nouvelle tâche. Presque toutes les informations de la tâche d’origine seront transférées par défaut à la tâche dupliquée, y compris la relation parent.
* Les éléments suivants ne sont pas transférés vers la nouvelle tâche :

   * Heures consignées
   * Notes
   * Problèmes
   * Seuls les prédécesseurs appartenant au même groupe de tâches copiées sont également copiés avec leurs tâches de remplacement.

     **EXEMPLE**

     Par exemple, si vous copiez simultanément la tâche 2 et son prédécesseur, la tâche 1, vous disposez d’une copie de la tâche 2 et d’une copie de la tâche 1. La copie de la tâche 1 sera le prédécesseur de la copie de la tâche 2. Mais si vous copiez uniquement la tâche 2 sans copier son prédécesseur, sa copie n’aura pas de prédécesseur.

* Lorsque vous dupliquez une tâche parent, toutes les tâches enfants sont également dupliquées, même si les tâches enfants ne sont pas sélectionnées.
* Vous pouvez dupliquer une ou plusieurs tâches en même temps.

  Cependant, vous ne pouvez pas dupliquer plusieurs tâches qui ne sont pas séquentielles en même temps.

* Les jalons sont déplacés vers la nouvelle tâche et supprimés de la tâche d’origine.

### Duplication de tâches

1. Accédez au projet contenant la ou les tâches que vous souhaitez dupliquer.
1. Cliquez sur **Tâche** dans le panneau de gauche.
1. Utilisez l’une des méthodes suivantes :

   * (Conditionnel) Cliquez sur le bouton **Mode Plan** icon ![](assets/qs-list-mode-or-save-mode-icon-small.png) et assurez-vous que **Enregistrement automatique** est activée, sélectionnez les tâches à dupliquer, puis cliquez sur le bouton **Plus de menu** ![](assets/qs-more-menu-29x11.png) > **Dupliquer**.

     ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * (Conditionnel) Cliquez sur le bouton **Mode Plan** icon ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Enregistrement manuel** > **Standard** ou **Planification chronologique**, puis procédez comme suit :

      1. Sélectionnez la ou les tâches à dupliquer, puis cliquez sur **Dupliquer**.
      1. (Facultatif) Cliquez sur **Annuler** pour annuler vos modifications et ne pas dupliquer les tâches.
      1. (facultatif et conditionnel) Cliquez sur **Rétablir** si vous avez précédemment cliqué **Annuler**, pour conserver les modifications et dupliquer les tâches.

      1. Cliquez sur **Enregistrer** pour enregistrer vos modifications.

         Les tâches sont dupliquées et ajoutées au même projet que les tâches d’origine.
