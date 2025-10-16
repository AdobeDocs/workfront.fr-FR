---
title: Désactivation ou réactivation d’un formulaire personnalisé
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez réactiver ou désactiver un formulaire personnalisé. Nous vous recommandons de désactiver les formulaires personnalisés plutôt que de supprimer les formulaires que vous n’utilisez plus pour conserver les données historiques.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 97%

---

# Désactiver ou réactiver un formulaire personnalisé

Vous pouvez réactiver ou désactiver un formulaire personnalisé. Nous vous recommandons de désactiver les formulaires personnalisés plutôt que de supprimer les formulaires que vous n’utilisez plus pour conserver les données historiques.

>[!NOTE]
>
>Si un formulaire personnalisé est désactivé mais fait toujours partie d’une rubrique de file d’attente ou d’une définition de file d’attente des demandes, il sera joint à de nouvelles demandes. Si vous ne souhaitez pas que le formulaire figure dans les demandes, vous devez le supprimer manuellement de la file d’attente des demandes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Désactiver un formulaire personnalisé

Vous pouvez désactiver les formulaires personnalisés que vous n’utilisez plus sans perdre les données historiques associées. Les personnes ne peuvent pas ajouter un formulaire personnalisé inactif aux objets, mais elles peuvent tout de même afficher et ajouter des données à ses champs sur les objets auxquels il était déjà joint.

Les champs d’un formulaire personnalisé inactif sont également disponibles pour la modification en ligne dans une vue. Si une personne ajoute un champ à partir d’un formulaire personnalisé inactif lors d’une modification en ligne, le formulaire se joint automatiquement à l’objet, même si le formulaire personnalisé est désactivé.

Pour désactiver un formulaire personnalisé :

{{step-1-to-setup}}

1. Dans le panneau de gauche, choisissez **Formulaires personnalisés**.
1. Dans la zone **Formulaires**, sélectionnez le formulaire personnalisé à désactiver.
1. Dans la colonne Est actif, sélectionnez **False** et cliquez en dehors de la colonne. Le formulaire n’est plus actif.

## Réactiver un formulaire personnalisé

Si vous réactivez un formulaire personnalisé, il conserve les paramètres dont il disposait et les personnes peuvent interagir avec celui-ci comme s’il n’avait jamais été désactivé.

{{step-1-to-setup}}

1. Dans le panneau de gauche, choisissez **Formulaires personnalisés**.
1. Dans la zone **Formulaires**, sélectionnez le formulaire personnalisé à réactiver.
1. Dans la colonne Est actif, sélectionnez **True** et cliquez en dehors de la colonne. Le formulaire est maintenant actif.
