---
product-area: projects;user-management
keywords: joindre,appliquer
navigation-topic: work-with-custom-forms
title: Ajouter un formulaire personnalisé à un objet
description: Vous pouvez ajouter un formulaire personnalisé existant à l’un des objets répertoriés ci-dessous. Un formulaire personnalisé contient des champs personnalisés dans lesquels vous pouvez stocker des informations sur l’objet.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 100%

---

# Ajouter un formulaire personnalisé à un objet

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Vous pouvez ajouter un formulaire personnalisé existant à l’un des objets répertoriés ci-dessous. Un formulaire personnalisé contient des champs personnalisés dans lesquels vous pouvez stocker des informations sur l’objet.

* Projets (y compris les business cases)
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
   <td> <p>Accès en modification aux objets pour lesquels vous gérez des formulaires personnalisés</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion sur l’objet pour lequel vous souhaitez joindre un formulaire personnalisé.</p> <p>Autorisations d’affichage ou supérieures sur le formulaire personnalisé, avec l’autorisation de <b>Joindre aux données personnalisées</b> des objets (projets, tâches et problèmes). Pour plus d’informations, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Partager un formulaire personnalisé</a>.</p> <p>Important : si vous ne disposez pas d’une licence de plan avec accès administratif aux formulaires personnalisés, vous devez disposer d’autorisations spécifiques pour au moins afficher le formulaire personnalisé, comme décrit dans la section <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Partager un formulaire personnalisé</a>. Ces autorisations doivent vous être accordées même si le formulaire est visible à l’échelle du système. </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Votre administrateur ou administratrice Workfront ou une personne disposant d’une licence de plan et d’un accès administratif aux formulaires personnalisés doit créer des formulaires personnalisés dans votre environnement avant que vous ne puissiez les ajouter aux objets. Pour plus d’informations, voir [Concevoir un formulaire à l’aide du créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Ajouter un formulaire personnalisé à un objet

Vous pouvez ajouter un formulaire personnalisé à un objet de deux manières :

* [Ajouter un formulaire personnalisé à un objet en modifiant l’objet](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Ajouter un formulaire personnalisé à un objet à partir de la zone Détails](#add-a-custom-form-to-an-object-from-the-details-area)

### Ajouter un formulaire personnalisé à un objet en modifiant l’objet {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Accédez à l’objet dans lequel vous souhaitez ajouter le formulaire personnalisé.
1. Cliquez sur le menu **Plus** ![](assets/more-icon.png), puis sur **Modifier** ![](assets/edit-icon.png).
1. Cliquez sur **Formulaires personnalisés** > **Ajouter des formulaires**, puis sélectionnez jusqu’à 10 formulaires dans le menu déroulant.

1. (Facultatif) Mettez à jour les informations dans les champs modifiables du formulaire personnalisé.

   Vous devez mettre à jour tous les champs obligatoires des formulaires que vous ajoutez.

1. Cliquer sur **Enregistrer**.

### Ajouter un formulaire personnalisé à un objet à partir de la zone Détails {#add-a-custom-form-to-an-object-from-the-details-area}

1. Accédez à l’objet dans lequel vous souhaitez ajouter le formulaire personnalisé.
1. Cliquez sur la section Détails **`<Object type>`** dans le panneau de gauche. Par exemple, cliquez sur **Détails du projet** pour ajouter des formulaires personnalisés à un projet ou **Détails du problème** pour ajouter des formulaires personnalisés à un problème.
1. Cliquez sur le champ **Ajouter un formulaire personnalisé** dans le coin supérieur droit, puis sélectionnez jusqu’à 10 formulaires personnalisés dans la liste qui s’affiche.

   Si le formulaire contient des champs obligatoires (marqués d’un astérisque rouge), il n’est pas nécessaire de les remplir pour l’instant.

   Les formulaires sélectionnés sont automatiquement joints à l’objet.

1. (Facultatif) Mettez à jour les informations dans les champs personnalisés du formulaire, puis cliquez sur **Enregistrer les modifications**.

## Plusieurs formulaires personnalisés sur un objet

Vous pouvez ajouter jusqu’à 10 formulaires personnalisés sur un objet donné, ce qui vous permet de rendre les champs disponibles pour certaines personnes et non pour d’autres, ou de mieux répondre aux exigences de formulaire de plusieurs projets.

**Exemple :** si un projet existant comporte déjà un formulaire personnalisé et que d’autres champs personnalisés sont nécessaires pour ce projet, qui existent sur un autre formulaire personnalisé, vous pouvez ajouter un deuxième formulaire au projet avec les champs supplémentaires, plutôt que d’ajouter les champs au formulaire personnalisé existant.

## Ajouter un formulaire personnalisé à plusieurs objets en masse

Vous pouvez ajouter des formulaires personnalisés à plusieurs objets en les sélectionnant dans une liste.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>L’ajout de formulaires personnalisés à des objets est identique pour tous les objets, à l’exception des projets.
>
>Pour plus d’informations sur l’ajout de formulaires personnalisés à des projets en masse, voir l’article [Modifier des projets](../../manage-work/projects/manage-projects/edit-projects.md).


1. Accédez à une liste d’objets.
1. Sélectionnez plusieurs objets dans la liste.

1. Cliquez sur le menu **Plus** ![](assets/more-icon.png), puis sur l’icône **Modifier** ![](assets/edit-icon.png).

   Ou

   Cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) en haut de la liste.
1. Cliquez sur **Formulaires personnalisés** dans le panneau de gauche.
1. Dans le menu déroulant **Effectuer une sélection**, sélectionnez le formulaire à associer à tous les objets sélectionnés.

   >[!NOTE]
   >
   >Si vous ne trouvez pas le formulaire dans le menu déroulant, cela signifie qu’au moins un des objets est déjà associé au formulaire. Déterminez de quel objet il s’agit et supprimez-le de votre sélection avant de pouvoir ajouter le formulaire aux objets restants.


1. Cliquez sur **Enregistrer les modifications**.

   Si le formulaire contient des champs obligatoires (marqués d’un astérisque rouge), il n’est pas nécessaire de les remplir pour l’instant.
