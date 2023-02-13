---
title: Ajouter une logique d’affichage et ignorer une logique dans un formulaire personnalisé
description: Ajouter une logique d’affichage et ignorer une logique dans un formulaire personnalisé
draft: Probably
source-git-commit: c0722924d6621b382050a10e9aac549fc1204d72
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# Ajouter une logique d’affichage et ignorer une logique dans un formulaire personnalisé

Vous pouvez utiliser des règles intelligentes pour rendre un formulaire personnalisé dynamique et plus pertinent pour les utilisateurs qui le remplissent. Lorsqu’un utilisateur répond d’une certaine manière à un champ à choix multiples sur un formulaire, une règle intelligente lui indique ce que vous souhaitez voir après, en fonction de cette réponse.

Les types de champ à choix multiples sont Liste déroulante, Cases à cocher et Boutons radio.

* **Logique d’affichage**: Vous configurez une règle de logique d’affichage sur le champ, le widget ou la section que vous souhaitez que l’utilisateur ne voit qu’après avoir sélectionné un choix spécifique dans un champ à choix multiples précédent.

   **Exemple :** Vous créez un formulaire de demande de contenu marketing dans lequel les membres de votre entreprise peuvent demander un nouveau logo, une mise à jour de site web, une brochure ou d’autres types de contenu marketing. En fonction du type de contenu souhaité par l’utilisateur, vous devez lui demander différents types de détails, tels que des couleurs et des idées de conception s’il a besoin d’un logo ou une liste des fonctionnalités du produit s’il a besoin d’une brochure.

   Sur le champ qui demande des couleurs et des détails pour un nouveau logo, vous pouvez ajouter une règle de logique d’affichage qui affiche ce champ uniquement une fois que l’utilisateur a sélectionné le bouton radio Logo dans le premier champ.

   De même, sur le champ qui demande des informations sur les fonctionnalités du produit, vous pouvez ajouter une règle de logique d’affichage qui n’affiche ce champ qu’après qu’un utilisateur a sélectionné le bouton radio Brochure dans le premier champ.

   ![](assets/display-logic-logo-request-350x196.png)

   Vous pouvez configurer des règles de logique d’affichage sur n’importe quel champ personnalisé, widget ou saut de section qui suit un champ à choix multiples.

* **Ignorer la règle logique**: Vous configurez cette règle pour masquer les parties d’un formulaire dont l’utilisateur n’a pas besoin. Lorsque l’utilisateur sélectionne un élément spécifique dans un champ à choix multiples précédent, la règle d’exclusion de la logique l’ignore jusqu’à la fin du formulaire ou dans un champ, un widget ou une section personnalisé que vous souhaitez voir.

   **Exemple :** Quelqu’un utilise le formulaire de demande de contenu marketing ci-dessus pour demander un livre blanc, qui est fourni par le service des ventes, et non par le service marketing. Pour cet utilisateur, une règle d’exclusion logique peut masquer la question qui entraîne des détails et passer à une ligne de texte qui le fait référence au service dont il a besoin.

   ![](assets/skip-logic-white-paper-request-350x221.png)

   Dans ce cas, vous pouvez ajouter un champ de texte descriptif qui renvoie l’utilisateur au service des ventes. Dans le premier champ personnalisé qui demande le type de contenu marketing dont l’utilisateur a besoin, vous pouvez ajouter une règle de logique de saut qui n’affiche que la ligne de texte lorsqu’un utilisateur sélectionne le bouton radio Papier blanc dans le premier champ.

   Cela serait particulièrement utile si vous ajoutez de nombreux autres champs concernant les logos, les mises à jour de site web et les brochures que cet utilisateur n&#39;a pas besoin de voir.
Vous pouvez appliquer une règle de logique de saut uniquement à un champ personnalisé, et non à un widget ou à une section.

Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Ajouter un champ personnalisé à un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) et [Ajout ou modification d’un widget de ressource dans un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Pour plus d’informations sur la manière dont les administrateurs de Workfront accordent cet accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur Workfront.

## Création d’un exemple de formulaire personnalisé avec une logique d’affichage et de saut

La meilleure façon d’apprendre à ajouter une logique d’affichage et d’exclusion à un formulaire personnalisé est de suivre l’exemple pratique décrit dans les deux sections suivantes :

* [Logique d’affichage - exemple pratique](#display-logic-practical-example)
* [Ignorer la logique - exemple pratique](#skip-logic-practical-example)

### Logique d’affichage - exemple pratique {#display-logic-practical-example}

Dans cet exemple, vous allez créer un formulaire personnalisé avec un champ de bouton radio à choix multiples. Vous allez ensuite ajouter une logique d’affichage qui connecte ce champ à un second champ.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, sélectionnez **Forms personnalisée** ![](assets/custom-forms-icon.png).

1. Cliquez sur **Nouveau formulaire personnalisé**, sélectionnez **Projet** dans la zone qui s’affiche, puis sélectionnez **Continuer**.

1. Dans le **Titre du formulaire** zone de texte, saisissez **Exemple de formulaire personnalisé : apprentissage de la logique d’affichage et de la logique de saut** pour nommer le formulaire.

   ![](assets/form-title-box-350x247.png)

1. Pour ajouter le premier champ du formulaire :

   1. Ouvrez le **Ajouter un champ** .

      ![](assets/add-a-field-tab-350x237.png)

   1. Sélectionnez la **Boutons radio** type de champ, puis saisissez *De quel type de contenu marketing avez-vous besoin ?* comme la propriété **Libellé** pour le champ .

   1. Sous **Choix**, remplacer **Choix 1** et **Choix 2** avec le texte suivant pour créer deux options, les utilisateurs peuvent choisir dans le champ :

      *Mise à jour du site web*

      *Conception de logo*

1. Pour ajouter le champ personnalisé suivant et lui ajouter une règle de logique d’affichage :

   1. Ouvrez le **Ajouter un champ** à nouveau et ajoutez une nouvelle **Boutons radio** champ appelé *De quel type de mise à jour de site web avez-vous besoin ?*

      Nous ajouterons les choix pour ce champ ultérieurement.

   1. Dans le **Paramètres supplémentaires** , sélectionnez **Ajouter logique**.

      ![](assets/add-logic-btn-350x408.png)

1. Dans la zone qui s’affiche, avec la fonction **Logique d’affichage** ouvrez l’onglet, configurez le second champ de sorte qu’il s’affiche uniquement pour les utilisateurs qui ont sélectionné *Conception de site web* dans le premier champ :

   1. Dans la première liste déroulante, sélectionnez **De quel type de contenu marketing avez-vous besoin ?**
   1. Dans la deuxième liste déroulante, sélectionnez **Conception de site web**.
   1. Laissez la troisième liste déroulante définie sur **Sélectionné**, sélectionnez **Enregistrer**.

   Notez les petits carrés de couleur avec un D, indiquant que le deuxième champ est connecté avec la logique d’affichage à la sélection de l’utilisateur dans le premier champ :

   ![](assets/red-display-logic-indicators-350x250.png)

1. Sélectionner **Aperçu** pour vous assurer que la logique fonctionne comme vous le souhaitez sur le formulaire, sélectionnez **Aperçu de la fin**.

1. Cliquez sur **Enregistrer + Fermer** enregistrez le formulaire, puis continuez sur [Ignorer la logique - exemple pratique](#skip-logic-practical-example) ci-dessous.

### Ignorer la logique - exemple pratique {#skip-logic-practical-example}

Les fonctions Ignorer la logique s’affichent de la même manière que la logique, mais agissent comme l’inverse : au lieu d’afficher des champs personnalisés à choix multiples spécifiques en fonction des sélections précédentes de l’utilisateur, vous déterminez ceux qui doivent être masqués (sautés), car ils ne sont pas pertinents pour l’utilisateur.

Pour en savoir plus à ce sujet, continuez à travailler sur l’exemple de formulaire personnalisé que vous avez créé dans la section . [Logique d’affichage - exemple pratique](#display-logic-practical-example) dans cet article.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Forms personnalisée**.
1. Cliquez sur le nom du formulaire. **Exemple de formulaire personnalisé : apprentissage de la logique d’affichage et de la logique de saut** que vous avez créé lors des étapes ci-dessus pour l’ouvrir en vue de la modifier.
1. Sélectionnez le champ déroulant que vous avez créé nommé *De quel type de site web avez-vous besoin ?*, ajoutez les options suivantes pour le champ, puis cliquez sur **Appliquer**:

   *Commerce électronique*

   *Brochure*

   *Abonnement*

1. Ouvrez le **Ajouter un champ** , créez un champ **Texte avec mise en forme **appelé&#x200B;*Quel est le but du site web ?*, puis cliquez sur **Appliquer**.

   Dans cette organisation, un site de documentation d’aide est créé par l’équipe d’écriture technique et non par le service marketing. Par conséquent, aucune information supplémentaire n’est nécessaire de la part d’un utilisateur qui sélectionne la documentation d’aide dans le deuxième champ. Nous allons créer une ligne de texte (un champ de texte descriptif) qui leur indiquera de voir l&#39;équipe d&#39;écriture technique à la place. Et nous utiliserons une règle de logique de saut qui ignore cet utilisateur dans cette ligne de texte.

1. Pour créer la ligne de texte :

   1. Ouvrez le **Ajouter un champ** et créez un **Champ de texte descriptif**.

   1. Pour le **Libellé**, type *Voir l’équipe d’écriture technique*.

   1. Pour le **Texte descriptif**, type *Consultez l’équipe d’écriture technique au sujet de la création de la documentation d’aide en ligne.*.

   1. Sélectionner **Appliquer**.

1. Pour créer la règle de logique de saut :

   1. Sélectionnez le second champ de liste déroulante, *De quel type de site web avez-vous besoin ?*
   1. Dans le **Paramètre supplémentaire** s , sélectionnez **Modifier la logique**.
   1. Dans la zone qui s’affiche, ouvrez le **Ignorer la logique** .
   1. Définissez la première liste déroulante sur **Documentation d’aide**, laissez la deuxième liste déroulante définie sur **Sélectionné**, puis définissez la troisième liste déroulante sur **Voir l’équipe d’écriture technique**.
   1. Sélectionner **Enregistrer**.

   Notez la petite logique de saut carrée avec un S, indiquant que l’utilisateur sautera quelque chose après avoir sélectionné un certain choix dans le deuxième champ.

   ![](assets/notice-skip-logic-squares-350x249.png)

1. Cliquez sur **Aperçu**  pour vous assurer que la logique s’applique comme vous le souhaitez.
1. Cliquez sur **Enregistrer +Fermer**.

En créant un formulaire comme celui-ci, vous pouvez ajouter d’autres champs de texte pour demander des informations aux utilisateurs qui sélectionnent E-commerce ou Brochure dans le deuxième champ. Ces champs peuvent demander qui est l’audience cible pour le site web, quel est l’objectif pour le créer, quel est le budget, etc.

Et avec les règles logiques, vous pouvez créer des chemins d’interrogation d’embranchement.

Par exemple, pour les utilisateurs qui sélectionnent le commerce électronique, vous pouvez créer des champs contenant des questions sur les photos, descriptions, prix et options de paiement des produits. Pour les utilisateurs qui sélectionnent Brochure, vous pouvez créer des champs en demandant du contenu.

Un utilisateur qui a sélectionné la documentation d’aide ne verrait jamais aucun de ces champs supplémentaires qui n’est pas pertinent pour lui.

>[!TIP]
>
>Vous pouvez ajouter une logique d’affichage et ignorer la logique à un champ personnalisé si tous les éléments suivants sont vrais sur le champ :
>
>* Il s’agit d’un champ à choix multiples (boutons radio, liste déroulante ou cases à cocher).
>* Il est précédé d’un champ à choix multiples.
>* Il est suivi d’un autre champ personnalisé
>


<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Multi-field display logic statements</h2>
-->

