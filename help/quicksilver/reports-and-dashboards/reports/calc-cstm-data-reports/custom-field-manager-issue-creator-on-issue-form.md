---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Exemple de champ personnalisé calculé : afficher le responsable de l’auteur d’une publication sur le formulaire personnalisé de publication"
description: A l’aide d’un champ personnalisé calculé, vous pouvez afficher le nom du responsable de l’auteur d’une publication sur un formulaire personnalisé associé à la publication. En utilisant la même instruction, vous pouvez créer des champs calculés similaires pour les projets, problèmes et autres objets.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 28%

---

# Exemple de champ personnalisé calculé : afficher la personne responsable du créateur ou de la créatrice d’un problème dans le formulaire personnalisé du problème

A l’aide d’un champ personnalisé calculé, vous pouvez afficher le nom du responsable de l’auteur d’une publication sur un formulaire personnalisé associé à la publication. En utilisant la même instruction, vous pouvez créer des champs calculés similaires pour les projets, problèmes et autres objets.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Forfait Adobe Workfront*</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configurations des niveau d’accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés<br>Pour plus d’informations sur l’octroi de l’accès administratif depuis le niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref"> Octroi aux utilisateurs de l’accès administratif à certaines zones</a>.</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet</p> </td> 
   <td> <p>Accès Contribute à l’objet auquel le formulaire est joint avec accès à l’option Modifier le formulaire personnalisé</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher le responsable du créateur d’un problème sur le formulaire personnalisé de problème

Les étapes suivantes montrent comment créer un champ calculé pour un formulaire personnalisé de problème où vous pouvez capturer le nom du responsable de l’utilisateur qui a créé le problème. Le processus est identique lorsque vous souhaitez capturer le nom du responsable d’un utilisateur qui a créé une tâche, un projet, un portfolio, par exemple.

1. Créez un formulaire personnalisé Problème et ajoutez-lui un champ calculé.

   Pour plus d’informations sur la création d’un formulaire personnalisé et l’ajout de champs calculés à ce dernier, reportez-vous aux articles suivants :

   * [Concevoir un formulaire avec le créateur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Ajouter des champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Copiez et collez le code de mode texte suivant dans le champ **Calcul** du formulaire personnalisé :

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Les calculs de champs personnalisés sont sensibles à la casse.

1. Cliquez sur **Terminé**, puis **Enregistrer + Fermer**.

   Le gestionnaire de l’utilisateur qui a créé le problème s’affiche dans le champ calculé lorsque le formulaire contenant le champ est joint à un problème.
