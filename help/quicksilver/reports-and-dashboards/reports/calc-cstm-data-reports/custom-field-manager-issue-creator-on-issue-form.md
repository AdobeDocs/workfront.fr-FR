---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: '« Exemple de champ personnalisé calculé : afficher la personne responsable du créateur ou de la créatrice d’un problème dans le formulaire personnalisé du problème »'
description: À l’aide d’un champ personnalisé calculé, vous pouvez afficher le nom de la personne responsable du créateur ou de la créatrice d’un problème dans un formulaire personnalisé associé au problème. En utilisant la même instruction, vous pouvez créer des champs calculés similaires pour les projets, problèmes et autres objets.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 98%

---

# Exemple de champ personnalisé calculé : afficher la personne responsable du créateur ou de la créatrice d’un problème dans le formulaire personnalisé du problème

À l’aide d’un champ personnalisé calculé, vous pouvez afficher le nom de la personne responsable du créateur ou de la créatrice d’un problème dans un formulaire personnalisé associé au problème. En utilisant la même instruction, vous pouvez créer des champs calculés similaires pour les projets, problèmes et autres objets.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configurations du niveau d’accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés<br>Pour plus d’informations sur l’octroi de l’accès administratif à partir du niveau d’accès, consultez <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones</a>.</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet</p> </td> 
   <td> <p>Accordez l’accès à l’objet auquel le formulaire est associé avec l’accès à Modifier le formulaire personnalisé.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, consultez la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher la personne responsable du créateur ou de la créatrice d’un problème dans le formulaire personnalisé du problème

Les étapes suivantes montrent comment créer un champ calculé pour un formulaire personnalisé de problème où vous pouvez capturer le nom de la personne responsable de l’utilisateur ou de l’utilisatrice qui a créé le problème. Le processus est identique lorsque vous souhaitez capturer le nom de la personne responsable d’un utilisateur ou d’une utilisatrice qui a créé une tâche, un projet ou un portfolio, par exemple.

1. Créez un formulaire personnalisé pour un problème et ajoutez-lui un champ calculé.

   Pour plus d’informations sur la création d’un formulaire personnalisé et l’ajout de champs calculés à ce dernier, consultez les articles suivants :

   * [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Ajouter des champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Copiez et collez le code de mode texte suivant dans le champ **Calcul** du formulaire personnalisé :

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Les calculs de champs personnalisés respectent la casse.

1. Cliquez sur **Terminé**, puis sur **Enregistrer+Fermer**.

   La personne responsable de l’utilisateur ou de l’utilisatrice qui a créé le problème s’affiche dans le champ calculé lorsque le formulaire contenant le champ est associé à un problème.
