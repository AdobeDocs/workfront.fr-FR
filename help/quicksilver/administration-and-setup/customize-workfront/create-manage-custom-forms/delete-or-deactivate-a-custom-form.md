---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Suppression ou désactivation d’un formulaire personnalisé
description: Vous pouvez supprimer ou désactiver un formulaire personnalisé du système.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d97badf-b6d0-4e7c-bff8-9ff63e83586b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Suppression ou désactivation d’un formulaire personnalisé

Vous pouvez supprimer ou désactiver un formulaire personnalisé du système.

>[!CAUTION]
>
>La suppression d’un formulaire personnalisé supprime également toutes les données personnalisées sur les objets associés au formulaire. Les données supprimées ne peuvent pas être récupérées. Envisagez plutôt de désactiver un formulaire personnalisé : lorsque vous désactivez un formulaire personnalisé que vous n’utilisez plus, vous conservez toutes les données historiques associées.

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
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Pour plus d’informations sur la manière dont les administrateurs de Workfront accordent cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur Workfront.

## Suppression d’un formulaire personnalisé

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Forms personnalisée.**
1. Sélectionnez le formulaire personnalisé, puis cliquez sur **Supprimer**.
1. Si vous souhaitez supprimer définitivement le formulaire personnalisé et toutes les données associées sur les objets auxquels il a été joint, cliquez sur **Oui, la supprimer**.

## Désactivation d’un formulaire personnalisé

Vous pouvez désactiver les formulaires personnalisés que vous n’utilisez plus sans perdre les données historiques associées. Les utilisateurs ne peuvent pas ajouter un formulaire personnalisé inactif aux objets, mais ils peuvent tout de même afficher et ajouter des données à ses champs sur les objets auxquels il était déjà joint.

Les champs d’un formulaire personnalisé inactif sont également disponibles pour la modification en ligne dans une vue. Si un utilisateur ajoute un champ à partir d’un formulaire personnalisé inactif lors d’une modification en ligne, le formulaire se joint automatiquement à l’objet, même si le formulaire personnalisé est désactivé.

Si vous réactivez un formulaire personnalisé, il conserve les paramètres dont il disposait auparavant et les utilisateurs peuvent interagir avec celui-ci comme s’il n’avait jamais été désactivé.

Pour désactiver un formulaire personnalisé :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur le nom du formulaire personnalisé à désactiver.
1. Cliquez sur le bouton **Paramètres de formulaire** .
1. Désactivez le **Est Principal** .
1. Cliquez sur **Enregistrer + Fermer**.
