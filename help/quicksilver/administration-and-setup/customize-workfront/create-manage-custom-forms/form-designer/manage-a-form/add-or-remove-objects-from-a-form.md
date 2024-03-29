---
title: Ajouter ou supprimer des types d’objet d’un formulaire personnalisé existant avec le concepteur de formulaire
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez ajouter ou supprimer des types d’objet de formulaires personnalisés à l’aide du concepteur de formulaire.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# Ajouter ou supprimer des types d’objet d’un formulaire personnalisé existant avec le concepteur de formulaire

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients ou dans l’environnement Production pour les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, voir [Présentation de la version du deuxième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Vous pouvez ajouter ou supprimer des types d’objet d’un formulaire personnalisé existant à l’aide du concepteur de formulaire.

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
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td><p>Accès administratif aux formulaires personnalisés</p></td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Ajout de types d’objet à un formulaire personnalisé existant

Vous pouvez ajouter d’autres types d’objet au formulaire afin de les joindre à plusieurs objets.

>[!NOTE]
>
>Les autorisations de saut de section peuvent être affectées par le type d’objet . L’autorisation Modification limitée pour les sauts de section de formulaire personnalisés est disponible uniquement pour les types d’objets Projet, Tâche, Problème et Utilisateur .
>
>Pour plus d’informations, voir [Comment plusieurs types d’objets peuvent affecter les autorisations de sauts de section](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Cliquez sur **Forms personnalisée** dans le panneau de gauche.

   Dans la vue qui s’affiche, vous pouvez passer en revue tous les formulaires personnalisés créés pour votre organisation. Vous pouvez également savoir qui a créé chaque formulaire, avec quel type d’objet il fonctionne et s’il est actif.

1. Sélectionnez le formulaire personnalisé auquel vous souhaitez ajouter d’autres types d’objets, puis cliquez sur **Modifier** <span class="preview">ou ![Icône Modifier](assets/edit-icon.png).</span>

1. Dans la partie supérieure du formulaire, cliquez sur le signe + après **Types d’objet**, puis sélectionnez le type souhaité dans le menu qui s’affiche. Vous pouvez répéter cette opération pour ajouter autant de types d’objet que vous le souhaitez.

   ![](assets/add-new-object.png)

1. Cliquez sur **Enregistrer et fermer**.

   >[!TIP]
   >
   >Cliquez sur **Appliquer** lorsque vous créez un formulaire personnalisé pour enregistrer vos modifications et garder le formulaire ouvert.

## Suppression de types d’objet sur un formulaire personnalisé

Vous pouvez supprimer des types d’objet d’un formulaire personnalisé existant. Un formulaire personnalisé doit comporter au moins un type d’objet.

>[!CAUTION]
>
>Si des personnes ont déjà joint le formulaire personnalisé à des objets du type que vous souhaitez supprimer et y ont ajouté des données, ces données sont définitivement supprimées lorsque vous supprimez ce type d’objet sur le formulaire. Il peut inclure des informations historiques dont les utilisateurs auront besoin ultérieurement.
>
>En règle générale, il est recommandé de réduire au minimum le nombre de fois où vous modifiez un formulaire personnalisé déjà utilisé. Il n’existe pas de système de notification pour alerter les personnes qui utilisent le formulaire personnalisé au sujet de vos modifications.

Pour supprimer un type d’objet :

{{step-1-to-setup}}

1. Cliquez sur **Forms personnalisée** dans le panneau de gauche.
1. Sélectionnez le formulaire personnalisé à modifier, puis cliquez sur **Modifier** <span class="preview">ou ![Icône Modifier](assets/edit-icon.png).</span>
1. Cliquez sur le X dans l’une des **Types d’objet** que vous souhaitez supprimer du formulaire.

   ![](assets/delete-object-types.png)

1. (Facultatif) Répétez l’étape précédente pour tout autre type d’objet que vous souhaitez supprimer du formulaire.
1. Cliquez sur **Terminé**, puis cliquez sur **Enregistrer et fermer**.
