---
title: Organisation et aperçu d’un formulaire
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez organiser un formulaire personnalisé avec le créateur de formulaires.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 3f7f4557c18bbb91ece850f910350d926a9e84bf
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 87%

---

# Organisation et prévisualisation d’un formulaire

Vous pouvez organiser un formulaire personnalisé avec le créateur de formulaires et le prévisualiser pour vérifier qu’il est correctement configuré.

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
   <p>ou</p>
   <p>Actuelle : formule</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter un saut de section

Vous pouvez regrouper les champs personnalisés et les widgets d’un formulaire personnalisé en sections avec des en-têtes. Cela s’avère utile pour présenter une expérience organisée aux utilisateurs et utilisatrices qui remplissent le formulaire. En outre, si vous devez limiter l’accès à certains champs et widgets personnalisés à des utilisateurs ou utilisatrices, vous pouvez les placer dans une section, puis accorder l’accès à la section à ces utilisateurs et utilisatrices uniquement.

Par exemple, si vous devez suivre des informations sensibles que seuls les administrateurs et administratrices système doivent être en mesure d’afficher ou de modifier, vous pouvez créer un saut de section avec les autorisations Admin uniquement et placer les champs sensibles dans cette section.

Les paramètres d’accès que vous sélectionnez pour une section sont directement liés aux autorisations dont disposent les utilisateurs et utilisatrices sur l’objet Workfront auquel le formulaire personnalisé est associé. Vous pouvez masquer ou afficher une section selon que l’utilisateur ou l’utilisatrice dispose d’un accès pour afficher, contribuer à ou gérer cet objet. Vous pouvez également définir une section sur Admin uniquement de sorte que seuls les utilisateurs et les utilisatrices disposant d’un niveau d’accès administrateur ou administratrice système puissent y accéder.

Pour plus d’informations sur les autorisations sur les objets, voir [Vue d’ensemble du partage des autorisations sur les objets](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

.Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Concevoir un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Créer et configurer l’accès pour une section dans un formulaire personnalisé

1. Commencez à créer ou modifier un formulaire personnalisé et à ajouter des champs, comme décrit dans [Concevoir un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Cliquez sur **Saut de section** et faites glisser à l’emplacement souhaité sur la zone de travail.

1. Dans le panneau de droite, configurez les options souhaitées pour la section :

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
       <p>Pour plus d’informations sur les autorisations sur les objets, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Vue d’ensemble du partage d’autorisations sur les objets</a>.</p> 
       <p><b>REMARQUE</b> :  
       <ul> 
       <li> <p>Les utilisateurs et utilisatrices ne disposant pas des autorisations que vous indiquez ici ne peuvent pas voir les champs personnalisés et les widgets de la section. </p> <p>C’est également le cas si vous affichez les valeurs des champs dans les rapports ou si vous les utilisez dans les champs calculés des rapports en mode texte.</p> </li> 
       <li><p>Pour les formulaires personnalisés de demande/publication : si l’accès Affichage est nécessaire pour voir les champs dans le saut de section, mais qu’un accès administrateur est nécessaire pour modifier les champs, la section et tous ses champs ne seront pas visibles par les non-administrateurs lorsqu’ils rempliront le formulaire. Une fois la requête créée, les utilisateurs disposant de l’accès Affichage peuvent afficher les champs de la section .</p></li>
       <li> <p>L’association de plusieurs types d’objets à votre formulaire peut modifier les autorisations d’affichage et de modification disponibles au cours de ces étapes. Pour plus d’informations, consultez la section <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Comment plusieurs types d’objets peuvent affecter les autorisations de saut de section dans un formulaire personnalisé</a> de cet article.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Ajouter une logique</p></td> 
      <td><p>Utilisez la logique d’affichage pour spécifier si la section doit s’afficher sur le formulaire, en fonction des sélections que les utilisateurs font dans des champs personnalisés à choix multiples lorsqu’ils remplissent le formulaire.</p><p><strong>REMARQUE :</strong> Si la logique d’affichage de tous les champs individuels d’un saut de section est appliquée à tous et qu’ils sont tous masqués en raison de la logique, la section entière est masquée sur le formulaire personnalisé. Cela se produit même si la logique d’affichage n’est pas appliquée au saut de section.</p><p>Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">Ajouter une logique d’affichage et de saut à l’aide du créateur de formulaire</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Faites glisser ou ajoutez au moins un champ personnalisé ou un widget à la nouvelle section. Cette opération est nécessaire pour enregistrer la section.

1. Cliquez sur **Terminé**.

   >[!TIP]
   >
   >Vous pouvez cliquer sur **Appliquer** à n’importe quel moment pendant que vous créez un formulaire personnalisé pour enregistrer vos modifications et garder le formulaire ouvert.

### Comment plusieurs types d’objets peuvent affecter les autorisations de saut de section {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

L’autorisation de modification limitée pour les sauts de section de formulaire personnalisés est disponible uniquement pour les types d’objets Projet, Tâche, Problème et Utilisateur ou Utilisatrice.

Dans un formulaire personnalisé avec un saut de section configuré et l’autorisation de modification limitée, si vous ajoutez l’un des autres types d’objets au formulaire (Portfolio, Programme, Document, Société, Enregistrement de facturation, Itération, Dépenses ou Groupe), Workfront vous demandera de passer à l’autorisation de modification, qui est compatible avec ce type d’objet et les types d’objets existants du formulaire.

>[!INFO]
>
>**Exemple :** dans un formulaire personnalisé associé au type d’objet Projet, un saut de section est configuré avec l’autorisation de modification limitée.
>
>Vous ajoutez le type d’objet Portfolio au formulaire, ce qui signifie que l’option d’autorisation de modification limitée n’est plus disponible pour le saut de section dans le formulaire.
>
>Un message à l’écran vous demande de passer à l’autorisation de modification, qui est le niveau d’autorisation le moins élevé compatible avec les types d’objet Projet et Portfolio.


## Positionner des champs personnalisés et des widgets dans un formulaire personnalisé


1. Commencez à créer ou à modifier un formulaire personnalisé, comme décrit dans la section [Concevoir un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Pour positionner un champ personnalisé et un widget sur la même ligne, faites glisser l’un à côté de l’autre jusqu’à ce qu’une ligne s’affiche entre eux.

   >[!NOTE]
   >
   >* Vous pouvez utiliser le bouton **Prévisualiser** dans le coin supérieur droit pour avoir un aperçu de la façon dont les champs personnalisés et les widgets s’affichent dans le formulaire.
   >* Les champs personnalisés et les widgets peuvent ne pas toujours s’afficher de la même manière dans le formulaire, selon l’espace disponible à l’écran lors de sa visualisation. Par exemple, le troisième champ d’une ligne de champs peut être renvoyé à la ligne suivante de champs si l’espace horizontal est limité.

1. (Facultatif) Pour positionner un champ personnalisé ou un widget au-dessus ou en dessous d’un autre, faites-le glisser au-dessus ou en dessous jusqu’à ce qu’une ligne bleue horizontale apparaisse entre les éléments.

1. Pour enregistrer vos modifications, cliquez sur **Appliquer**.

   ou

   Cliquez sur **Enregistrer et fermer**.

## Prévisualiser un formulaire personnalisé

1. Commencez à créer ou modifier un formulaire personnalisé et à ajouter des champs, comme décrit dans la section [Concevoir un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Cliquez sur **Prévisualiser** dans le coin supérieur droit pour avoir un aperçu du formulaire lors de son utilisation, puis cliquez sur **Fermer la prévisualisation** pour revenir à la modification du formulaire.

