---
title: Ajout ou modification d’une image ou d’un autre widget de ressource dans un formulaire personnalisé à l’aide de l’ancien créateur de formulaires
description: Vous pouvez ajouter ou modifier les propriétés de l’un des widgets de ressource suivants, tels que des images, des vidéos, des fichiers de PDF et des fichiers Adobe XD, dans un formulaire personnalisé. Cela s’avère utile lorsque vous devez inclure du contenu visuel tel que des images de marque, une vidéo pédagogique ou un prototype interactif pour une application que vous concevez.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 63%

---

# Ajout ou modification d’une image ou d’un autre widget de ressource dans un formulaire personnalisé à l’aide de l’ancien créateur de formulaires

{{form-designer-default}}

Vous pouvez ajouter ou modifier les propriétés de l’un des widgets de ressource suivants dans un formulaire personnalisé :

* Image
* Vidéo
* Fichier PDF
* Fichier Adobe XD

Cela s’avère utile lorsque vous devez inclure du contenu visuel tel que des images de marque, une vidéo pédagogique ou un prototype interactif pour une application que vous concevez.

Lorsqu’un formulaire personnalisé contenant un widget est associé à un objet, les utilisateurs qui travaillent avec l’objet peuvent le voir dans les zones suivantes :

* La zone de détails de l’objet (par exemple, la zone de détails du projet pour un projet)
* La zone Modifier de l’objet, si elle a l’aspect de la nouvelle expérience d’Adobe Workfront (par exemple, les zones Modifier le projet et Modifier la tâche)

Actuellement, les utilisateurs ne peuvent pas voir le widget dans les zones suivantes : &#x200B;

* Listes et rapports
* Accueil et Récapitulatif
* La zone Modifier de l’objet, s’il ne présente pas l’apparence de la nouvelle expérience Adobe Workfront (par exemple, la zone Modifier les dépenses)
* L’application mobile Workfront


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
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Pour plus d’informations sur la manière dont les administrateurs et administratrices de Workfront accordent cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroyer aux utilisateurs et utilisatrices un accès administratif à certaines zones</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur Workfront.

## Ajout ou modification d’un widget de ressource dans un formulaire personnalisé

1. Commencez à travailler sur un formulaire personnalisé, comme décrit dans la section [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Avec la variable **Ajouter un champ** ouvrez l’onglet , effectuez l’une des opérations suivantes :

   * Si vous ajoutez un nouveau widget, sélectionnez **Image**, **PDF**, ou **Vidéo** pour l’ajouter au bas du formulaire, ou faites-le glisser là où vous le souhaitez sur le formulaire.

     ![](assets/add-widget.png)


   * Si vous souhaitez ajouter un widget déjà ajouté à un autre formulaire personnalisé, cliquez sur **Bibliothèque de champs**, puis cliquez sur le nom du widget dans la liste qui s’affiche. Pour plus d’informations, voir [Réutilisation d’un champ ou d’un widget personnalisé dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * Si vous modifiez un widget déjà ajouté au formulaire personnalisé, sélectionnez-le.

1. Saisissez ou modifiez l’une des propriétés suivantes pour le widget :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du widget. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b> : évitez d’utiliser des caractères spéciaux dans cette étiquette. Ils ne s’affichent pas correctement dans les rapports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom correspond à la manière dont le système identifie le widget.</p> <p>Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom se remplit automatiquement pour correspondre au libellé. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la liberté de modifier le libellé que vos utilisateurs et utilisatrices voient sans avoir à modifier le nom que le système voit.</p> <p><b>IMPORTANT</b>: bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans le widget. Si vous le faites, le système ne reconnaîtra plus le widget là où il peut maintenant être référencé dans d’autres zones de Workfront. </p> <p>Chaque nom de widget doit être unique dans l’instance Workfront de votre entreprise. Vous pouvez ainsi en réutiliser un déjà créé pour un autre formulaire personnalisé. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoire) Saisissez ou collez l’URL du widget où il est stocké sur Internet.</p> 
       <p><strong>Important</strong>: l’URL de doit être une URL publique. </p>
      <p>Si vous ajoutez un widget vidéo, vous pouvez le faire en ajoutant ce qui suit dans la zone URL :</p> 
      <ul> 
      <li> <p>Lien YouTube ou Vimeo</p> </li> 
      <li> <p>Lien vidéo Google Drive</p> </li> 
      <li> <p>Lien vers une vidéo avec les extensions MP4 et MOV</p> </li> 
      <li> <p>Lien vers une vidéo déjà chargée dans la zone Documents de votre instance Workfront. Pour obtenir des instructions, voir <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Ajouter un widget vidéo à un formulaire personnalisé à partir de la zone Documents</a> dans cet article.</p> 
      </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez toute information supplémentaire concernant le widget. Lorsque les personnes remplissent le formulaire personnalisé, ils peuvent pointer sur l’icône en forme de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taille</td> 
      <td>Modifiez la taille d’affichage du widget selon vos besoins.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Appliquer**.
1. Si vous souhaitez continuer à créer votre formulaire personnalisé d’une autre manière, consultez les articles suivants :

   * [Positionner des champs personnalisés et des widgets dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Ajouter un champ personnalisé à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Réutilisation d’un champ ou d’un widget personnalisé dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Ajouter des données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Réutiliser un champ personnalisé calculé existant dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Ajouter une logique d’affichage et une logique de saut dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Prévisualiser et finaliser un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## Ajout d’un fichier XD à un formulaire personnalisé

1. Commencez à travailler sur un formulaire personnalisé, comme décrit dans la section [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Avec la variable **Ajouter un champ** ouvrir, sélectionnez **Adobe XD**.
1. Saisissez ou modifiez l’une des propriétés suivantes pour le widget :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du widget. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b> : évitez d’utiliser des caractères spéciaux dans cette étiquette. Ils ne s’affichent pas correctement dans les rapports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom correspond à la manière dont le système identifie le widget.</p> <p>Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom se remplit automatiquement pour correspondre au libellé. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la liberté de modifier le libellé que vos utilisateurs et utilisatrices voient sans avoir à modifier le nom que le système voit.</p> <p><b>IMPORTANT</b>: bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans le widget. Si vous le faites, le système ne reconnaîtra plus le widget là où il peut maintenant être référencé dans d’autres zones de Workfront. </p> <p>Chaque nom de widget doit être unique dans l’instance Workfront de votre entreprise. Vous pouvez ainsi en réutiliser un déjà créé pour un autre formulaire personnalisé. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoire) Saisissez ou collez un lien de prototype XD valide.</p> 
      <p>Remarque : le paramètre Accès au lien de l’onglet Partager d’Adobe XD doit être défini sur oute personne disposant du lien. Sinon, les utilisateurs et utilisatrices ne pourront pas afficher le prototype. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>(Facultatif) Saisissez des informations supplémentaires sur le widget. Lorsque les personnes remplissent le formulaire personnalisé, ils peuvent pointer sur l’icône en forme de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taille</td> 
      <td>(Facultatif) Modifiez la taille d’affichage du widget selon vos besoins.</td> 
     </tr> 
    </tbody> 
   </table>

1. Si vous souhaitez continuer à créer votre formulaire personnalisé d’une autre manière, consultez les articles suivants :

   * [Positionner des champs personnalisés et des widgets dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Ajouter un champ personnalisé à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Réutilisation d’un champ ou d’un widget personnalisé dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Ajouter des données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Réutiliser un champ personnalisé calculé existant dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Ajouter une logique d’affichage et une logique de saut dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Prévisualiser et finaliser un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Ajouter un widget vidéo à un formulaire personnalisé à partir de la zone Documents {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Lorsque vous ajoutez une vidéo à un formulaire personnalisé, seules les autorisations définies pour le formulaire personnalisé s’appliquent à la vidéo lorsque les utilisateurs et utilisatrices accèdent au formulaire sur un objet, et non aux autorisations définies pour la vidéo dans la zone Documents.

1. Accédez à la vidéo dans la zone Documents et générez une épreuve pour celle-ci, comme décrit dans la section [Créer une épreuve interactive pour un site web ou un autre contenu web](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Ouvrez l’épreuve.
1. Cliquez avec le bouton droit de la souris sur la vidéo, puis sélectionnez **Copier l’adresse de la vidéo**.
1. Dans le formulaire personnalisé dans lequel vous ajoutez le widget vidéo, collez l’adresse copiée dans la zone **URL**.
