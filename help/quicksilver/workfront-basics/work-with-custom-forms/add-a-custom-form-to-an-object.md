---
product-area: projects;user-management
keywords: attach,apply
navigation-topic: work-with-custom-forms
title: Ajout d’un formulaire personnalisé à un objet
description: Vous pouvez ajouter un formulaire personnalisé existant à l’un des objets répertoriés ci-dessous. Un formulaire personnalisé contient des champs personnalisés dans lesquels vous pouvez stocker des informations sur l’objet.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# Ajout d’un formulaire personnalisé à un objet

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu .</span>

Vous pouvez ajouter un formulaire personnalisé existant à l’un des objets répertoriés ci-dessous. Un formulaire personnalisé contient des champs personnalisés dans lesquels vous pouvez stocker des informations sur l’objet.

* Projets (y compris les affaires)
* Tâches
* Événements
* Entreprises
* Portefeuilles
* Programmes
* Documents
* Utilisateurs
* Itérations
* Frais
* Enregistrements de facturation

Vous pouvez ajouter un formulaire personnalisé uniquement aux types d’objets pour lesquels le formulaire a été créé.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les actions décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux objets pour lesquels vous gérez des formulaires personnalisés</p> <p><b>NOTE</b></p>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérez les autorisations liées à l’objet pour lequel vous souhaitez joindre un formulaire personnalisé.</p> <p>Affichage ou autorisations supérieures du formulaire personnalisé, avec l’autorisation de <b>Joindre aux données personnalisées</b> objets (projets, tâches et problèmes). Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Partage d’un formulaire personnalisé</a>.</p> <p>Important : Si vous ne disposez pas d’une licence Plan avec accès administratif à Forms personnalisé, vous devez disposer d’autorisations spécifiques pour au moins afficher le formulaire personnalisé, comme décrit dans la section <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Partage d’un formulaire personnalisé</a>. Ces autorisations doivent vous être accordées même si le formulaire est visible à l’échelle du système. </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Condition requise

Votre administrateur Workfront ou un utilisateur disposant d’une licence Plan et d’un accès administratif à des formulaires personnalisés doit créer des formulaires personnalisés dans votre environnement avant de pouvoir les ajouter aux objets. Pour plus d’informations, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Ajout d’un formulaire personnalisé à un objet

Vous pouvez ajouter un formulaire personnalisé à un objet de deux manières :

* [Ajouter un formulaire personnalisé à un objet en modifiant l’objet](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Ajout d’un formulaire personnalisé à un objet à partir de la zone Détails](#add-a-custom-form-to-an-object-from-the-details-area)

### Ajouter un formulaire personnalisé à un objet en modifiant l’objet {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Accédez à l’objet dans lequel vous souhaitez ajouter le formulaire personnalisé.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-icon.png), puis cliquez sur **Modifier** ![](assets/edit-icon.png).
1. Cliquez sur **Forms personnalisée** > **Ajouter Forms**, puis sélectionnez jusqu’à 10 formulaires dans le menu déroulant.

1. (Facultatif) Mettez à jour les informations dans les champs modifiables du formulaire personnalisé.

   Vous devez mettre à jour tous les champs requis des formulaires que vous ajoutez.

1. Cliquer sur **Enregistrer**.

### Ajout d’un formulaire personnalisé à un objet à partir de la zone Détails {#add-a-custom-form-to-an-object-from-the-details-area}

1. Accédez à l’objet dans lequel vous souhaitez ajouter le formulaire personnalisé.
1. Cliquez sur le bouton **`<Object type>`Détails** dans le panneau de gauche. Par exemple, cliquez sur **Détails du projet** pour ajouter des formulaires personnalisés à un projet ou **Détails du problème** pour ajouter des formulaires personnalisés à un problème.
1. Cliquez sur le bouton **Ajouter un formulaire personnalisé** dans le coin supérieur droit, puis sélectionnez jusqu’à 10 formulaires personnalisés dans la liste qui s’affiche.

   Si le formulaire contient des champs obligatoires (marqués d’un astérisque rouge), il n’est pas nécessaire de les remplir pour l’instant.

   Les formulaires sélectionnés sont automatiquement joints à l’objet.

1. (Facultatif) Mettez à jour les informations dans les champs personnalisés du formulaire, puis cliquez sur **Enregistrer les modifications**.

## Plusieurs formulaires personnalisés sur un objet

Vous pouvez ajouter jusqu’à 10 formulaires personnalisés sur un objet donné, ce qui vous permet de rendre les champs disponibles pour certains utilisateurs et non pour d’autres, ou de mieux répondre aux exigences de formulaire de plusieurs projets.

**Exemple :** Si un projet existant comporte déjà un formulaire personnalisé et que d’autres champs personnalisés sont nécessaires sur un autre formulaire personnalisé, vous pouvez ajouter un deuxième formulaire au projet avec les champs supplémentaires, plutôt que d’ajouter les champs au formulaire personnalisé existant, si ces champs sont nécessaires uniquement pour ce projet.

## Ajouter un formulaire personnalisé à plusieurs objets en bloc

Vous pouvez ajouter des formulaires personnalisés à plusieurs objets en les sélectionnant dans une liste.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
><span class="preview">Pour plus d’informations sur l’ajout de formulaires personnalisés à des projets en bloc dans l’environnement Aperçu, reportez-vous à l’article [Modification de projets](../../manage-work/projects/manage-projects/edit-projects.md)</span>.


1. Accédez à une liste d’objets.
1. Sélectionnez plusieurs objets dans la liste.

1. Cliquez sur le bouton **Plus** menu ![](assets/more-icon.png), puis cliquez sur le bouton **Modifier** icon  ![](assets/edit-icon.png)ou cliquez simplement sur le bouton **Modifier** icon ![](assets/edit-icon.png).
1. Cliquez sur **Forms personnalisée** dans le panneau de gauche.
1. Sélectionnez le formulaire à associer à tous les objets sélectionnés dans la **Effectuer une sélection** menu déroulant.
   >[!NOTE]
   >
   >Si vous ne trouvez pas le formulaire dans le menu déroulant, cela signifie qu’au moins un des objets est déjà associé au formulaire. Déterminez l’objet qui vous intéresse et supprimez-le de votre sélection avant de pouvoir ajouter le formulaire aux objets restants.

1. Cliquez sur **Enregistrer les modifications**.

   Si le formulaire contient des champs obligatoires (marqués d’un astérisque rouge), il n’est pas nécessaire de les remplir pour l’instant.
