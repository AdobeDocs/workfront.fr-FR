---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Configurer le partage de champs et de widgets personnalisés avec le créateur de formulaire hérité
description: Par défaut, lorsque vous ajoutez un nouveau champ ou widget personnalisé à un formulaire personnalisé, toute personne du système ayant accès à des formulaires personnalisés peut modifier les propriétés de cet élément, telles que son libellé et son nom. Vous pouvez modifier ce paramètre en contrôlant avec qui il peut être partagé.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 100%

---

# Configurer le partage de champs et de widgets personnalisés avec le créateur de formulaire hérité

{{form-designer-default}}

Par défaut, lorsque vous ajoutez un nouveau champ ou widget personnalisé à un formulaire personnalisé, toute personne du système ayant accès à des formulaires personnalisés peut modifier les propriétés de cet élément, telles que son libellé et son nom. Vous pouvez modifier ce paramètre en contrôlant avec qui il peut être partagé.

Pour plus d’informations sur les champs et les widgets personnalisés dans les formulaires personnalisés, voir [Ajouter un champ personnalisé à un formulaire personnalisé à l’aide du créateur de formulaires hérité](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) et [Ajouter ou modifier un widget de ressource dans un formulaire personnalisé à l’aide du créateur de formulaire hérité](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Conditions d’accès

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

## Configurer le partage pour un champ ou un widget personnalisé

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Si vous configurez le partage d’un champ ou d’un widget personnalisé dans l’instance Workfront de votre organisation, procédez comme suit :

   1. Cliquez sur **Champs** pour ouvrir la zone Champs.
   1. Sélectionnez l’élément pour lequel configurer le partage, puis cliquez sur l’![icône Partager](assets/share-icon.png).

   Ou, si vous configurez le partage d’un champ ou d’un widget personnalisé dans un formulaire personnalisé existant, procédez comme suit :

   1. Sélectionnez le formulaire personnalisé, puis cliquez sur l’![icône Modifier](assets/edit-icon.png).
   1. Dans la zone d’édition du formulaire à droite, sélectionnez l’élément pour lequel configurer le partage.
   1. Dans le panneau de gauche, cliquez sur le champ **Partager**.

1. Dans la zone **Accès aux champs personnalisés** qui s’affiche, indiquez avec qui partager l’élément et comment le partager :

   1. Près du coin inférieur gauche de la zone **Accès aux champs personnalisés** sous **Autoriser l’accès aux champs personnalisés à**, commencez à saisir le nom d’une personne, d’une équipe, d’une fonction, d’un groupe ou d’une entreprise avec qui partager l’élément, puis cliquez dessus lorsqu’il apparaît.

      ![](assets/share-field-give-access-to.jpg)

   1. Pour plus de précision sur la manière dont partager l’élément, cliquez sur la liste déroulante à droite du nom, puis utilisez l’une des options suivantes :

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">L'afficher</td> 
         <td> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que la ou les personnes puissent utiliser leur accès pour ajouter l’élément à un formulaire personnalisé ou le partager avec d’autres personnes.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Le gérer</td> 
         <td> <p>Permet de modifier le champ personnalisé, puis de l’afficher dans la bibliothèque de champs et sur la page sur laquelle vous créez des formulaires personnalisés.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que la ou le personnes puissent utiliser leur accès pour supprimer l’élément du système ou le partager avec d’autres personnes.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) dans le coin supérieur droit pour choisir une option de partage à l’échelle du système pour le champ.

   Toutes les options suivantes ne s’affichent pas simultanément dans ce menu déroulant. Par exemple, la seconde s’affiche uniquement lorsque l’une des deux autres est sélectionnée.

   * **Rendre cette option modifiable à l’échelle du système afin que l’ensemble des utilisateurs et utilisatrices de Workfront puissent la modifier** (option par défaut)

     Lorsque vous ajoutez un champ ou un widget personnalisé et que vous ne limitez pas le partage, l’ensemble des utilisateurs et utilisatrices du système ayant accès à des formulaires personnalisés peuvent le consulter et modifier ses propriétés.

   * **Supprimer l’accès à la modification sur tout le système**

     Limite l’accès aux personnes vous avez ajoutées à la liste.

   * **Rendre cette option visible à l’échelle du système de sorte que l’ensemble des utilisateurs et utilisatrices de Workfront puissent la voir**

1. Cliquez sur **Enregistrer** ou **Enregistrer + Fermer**.

## Accès hérité aux champs et widgets personnalisés lorsqu’un formulaire personnalisé est partagé

Lorsqu’une personne partage un formulaire personnalisé avec un groupe, une fonction, une équipe ou une entreprise, les destinataires héritent de l’option Afficher l’accès à tous les champs et widgets personnalisés du formulaire. Ce niveau d’accès à ces éléments du formulaire est toujours conservé, afin que le formulaire puisse fonctionner pour les destinataires comme l’a prévu la personne qui l’a créé. C’est le cas même pour les destinataires disposant de l’accès en modification pour le formulaire.

Vous pouvez déterminer qui bénéficie d’un accès hérité à un champ ou à un widget personnalisé et supprimer cet accès.

>[!NOTE]
>
>Si un destinataire dispose de l’option Gérer l’accès à un champ ou à un widget personnalisé sur le formulaire personnalisé partagé, cet accès est conservé pour le destinataire.

* [Découvrez qui bénéficie d’un accès hérité à un champ ou à un widget personnalisé.](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Supprimer l’accès à un champ ou à un widget personnalisé dans un formulaire personnalisé qui a été partagé](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Découvrez qui bénéficie d’un accès hérité à un champ ou à un widget personnalisé. {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Cliquez sur **Champs**, puis sélectionnez le champ, l’image ou le widget d’accès.
1. Dans la zone qui s’affiche, cliquez sur **Anciennes autorisations** et consultez les noms qui s’affichent.
1. Cliquez sur **Annuler**.

### Supprimer l’accès à un champ ou à un widget personnalisé dans un formulaire personnalisé qui a été partagé {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Si vous devez supprimer l’accès à un champ ou à un widget personnalisé dans un formulaire personnalisé qui a été partagé, vous devez annuler le partage du formulaire. Pour obtenir des instructions, voir dans la section [Supprimer l’accès à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) dans l’article [Partager un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
