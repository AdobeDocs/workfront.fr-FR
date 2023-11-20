---
title: Désactivation ou réactivation d’un formulaire personnalisé
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez réactiver ou désactiver un formulaire personnalisé. Nous vous recommandons de désactiver les formulaires personnalisés plutôt que de supprimer les formulaires que vous n’utilisez plus pour conserver les données historiques.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 3319fbfad98350635b7194a434f26e8528753e7b
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Désactivation ou réactivation d’un formulaire personnalisé

Vous pouvez réactiver ou désactiver un formulaire personnalisé. Nous vous recommandons de désactiver les formulaires personnalisés plutôt que de supprimer les formulaires que vous n’utilisez plus pour conserver les données historiques.

>[!NOTE]
>
>Si un formulaire personnalisé est désactivé mais fait toujours partie d’une rubrique de file d’attente ou d’une définition de file d’attente de requêtes, il sera joint à de nouvelles requêtes. Si vous ne souhaitez pas que le formulaire figure dans les requêtes, vous devez le supprimer manuellement de la file d’attente des requêtes.

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
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Pour plus d’informations sur la manière dont les administrateurs de Workfront accordent cet accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur Workfront.

## Désactivation d’un formulaire personnalisé

Vous pouvez désactiver les formulaires personnalisés que vous n’utilisez plus sans perdre les données historiques associées. Les utilisateurs ne peuvent pas ajouter un formulaire personnalisé inactif aux objets, mais ils peuvent tout de même afficher et ajouter des données à ses champs sur les objets auxquels il était déjà joint.

Les champs d’un formulaire personnalisé inactif sont également disponibles pour la modification en ligne dans une vue. Si un utilisateur ajoute un champ à partir d’un formulaire personnalisé inactif lors d’une modification en ligne, le formulaire se joint automatiquement à l’objet, même si le formulaire personnalisé est désactivé.

Pour désactiver un formulaire personnalisé :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).
1. Dans le panneau de gauche, choisissez **Forms personnalisée**.
1. Sur le **Forms** , sélectionnez le formulaire personnalisé à désactiver.
1. Dans la colonne Est actif, sélectionnez **False** et cliquez en dehors de la colonne . Le formulaire n’est plus actif.

## Réactivation d’un formulaire personnalisé

Si vous réactivez un formulaire personnalisé, il conserve les paramètres dont il disposait et les utilisateurs peuvent interagir avec celui-ci comme s’il n’avait jamais été désactivé.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).
1. Dans le panneau de gauche, choisissez **Forms personnalisée**.
1. Sur le **Forms** , sélectionnez le formulaire personnalisé à réactiver.
1. Dans la colonne Est actif, sélectionnez **True** et cliquez en dehors de la colonne . Le formulaire est maintenant actif.
