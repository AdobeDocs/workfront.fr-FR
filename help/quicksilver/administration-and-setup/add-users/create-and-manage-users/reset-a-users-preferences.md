---
title: Réinitialisation des préférences d’un utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur Adobe Workfront, vous pouvez réinitialiser ou supprimer les paramètres de préférences utilisateur pour n’importe quel utilisateur du système Workfront. Les utilisateurs individuels peuvent également réinitialiser leurs propres paramètres de préférences utilisateur.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: c3cb97a36c29b90bbc9d8438d8811cc23266d894
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 2%

---

# Réinitialisation des préférences d’un utilisateur

<!-- Audited: 12/2023 -->

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
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Restauration de la valeur par défaut du système</p> <p>Les notifications par e-mail sont restaurées aux valeurs par défaut du système. Les notifications par défaut sont répertoriées dans la section <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Notifications d’événements disponibles dans Adobe Workfront</a>.</p> </td> 
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

{{step-1-to-setup}}

1. Sélectionner **Connexion en tant que**.
1. Commencez à saisir le nom de l’utilisateur dont vous souhaitez réinitialiser les préférences, puis cliquez sur le nom qui apparaît dans la liste déroulante.
1. Sélectionner  **Connexion**.
1. Dans le champ URL situé en haut de votre navigateur web, ajoutez `/resetUser` after `workfront.com`.

   >[!NOTE]
   >
   >Ceci est sensible à la casse. L&#39;U doit être majuscule et les autres caractères doivent être en minuscules. Par exemple :
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. Presse **Entrée**.
1. Pour réinitialiser toutes les préférences utilisateur, sélectionnez **Réinitialiser**.

   Ou

   Pour réinitialiser uniquement les onglets personnalisés, sélectionnez **Réinitialisation des onglets**.
