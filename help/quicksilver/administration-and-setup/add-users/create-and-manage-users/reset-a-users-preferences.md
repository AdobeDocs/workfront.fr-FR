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
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 17%

---

# Réinitialiser les préférences d’un utilisateur ou d’une utilisatrice

<!-- Audited: 12/2023 -->

En tant qu’administrateur Adobe Workfront, vous pouvez réinitialiser ou supprimer les paramètres de préférences utilisateur pour n’importe quel utilisateur du système Workfront.

Les utilisateurs individuels peuvent également réinitialiser leurs propres paramètres de préférences utilisateur.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouvelle : standard</p>
       <p>ou</p>
       <p>Actuelle : formule</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## À propos des paramètres affectés

Lorsque vous réinitialisez les préférences utilisateur, certaines préférences sont rétablies par défaut du système, tandis que d’autres sont effacées ou supprimées :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
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
   <td> <p>Restauration de la valeur par défaut du système</p> <p>Les notifications par e-mail sont restaurées aux valeurs par défaut du système. Les notifications par défaut sont répertoriées dans les <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">notifications d’événement disponibles dans Adobe Workfront</a>.</p> </td> 
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

1. Sélectionnez **Se connecter en tant que**.
1. Commencez à saisir le nom de l’utilisateur dont vous souhaitez réinitialiser les préférences, puis cliquez sur le nom qui apparaît dans la liste déroulante.
1. Sélectionnez **Log In**.
1. Dans le champ URL situé en haut de votre navigateur web, ajoutez `/resetUser` après `workfront.com`.

   >[!NOTE]
   >
   >Ceci est sensible à la casse. L&#39;U doit être majuscule et les autres caractères doivent être en minuscules. Par exemple :
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. Appuyez sur **Entrée**.
1. Pour réinitialiser toutes les préférences utilisateur, sélectionnez **Réinitialiser**.

   Ou

   Pour réinitialiser uniquement les onglets personnalisés, sélectionnez **Réinitialiser les onglets**.
