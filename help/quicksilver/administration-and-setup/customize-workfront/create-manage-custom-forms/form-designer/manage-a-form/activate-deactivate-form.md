---
title: Désactiver ou réactiver un formulaire personnalisé
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez réactiver ou désactiver un formulaire personnalisé. Nous vous recommandons de désactiver les formulaires personnalisés plutôt que de supprimer les formulaires que vous n’utilisez plus pour conserver les données historiques.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 35de4535970d5cd15fcd68f79bf849803f94a77e
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 17%

---

# Désactiver ou réactiver un formulaire personnalisé

Vous pouvez réactiver ou désactiver un formulaire personnalisé. Nous vous recommandons de désactiver les formulaires personnalisés plutôt que de supprimer les formulaires que vous n’utilisez plus pour conserver les données historiques.

>[!NOTE]
>
>Si un formulaire personnalisé est désactivé mais fait toujours partie d’une rubrique de file d’attente ou d’une définition de file d’attente de requêtes, il sera joint à de nouvelles requêtes. Si vous ne souhaitez pas que le formulaire figure dans les requêtes, vous devez le supprimer manuellement de la file d’attente des requêtes.

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
   <td> <p>Accès administratif aux formulaires personnalisés</p></td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Désactivation d’un formulaire personnalisé

Vous pouvez désactiver les formulaires personnalisés que vous n’utilisez plus sans perdre les données historiques associées. Les utilisateurs ne peuvent pas ajouter un formulaire personnalisé inactif aux objets, mais ils peuvent tout de même afficher et ajouter des données à ses champs sur les objets auxquels il était déjà joint.

Les champs d’un formulaire personnalisé inactif sont également disponibles pour la modification en ligne dans une vue. Si un utilisateur ajoute un champ à partir d’un formulaire personnalisé inactif lors d’une modification en ligne, le formulaire se joint automatiquement à l’objet, même si le formulaire personnalisé est désactivé.

Pour désactiver un formulaire personnalisé :

{{step-1-to-setup}}

1. Dans le panneau de gauche, sélectionnez **Forms personnalisé**.
1. Dans la zone **Forms**, sélectionnez le formulaire personnalisé à désactiver.
1. Dans la colonne Est actif, sélectionnez **False** et cliquez en dehors de la colonne. Le formulaire n’est plus actif.

## Réactivation d’un formulaire personnalisé

Si vous réactivez un formulaire personnalisé, il conserve les paramètres dont il disposait et les utilisateurs peuvent interagir avec celui-ci comme s’il n’avait jamais été désactivé.

{{step-1-to-setup}}

1. Dans le panneau de gauche, sélectionnez **Forms personnalisé**.
1. Dans la zone **Forms**, sélectionnez le formulaire personnalisé à réactiver.
1. Dans la colonne Est actif, sélectionnez **True** et cliquez en dehors de la colonne. Le formulaire est maintenant actif.
