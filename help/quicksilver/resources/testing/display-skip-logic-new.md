---
title: Ajouter une logique d’affichage et une logique de saut à un formulaire personnalisé
description: Ajouter une logique d’affichage et une logique de saut à un formulaire personnalisé
draft: Probably
source-git-commit: c0722924d6621b382050a10e9aac549fc1204d72
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 10%

---

# Ajouter une logique d’affichage et une logique de saut à un formulaire personnalisé

Vous pouvez utiliser des règles intelligentes pour rendre un formulaire personnalisé dynamique et plus pertinent pour les utilisateurs qui le remplissent. Lorsqu’un utilisateur répond d’une certaine manière à un champ à choix multiples sur un formulaire, une règle intelligente lui indique ce que vous souhaitez voir après, en fonction de cette réponse.

Les types de champ à choix multiples sont Liste déroulante, Cases à cocher et Boutons radio.

* **Logique d’affichage** : vous configurez une règle de logique d’affichage sur le champ, le widget ou la section que vous souhaitez que l’utilisateur affiche uniquement après avoir sélectionné un choix spécifique dans un champ à choix multiples précédent.

  **Exemple :** Vous créez un formulaire de demande de contenu marketing dans lequel les membres de votre entreprise peuvent demander un nouveau logo, une mise à jour de site web, une brochure ou d’autres types de contenu marketing. En fonction du type de contenu souhaité par l’utilisateur, vous devez lui demander différents types de détails, tels que des couleurs et des idées de conception s’il a besoin d’un logo, ou une liste des fonctionnalités du produit s’il a besoin d’une brochure.

  Sur le champ qui demande des couleurs et des détails pour un nouveau logo, vous pouvez ajouter une règle de logique d’affichage qui affiche ce champ uniquement une fois que l’utilisateur a sélectionné le bouton radio Logo dans le premier champ.

  De même, sur le champ qui demande des informations sur les fonctionnalités du produit, vous pouvez ajouter une règle de logique d’affichage qui n’affiche ce champ qu’après qu’un utilisateur a sélectionné le bouton radio Brochure dans le premier champ.

  ![](assets/display-logic-logo-request-350x196.png)

  Vous pouvez configurer des règles de logique d’affichage sur n’importe quel champ personnalisé, widget ou saut de section qui suit un champ à choix multiples.

* **Ignorer la règle logique** : vous configurez cette règle pour masquer les parties d’un formulaire dont l’utilisateur n’a pas besoin. Lorsque l’utilisateur sélectionne un élément spécifique dans un champ à choix multiples précédent, la règle d’exclusion de la logique l’ignore jusqu’à la fin du formulaire ou dans un champ, un widget ou une section personnalisé que vous souhaitez voir.

  **Exemple :** Quelqu’un utilise le formulaire de demande de contenu marketing ci-dessus pour demander un livre blanc, fourni par le service commercial, et non par le service marketing. Pour cet utilisateur, une règle d’exclusion logique peut masquer la question qui entraîne des détails et passer à une ligne de texte qui le fait référence au service dont il a besoin.

  ![](assets/skip-logic-white-paper-request-350x221.png)

  Dans ce cas, vous pouvez ajouter un champ de texte descriptif qui renvoie l’utilisateur au service des ventes. Dans le premier champ personnalisé qui demande le type de contenu marketing dont l’utilisateur a besoin, vous pouvez ajouter une règle de logique de saut qui n’affiche que la ligne de texte lorsqu’un utilisateur sélectionne le bouton radio Papier blanc dans le premier champ.

  Cela serait particulièrement utile si vous ajoutez de nombreux autres champs concernant les logos, les mises à jour de site web et les brochures que cet utilisateur n&#39;a pas besoin de voir.
Vous pouvez appliquer une règle de logique de saut uniquement à un champ personnalisé, et non à un widget ou à une section.

Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Ajouter un champ personnalisé à un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) et [Ajouter ou modifier un widget de ressource dans un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Forfait Adobe Workfront*</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Pour plus d’informations sur la manière dont les administrateurs et administratrices de Workfront accordent cet accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroyer aux utilisateurs et utilisatrices un accès administratif à certaines zones</a>.</p> </td> 
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

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, sélectionnez **Forms personnalisé** ![](assets/custom-forms-icon.png).

1. Cliquez sur **New Custom Form**, sélectionnez **Project** dans la zone qui s’affiche, puis sélectionnez **Continue**.

1. Dans la zone de texte **Titre du formulaire**, saisissez **Exemple de formulaire personnalisé - Logique d’affichage d’apprentissage et ignorer la logique** pour nommer le formulaire.

   ![](assets/form-title-box-350x247.png)

1. Pour ajouter le premier champ du formulaire :

   1. Ouvrez l’onglet **Ajouter un champ** .

      ![](assets/add-a-field-tab-350x237.png)

   1. Sélectionnez le type de champ **Boutons radio**, puis saisissez *Quel type de contenu marketing avez-vous besoin ?* comme **Libellé** pour le champ.

   1. Sous **Choix**, remplacez **Choix 1** et **Choix 2** par le texte suivant pour créer deux options que les utilisateurs peuvent choisir dans le champ :

      *Mise à jour du site Web*

      *Conception du logo*

1. Pour ajouter le champ personnalisé suivant et lui ajouter une règle de logique d’affichage :

   1. Ouvrez à nouveau l’onglet **Ajouter un champ** et ajoutez un nouveau champ **Boutons radio** appelé *De quel type de mise à jour de site web avez-vous besoin ?*

      Nous ajouterons les choix pour ce champ ultérieurement.

   1. Dans la section **Additional settings**, sélectionnez **Add Logic**.

      ![](assets/add-logic-btn-350x408.png)

1. Dans la zone qui s’affiche, avec l’onglet **Afficher la logique** ouvert, configurez le second champ de sorte qu’il s’affiche uniquement pour les utilisateurs qui ont sélectionné *Conception de site Web* dans le premier champ :

   1. Dans la première liste déroulante, sélectionnez **Quel type de contenu marketing avez-vous besoin ?**
   1. Dans la seconde liste déroulante, sélectionnez **Conception de site Web**.
   1. Si vous laissez la troisième liste déroulante définie sur **Selected**, sélectionnez **Save**.

   Notez les petits carrés de couleur avec un D, indiquant que le deuxième champ est connecté avec la logique d’affichage à la sélection de l’utilisateur dans le premier champ :

   ![](assets/red-display-logic-indicators-350x250.png)

1. Sélectionnez **Aperçu** pour vous assurer que la logique fonctionne comme vous le souhaitez sur le formulaire, puis sélectionnez **Aperçu de fin**.

1. Cliquez sur **Enregistrer + Fermer** pour enregistrer le formulaire, puis passez à [Ignorer la logique - exemple pratique](#skip-logic-practical-example) ci-dessous.

### Ignorer la logique - exemple pratique {#skip-logic-practical-example}

Ignorer la logique fonctionne de la même manière que pour afficher la logique, mais agit comme l’inverse : au lieu d’afficher des champs personnalisés à choix multiples spécifiques en fonction des sélections précédentes, vous déterminez ceux qui doivent être masqués (ignorés), car ils ne sont pas pertinents pour l’utilisateur.

Pour en savoir plus à ce sujet, continuez à travailler sur l’exemple de formulaire personnalisé que vous avez créé dans la section [Logique d’affichage - exemple pratique](#display-logic-practical-example) de cet article.

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Formulaires personnalisés**.
1. Cliquez sur le nom du formulaire **Exemple de formulaire personnalisé - Logique d’affichage d’apprentissage et ignorer la logique** que vous avez créée lors des étapes ci-dessus pour l’ouvrir en vue de la modifier.
1. Sélectionnez le champ de liste déroulante que vous avez créé nommé *De quel type de site avez-vous besoin ?*, ajoutez les choix suivants pour le champ, puis cliquez sur **Appliquer** :

   *E-commerce*

   *Brochure*

   *Adhésion*

1. Ouvrez l’onglet **Ajouter un champ** , créez un champ **Texte avec formatage** appelé&#x200B;*Quel est l’objectif du site web ?*, puis cliquez sur **Apply**.

   Dans cette organisation, un site de documentation d’aide est créé par l’équipe d’écriture technique et non par le service marketing. Par conséquent, aucune information supplémentaire n’est nécessaire de la part d’un utilisateur qui sélectionne la documentation d’aide dans le deuxième champ. Nous allons créer une ligne de texte (un champ de texte descriptif) qui leur indiquera de voir l&#39;équipe d&#39;écriture technique à la place. Et nous utiliserons une règle de logique de saut qui ignore cet utilisateur dans cette ligne de texte.

1. Pour créer la ligne de texte :

   1. Ouvrez l’onglet **Ajouter un champ** et créez un **champ de texte descriptif**.

   1. Pour le **libellé**, saisissez *Voir équipe d’écriture technique*.

   1. Pour le **texte descriptif**, saisissez *Veuillez consulter l’équipe d’écriture technique au sujet de la création de la documentation d’aide en ligne*.

   1. Sélectionnez **Apply**.

1. Pour créer la règle de logique de saut :

   1. Sélectionnez le second champ de liste déroulante, *De quel type de site avez-vous besoin ?*
   1. Dans la section **Paramètre supplémentaire** , sélectionnez **Modifier la logique**.
   1. Dans la zone qui s’affiche, ouvrez l’onglet **Ignorer la logique** .
   1. Définissez la première liste déroulante sur **Documentation d’aide**, laissez la deuxième liste déroulante définie sur **Sélectionné** et définissez la troisième liste déroulante sur **Voir l’équipe d’écriture technique**.
   1. Sélectionnez **Enregistrer**.

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
>* Il est suivi d’un autre champ personnalisé.
>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Multi-field display logic statements</h2>
-->

