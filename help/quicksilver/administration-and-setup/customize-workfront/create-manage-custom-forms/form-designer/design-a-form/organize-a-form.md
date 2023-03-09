---
title: Organisation et prévisualisation d’un formulaire à l’aide du Concepteur de formulaire
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez organiser un formulaire personnalisé à l’aide du concepteur de formulaire.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 529de9d31be883325d425dceb286d750397c5d8e
workflow-type: tm+mt
source-wordcount: '1107'
ht-degree: 0%

---


# Organisation et prévisualisation d’un formulaire avec le concepteur de formulaires

{{highlighted-preview-article-level}}

Vous pouvez organiser un formulaire personnalisé avec le concepteur de formulaire.

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
   <p>Plan hérité : Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Pour plus d’informations sur la manière dont les administrateurs de Workfront accordent cet accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## Ajout d’un saut de section

Vous pouvez regrouper les champs personnalisés et les widgets d’un formulaire personnalisé en sections avec des en-têtes. Cela s’avère utile pour présenter une expérience organisée aux utilisateurs qui remplissent le formulaire. En outre, si vous devez limiter l’accès à certains champs et widgets personnalisés à certains utilisateurs, vous pouvez les placer dans une section, puis accorder l’accès à la section à ces utilisateurs uniquement.

Par exemple, si vous devez suivre des informations sensibles que seuls les administrateurs système doivent être en mesure d’afficher ou de modifier, vous pouvez créer un saut de section avec les autorisations Admin uniquement et placer les champs sensibles dans cette section.

Les paramètres d’accès que vous sélectionnez pour une section sont directement liés aux autorisations dont disposent les utilisateurs sur l’objet Workfront auquel est associé le formulaire personnalisé. Vous pouvez masquer ou afficher une section selon que l’utilisateur a accès à l’affichage, à la contribution ou à la gestion de cet objet. Vous pouvez également définir une section sur Administrateur uniquement afin que seuls les utilisateurs disposant d’un niveau d’accès administrateur système puissent y accéder.

Pour plus d’informations sur les autorisations relatives aux objets, voir [Présentation des autorisations de partage sur les objets](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Conception d’un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Création et configuration de l’accès à une section dans un formulaire personnalisé

1. Commencez à créer ou modifier un formulaire personnalisé et à ajouter des champs, comme décrit dans la section [Conception d’un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Cliquez sur **Saut de section** et faites-le glisser à l’emplacement souhaité sur la zone de travail.

1. Dans le panneau de droite, configurez les options de la section :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus de la section. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b>: Évitez d’utiliser des caractères spéciaux dans ce libellé. Elles ne s’affichent pas correctement dans les rapports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Saisissez du texte si vous souhaitez expliquer aux utilisateurs à quoi sert la section . Celui-ci s’affiche sous le libellé de la section sur le formulaire personnalisé.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>Accorder l’accès</p> </td> 
      <td> <p> Sélectionnez les autorisations dont les utilisateurs ont besoin sur un objet où le formulaire personnalisé est joint afin d’afficher cette section et de modifier ses valeurs de champ. 
       <p>Les autorisations suivantes sont disponibles sous <b>Les utilisateurs disposant de cet accès à l’objet peuvent afficher les valeurs de champ.</b>:</p> 
         <ul>  
          <li><p><b>Modification limitée</b>: (Disponible uniquement si l’objet est un projet, une tâche, un problème ou un utilisateur) :</p> 
          <p>Permet aux utilisateurs de contribuer à l’objet s’il s’agit d’un projet, d’une tâche ou d’un problème.</p>
          <p>Permet aux utilisateurs de modifier le profil ou de posséder l’autorisation de profil pour l’objet s’il s’agit d’un utilisateur.</p></li> 
          <li><b>Modifier</b>: Gestion des autorisations pour l’objet </li> 
          <li><b>Administrateur uniquement</b>: Niveau d’accès administrateur système</li> 
         </ul> </li> 
        <p>Les autorisations suivantes sont disponibles sous <b>Les utilisateurs disposant de cet accès à l’objet peuvent modifier les valeurs de champ.</b>: </p> 
         <ul> 
          <li> <p><b>Modification limitée</b>: (Disponible uniquement si l’objet est un projet, une tâche, un problème ou un utilisateur) :</p> 
           <p>Si l’objet est un projet, une tâche ou un problème, cette autorisation permet aux utilisateurs de contribuer à l’objet</p>
          <p>Si l’objet est un utilisateur, cette autorisation permet aux utilisateurs de modifier le profil ou de posséder l’autorisation de profil pour l’objet.</p> 
          <li><b>Modifier</b>: Gestion des autorisations pour l’objet </li> 
          <li><b>Administrateur uniquement</b>: Niveau d’accès administrateur système</li> 
         </ul> </li> 
       </ul> 
       <p>Pour plus d’informations sur les autorisations relatives aux objets, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Présentation des autorisations de partage sur les objets</a>.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li> <p>Les utilisateurs ne disposant pas des autorisations que vous indiquez ici ne peuvent pas voir les champs personnalisés et les widgets dans la section . </p> <p>C’est également le cas si vous affichez les valeurs des champs dans les rapports ou si vous les utilisez dans les champs calculés dans les rapports de mode texte.</p> </li> 
       <li> <p>L’association de plusieurs types d’objets à votre formulaire peut modifier les autorisations d’affichage et de modification disponibles au cours de ces étapes. Pour plus d’informations, voir <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Comment plusieurs types d’objets peuvent affecter les autorisations de saut de section dans un formulaire personnalisé</a> dans cet article.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Faites glisser ou ajoutez au moins un champ ou un widget personnalisé à la nouvelle section. Cela est nécessaire avant d’enregistrer la section .

1. Cliquez sur **Terminé**.

   >[!TIP]
   >
   >Vous pouvez cliquer sur **Appliquer** lorsque vous créez un formulaire personnalisé pour enregistrer vos modifications et garder le formulaire ouvert.

### Comment plusieurs types d’objets peuvent affecter les autorisations de sauts de section {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

L’autorisation Modification limitée pour les sauts de section de formulaire personnalisés est disponible uniquement pour les types d’objets Projet, Tâche, Problème et Utilisateur .

Dans un formulaire personnalisé avec saut de section configuré avec l’autorisation Modifier limité , si vous ajoutez l’un des autres types d’objets au formulaire (Portfolio, Programme, Document, Société, Enregistrement de facturation, Itération, Dépenses ou Groupe), vous serez invité à passer à l’autorisation Modifier, qui est compatible avec ce type d’objet et les types d’objets existants dans le formulaire.

>[!INFO]
>
>**Exemple :** Dans un formulaire personnalisé associé au type d’objet Projet , un saut de section est configuré avec l’autorisation Modification limitée .
>
>Vous ajoutez le type d’objet Portfolio au formulaire, ce qui signifie que l’option d’autorisation Modification limitée n’est plus disponible pour le saut de section dans le formulaire.
>
>Un message à l’écran vous invite à passer à l’autorisation Modifier , qui est le niveau d’autorisation le moins élevé compatible avec le type d’objet Projet et le type d’objet Portfolio.


## Placement de champs et de widgets personnalisés dans un formulaire personnalisé


1. Commencez à créer ou modifier un formulaire personnalisé, comme décrit dans la section [Conception d’un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Pour positionner des champs et des widgets personnalisés sur la même ligne, faites glisser l’un à côté de l’autre jusqu’à ce qu’une ligne s’affiche entre eux.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* Vous pouvez utiliser la variable **Aperçu** dans le coin supérieur droit pour obtenir une idée de la façon dont les champs personnalisés et les widgets s’affichent dans le formulaire.
>* Les champs personnalisés et les widgets peuvent ne pas toujours s’afficher de la même manière dans le formulaire, selon l’espace disponible lorsqu’un utilisateur le visualise. Par exemple, le troisième champ d’une ligne de champs peut être renvoyé à la ligne suivante de champs si l’espace horizontal est limité.


1. (Facultatif) Pour positionner un champ ou un widget personnalisé au-dessus ou en dessous d’un autre, faites-le glisser au-dessus ou en dessous jusqu’à ce qu’une ligne bleue horizontale apparaisse entre les éléments.

1. Pour enregistrer vos modifications, cliquez sur **Appliquer**

   ou

   Cliquez sur **Enregistrer et fermer**.

## Aperçu d’un formulaire personnalisé

1. Commencez à créer ou modifier un formulaire personnalisé et à ajouter des champs, comme décrit dans la section [Conception d’un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Cliquez sur **Aperçu** dans le coin supérieur gauche pour voir à quoi ressemblera le formulaire lors de son utilisation, puis cliquez sur **Aperçu de la fin** pour revenir à la modification du formulaire.