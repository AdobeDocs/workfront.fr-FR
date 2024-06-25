---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Supprimer des types d’objets sur un formulaire personnalisé
description: Sur un formulaire personnalisé existant, vous pouvez supprimer les types d’objets associés au formulaire. Après cela, les utilisateurs et les utilisatrices ne peuvent plus joindre le formulaire à des objets de ce type.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 100%

---

# Supprimer des types d’objets sur un formulaire personnalisé

{{form-designer-default}}

Sur un formulaire personnalisé existant, vous pouvez supprimer les types d’objets associés au formulaire. Après cela, les utilisateurs et les utilisatrices ne peuvent plus joindre le formulaire à des objets de ce type.

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

## Supprimer des types d’objets sur un formulaire personnalisé

Vous pouvez supprimer des types d’objets d’un formulaire personnalisé existant.

Un formulaire personnalisé doit comporter au moins un type d’objet.

>[!CAUTION]
>
>Si des personnes ont déjà joint le formulaire personnalisé à des objets du type que vous souhaitez supprimer et y ont ajouté des données, ces données sont définitivement supprimées lorsque vous supprimez ce type d’objet sur le formulaire. Cela peut inclure des informations historiques dont les utilisateurs et les utilisatrices auront besoin ultérieurement.
>
>En règle générale, il est recommandé de réduire au minimum le nombre de fois où vous modifiez un formulaire personnalisé déjà utilisé. Il n’existe pas de système de notification pour informer les personnes qui utilisent le formulaire personnalisé de vos modifications.

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés** dans le panneau de gauche.
1. Sélectionnez le formulaire personnalisé que vous souhaitez modifier, puis cliquez sur l’![icône Modifier](assets/edit-icon.png).
1. Cliquez sur X sur l’un des **Types d’objets** que vous souhaitez supprimer du formulaire, puis sur **Supprimer** dans le message d’avertissement qui s’affiche.

   ![](assets/click-x-object-types.jpg)

1. (Facultatif) Répétez l’étape précédente pour tout autre type d’objet que vous souhaitez supprimer du formulaire.
1. Cliquez sur **Terminé**, puis sur **Enregistrer et fermer**.
