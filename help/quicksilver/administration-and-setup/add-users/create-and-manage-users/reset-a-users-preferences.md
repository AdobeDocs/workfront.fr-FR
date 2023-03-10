---
title: Réinitialisation des préférences d’un utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur Adobe Workfront, vous pouvez réinitialiser ou supprimer les paramètres de préférences utilisateur pour n’importe quel utilisateur du système Workfront. Les utilisateurs individuels peuvent également réinitialiser leurs propres paramètres de préférences utilisateur.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 2%

---

# Réinitialisation des préférences d’un utilisateur

En tant qu’administrateur Adobe Workfront, vous pouvez réinitialiser ou supprimer les paramètres de préférences utilisateur pour n’importe quel utilisateur du système Workfront.

Les utilisateurs individuels peuvent également réinitialiser leurs propres paramètres de préférences utilisateur.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## À propos des paramètres affectés

Lorsque vous réinitialisez les préférences utilisateur, certaines préférences sont rétablies par défaut du système, tandis que d’autres sont effacées ou supprimées :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Préférence</strong> </th> 
   <th><strong>État après la réinitialisation</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Vues</td> 
   <td> <p> Restauration de la valeur par défaut du système</p> <p>Les vues existantes ne sont pas supprimées. Vous pouvez les sélectionner à nouveau.</p> </td> 
  </tr> 
  <tr> 
   <td>Filtres</td> 
   <td> <p>Restauration de la valeur par défaut du système</p> <p>Les filtres existants ne sont pas supprimés. Vous pouvez les sélectionner à nouveau.</p> </td> 
  </tr> 
  <tr> 
   <td>Regroupements</td> 
   <td> <p>Restauration de la valeur par défaut du système</p> <p>Les regroupements existants ne sont pas supprimés. Vous pouvez les sélectionner à nouveau.</p> </td> 
  </tr> 
  <tr> 
   <td>Liste des éléments récents</td> 
   <td>Effacé</td> 
  </tr> 
  <tr> 
   <td>Liste Favoris</td> 
   <td>Non affecté</td> 
  </tr> 
  <tr> 
   <td>Préférences utilisateur</td> 
   <td> <p>Restauration de la valeur par défaut du système</p> <p>Les notifications par e-mail sont rétablies par défaut sur le système</p> </td> 
  </tr> 
  <tr> 
   <td>Onglets personnalisés définis par l’utilisateur</td> 
   <td>Supprimé</td> 
  </tr> 
  <tr> 
   <td>Options de navigation globale définies par l’utilisateur</td> 
   <td>Redéfinissez la définition du modèle de mise en page ou la valeur par défaut du système si aucun modèle de mise en page n’est affecté.</td> 
  </tr> 
 </tbody> 
</table>

## Réinitialisation des préférences utilisateur

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Sélectionner **Connectez-vous en tant que**.
1. Commencez à saisir le nom de l’utilisateur dont vous souhaitez réinitialiser les préférences, puis cliquez sur le nom qui apparaît dans la liste déroulante.
1. Sélectionner  **Connexion**.
1. Dans le champ URL situé en haut de votre navigateur web, ajoutez `/resetUser` after `workfront.com`.

   >[!NOTE]
   >
   >Ceci est sensible à la casse. L&#39;U doit être majuscule et les autres caractères doivent être en minuscules. Par exemple :
   >
   >
   ```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. Press **Entrée**.
1. Pour réinitialiser toutes les préférences utilisateur, sélectionnez **Réinitialiser**.

   Ou

   Pour réinitialiser uniquement les onglets personnalisés, sélectionnez **Réinitialisation des onglets**.
