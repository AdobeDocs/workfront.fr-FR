---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Exemple de champ personnalisé calculé : afficher la personne responsable du créateur ou de la créatrice d’un problème dans le formulaire personnalisé du problème'
description: À l’aide d’un champ personnalisé calculé, vous pouvez afficher le nom de la personne responsable du créateur ou de la créatrice d’un problème dans un formulaire personnalisé associé au problème. En utilisant la même instruction, vous pouvez créer des champs calculés similaires pour les projets, problèmes et autres objets.
author: Jenny
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 95%

---

# Exemple de champ personnalisé calculé : afficher la personne responsable du créateur ou de la créatrice d’un problème dans le formulaire personnalisé du problème

À l’aide d’un champ personnalisé calculé, vous pouvez afficher le nom de la personne responsable du créateur ou de la créatrice d’un problème dans un formulaire personnalisé associé au problème. En utilisant la même instruction, vous pouvez créer des champs calculés similaires pour les projets, problèmes et autres objets.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Package Adobe Workfront</p> </td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Configurations des niveaux d’accès</p></td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorisations d’objet</p> </td> 
   <td> <p>Accordez l’accès à l’objet auquel le formulaire est associé avec l’accès à Modifier le formulaire personnalisé.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher la personne responsable du créateur ou de la créatrice d’un problème dans le formulaire personnalisé du problème

Les étapes suivantes montrent comment créer un champ calculé pour un formulaire personnalisé de problème où vous pouvez capturer le nom de la personne responsable de l’utilisateur ou de l’utilisatrice qui a créé le problème. Le processus est identique lorsque vous souhaitez capturer le nom de la personne responsable d’un utilisateur ou d’une utilisatrice qui a créé une tâche, un projet ou un portfolio, par exemple.

1. Créez un formulaire personnalisé pour un problème et ajoutez-lui un champ calculé.

   Pour plus d’informations sur la création d’un formulaire personnalisé et l’ajout de champs calculés à ce dernier, consultez les articles suivants :

   * [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Copiez et collez le code de mode texte suivant dans le champ **Calcul** du formulaire personnalisé :

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Les calculs de champs personnalisés respectent la casse.

1. Cliquez sur **Terminé**, puis sur **Enregistrer+Fermer**.

   La personne responsable de l’utilisateur ou de l’utilisatrice qui a créé le problème s’affiche dans le champ calculé lorsque le formulaire contenant le champ est associé à un problème.
