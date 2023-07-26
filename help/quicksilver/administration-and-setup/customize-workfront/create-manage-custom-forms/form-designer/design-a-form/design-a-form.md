---
title: Concevoir un formulaire avec le concepteur de formulaires
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez concevoir un formulaire personnalisé à l’aide du concepteur de formulaire.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '3803'
ht-degree: 4%

---

# Concevoir un formulaire avec le concepteur de formulaires

Vous pouvez concevoir un formulaire personnalisé à l’aide du concepteur de formulaire. Vous pouvez joindre des formulaires personnalisés à différents objets Workfront pour capturer des données sur ces objets.

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
   <td>
   <p>Formule actuelle : Standard</p>
   <p>ou</p>
   <p>Formule héritée : Planifier</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Pour plus d’informations sur la manière dont les administrateurs de Workfront accordent cet accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur Workfront.

## Commencer à concevoir un formulaire personnalisé

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Forms personnalisée** dans le panneau de gauche.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Cliquez sur **Nouveau formulaire personnalisé.**
1. Sélectionnez les types d’objets auxquels vous souhaitez joindre le formulaire personnalisé, puis cliquez sur **Continuer**.

   ![](assets/choose-object-type.jpg)

1. Dans le **Le titre est obligatoire** , saisissez le titre personnalisé du formulaire.
1. (Facultatif) Si vous souhaitez ajouter d’autres types d’objets au formulaire afin de pouvoir les joindre à d’autres objets, cliquez sur le bouton **Ajouter** icon ![](assets/add-objects-icon.png) after **Types d’objet**, puis sélectionnez le type souhaité dans le menu qui s’affiche. Vous pouvez répéter cette opération pour ajouter autant de types d’objet que vous le souhaitez.

   Vous pouvez également cliquer sur le X d’un type d’objet pour le supprimer du formulaire.

   >[!CAUTION]
   >
   >La suppression d’un formulaire personnalisé supprime également toutes les données personnalisées sur les objets associés au formulaire. Les données supprimées ne peuvent pas être récupérées. Envisagez plutôt de désactiver un formulaire personnalisé : lorsque vous désactivez un formulaire personnalisé que vous n’utilisez plus, vous conservez toutes les données historiques associées.
   >
   >Pour plus d’informations, voir [Suppression de types d’objet sur un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).


1. Vous pouvez ensuite commencer à ajouter des champs à votre formulaire personnalisé. Reportez-vous aux sections suivantes :
   * [Réutiliser un champ ou un widget existant déjà utilisé dans un autre formulaire personnalisé](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Ajouter des champs de texte](#add-text-fields)
   * [Ajouter des champs calculés](#add-calculated-fields)
   * [Ajout de boutons radio, de groupes de cases à cocher et de listes déroulantes](#add-radio-buttons-checkboxes-and-dropdowns)
   * [Ajout de champs de type anticipé et date](#add-typeahead-and-date-fields)
   * [Ajout d’images, de PDF et de vidéos](#add-images-pdfs-and-videos)
   * [Ajout de fichiers Adobe XD](#add-adobe-xd-files)

## Ajouter des champs nouveaux ou existants à votre formulaire personnalisé

Vous pouvez utiliser des champs nouveaux ou existants lors de la conception de votre formulaire personnalisé.

## Réutiliser un champ ou un widget existant déjà utilisé dans un autre formulaire personnalisé

1. Dans le coin supérieur gauche de l’écran, cliquez sur **Bibliothèque de champs**.

1. Faites glisser le champ ou le widget ici de votre choix dans le formulaire personnalisé.
1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   >[!NOTE]
   >
   >Vous pouvez ajouter jusqu’à 500 champs et widgets sur un seul formulaire personnalisé. Cependant, une dégradation des performances peut se produire lorsque plus de 100 sur un formulaire existent, selon sa complexité.
   >
   >
   >Parmi les exemples de formulaires complexes, citons les formulaires avec des paramètres en cascade, des champs de données personnalisés calculés et plusieurs options de valeur dans un seul champ.

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   ou

   Cliquez sur **Enregistrer et fermer**.

### Ajouter des champs de texte

Vous pouvez ajouter plusieurs champs de texte différents à un formulaire personnalisé.

+++ **Développer pour afficher les descriptions des champs de texte disponibles**

* **Champ de texte d’une seule ligne**: permet aux utilisateurs de saisir une seule ligne de texte dans le champ.
* **Champ de texte de paragraphe**: permet aux utilisateurs de saisir plusieurs lignes de texte dans le champ.
* **Champ de texte avec mise en forme**: permet aux utilisateurs de saisir plusieurs lignes de texte dans le champ et de mettre en forme le texte en gras, italique, souligné, puces, numérotation, liens hypertexte et guillemets. Une limite de caractères de 15 000 permet d’utiliser beaucoup de texte et de formatage.

  Pour plus d’informations sur l’accès à ce champ par le biais de l’API, voir Stockage de champs de texte enrichi dans l’API.

  >[!NOTE]
  >
  >Les champs de texte avec mise en forme ne sont pas disponibles pour les applications mobiles Workfront (disponibles dans les prochaines versions).

* **Texte descriptif**: vous permet d’inclure des instructions et de créer des liens vers des pages en dehors de Workfront.

+++

Pour ajouter un champ de texte :

1. Dans la partie gauche de l’écran, recherchez l’un des champs de texte suivants et faites-le glisser vers une section du canevas :

   * Une seule ligne de texte :
   * Texte du paragraphe
   * Champ de texte avec formatage
   * Texte descriptif

   ![](assets/drag-field-to-section.png)

1. Dans la partie droite de l’écran, configurez les options disponibles pour le type de champ personnalisé que vous ajoutez :

   <table>
    <tr>
    <td>Entrée dans</td>
    <td>Description</td>
    <td>Disponible pour </td>
    </tr>
    <tr>
    <td>Taille</td>
    <td><p>Modifiez la taille des champs de texte du formulaire.<p>
   </td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe de texte</li>
    <li>Texte avec formatage</li>
    <li>Texte descriptif - À venir bientôt</li>
    </ul></td>
    </tr>
    <tr>
    <td>Étiquette</td>
    <td><p>Saisissez un libellé descriptif à afficher au-dessus du widget. Vous pouvez modifier le libellé à tout moment.<p>
    <p>IMPORTANT : évitez d’utiliser des caractères spéciaux dans ce libellé. Elles ne s’affichent pas correctement dans les rapports.</p></td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe de texte</li>
    <li>Texte avec formatage</li>
    </ul></td>
    </tr>
    <tr>
     <td>Nom</td>
    <td><p>(Obligatoire) Ce nom est la manière dont le système identifie le champ. Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé que vos utilisateurs voient sans avoir à modifier le nom que le système voit.</p>
    <p><b>IMPORTANT</b>:   
      <ul> 
      <li>Bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans Workfront. Si vous le faites, le système ne reconnaîtra plus le champ personnalisé où il peut maintenant être référencé dans d’autres zones de Workfront. <p>Par exemple, si vous ajoutez le champ personnalisé à un rapport et que vous modifiez ensuite son nom, Workfront ne le reconnaît pas dans le rapport et il ne fonctionnera plus correctement à moins de le rajouter au rapport en utilisant le nouveau nom.</p> </li>
      <li> <p>Nous vous recommandons de ne pas saisir de nom déjà utilisé pour les champs Workfront intégrés.</p> </li>
      <li><p>Il est recommandé de ne pas utiliser le caractère point/point dans le nom du champ personnalisé afin d’éviter toute erreur lors de l’utilisation du champ dans différentes zones de Workfront.</p></li>
    </td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe de texte</li>
    <li>Texte avec formatage</li>
    <li>Texte descriptif</li>
    </ul></td>
    </tr>
    <tr>
    <td>Instructions</td>
    <td>Saisissez des informations supplémentaires sur le widget. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations saisies ici.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe de texte</li>
    <li>Texte avec formatage</li>
    </ul></td>
    </tr>
    <tr>
    <td>Format</td>
    <td><p>Sélectionnez le type de données qui sera capturé dans le champ personnalisé.</p> <p><b>NOTE</b>:   
    <ul> 
    <li>Une fois le formulaire enregistré, ce champ ne peut plus être modifié. Si vous envisagez d’utiliser votre champ dans des calculs mathématiques, veillez à sélectionner le format Nombre ou Devise .<br></li> 
    <li>Lorsque vous sélectionnez Nombre ou Devise, le système tronque automatiquement les nombres qui commencent par 0.</li> 
     </ul></p></td> </td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe de texte</li>
    </ul></td>
    </tr>
    <tr>
    <td>Type d'affichage</td>
    <td>Basculer entre les champs de texte d’une seule ligne et d’un paragraphe.</td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe de texte</li>
    </ul></td>
    </tr>
    <tr>
    <td>Lien hypertexte</td>
    <td> Si vous souhaitez appliquer un lien hypertexte au texte descriptif que vous avez saisi, ajoutez-le ici. Le texte descriptif s’affiche sous la forme d’un lien sur les objets auxquels le formulaire est joint.</td>
    <td><ul><li>Texte descriptif</li></ul></td>
    </tr>
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   ou

   Pour copier un champ, pointez dessus, puis cliquez sur l’icône Copier.

   ![icône de copie](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   ou

   Cliquez sur **Enregistrer et fermer**.

### Ajouter des champs calculés

Dans un formulaire personnalisé, vous pouvez ajouter un champ personnalisé calculé qui utilise les données existantes pour générer de nouvelles données lorsque le formulaire personnalisé est joint à un objet.

Pour ajouter un champ calculé, reportez-vous à la section [Ajouter des champs calculés avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Ajout de boutons radio, de cases à cocher et de listes déroulantes

Vous pouvez ajouter des boutons radio, des cases à cocher et des listes déroulantes à un formulaire personnalisé.

+++ **Développer pour afficher les descriptions des champs disponibles**

* **Boutons radio**: nécessite que les utilisateurs sélectionnent un seul choix.
* **Groupe de cases à cocher**: permet aux utilisateurs de sélectionner plusieurs choix.
* **Liste déroulante**: fournit une liste de choix de liste déroulante.

+++

Pour ajouter des boutons radio et des cases à cocher :

1. Dans la partie gauche de l’écran, recherchez l’un des champs suivants et faites-le glisser vers une section du canevas.

   * Cases d’option
   * Groupe Case à cocher
   * Menu déroulant

   ![](assets/drag-field-to-section.png)

1. Dans la partie droite de l’écran, configurez les options disponibles pour le type de champ personnalisé que vous ajoutez :

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Entrée dans</td>
    <td>Description</td>
    <td>Disponible pour </td>
    </tr>
    <tr> 
     <td role="rowheader">Étiquette</td> 
     <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ personnalisé. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b>: évitez d’utiliser des caractères spéciaux dans ce libellé. Elles ne s’affichent pas correctement dans les rapports.</p> </td> 
     <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Menu déroulant</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Nom</td> 
     <td> <p>(Obligatoire) Ce nom est la manière dont le système identifie le champ personnalisé lorsque vous l’ajoutez à différentes zones dans Workfront, telles que les rapports, l’accueil et les interactions avec l’API.</p> <p>Lorsque vous configurez le champ personnalisé pour la première fois et que vous tapez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé que vos utilisateurs voient sans avoir à modifier le nom que le système voit.</p> 
    <p><b>IMPORTANT</b>:   
     <ul> 
    <li>Bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans Workfront. Si vous le faites, le système ne reconnaîtra plus le champ personnalisé où il peut maintenant être référencé dans d’autres zones de Workfront. <p>Par exemple, si vous ajoutez le champ personnalisé à un rapport et que vous modifiez ensuite son nom, Workfront ne le reconnaît pas dans le rapport et il ne fonctionnera plus correctement à moins de le rajouter au rapport en utilisant le nouveau nom.</p> </li>
    <li> <p>Nous vous recommandons de ne pas saisir de nom déjà utilisé pour les champs Workfront intégrés.</p> </li>
     <li><p>Il est recommandé de ne pas utiliser le caractère point/point dans le nom du champ personnalisé afin d’éviter toute erreur lors de l’utilisation du champ dans différentes zones de Workfront.</p></li>
     </ul> <p>Chaque nom de champ personnalisé doit être unique dans l’instance Workfront de votre entreprise. Ainsi, vous pouvez réutiliser un formulaire déjà créé pour un autre formulaire personnalisé. Pour plus d’informations, voir <a href="#Add" class="MCXref xref">Ajouter un champ personnalisé à un formulaire personnalisé</a> dans cet article.</p> </td>
     <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Menu déroulant</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Instructions</td> 
    <td> <p>Saisissez des informations supplémentaires sur le champ personnalisé. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations saisies ici.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Menu déroulant</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Format</td> 
    <td> <p>Sélectionnez le type de données qui sera capturé dans le champ personnalisé.</p> <p><b>NOTE</b>:   
     <ul> 
    <li>Une fois le formulaire enregistré, ce champ ne peut plus être modifié. Si vous envisagez d’utiliser votre champ dans des calculs mathématiques, veillez à sélectionner le format Nombre ou Devise .<br></li> 
    <li>Lorsque vous sélectionnez Nombre ou Devise, le système tronque automatiquement les nombres qui commencent par 0.</li> 
     </ul></p></td> 
     <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Menu déroulant</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Type d'affichage</td> 
    <td>Basculez entre les boutons radio, les groupes de cases à cocher ou les listes déroulantes pour le champ.</td> 
    <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Menu déroulant</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Créer un champ obligatoire</td> 
    <td>Sélectionnez cette option si vous souhaitez que le champ soit obligatoire pour que l’utilisateur puisse remplir le formulaire personnalisé. </td> 
    <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Menu déroulant</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Choix </td> 
    <td> 
    <ol> 
    <li> <p>Cliquez sur <b>Options</b>, puis activez l’une des options suivantes :</p> 
    <ul> 
    <li><strong>Afficher les valeurs</strong>: affiche les valeurs de chaque choix dans le champ. Le libellé de chaque choix s’affiche par défaut.</li> 
     <li><strong>Choix de tri A-Z</strong>: trie par ordre alphabétique les choix que vous ajoutez dans le champ.</li> 
    </ul> 
    </li> 
    <li> <p>Pour chaque choix que vous ajoutez à l’utilisateur, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-settings.png">, puis sélectionnez l’une des options suivantes :</p> 
    <ul> 
    <li><strong>Sélection par défaut</strong>: sélectionnez le choix par défaut dans le champ.</li> 
    <li> <p><strong>Masquer le choix</strong>: masque le choix dans le champ. Les choix masqués restent accessibles dans les rapports.</p> </li> 
    <li> <p><strong>Supprimer le choix</strong>: supprimez le choix du champ.</p> <p><b>Avertissement</b>: si ce choix est utilisé pour les objets en cours, ne le supprimez pas du champ. Sa suppression entraînera la perte de données historiques. Sélectionnez plutôt l’option pour la masquer, ce qui empêche les utilisateurs de la sélectionner ultérieurement.</p> </li> 
    </ul> 
     </li> 
    </ol> </td> 
    <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Menu déroulant</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   ou

   Pour copier un champ, pointez dessus, puis cliquez sur l’icône Copier.

   ![icône de copie](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   ou

   Cliquez sur **Enregistrer et fermer**.

### Ajout de champs de type anticipé et date

Vous pouvez ajouter des champs de saisie anticipée et de date à un formulaire personnalisé.

+++ **Développer pour afficher les descriptions des champs disponibles**

* **Tirage anticipé**: permet aux utilisateurs de saisir le nom d’un objet existant dans Workfront. Une liste de suggestions s’affiche lorsque l’utilisateur commence à saisir du texte. Ce type de champ prend en charge les objets suivants :
   * Utilisateur
   * Groupe
   * Fonction
   * Portfolio
   * Programme
   * Projet
   * Équipe
   * Modèle
   * Entreprise
* **Champ de date**: affiche un calendrier dans lequel les utilisateurs peuvent sélectionner une date et une heure.

+++

Pour ajouter des champs de date de saisie anticipée :

1. Dans la partie gauche de l’écran, recherchez l’un des champs suivants et faites-le glisser vers une section du canevas.

   * Frappe continue
   * Champ de date

   ![](assets/drag-field-to-section.png)

1. Dans la partie droite de l’écran, configurez les options disponibles pour le type de champ personnalisé que vous ajoutez :

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Paramètre de champ</td>
    <td>Description</td>
    <td>Disponible pour </td>
    </tr>
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ personnalisé. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b>: évitez d’utiliser des caractères spéciaux dans ce libellé. Elles ne s’affichent pas correctement dans les rapports.</p> </td> 
       <td><ul>
    <li>Frappe continue</li>
    <li>Champ de date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom est la manière dont le système identifie le champ personnalisé lorsque vous l’ajoutez à différentes zones dans Workfront, telles que les rapports, l’accueil et les interactions avec l’API.</p> <p>Lorsque vous configurez le champ personnalisé pour la première fois et que vous tapez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé que vos utilisateurs voient sans avoir à modifier le nom que le système voit.</p> 
      <p><b>IMPORTANT</b>:   
      <ul> 
      <li>Bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans Workfront. Si vous le faites, le système ne reconnaîtra plus le champ personnalisé où il peut maintenant être référencé dans d’autres zones de Workfront. <p>Par exemple, si vous ajoutez le champ personnalisé à un rapport et que vous modifiez ensuite son nom, Workfront ne le reconnaît pas dans le rapport et il ne fonctionnera plus correctement à moins de le rajouter au rapport en utilisant le nouveau nom.</p> </li>
      <li> <p>Nous vous recommandons de ne pas saisir de nom déjà utilisé pour les champs Workfront intégrés.</p> </li>
      <li><p>Il est recommandé de ne pas utiliser le caractère point/point dans le nom du champ personnalisé afin d’éviter toute erreur lors de l’utilisation du champ dans différentes zones de Workfront.</p></li>
      </ul> <p>Chaque nom de champ personnalisé doit être unique dans l’instance Workfront de votre entreprise. Ainsi, vous pouvez réutiliser un formulaire déjà créé pour un autre formulaire personnalisé. Pour plus d’informations, voir <a href="#Add" class="MCXref xref">Ajouter un champ personnalisé à un formulaire personnalisé</a> dans cet article.</p> </td>
         <td><ul>
    <li>Frappe continue</li>
    <li>Champ de date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le champ personnalisé. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations saisies ici.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Frappe continue</li>
    <li>Champ de date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Afficher l'heure</td> 
      <td>Sélectionnez cette option si vous souhaitez afficher l’heure et la date dans le champ.</td> 
         <td><ul>
    <li>Champ de date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Type d'objet référencé</td> 
      <td> <p>Sélectionnez le type d’objet à associer au champ.</p> <p>Une fois que vous avez cliqué sur Appliquer ou sur Enregistrer+Fermer, vous ne pouvez pas modifier le type d’objet du champ.</p> <p><b>NOTE</b>:   
        <ul> 
         <li>Si votre administrateur Workfront a personnalisé le nom des Portfolios, programmes ou projets dans l’interface utilisateur de Workfront, le nom Workfront par défaut de l’objet s’affiche dans cette liste déroulante et non dans le nom personnalisé. Contactez votre administrateur Workfront si vous avez besoin d’aide.<br></li> 
         <li>Les types d’objets suivants sont pris en charge dans les applications mobiles iOS et Android Workfront : Utilisateur, Société, Groupe, Rôle de tâche, Portfolio, Programme, Projet et Modèle.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Frappe continue</li>
    </ul></td>
     </tr>
     <tr> 
      <td role="rowheader">Créer un champ obligatoire</td> 
      <td>Sélectionnez cette option si vous souhaitez que le champ soit obligatoire pour que l’utilisateur puisse remplir le formulaire personnalisé. </td> 
       <td><ul>
    <li>Frappe continue</li>
    <li>Champ de date</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   ou

   Pour copier un champ, pointez dessus, puis cliquez sur l’icône Copier.

   ![icône de copie](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   ou

   Cliquez sur **Enregistrer et fermer**.

### Ajout d’images, de PDF et de vidéos

Vous pouvez ajouter des images, PDF et vidéos à un formulaire personnalisé. Les utilisateurs qui utilisent l’objet auquel le formulaire personnalisé est joint peuvent afficher l’image, le PDF ou la vidéo uniquement dans les zones suivantes :

* Zone Détails de l’objet (par exemple, pour un projet, la zone Détails du projet)
* La zone Modifier de l’objet, si l’aspect de l’expérience Adobe Workfront est nouveau (par exemple, les zones Modifier le projet et Modifier la tâche).

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **Développer pour afficher les descriptions des champs disponibles**

* **Image**: permet aux utilisateurs d’ajouter _____ fichiers image.
* **PDF**: permet aux utilisateurs d’ajouter des PDF.
* **Vidéos**: permet aux utilisateurs d’ajouter ____ fichiers vidéo.

+++

Pour ajouter des images, des PDF ou des vidéos :

1. Dans la partie gauche de l’écran, recherchez l’un des champs suivants et faites-le glisser vers une section du canevas.

   * Image
   * PDF
   * Vidéo

   ![](assets/drag-field-to-section.png)

1. Saisissez ou modifiez l’une des propriétés suivantes pour le widget :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du widget. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b>: évitez d’utiliser des caractères spéciaux dans ce libellé. Elles ne s’affichent pas correctement dans les rapports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom indique comment le système identifie le widget.</p> <p>Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé que vos utilisateurs voient sans avoir à modifier le nom que le système voit.</p> <p><b>IMPORTANT</b>: bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans le widget. Si vous le faites, le système ne reconnaîtra plus le widget où il peut maintenant être référencé dans d’autres zones de Workfront. </p> <p>Chaque nom de widget doit être unique dans l’instance Workfront de votre entreprise. Ainsi, vous pouvez réutiliser un formulaire déjà créé pour un autre formulaire personnalisé. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoire) Saisissez ou collez l’URL du widget où il est stocké sur Internet.</p> 
      <p>Si vous ajoutez un widget vidéo, vous pouvez le faire en ajoutant ce qui suit dans la zone URL :</p> 
      <ul> 
      <li> <p>Lien YouTube ou Vimeo</p> </li> 
      <li> <p>Lien vidéo de Google Drive</p> </li> 
      <li> <p>Lien vers une vidéo avec les extensions MP4 et MOV</p> </li> 
      <li> <p>Lien vers la vidéo déjà téléchargée dans la zone Documents de votre instance Workfront. Pour obtenir des instructions, voir <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Ajout d’un widget vidéo à un formulaire personnalisé à partir de la zone Documents</a> dans cet article.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le widget. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations saisies ici.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taille</td> 
      <td>Modifiez la taille d’affichage du widget selon vos besoins.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   ou

   Pour copier un champ, pointez dessus, puis cliquez sur l’icône Copier.

   ![icône de copie](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   ou

   Cliquez sur **Enregistrer et fermer**.

#### **Ajout d’un widget vidéo à un formulaire personnalisé à partir de la zone Documents**{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Lorsque vous ajoutez ainsi une vidéo à un formulaire personnalisé, seules les autorisations définies pour le formulaire personnalisé s’appliquent à la vidéo lorsque les utilisateurs accèdent au formulaire sur un objet, et non les autorisations définies pour la vidéo dans la zone Documents.

1. Accédez à la vidéo dans la zone Documents et générez un BAT pour celle-ci, comme décrit dans la section [Créer un BAT interactif pour un site web ou tout autre contenu web](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Ouvrez le BAT.
1. Cliquez avec le bouton droit de la souris sur la vidéo, puis sélectionnez **Copier l’adresse vidéo**.
1. Dans le formulaire personnalisé dans lequel vous ajoutez le widget vidéo, collez l’adresse copiée dans le **URL** de la boîte.
1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   ou

   Cliquez sur **Enregistrer et fermer**.

### Ajout de fichiers Adobe XD

Vous pouvez ajouter un prototype Adobe XD directement à un formulaire personnalisé. Les utilisateurs qui utilisent l’objet auquel le formulaire personnalisé est joint ne peuvent afficher le fichier Adobe XD que dans les zones suivantes :

* Zone Détails de l’objet (par exemple, pour un projet, la zone Détails du projet)
* La zone Modifier de l’objet, si l’aspect de l’expérience Adobe Workfront est nouveau (par exemple, les zones Modifier le projet et Modifier la tâche).

Pour ajouter un fichier Adobe XD :

1. Dans la partie gauche de l’écran, recherchez **Adobe XD** et faites-le glisser vers une section de la zone de travail.
1. Saisissez ou modifiez l’une des propriétés suivantes pour le widget :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du widget. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b>: évitez d’utiliser des caractères spéciaux dans ce libellé. Elles ne s’affichent pas correctement dans les rapports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom indique comment le système identifie le widget. Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé que vos utilisateurs voient sans avoir à modifier le nom que le système voit.</p>
    <p><b>IMPORTANT</b>:   
      <ul> 
      <li>Bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans Workfront. Si vous le faites, le système ne reconnaîtra plus le champ personnalisé où il peut maintenant être référencé dans d’autres zones de Workfront. <p>Par exemple, si vous ajoutez le champ personnalisé à un rapport et que vous modifiez ensuite son nom, Workfront ne le reconnaît pas dans le rapport et il ne fonctionnera plus correctement à moins de le rajouter au rapport en utilisant le nouveau nom.</p> </li>
      <li> <p>Nous vous recommandons de ne pas saisir de nom déjà utilisé pour les champs Workfront intégrés.</p> </li>
      <li><p>Il est recommandé de ne pas utiliser le caractère point/point dans le nom du champ personnalisé afin d’éviter toute erreur lors de l’utilisation du champ dans différentes zones de Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoire) Saisissez ou collez un lien de prototype XD valide.</p> 
      <p>Remarque : le paramètre Accès au lien de l’onglet Partager d’Adobe XD doit être défini sur N’importe qui avec le lien. Sinon, les utilisateurs ne pourront pas afficher le prototype. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le widget. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations saisies ici.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taille</td> 
      <td>(Facultatif) Modifiez la taille d’affichage du widget selon vos besoins.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   ou

   Pour copier un champ, pointez dessus, puis cliquez sur l’icône Copier.

   ![icône de copie](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   ou

   Cliquez sur **Enregistrer et fermer**.

## Organisation et prévisualisation d’un formulaire avec le concepteur de formulaires

Pour plus d’informations sur l’organisation et l’affichage d’un aperçu de votre formulaire, voir [Organisation et prévisualisation d’un formulaire avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
