---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Configuration du partage de champs et de widgets personnalisés avec le créateur de formulaires hérité
description: Par défaut, lorsque vous ajoutez un nouveau champ ou widget personnalisé à un formulaire personnalisé, toute personne du système ayant accès à des formulaires personnalisés peut modifier les propriétés de cet élément, telles que son libellé et son nom. Vous pouvez modifier ce paramètre en contrôlant avec qui il peut être partagé.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 0%

---

# Configuration du partage de champs et de widgets personnalisés avec le créateur de formulaires hérité

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients ou dans l’environnement Production pour les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, voir [Présentation de la version du deuxième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Par défaut, lorsque vous ajoutez un nouveau champ ou widget personnalisé à un formulaire personnalisé, toute personne du système ayant accès à des formulaires personnalisés peut modifier les propriétés de cet élément, telles que son libellé et son nom. Vous pouvez modifier ce paramètre en contrôlant avec qui il peut être partagé.

Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Ajout d’un champ personnalisé à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) et [Ajout ou modification d’un widget de ressource dans un formulaire personnalisé à l’aide de l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Configuration du partage pour un champ ou un widget personnalisé

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Forms personnalisée**.
1. Si vous configurez le partage d’un champ ou d’un widget personnalisé dans l’instance Workfront de votre entreprise, procédez comme suit :

   1. Cliquez sur **Champs** pour ouvrir la zone Champs .
   1. Sélectionnez l’élément pour lequel vous souhaitez configurer le partage, puis cliquez sur **Partager** <span class="preview">ou ![Icône Partager](assets/share-icon.png).</span>

   Ou, si vous configurez le partage d’un champ ou d’un widget personnalisé dans un formulaire personnalisé existant, procédez comme suit :

   1. Sélectionnez le formulaire personnalisé, puis cliquez sur **Modifier** <span class="preview">ou ![Icône Modifier](assets/edit-icon.png).</span>
   1. Dans la zone d’édition du formulaire à droite, sélectionnez l’élément pour lequel vous souhaitez configurer le partage.
   1. Dans le panneau de gauche, cliquez sur **Partager le champ**.

1. Dans le **Accès aux champs personnalisés** qui s’affiche, indiquez avec qui partager l’élément et comment le partager :

   1. Près du coin inférieur gauche du **Accès aux champs personnalisés** sous **Autoriser l’accès aux champs personnalisés**, commencez à saisir le nom d’un utilisateur, d’une équipe, d’un rôle de tâche, d’un groupe ou d’une société avec lequel vous souhaitez partager l’élément, puis cliquez sur le nom lorsqu’il apparaît.

      ![](assets/share-field-give-access-to.jpg)

   1. Si vous souhaitez être plus précis sur la manière dont vous souhaitez partager l’élément, cliquez sur la liste déroulante à droite du nom, puis utilisez l’une des options suivantes :

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">L'afficher</td> 
         <td> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que l’utilisateur ou les utilisateurs puissent utiliser leur accès pour ajouter l’élément à un formulaire personnalisé ou le partager avec d’autres utilisateurs.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Le gérer</td> 
         <td> <p>Permet d’accéder à la modification du champ personnalisé et de l’afficher dans la bibliothèque de champs et sur la page sur laquelle vous créez des formulaires personnalisés.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que l’utilisateur ou les utilisateurs puissent utiliser leur accès pour supprimer l’élément du système ou le partager avec d’autres utilisateurs.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) dans le coin supérieur droit si vous souhaitez choisir une option de partage à l’échelle du système pour le champ .

   Toutes les options suivantes ne s’affichent pas simultanément dans ce menu déroulant. Par exemple, la seconde s’affiche uniquement lorsque l’une des deux autres est sélectionnée.

   * **Rendre cette modification possible à l’échelle du système afin que tous les utilisateurs de Workfront puissent la modifier.** (option par défaut)

     Lorsque vous ajoutez un champ ou un widget personnalisé et que vous ne limitez pas le partage, tous les utilisateurs du système ayant accès à des formulaires personnalisés peuvent le consulter et modifier ses propriétés.

   * **Suppression de l’accès de modification à l’échelle du système**

     Limite l’accès à ceux que vous avez ajoutés à la liste.

   * **rendre visible à l’échelle du système afin que tous les utilisateurs de Workfront puissent le voir ;**

1. Cliquez sur **Enregistrer** ou **Enregistrer + Fermer**.

## Accès hérité aux champs et widgets personnalisés lorsqu’un formulaire personnalisé est partagé

Lorsqu’une personne partage un formulaire personnalisé avec un groupe, un rôle de tâche, une équipe ou une entreprise, les destinataires héritent de l’option Afficher l’accès à tous les champs et widgets personnalisés du formulaire. Ce niveau d’accès à ces éléments du formulaire est toujours conservé afin que le formulaire puisse fonctionner pour les destinataires comme l’a prévu la personne qui l’a créé. C’est le cas même pour les destinataires disposant de l’accès Modifier au formulaire.

Vous pouvez déterminer qui a hérité de l’accès à un champ ou à un widget personnalisé et vous pouvez en supprimer l’accès.

>[!NOTE]
>
>Si un destinataire dispose de l’option Gérer l’accès à un champ ou à un widget personnalisé sur le formulaire personnalisé partagé, cet accès est conservé pour le destinataire.

* [Découvrez qui a hérité de l’accès à un champ ou à un widget personnalisé](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Supprimer l’accès à un champ ou à un widget personnalisé dans un formulaire personnalisé qui a été partagé](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Découvrez qui a hérité de l’accès à un champ ou à un widget personnalisé {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Forms personnalisée**.
1. Cliquez sur le bouton **Champs** , puis sélectionnez le champ, l’image ou le widget d’accès.
1. Dans la zone qui s’affiche, cliquez sur **Autorisations héritées** et afficher les noms qui s’affichent.
1. Cliquez sur **Annuler**.

### Supprimer l’accès à un champ ou à un widget personnalisé dans un formulaire personnalisé qui a été partagé {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Si vous devez supprimer l’accès à un champ ou à un widget personnalisé dans un formulaire personnalisé qui a été partagé, vous devez annuler le partage du formulaire. Pour obtenir des instructions, voir dans la section [Supprimer l’accès à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) dans l’article [Partage d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
