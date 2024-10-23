---
product-area: projects
navigation-topic: financials
title: Gérer les dépenses liées à un projet
description: Le processus de création et de gestion des dépenses est le même pour les dépenses liées à un projet ou à une tâche. Toutes les dépenses ajoutées au projet dans le business case sont ajoutées à l’onglet Dépenses en tant que dépenses prévues. Pour plus d’informations sur le business case, voir l’article Créer un business case pour un projet.
author: Alina
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 97%

---

# Gérer les dépenses liées à un projet

Le processus de création et de gestion des dépenses est le même pour les dépenses liées à un projet ou à une tâche. Toutes les dépenses ajoutées au projet dans le business case sont ajoutées à l’onglet Dépenses en tant que dépenses prévues. Pour plus d’informations sur le business case, voir l’article [Créer un business case pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Le montant total de vos dépenses pour toutes les tâches et le projet contribue au coût total du projet. Le montant prévu des dépenses contribue au coût prévu du projet, et le montant réel des dépenses contribue au coût réel du projet.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou supérieur </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en modification aux projets et aux données financières</p> <p><b>NOTE</b> </p>
   <p> Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de contribution ou de niveau supérieur sur le projet avec des autorisations d’affichage ou de gestion sur les finances</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

## Ajouter des frais

1. Accédez au projet pour lequel vous souhaitez saisir des dépenses.\
   Si vous souhaitez ajouter des dépenses à une tâche, accédez plutôt à une tâche. 
1. Cliquez sur **Afficher plus**, puis sur **Dépenses**.
1. Cliquez sur **Ajouter une dépense**.
La boîte de dialogue **Ajouter une dépense** s’affiche.
1. Mettez à jour les informations suivantes :

   * **Description :** description de la dépense.

   * **Type de dépense :** (obligatoire) sélectionnez la catégorie qui décrit le mieux la dépense.
   * **Tâche :** commencez à saisir le nom de la tâche à laquelle cette dépense est associée, puis cliquez dessus lorsqu’elle apparaît dans la liste déroulante.
   * **Montant prévu :** montant budgété prévu pour la dépense.\
     Cela affecte le coût budgété du projet.

   * **Montant réel :** ce que la dépense a réellement coûté.\
     Cela a une incidence sur le coût réel du projet.

   * **Date prévue :** date prévue à laquelle aura lieu la dépense. Vous pouvez saisir la date dans le champ en utilisant le format *mm/jj/aa*, ou vous pouvez cliquer sur l’icône du calendrier ![](assets/calendar-icon.png) et sélectionner la date de manière dynamique.

   * **Date du règlement :** date à laquelle la dépense a été payée.
   * **Facturable :** sélectionnez cette option si vous souhaitez facturer cette dépense. Il est important de classer une dépense dans la catégorie des dépenses facturables lors de la création d’enregistrements de facturation.
   * **Remboursable :** sélectionnez cette option si la dépense doit être remboursée. Vous pouvez ensuite marquer la dépense comme remboursée une fois le remboursement effectué.

1. Sélectionnez un **formulaire personnalisé** et spécifiez toute information supplémentaire requise. Vous devez créer un formulaire personnalisé avant de pouvoir l’associer à une dépense. Seuls les formulaires personnalisés actifs sont affichés dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, reportez-vous à l’article [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Cliquez sur **Enregistrer les modifications**.

## Supprimer des dépenses

1. Accédez au projet dans lequel vous souhaitez supprimer des dépenses.
1. Cliquez sur **Afficher plus**, puis cliquez sur **Dépenses**.
1. Sélectionnez les dépenses que vous souhaitez supprimer, puis cliquez sur **Supprimer** ![Supprimer](assets/delete.png).

1. Cliquez sur **Oui, supprimer** pour confirmer la suppression.
