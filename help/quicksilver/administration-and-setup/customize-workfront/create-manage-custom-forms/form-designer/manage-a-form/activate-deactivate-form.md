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
TQID: https://experienceleague.adobe.com/w4GbXu2z8f8kymWMp7mGn5qRm5gf5X0u9WAI2b5Lcdk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 346
ht-degree: 98%

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
   <td>Package Adobe Workfront</td> 
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
