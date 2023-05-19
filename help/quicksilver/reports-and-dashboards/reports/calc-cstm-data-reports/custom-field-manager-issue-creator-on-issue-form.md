---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Exemple de champ personnalisé calculé : afficher le responsable du créateur d’une publication sur le formulaire personnalisé de publication."
description: A l’aide d’un champ personnalisé calculé, vous pouvez afficher le nom du responsable de l’auteur d’une publication sur un formulaire personnalisé associé à la publication. En utilisant la même instruction, vous pouvez créer des champs calculés similaires pour les projets, problèmes et autres objets.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Exemple de champ personnalisé calculé : afficher le responsable du créateur d’une publication sur le formulaire personnalisé de publication ;

A l’aide d’un champ personnalisé calculé, vous pouvez afficher le nom du responsable de l’auteur d’une publication sur un formulaire personnalisé associé à la publication. En utilisant la même instruction, vous pouvez créer des champs calculés similaires pour les projets, problèmes et autres objets.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td>Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés<br>Pour plus d’informations sur l’octroi de l’accès administrateur à partir du niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet</p> </td> 
   <td> <p>Accordez l’accès à l’objet auquel le formulaire est joint avec l’accès à Modifier le formulaire personnalisé.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Afficher le responsable du créateur d’un problème sur le formulaire personnalisé de problème

Les étapes suivantes montrent comment créer un champ calculé pour un formulaire personnalisé de problème où vous pouvez capturer le nom du responsable de l’utilisateur qui a créé le problème. Le processus est identique lorsque vous souhaitez capturer le nom du responsable d’un utilisateur qui a créé une tâche, un projet, un portfolio, par exemple.

1. Créez un formulaire personnalisé Problème et ajoutez-lui un champ calculé.

   Pour plus d’informations sur la création d’un formulaire personnalisé et l’ajout de champs calculés à ce dernier, reportez-vous aux articles suivants :

   * [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [Ajout de données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. Copiez et collez le code de mode texte suivant dans le **Calcul** champ du formulaire personnalisé :

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Les calculs de champs personnalisés sont sensibles à la casse.

1. Cliquez sur **Terminé**, puis **Enregistrer + Fermer**.

   Le gestionnaire de l’utilisateur qui a créé le problème s’affiche dans le champ calculé lorsque le formulaire contenant le champ est joint à un problème.
