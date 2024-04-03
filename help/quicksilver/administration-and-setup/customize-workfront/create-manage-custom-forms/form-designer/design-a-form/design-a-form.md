---
title: Concevoir un formulaire avec le concepteur de formulaires
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez concevoir un formulaire personnalisé à l’aide du concepteur de formulaire. Vous pouvez joindre des formulaires personnalisés à différents objets Workfront pour capturer des données sur ces objets.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: 83036270d430dcc80069f4de87b6ac1e8da689e3
workflow-type: tm+mt
source-wordcount: '6079'
ht-degree: 4%

---

# Concevoir un formulaire avec le concepteur de formulaires

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients ou dans l’environnement Production pour les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, voir [Présentation de la version du deuxième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Vous pouvez concevoir un formulaire personnalisé à l’aide du concepteur de formulaire. Vous pouvez joindre des formulaires personnalisés à différents objets Workfront pour capturer des données sur ces objets.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Commencer à concevoir un formulaire personnalisé

{{step-1-to-setup}}

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
   * [Ajout de champs de recherche externes](#add-external-lookup-fields)
   * [Ajout d’images, de PDF et de vidéos](#add-images-pdfs-and-videos)
   * [Ajout de champs natifs Workfront](#add-workfront-native-fields)
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

  Ce type de champ personnalisé n’est pas pris en charge dans les filtres sur les listes et les rapports.

  Pour plus d’informations sur l’accès à ce champ par le biais de l’API, voir [Stockage de champs de texte enrichi dans l’API](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md).

  >[!NOTE]
  >
  >Les champs de texte avec mise en forme ne sont pas disponibles pour les applications mobiles Workfront (disponibles dans les prochaines versions).

* **Texte descriptif**: vous permet d’inclure des instructions et de créer des liens vers des pages en dehors de Workfront.

+++

Pour ajouter un champ de texte :

1. Dans la partie gauche de l’écran, recherchez l’un des champs de texte suivants et faites-le glisser vers une section du canevas :

   * Une seule ligne de texte
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
    <td><p>Sélectionnez le type de données qui sera capturé dans le champ personnalisé.</p> <p><b>REMARQUE</b>:   
    <ul> 
    <li>Une fois le formulaire enregistré, ce champ ne peut plus être modifié. Si vous envisagez d’utiliser votre champ dans des calculs mathématiques, veillez à sélectionner le format Nombre ou Devise .</li> 
    <li>Lorsque vous sélectionnez Nombre ou Devise, le système tronque automatiquement les nombres qui commencent par 0.</li>
    <li>La limite de caractères pour les champs Nombre est 16. Vous pouvez également utiliser un champ Texte pour saisir des nombres et éviter la limite.</li>
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

>[!NOTE]
>
>Les champs qui autorisent plusieurs sélections, tels que Groupe de cases à cocher et Liste déroulante, sont difficiles à associer et à associer dans les rapports. Pour simplifier la création de graphiques et de regroupements dans les rapports, vous pouvez créer des champs distincts pour chaque choix (par exemple, un champ de texte d’une seule ligne).

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
    <td> <p>Sélectionnez le type de données qui sera capturé dans le champ personnalisé.</p> <p><b>REMARQUE</b>:   
     <ul> 
    <li>Une fois le formulaire enregistré, ce champ ne peut plus être modifié. Si vous envisagez d’utiliser votre champ dans des calculs mathématiques, veillez à sélectionner le format Nombre ou Devise .<br></li> 
    <li>Lorsque vous sélectionnez Nombre ou Devise, le système tronque automatiquement les nombres qui commencent par 0.</li>
    <li>La limite de caractères pour les champs Nombre est 16. Vous pouvez également utiliser un champ Texte pour saisir des nombres et éviter la limite.</li>
     </ul></p></td> 
     <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Menu déroulant</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Type d'affichage</td> 
    <td>Basculez entre les boutons radio, les groupes de cases à cocher, les listes déroulantes ou les listes déroulantes à sélection multiple pour le champ.</td> 
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
   * l’utilisateur ou de l’utilisatrice
   * Groupe
   * Fonction
   * Portfolio
   * Programme
   * Projet
   * Equipe
   * Modèle
   * Entreprise
* **Champ de date**: affiche un calendrier dans lequel les utilisateurs peuvent sélectionner une date et une heure.

+++

Pour ajouter des champs de saisie anticipée et de date :

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
      <td> <p>Sélectionnez le type d’objet à associer au champ.</p> <p>Une fois que vous avez cliqué sur Appliquer ou sur Enregistrer+Fermer, vous ne pouvez pas modifier le type d’objet du champ.</p> <p><b>REMARQUE</b>:   
        <ul> 
         <li>Si votre administrateur Workfront a personnalisé le nom des Portfolios, programmes ou projets dans l’interface utilisateur de Workfront, le nom Workfront par défaut de l’objet s’affiche dans cette liste déroulante et non dans le nom personnalisé. Contactez votre administrateur Workfront si vous avez besoin d’aide.<br></li> 
         <li>Les types d’objets suivants sont pris en charge dans les applications mobiles iOS et Android Workfront : Utilisateur, Société, Groupe, Rôle de tâche, Portfolio, Programme, Projet et Modèle.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Frappe continue</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">Ajouter filtre</td>
      <td><p>Ajoutez un filtre pour un type d’objet afin de limiter les objets que les utilisateurs peuvent sélectionner lorsqu’ils utilisent le champ . </p> <p>Par exemple, vous pouvez limiter un champ afin que les noms d’utilisateur ne puissent être sélectionnés que s’ils répondent aux critères suivants :</p> 
       <ul> 
        <li>Ils appartiennent à un ou à des groupes que vous spécifiez.</li> 
        <li>Ils sont associés à un rôle ou à un titre de tâche que vous spécifiez.</li> 
        <li>Ils appartiennent au même groupe que la personne qui utilise le champ.</li> 
       </ul> <p>Vous devez définir le filtre correspondant au type d’objet sélectionné à l’aide de la syntaxe Mode texte . Pour plus d’informations sur la création d’un filtre à l’aide du mode Texte, voir <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Modification d’un filtre à l’aide du mode texte</a>.</p>
       <p><b>REMARQUE</b>:
       <ul> 
        <li>Si vous modifiez un formulaire personnalisé existant, l’ajout d’un filtre à un champ de type anticipée ne supprime aucun objet (hors portée du filtre) déjà ajouté par les utilisateurs à l’aide du champ.</li> 
        <li>Ce filtre n’est pas disponible sur les appareils mobiles. Si vous utilisez le filtre pour un champ Type , il apparaîtra sur les appareils mobiles des utilisateurs qui ne sont pas affectés par le filtre.</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>Frappe continue</li>
       </ul>
      </td>
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

### Ajout de champs de recherche externes

Un champ de recherche externe appelle une API externe et renvoie les valeurs sous forme d’options dans un champ déroulant. Les utilisateurs qui utilisent l’objet auquel le formulaire personnalisé est joint peuvent sélectionner une ou plusieurs de ces options dans la liste déroulante. Le champ de recherche externe est également disponible dans les listes et les rapports.

Pour des exemples d’utilisation du champ Recherche externe pour appeler la même instance de Workfront ou une API publique, voir [Exemples de champs de recherche externe dans un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>La fonctionnalité de recherche externe n’est pas disponible sur les objets Document ou Utilisateur.
>
>Les champs de recherche externes des formulaires personnalisés ne sont actuellement pas pris en charge dans les tableaux de bord. Vous ne pouvez pas modifier la valeur du champ en ligne et elle peut ne pas s’afficher correctement dans un tableau de bord.

Pour ajouter une recherche externe :

1. Dans la partie gauche de l’écran, recherchez **Recherche externe** et faites-le glisser vers une section de la zone de travail.
1. Dans la partie droite de l’écran, configurez les options du champ personnalisé :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ personnalisé. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b>: évitez d’utiliser des caractères spéciaux dans ce libellé. Elles ne s’affichent pas correctement dans les rapports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom est la manière dont le système identifie le champ personnalisé.</p> <p>Lorsque vous configurez le champ personnalisé pour la première fois et que vous tapez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé que vos utilisateurs voient sans avoir à modifier le nom que le système voit.</p> 
      <p><b>IMPORTANT</b>:   
      <ul> 
      <li>Bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans Workfront. Si vous le faites, le système ne reconnaîtra plus le champ personnalisé où il peut maintenant être référencé dans d’autres zones de Workfront. <p>Par exemple, si vous ajoutez le champ personnalisé à un rapport et que vous modifiez ensuite son nom, Workfront ne le reconnaît pas dans le rapport et il ne fonctionnera plus correctement à moins de le rajouter au rapport en utilisant le nouveau nom.</p> </li>
      <li> <p>Nous vous recommandons de ne pas saisir de nom déjà utilisé pour les champs Workfront intégrés.</p> </li>
      <li><p>Il est recommandé de ne pas utiliser le caractère point/point dans le nom du champ personnalisé afin d’éviter toute erreur lors de l’utilisation du champ dans différentes zones de Workfront.</p></li>
      </ul> <p>Chaque nom de champ personnalisé doit être unique dans l’instance Workfront de votre entreprise. Ainsi, vous pouvez réutiliser un formulaire déjà créé pour un autre formulaire personnalisé. Pour plus d’informations, voir <a href="#Add" class="MCXref xref">Ajouter un champ personnalisé à un formulaire personnalisé</a> dans cet article.</p> </td>
     </tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le champ personnalisé. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations saisies ici.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td>
      <td><p>Sélectionnez le type de données qui sera capturé dans le champ personnalisé.</p>
      <p><strong>REMARQUE :</strong></p>
      <ul><li>Vous pouvez modifier le type de format après l’enregistrement du formulaire, avec une limitation : toutes les valeurs existantes sur les objets doivent pouvoir être converties dans le nouveau type. (Par exemple, si le type de format est Texte et qu’un objet stocke la valeur "abc", vous ne pouvez pas convertir le champ et obtenez une erreur indiquant que le système ne peut pas convertir "abc" en nombre/devise.) Si vous envisagez d’utiliser votre champ dans des calculs mathématiques, veillez à sélectionner le format Nombre ou Devise .</li>
      <li>Lorsque vous sélectionnez Nombre ou Devise, le système tronque automatiquement les nombres qui commencent par 0.</li>
      <li>La limite de caractères pour les champs Nombre est 16. Vous pouvez également utiliser un champ Texte pour saisir des nombres et éviter la limite.</li>
      </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">URL API de base</td> 
      <td><p>Saisissez ou collez l’URL de l’API.</p><p>L’URL de l’API doit renvoyer un contenu JSON des options que vous souhaitez afficher dans la liste déroulante. Vous pouvez utiliser le champ Chemin d’accès JSON pour sélectionner les valeurs spécifiques du fichier JSON renvoyé dans les options de liste déroulante.</p><p>Lorsque vous saisissez l’URL de l’API, vous pouvez éventuellement transmettre les valeurs suivantes dans l’URL :</p>
      <ul>
      <li>$$HOST : il représente l’hôte Workfront actuel et peut être utilisé pour effectuer des appels d’API /search à l’API Workfront. Lorsque ce caractère générique est utilisé, l’authentification est gérée et les utilisateurs n’ont pas besoin d’envoyer d’en-têtes d’authentification. (Par exemple, les utilisateurs peuvent rechercher des tâches à l’aide de l’URL de base. <code>$$HOST/attask/api/task/search</code> et permet de rechercher des tâches et de sélectionner des valeurs dans une liste de tâches renvoyée.)</li>
      <li><p>$$QUERY : il s’agit du texte de recherche saisi par l’utilisateur final dans le champ et qui vous permet d’implémenter le filtrage des requêtes pour vos utilisateurs finaux. (L’utilisateur recherche la valeur dans la liste déroulante.)</p>
      <p>Si l’API que vous référencez l’autorise, vous pouvez également inclure des modificateurs dans votre requête de recherche pour identifier le fonctionnement de la recherche. Par exemple, vous pouvez utiliser les éléments suivants comme URL de l’API de base pour permettre aux utilisateurs de rechercher des projets Workfront contenant du texte spécifique : <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>En savoir plus sur les modificateurs de recherche Workfront dans <a href="/help/quicksilver/wf-api/general/api-basics.md">Principes de base des API</a>.</p>
      <p><strong>REMARQUE :</strong> Si vous n’utilisez pas $$QUERY et que l’utilisateur saisit du texte dans la zone de recherche, les choix que vous avez déjà sont réduits. Cependant, si vous utilisez $$QUERY et que l’utilisateur saisit quoi que ce soit, un nouvel appel réseau à votre API est effectué. Par conséquent, si votre API contient plus de 2 000 valeurs et que l’API prend en charge l’interrogation, vous pouvez utiliser $$QUERY pour effectuer une recherche non seulement à partir des valeurs 2 000 existantes, mais aussi à partir de l’API d’origine avec les options restreintes.</p></li>
      <li><p>{fieldName} - Où fieldName est un champ personnalisé ou natif dans Workfront. Ainsi, vous pouvez implémenter des filtres d’options de liste déroulante en cascade lorsque vous transmettez la valeur d’un champ déjà sélectionné au champ Recherche externe pour filtrer les options. (Par exemple, le champ Région existe déjà sur le formulaire et vous limitez une liste de pays de l’API à ceux d’une région spécifique.)</p>
      <p>Pour un champ de recherche externe qui dépend d’autres champs (à l’aide de la variable {fieldName} ), les options renvoyées par l’API sont limitées à celles qui correspondent à toutes les chaînes ou valeurs saisies dans les autres champs. (Cette fonctionnalité n’est pas prise en charge dans les listes et les rapports.)</p></li>
      <li>{referenceObject}.{fieldName} - Où le champ fait partie d’un objet. Cette syntaxe est similaire aux expressions personnalisées. (Par exemple, portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>REMARQUE :</strong> Consultez la documentation de l’API que vous utilisez pour les requêtes spécifiques que vous pouvez définir.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Méthode HTTP</td> 
      <td>Sélectionner <strong>Get</strong>, <strong>Post</strong>, ou <strong>Put</strong> pour la méthode .</td> 
     </tr>
     <tr> 
      <td role="rowheader">Chemin JSON</td>
      <td><p>Saisissez ou collez le chemin JSON de l’API.</p> <p>Cette option permet d’extraire des données du code JSON renvoyé par l’URL de l’API. Il sert à sélectionner les valeurs qui, à l’intérieur du fichier JSON, apparaîtront dans les options de la liste déroulante.</p><p>Par exemple, si votre URL d’API renvoie JSON au format suivant :</br>
      <pre>
      { data: { name: "USA"}, { name: "Canada"} } }
      </pre>
      </p>
      <p>vous pouvez ensuite utiliser "$.data[*].name" pour sélectionner les États-Unis et le Canada comme options de liste déroulante.</p> <p>Pour plus d’informations sur le chemin JSON et pour vous assurer que vous écrivez le chemin JSON correct, reportez-vous à la section <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">En-têtes</td>
      <td><p>Cliquez sur <strong>Ajouter un en-tête</strong>et saisissez ou collez la paire clé-valeur requise pour l’authentification avec l’API.</p><p><strong>REMARQUE :</strong> Les champs En-tête ne sont pas un lieu sécurisé pour stocker les informations d’identification. Vous devez donc veiller à ce que vous saisissiez et enregistrez.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Menu déroulant multi-sélection</td>
      <td><p>Sélectionnez cette option pour permettre à l’utilisateur de sélectionner plusieurs valeurs dans la liste déroulante.</p></td>
     </tr>
     </tr>
     <tr> 
      <td role="rowheader">Créer un champ obligatoire</td>
      <td><p>Sélectionnez cette option si vous souhaitez que le champ soit obligatoire pour que l’utilisateur puisse remplir le formulaire personnalisé.</p></td>
     </tr>       
    </tbody>
   </table>

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   ou

   Cliquez sur **Enregistrer et fermer**.

>[!NOTE]
>
>Les éléments suivants sont des limites techniques de l’appel à l’API externe :
>
>* Nombre maximal d’options : 2 000 (seules les 2 000 premières options uniques du fichier JSON renvoyé sont affichées)
>* Timeout : 3 secondes
>* Nombre de reprises : 3
>* Durée d’attente entre deux tentatives : 500 ms
>* Statuts de réponse attendus : 2xx

### Ajout d’images, de PDF et de vidéos

Vous pouvez ajouter des images, des PDF et des vidéos à un formulaire personnalisé. Les utilisateurs qui utilisent l’objet auquel le formulaire personnalisé est joint peuvent afficher l’image, le PDF ou la vidéo uniquement dans les zones suivantes :

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
      <td> <p>(Obligatoire) Ce nom correspond à la manière dont le système identifie le widget.</p> <p>Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé que vos utilisateurs voient sans avoir à modifier le nom que le système voit.</p> <p><b>IMPORTANT</b>: bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans Workfront. Si vous le faites, le système ne reconnaîtra plus le widget où il peut maintenant être référencé dans d’autres zones de Workfront. </p> <p>Chaque nom de widget doit être unique dans l’instance Workfront de votre entreprise. Ainsi, vous pouvez réutiliser un formulaire déjà créé pour un autre formulaire personnalisé. </p> </td> 
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

#### Ajout d’un widget vidéo à un formulaire personnalisé à partir de la zone Documents{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

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

<div class="preview">

### Ajout de champs natifs Workfront

Vous pouvez ajouter des champs natifs Workfront à vos formulaires personnalisés. Lorsque le formulaire personnalisé est associé à un objet, le champ est renseigné à partir des données de l’objet. Par exemple, le champ Description d’un formulaire personnalisé joint à un projet extrait la description du projet. (Le champ peut afficher &quot;S.O.&quot; si aucune donnée n’est disponible.)

+++ **Développer pour afficher la liste des champs natifs pris en charge**

Ce tableau répertorie les champs natifs disponibles pour des objets Workfront spécifiques dans un formulaire personnalisé.

| Nom du champ | Projet | Tâche | Problème | Modèle | Tâche de modèle | Portfolio | Programme | Groupe |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| Date d&#39;achèvement effective | ✓ | ✓ | ✓ |   |   |   |   |   |
| Durée effective | ✓ |   |   |   |   |   |   |   |
| Heures effectives | ✓ |   | ✓ |   |   |   |   |   |
| Date de début effective | ✓ | ✓ | ✓ |   |   |   |   |   |
| Entreprise | ✓ |   |   | ✓ |   |   |   |   |
| Condition | ✓ | ✓ | ✓ |   |   |   |   |   |
| Type de condition | ✓ |   |   | ✓ |   |   |   |   |
| Description | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Durée |   | ✓ |   |   | ✓ |   |   |   |
| Type de durée |   | ✓ |   |   | ✓ |   |   |   |
| Unité de durée |   | ✓ |   |   | ✓ |   |   |   |
| Entré par | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Date d’entrée | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Groupe | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Dernière mise à jour par | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Date de dernière mise à jour | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Nom | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Propriétaire | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Date d&#39;achèvement prévue | ✓ | ✓ | ✓ |   |   |   |   |   |
| Durée prévue | ✓ |   |   | ✓ |   |   |   |   |
| Heures prévues | ✓ | ✓ | ✓ |   | ✓ |   |   |   |
| Date de début prévue | ✓ |   |   |   |   |   |   |   |
| Portfolio | ✓ |   |   | ✓ |   |   | ✓ |   |
| Priorité | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Programme | ✓ |   |   | ✓ |   |   |   |   |
| Date d&#39;achèvement prévisionnelle | ✓ | ✓ |   |   |   |   |   |   |
| Durée prévisionnelle en minutes |   | ✓ |   |   |   |   |   |   |
| Date de début prévisionnelle | ✓ | ✓ |   |   |   |   |   |   |
| Numéro de référence | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Mode horaire | ✓ |   |   | ✓ |   |   |   |   |
| Gravité |   |   | ✓ |   |   |   |   |   |
| Sponsor | ✓ |   |   | ✓ |   |   |   |   |
| Statut | ✓ | ✓ |   |   |   |   |   |   |
| Points de l&#39;histoire |   | ✓ |   |   |   |   |   |   |
| Modèle | ✓ |   |   |   |   |   |   |   |
| URL | ✓ | ✓ |   | ✓ | ✓ |   |   |   |

{style="table-layout:auto"}

+++

1. Dans la partie gauche de l’écran, recherchez **Champ natif** et faites-le glisser vers une section de la zone de travail.
1. Dans la partie droite de l’écran, configurez les options du champ personnalisé :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b>: évitez d’utiliser des caractères spéciaux dans ce libellé. Elles ne s’affichent pas correctement dans les rapports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom est la manière dont le système identifie le champ.</p><p> Lorsque vous configurez le champ pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé que vos utilisateurs voient sans avoir à modifier le nom que le système voit.</p>
      <p><b>IMPORTANT</b>:
      <ul> 
      <li>Bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans Workfront. Si vous le faites, le système ne reconnaîtra plus le champ où il peut maintenant être référencé dans d’autres zones de Workfront.</p> </li>
      <li> <p>Chaque nom de champ doit être unique dans l’instance Workfront de votre entreprise. Ainsi, vous pouvez réutiliser un formulaire déjà créé pour un autre formulaire personnalisé.</p> </li>
      <li><p>Il est recommandé de ne pas utiliser le caractère point/point dans le nom du champ personnalisé afin d’éviter toute erreur lors de l’utilisation du champ dans différentes zones de Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le champ. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations saisies ici.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Champ de référence</td> 
      <td><p>(Obligatoire) Sélectionnez un champ natif Workfront.<p><p>Seuls les champs natifs des objets de formulaire sont disponibles. Par exemple, si la liste Types d’objet située en haut du concepteur de formulaire affiche Projet, vous pouvez sélectionner des champs natifs pour les projets, mais pas des champs spécifiques aux tâches.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Taille</td> 
      <td>(Facultatif) Modifiez la taille d’affichage du champ selon vos besoins.</td> 
     </tr> 
    </tbody> 
   </table>

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   ou

   Cliquez sur **Enregistrer et fermer**.

</div>

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
      <td> <p>(Obligatoire) Ce nom correspond à la manière dont le système identifie le widget. Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé que vos utilisateurs voient sans avoir à modifier le nom que le système voit.</p>
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
