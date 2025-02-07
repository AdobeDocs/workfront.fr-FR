---
title: Ajouter ou supprimer des types d’objet d’un formulaire personnalisé existant
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez ajouter ou supprimer des types d’objet de formulaires personnalisés à l’aide du créateur de formulaire.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 94%

---

# Ajouter ou supprimer des types d’objet d’un formulaire personnalisé existant

Vous pouvez ajouter ou supprimer des types d’objet d’un formulaire personnalisé existant à l’aide du créateur de formulaire.

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
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td><p>Accès administratif aux formulaires personnalisés</p></td> 
  </tr>  
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter des types d’objet à un formulaire personnalisé existant

Vous pouvez ajouter d’autres types d’objet au formulaire pour les joindre à plusieurs objets.

>[!NOTE]
>
>Les autorisations de saut de section peuvent être affectées par le type d’objet. L’autorisation « Modification limitée » pour les sauts de section de formulaires personnalisés est disponible uniquement pour les types d’objets « Projet », « Tâche », « Problème » et « Utilisateur ou Utilisatrice ».
>
>Pour plus d’informations, consultez la section [Comment plusieurs types d’objets peuvent affecter les autorisations de sauts de section](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés** dans le panneau de gauche.

   Dans la vue qui s’affiche, vous pouvez passer en revue tous les formulaires personnalisés créés pour votre organisation. Vous pouvez également savoir la personne créatrice de chaque formulaire, le type d’objet avec lequel il fonctionne et s’il est actif.

1. Sélectionnez le formulaire personnalisé auquel vous souhaitez ajouter d’autres types d’objets, puis cliquez sur l’![icône Modifier](assets/edit-icon2.png).

1. En haut du formulaire, cliquez sur le signe + après **Types d’objets**, puis sélectionnez le type souhaité dans le menu qui s’affiche. Vous pouvez répéter cette opération pour ajouter autant de types d’objet que vous le souhaitez.

   ![Ajouter un nouvel objet](assets/add-new-object.png)

1. Cliquez sur **Enregistrer et fermer**.

   >[!TIP]
   >
   >À tout moment de la création d’un formulaire personnalisé, vous pouvez cliquer sur **Appliquer** pour enregistrer vos modifications et garder le formulaire ouvert.

## Supprimer des types d’objets sur un formulaire personnalisé

Vous pouvez supprimer des types d’objet d’un formulaire personnalisé existant. Un formulaire personnalisé doit comporter au moins un type d’objet.

>[!CAUTION]
>
>Si des personnes ont déjà joint le formulaire personnalisé à des objets du type que vous souhaitez supprimer et y ont ajouté des données, ces données sont définitivement supprimées lorsque vous supprimez ce type d’objet sur le formulaire. Il peut inclure des informations d’historique dont les utilisateurs et utilisatrices auront besoin ultérieurement.
>
>En règle générale, il est recommandé de réduire au minimum le nombre de fois où vous modifiez un formulaire personnalisé déjà utilisé. Il n’existe pas de système de notification pour alerter les personnes qui utilisent le formulaire personnalisé au sujet de vos modifications.

Pour supprimer un type d’objet :

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés** dans le panneau de gauche.
1. Sélectionnez le formulaire personnalisé que vous souhaitez modifier, puis cliquez sur l’![icône Modifier](assets/edit-icon2.png).
1. Cliquez sur X sur l’un des **Types d’objets** que vous souhaitez supprimer du formulaire.

   ![Supprimer des types d’objet](assets/delete-object-types.png)

1. (Facultatif) Répétez l’étape précédente pour tout autre type d’objet que vous souhaitez supprimer du formulaire.
1. Cliquez sur **Appliquer**, puis sur **Enregistrer et fermer**.
