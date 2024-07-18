---
product-area: projects;user-management
keywords: attach,apply
navigation-topic: work-with-custom-forms
title: Ajouter un formulaire personnalisé à un objet
description: Vous pouvez ajouter un formulaire personnalisé existant à l’un des objets répertoriés ci-dessous. Un formulaire personnalisé contient des champs personnalisés dans lesquels vous pouvez stocker des informations sur l’objet.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 13%

---

# Ajouter un formulaire personnalisé à un objet

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Vous pouvez ajouter un formulaire personnalisé existant à l’un des objets répertoriés ci-dessous. Un formulaire personnalisé contient des champs personnalisés dans lesquels vous pouvez stocker des informations sur l’objet.

* Projets (y compris les affaires)
* Tâches
* Problèmes
* Entreprises
* Portefeuilles
* Programmes
* Documents
* Utilisateurs
* Itérations
* Frais
* Enregistrements de facturation

Vous pouvez ajouter un formulaire personnalisé uniquement aux types d’objets pour lesquels le formulaire a été créé.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Pour effectuer les actions décrites dans cet article, vous devez disposer de l’accès suivant :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Licence Adobe Workfront</td> 
  <td> <p>Nouvelle : contributeur ou contributrice ou supérieure </p>
 <p>ou</p> 
<p>Actuelle : demande ou supérieure </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux objets pour lesquels vous gérez des formulaires personnalisés</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérez les autorisations liées à l’objet pour lequel vous souhaitez joindre un formulaire personnalisé.</p> <p>Afficher ou des autorisations supérieures pour le formulaire personnalisé, avec l’autorisation de <b>Joindre aux objets de données personnalisées</b> (projets, tâches et problèmes). Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Partage d’un formulaire personnalisé</a>.</p> <p>Important : Si vous ne disposez pas d’une licence Plan avec accès administratif à Forms personnalisé, vous devez disposer d’autorisations spécifiques pour au moins afficher le formulaire personnalisé, comme décrit dans la section <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Partager un formulaire personnalisé</a>. Ces autorisations doivent vous être accordées même si le formulaire est visible à l’échelle du système. </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Votre administrateur Workfront ou un utilisateur disposant d’une licence Plan et d’un accès administratif à des formulaires personnalisés doit créer des formulaires personnalisés dans votre environnement avant de pouvoir les ajouter aux objets. Pour plus d’informations, voir [Concevoir un formulaire à l’aide du créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Ajouter un formulaire personnalisé à un objet

Vous pouvez ajouter un formulaire personnalisé à un objet de deux manières :

* [Ajoutez un formulaire personnalisé à un objet en modifiant l’objet](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Ajout d’un formulaire personnalisé à un objet à partir de la zone Détails](#add-a-custom-form-to-an-object-from-the-details-area)

### Ajouter un formulaire personnalisé à un objet en modifiant l’objet {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Accédez à l’objet dans lequel vous souhaitez ajouter le formulaire personnalisé.
1. Cliquez sur le menu **Plus** ![](assets/more-icon.png), puis sur **Modifier** ![](assets/edit-icon.png).
1. Cliquez sur **Forms personnalisée** > **Ajouter Forms**, puis sélectionnez jusqu’à 10 formulaires dans le menu déroulant.

1. (Facultatif) Mettez à jour les informations dans les champs modifiables du formulaire personnalisé.

   Vous devez mettre à jour tous les champs requis des formulaires que vous ajoutez.

1. Cliquer sur **Enregistrer**.

### Ajout d’un formulaire personnalisé à un objet à partir de la zone Détails {#add-a-custom-form-to-an-object-from-the-details-area}

1. Accédez à l’objet dans lequel vous souhaitez ajouter le formulaire personnalisé.
1. Cliquez sur la section **`<Object type>`Détails** dans le panneau de gauche. Par exemple, cliquez sur **Détails du projet** pour ajouter des formulaires personnalisés à un projet ou sur **Détails du problème** pour ajouter des formulaires personnalisés à un problème.
1. Cliquez sur le champ **Ajouter un formulaire personnalisé** dans le coin supérieur droit, puis sélectionnez jusqu’à 10 formulaires personnalisés dans la liste qui s’affiche.

   Si le formulaire contient des champs obligatoires (marqués d’un astérisque rouge), il n’est pas nécessaire de les remplir pour l’instant.

   Les formulaires sélectionnés sont automatiquement joints à l’objet.

1. (Facultatif) Mettez à jour les informations dans les champs personnalisés du formulaire, puis cliquez sur **Enregistrer les modifications**.

## Plusieurs formulaires personnalisés sur un objet

Vous pouvez ajouter jusqu’à 10 formulaires personnalisés sur un objet donné, ce qui vous permet de rendre les champs disponibles pour certains utilisateurs et non pour d’autres, ou de mieux répondre aux exigences de formulaire de plusieurs projets.

**Exemple :** Si un projet existant comporte déjà un formulaire personnalisé et que d’autres champs personnalisés sont nécessaires pour ce projet, qui existent sur un autre formulaire personnalisé, vous pouvez ajouter un second formulaire au projet avec les champs supplémentaires, plutôt que d’ajouter les champs au formulaire personnalisé existant.

## Ajouter un formulaire personnalisé à plusieurs objets en bloc

Vous pouvez ajouter des formulaires personnalisés à plusieurs objets en les sélectionnant dans une liste.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>L’ajout de formulaires personnalisés à des objets est identique pour tous les objets, à l’exception des projets.
>
>Pour plus d’informations sur l’ajout en masse de formulaires personnalisés à des projets, reportez-vous à l’article [Modification de projets](../../manage-work/projects/manage-projects/edit-projects.md).


1. Accédez à une liste d’objets.
1. Sélectionnez plusieurs objets dans la liste.

1. Cliquez sur le menu **Plus** ![](assets/more-icon.png), puis sur l&#39;icône **Modifier** ![](assets/edit-icon.png).

   Ou

   Cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) en haut de la liste.
1. Cliquez sur **Formulaires personnalisés** dans le panneau de gauche.
1. dans le menu déroulant **Effectuer une sélection** , sélectionnez le formulaire à associer à tous les objets sélectionnés.

   >[!NOTE]
   >
   >Si vous ne trouvez pas le formulaire dans le menu déroulant, cela signifie qu’au moins un des objets est déjà associé au formulaire. Déterminez l’objet qui vous intéresse et supprimez-le de votre sélection avant de pouvoir ajouter le formulaire aux objets restants.


1. Cliquez sur **Enregistrer les modifications**.

   Si le formulaire contient des champs obligatoires (marqués d’un astérisque rouge), il n’est pas nécessaire de les remplir pour l’instant.
