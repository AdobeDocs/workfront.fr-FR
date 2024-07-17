---
product-area: templates
navigation-topic: templates-navigation-topic
title: Créer un modèle à partir d’un projet
description: Vous pouvez créer des modèles lorsque vous enregistrez un projet existant en tant que modèle.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 37%

---

# Créer un modèle à partir d’un projet

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

Vous pouvez créer des modèles lorsque vous enregistrez un projet existant en tant que modèle.

Après avoir enregistré un projet existant en tant que modèle, vous pouvez utiliser le nouveau modèle pour créer de nouveaux projets. Cela simplifie et accélère le processus de création du projet.

>[!NOTE]
>
>Lors de l’enregistrement d’un projet en tant que modèle, les dates réelles des tâches et du projet ne sont pas enregistrées pour le modèle.
>
>Un modèle et ses tâches n’ont pas de dates réelles, mais plutôt une indication du jour (à partir duquel le projet peut démarrer) où une tâche peut commencer et le jour où la tâche devra être terminée. Lors de l’utilisation de modèles pour créer les projets futurs, les projets recevront des dates réelles. Pour plus d’informations, voir [Créer un projet](../create-projects/create-project.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux modèles</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures d’un projet </p> <p>Une fois le modèle créé, vous obtenez l’autorisation Gérer .</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Créer un modèle à partir d’un projet

1. Accédez au projet que vous souhaitez enregistrer en tant que modèle.
1. Cliquez sur le menu **Plus** ![](assets/qs-more-icon-on-an-object.png), puis sur **Enregistrer comme modèle**.
1. Indiquez les informations suivantes pour le modèle :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td>Nommez le modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Fournissez une description du modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est actif</td> 
      <td> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Oui</strong> : d’autres utilisateurs peuvent trouver le modèle et le joindre à des projets.</p> </li> 
        <li><strong>Non</strong> : les autres utilisateurs ne peuvent pas trouver le modèle et ne peuvent pas le joindre aux projets.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés</td> 
      <td>Utilisez la liste déroulante pour sélectionner les formulaires personnalisés à joindre au modèle. Si des formulaires personnalisés ont déjà été associés au projet, tous les champs de données de ces formulaires personnalisés s’affichent.<br>Vous pouvez inclure jusqu’à 10 formulaires personnalisés sur un seul modèle.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Gérer Forms** pour supprimer ou réorganiser les formulaires. Pour plus d’informations sur la suppression et la réorganisation des formulaires personnalisés sur le modèle, voir [Formulaires personnalisés](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Cliquez sur **Étape suivante.**
1. Dans la section **Options** , cochez la case en regard des informations que vous souhaitez effacer du modèle.

   ![](assets/save-as-template-options-step-350x109.png)

1. Cliquez sur **Étape suivante.**
1. Dans la section **Exclure** , sélectionnez les tâches à exclure du projet.

   ![](assets/save-as-template-exclude-350x205.png)

1. Cliquez sur **Terminer et enregistrer le modèle.**

   Votre modèle apparaît désormais dans la liste des modèles disponibles et peut être joint à un projet existant ou utilisé pour en créer un nouveau.

 
