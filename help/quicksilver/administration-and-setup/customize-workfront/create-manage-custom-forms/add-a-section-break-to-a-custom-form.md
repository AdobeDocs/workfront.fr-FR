---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Ajout d’un saut de section à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires
description: Vous pouvez regrouper les champs personnalisés et les widgets d’un formulaire personnalisé en sections avec des en-têtes. Cela s’avère utile pour présenter une expérience organisée aux utilisateurs et utilisatrices qui remplissent le formulaire. En outre, si vous devez limiter l’accès à certains champs et widgets personnalisés à des utilisateurs ou utilisatrices, vous pouvez les placer dans une section, puis accorder l’accès à la section à ces utilisateurs et utilisatrices uniquement.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 76%

---

# Ajout d’un saut de section à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires

{{form-designer-default}}

Vous pouvez regrouper les champs personnalisés et les widgets d’un formulaire personnalisé en sections avec des en-têtes. Cela s’avère utile pour présenter une expérience organisée aux utilisateurs et utilisatrices qui remplissent le formulaire. En outre, si vous devez limiter l’accès à certains champs et widgets personnalisés à des utilisateurs ou utilisatrices, vous pouvez les placer dans une section, puis accorder l’accès à la section à ces utilisateurs et utilisatrices uniquement.

Par exemple, si vous devez suivre des informations sensibles que seuls les administrateurs et administratrices système doivent être en mesure d’afficher ou de modifier, vous pouvez créer un saut de section avec les autorisations Admin uniquement et placer les champs sensibles dans cette section.

Les paramètres d’accès que vous sélectionnez pour une section sont directement liés aux autorisations dont disposent les utilisateurs et utilisatrices sur l’objet Workfront auquel le formulaire personnalisé est associé. Vous pouvez masquer ou afficher une section selon que l’utilisateur ou l’utilisatrice dispose d’un accès pour afficher, contribuer à ou gérer cet objet. Vous pouvez également définir une section sur Admin uniquement de sorte que seuls les utilisateurs et les utilisatrices disposant d’un niveau d’accès administrateur ou administratrice système puissent y accéder.

Pour plus d’informations sur les autorisations sur les objets, voir [Vue d’ensemble du partage des autorisations sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Ajouter un champ personnalisé à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) et [Ajouter ou modifier un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Forfait Adobe Workfront</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouvelle : standard</p>
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p></td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer et configurer l’accès pour une section dans un formulaire personnalisé

1. Commencez à créer ou modifier un formulaire personnalisé, comme décrit dans la section [Créer ou modifier un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Ajoutez des champs et des widgets personnalisés au formulaire, comme décrit dans [Ajouter un champ personnalisé à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) et [Ajouter ou modifier un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. Lors de la création ou de la modification du formulaire personnalisé, dans l’onglet **Ajouter un champ**, cliquez sur **Saut de section**.

   ![](assets/click-section-break.jpg)

1. Dans l’onglet **Paramètres du champ**, configurez les options de la section :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus de la section. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b> : évitez d’utiliser des caractères spéciaux dans cette étiquette. Ils ne s’affichent pas correctement dans les rapports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Saisissez du texte si vous souhaitez expliquer aux utilisateurs et utilisatrices à quoi sert la section. Celui-ci s’affiche sous le libellé de la section sur le formulaire personnalisé.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Ajouter une logique</p></td> 
      <td><p>Utilisez la logique d’affichage pour spécifier si la section doit s’afficher sur le formulaire, en fonction des sélections que les utilisateurs font dans des champs personnalisés à choix multiples lorsqu’ils remplissent le formulaire.</p><p><strong>REMARQUE :</strong> Si la logique d’affichage de tous les champs individuels d’un saut de section est appliquée à tous et qu’ils sont tous masqués en raison de la logique, la section entière est masquée sur le formulaire personnalisé. Cela se produit même si la logique d’affichage n’est pas appliquée au saut de section.</p><p>Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Ajouter une logique d’affichage et une logique de saut dans un formulaire personnalisé</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Accorder l’accès</p> </td> 
      <td> <p> Sélectionnez les autorisations dont les utilisateurs et les utilisatrices ont besoin sur un objet où le formulaire personnalisé est joint afin d’afficher cette section et de modifier ses valeurs de champ.
       <p>Les autorisations suivantes sont disponibles sous <b>Les utilisateurs et utilisatrices avec cet accès à l’objet peuvent afficher les valeurs de champ</b> :</p> 
         <ul>
          <li><strong>Afficher</strong> : autorisations d’affichage sur l’objet.</li>
          <li><p><b>Modification limitée</b> : (disponible uniquement si l’objet est un projet, une tâche, un problème ou un utilisateur ou une utilisatrice) :</p> 
          <p>Permet aux utilisateurs et utilisatrices de contribuer à l’objet s’il s’agit d’un projet, d’une tâche ou d’un problème.</p>
          <p>Permet aux utilisateurs et utilisatrices de modifier le profil ou de posséder l’autorisation de profil sur l’objet s’il s’agit d’un utilisateur ou d’une utilisatrice.</p></li> 
          <li><b>Modifier</b> : autorisations de gestion sur l’objet. </li> 
          <li><b>Admin uniquement</b> : niveau d’accès administrateur ou administratrice système.</li> 
         </ul> </li> 
        <p>Les autorisations suivantes sont disponibles sous <b>Les utilisateurs et utilisatrices avec cet accès à l’objet peuvent modifier les valeurs de champ</b> : </p> 
         <ul> 
          <li> <p><b>Modification limitée</b> : (disponible uniquement si l’objet est un projet, une tâche, un problème ou un utilisateur ou une utilisatrice) :</p> 
           <p>Si l’objet est un projet, une tâche ou un problème, cette autorisation permet aux utilisateurs et utilisatrices de contribuer à l’objet.</p>
          <p>Si l’objet est un utilisateur ou une utilisatrice, cette autorisation permet aux utilisateurs et utilisatrices de modifier le profil ou de posséder l’autorisation de profil sur l’objet.</p> 
          <li><b>Modification</b> : autorisations de gestion pour l’objet </li> 
          <li><b>Administrateur ou administratrice uniquement</b> : niveau d’accès administration système</li> 
         </ul> </li> 
       </ul> 
       <p>Pour plus d’informations sur les autorisations sur les objets, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Vue d’ensemble du partage d’autorisations sur les objets</a>.</p> 
       <p><b>REMARQUE</b> :  
       <ul> 
       <li> <p>Les utilisateurs et utilisatrices ne disposant pas des autorisations que vous indiquez ici ne peuvent pas voir les champs personnalisés et les widgets de la section. </p> <p>C’est également le cas si vous affichez les valeurs des champs dans les rapports ou si vous les utilisez dans les champs calculés des rapports en mode texte.</p> </li>
       <li><p>Pour les formulaires personnalisés de demande/publication : si l’accès Affichage est nécessaire pour voir les champs dans le saut de section, mais qu’un accès administrateur est nécessaire pour modifier les champs, la section et tous ses champs ne seront pas visibles par les non-administrateurs lorsqu’ils rempliront le formulaire. Une fois la requête créée, les utilisateurs disposant de l’accès Affichage peuvent afficher les champs de la section .</p></li>
       <li> <p>L’association de plusieurs types d’objets à votre formulaire peut modifier les autorisations d’affichage et de modification disponibles au cours de ces étapes. Pour plus d’informations, consultez la section <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Comment plusieurs types d’objets peuvent affecter les autorisations de saut de section dans un formulaire personnalisé</a> de cet article.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Faites glisser ou ajoutez au moins un champ ou un widget personnalisé à la nouvelle section.

   Cette opération est nécessaire pour enregistrer la section.

1. Cliquez sur **Terminé**.

   >[!TIP]
   >
   >Cliquez sur **Appliquer** lorsque vous créez un formulaire personnalisé pour enregistrer vos modifications et garder le formulaire ouvert.

1. Si vous souhaitez continuer à créer votre formulaire personnalisé d’une autre manière, consultez les articles suivants :

   * [Ajouter un champ personnalisé à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [Ajouter ou modifier un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Ajouter des données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Positionner des champs personnalisés et des widgets dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Ajouter une logique d’affichage et une logique de saut dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Prévisualiser et finaliser un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
DRAFTED IN FLARE:
<h2>Configure access for fields without section breaks</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields

and widgets

to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## Comment plusieurs types d’objets peuvent affecter les autorisations de saut de section {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

L’autorisation de modification limitée pour les sauts de section de formulaire personnalisés est disponible uniquement pour les types d’objets Projet, Tâche, Problème et Utilisateur ou Utilisatrice.

Dans un formulaire personnalisé avec un saut de section configuré et l’autorisation de modification limitée, si vous ajoutez l’un des autres types d’objets au formulaire (Portfolio, Programme, Document, Société, Enregistrement de facturation, Itération, Dépenses ou Groupe), Workfront vous demandera de passer à l’autorisation de modification, qui est compatible avec ce type d’objet et les types d’objets existants du formulaire.

>[!INFO]
>
>**Exemple :** dans un formulaire personnalisé associé au type d’objet Projet, un saut de section est configuré avec l’autorisation de modification limitée.
>
>Vous ajoutez le type d’objet Portfolio au formulaire, ce qui signifie que l’option d’autorisation de modification limitée n’est plus disponible pour le saut de section dans le formulaire.
>
>Un message à l’écran vous invite à passer à l’autorisation Modifier, qui est l’option la plus similaire à Modifier limité. Elle est compatible avec le type d’objet Projet et le type d’objet Portfolio.

