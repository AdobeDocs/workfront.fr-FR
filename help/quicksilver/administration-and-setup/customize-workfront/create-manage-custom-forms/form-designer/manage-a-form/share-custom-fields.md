---
title: Configuration du partage pour les champs et widgets personnalisés
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Par défaut, lorsque vous ajoutez un nouveau champ personnalisé ou widget à un formulaire personnalisé, toute personne dans le système ayant accès aux formulaires personnalisés peut modifier les propriétés de cet élément, telles que son libellé et son nom. Vous pouvez modifier ce paramètre en contrôlant avec qui l’information peut être partagée.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
source-git-commit: c1bc2832d1c52885e737056172e7aec93a951e6c
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 71%

---

# Configuration du partage pour les champs et widgets personnalisés

Par défaut, lorsque vous ajoutez un nouveau champ personnalisé ou widget à un formulaire personnalisé, toute personne dans le système ayant accès aux formulaires personnalisés peut modifier les propriétés de cet élément, telles que son libellé et son nom. Vous pouvez modifier ce paramètre en contrôlant avec qui l’information peut être partagée.

Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Concevoir un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuration du partage d’un champ ou d’un widget personnalisé à partir de la liste des formulaires

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Cliquez sur **Champs** pour ouvrir la zone Champs.
1. Sélectionnez l’élément pour lequel configurer le partage, puis cliquez sur l’![icône Partager](assets/share-icon.png).
1. Dans la zone Accès aux champs personnalisés qui s’affiche, indiquez avec qui partager l’élément et comment le partager :

   1. Dans le coin inférieur gauche de la zone **Accès au champ personnalisé**, dans **Accorder l’accès au champ personnalisé à**, commenceZ à saisir le nom d’un utilisateur, d’une utilisatrice, d’une équipe, d’une fonction, d’un groupe ou d’une entreprise avec lequel vous souhaitez partager l’élément, puis cliquez sur son nom lorsque celui-ci apparaît.

      ![Zone d’accès aux champs personnalisés](assets/share-field-give-access-to.jpg)

   1. Si vous souhaitez préciser la façon dont vous voulez partager l’élément, cliquez sur la liste déroulante à droite du nom, puis utilisez l’une des options suivantes :

      ![Options de partage](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">L'afficher</td> 
         <td> <p>Vous pouvez cliquer sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que les utilisateurs et les utilisatrices puissent utiliser leur accès pour ajouter l’élément à un formulaire personnalisé ou le partager avec d’autres utilisateurs et utilisatrices.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Le gérer</td> 
         <td> <p>Accorde l’accès permettant de modifier le champ personnalisé et de l’afficher dans la bibliothèque de champs ainsi que sur la page sur laquelle vous créez des formulaires personnalisés.</p> <p>Vous pouvez cliquer sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que les utilisateurs et les utilisatrices puissent utiliser leur accès pour supprimer l’élément du système ou pour le partager avec d’autres utilisateurs et utilisatrices.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Cliquez sur l’icône d’engrenage ![Icône Paramètres](assets/gear-icon-settings.png) dans le coin supérieur droit si vous souhaitez choisir une option de partage à l’échelle du système pour le champ.

   Toutes les options ci-après ne s’affichent pas en même temps dans ce menu déroulant. Par exemple, la seconde option ne s’affiche que si l’une des deux autres est sélectionnée.

   * **Rendre cet élément modifiable sur l’ensemble du système, de sorte que tous les utilisateurs et utilisatrices Workfront puissent le modifier** (option par défaut).

     Lorsque vous ajoutez un champ personnalisé ou un widget et que vous n’en limitez pas le partage, tous les utilisateurs et utilisatrices du système qui ont accès aux formulaires personnalisés peuvent le voir et modifier ses propriétés.

   * **Supprimer l’accès à distance sur tout le système**

     Limite l’accès aux seules personnes que vous avez ajoutées à la liste.

   * **Rendre cet élément visible sur l’ensemble du système de sorte que tous les utilisateurs et utilisatrices Workfront puissent le voir**.

1. Cliquer sur **Enregistrer**.

## Configuration du partage d’un champ ou d’un widget personnalisé à partir du concepteur de formulaires

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Ouvrez un formulaire personnalisé ou créez un formulaire personnalisé.
1. Dans le concepteur de formulaires, sélectionnez l’élément pour lequel vous souhaitez configurer le partage, puis cliquez sur **Partager** dans la zone d’édition du champ à droite.
1. Dans la zone qui s’affiche, sous **Accorder l’accès au formulaire personnalisé à**, commencez à saisir le nom de l’utilisateur, de l’équipe, du rôle de tâche, du groupe ou de la société avec lequel vous souhaitez partager l’élément, puis appuyez sur **Entrée** lorsque le nom s’affiche.
1. Si vous souhaitez être plus précis sur la manière dont vous partagez l’élément, cliquez sur le menu déroulant à droite du nom, puis utilisez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">L'afficher</td> 
        <td> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que les utilisateurs puissent ajouter l’élément à un formulaire personnalisé ou le partager avec d’autres utilisateurs.</p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Le gérer</td> 
        <td> <p>Permet d’accéder à la modification du champ personnalisé et de l’afficher dans la bibliothèque de champs et dans le concepteur de formulaires.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que les utilisateurs puissent supprimer l’élément du système ou le partager avec d’autres utilisateurs.</p> </td> 
       </tr> 
     </tbody> 
    </table>

1. (Facultatif) Répétez les étapes 5 et 6 pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Choisissez une option de partage à l’échelle du système pour le champ :

   * **Tout le monde dans le système peut modifier** (option par défaut)

     Lorsque vous ajoutez un champ personnalisé ou un widget et que vous n’en limitez pas le partage, tous les utilisateurs et utilisatrices du système qui ont accès aux formulaires personnalisés peuvent le voir et modifier ses propriétés.

   * **Tout le monde dans le système peut afficher**
   * **Seules les personnes invitées peuvent accéder à**

     Limite l’accès à ceux que vous avez ajoutés à la liste.

   ![Options de partage](assets/share-field-in-designer.png)

1. Cliquer sur **Enregistrer**.

## Accès hérité aux champs personnalisés et aux widgets lorsqu’un formulaire personnalisé est partagé.

Lorsqu’une personne partage un formulaire personnalisé avec un groupe, une fonction, une équipe ou une entreprise, les personnes destinataires héritent de l’accès Afficher à tous les champs personnalisés et à tous les widgets qui se trouvent dans le formulaire. Ce niveau d’accès à ces éléments du formulaire est toujours conservé afin que le formulaire puisse fonctionner pour les personnes destinataires comme prévu par la personne qui l’a créé. Ceci est également valable pour les personnes destinataires qui disposent d’un accès Modifier au formulaire.

Vous pouvez savoir qui dispose d’un accès hérité à un champ personnalisé ou à un widget et vous pouvez supprimer cet accès.

>[!NOTE]
>
>Si une personne destinataire dispose d’un accès en gestion à un champ personnalisé ou à un widget sur le formulaire personnalisé partagé, cet accès est conservé pour la personne destinataire.

### Connaître les personnes disposant d’un accès hérité à un champ personnalisé ou à un widget {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Cliquez sur **Champs**, puis sélectionnez le champ, l’image ou le widget d’accès.
1. Dans la zone qui s’affiche, cliquez sur **Anciennes autorisations** et consultez les noms qui s’affichent.
1. Cliquez sur **Annuler**.

### Supprimer l’accès à un champ personnalisé ou à un widget dans un formulaire personnalisé qui a été partagé. {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Si vous devez supprimer l’accès à un champ personnalisé ou à un widget dans un formulaire personnalisé qui a été partagé, vous devez annuler le partage du formulaire. Pour plus d’informations, reportez-vous à la section [Suppression de l’accès à un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form-from-the-list-of-forms) de l’article [Partager un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
