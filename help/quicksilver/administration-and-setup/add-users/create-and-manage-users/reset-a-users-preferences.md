---
title: Réinitialisation des préférences d’un utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez réinitialiser ou supprimer les paramètres des préférences d’un utilisateur ou d’une utilisatrice pour tout utilisateur ou toute utilisatrice du système Workfront. Les utilisateurs et utilisatrices individuels peuvent également réinitialiser leurs propres préférences.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 88%

---

# Réinitialiser les préférences d’un utilisateur ou d’une utilisatrice

<!-- Audited: 12/2023 -->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez réinitialiser ou supprimer les paramètres des préférences d’un utilisateur ou d’une utilisatrice pour tout utilisateur ou toute utilisatrice du système Workfront.

Les utilisateurs et utilisatrices individuels peuvent également réinitialiser leurs propres préférences.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## À propos des paramètres affectés

Lorsque vous réinitialisez les préférences d’un utilisateur ou d’une utilisatrice, certaines préférences sont ramenées à la valeur par défaut du système, tandis que d’autres sont effacées ou supprimées :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Préférence</strong> </th> 
   <th><strong>Statut après la réinitialisation</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Vues</td> 
   <td> <p> Revient à la valeur par défaut du système</p> <p>Les vues existantes ne sont pas supprimées. Vous pouvez les sélectionner à nouveau.</p> </td> 
  </tr> 
  <tr> 
   <td>Filtres</td> 
   <td> <p>Revient à la valeur par défaut du système</p> <p>Les filtres existants ne sont pas supprimés. Vous pouvez les sélectionner à nouveau.</p> </td> 
  </tr> 
  <tr> 
   <td>Regroupements</td> 
   <td> <p>Revient à la valeur par défaut du système</p> <p>Les regroupements existants ne sont pas supprimés. Vous pouvez les sélectionner à nouveau.</p> </td> 
  </tr> 
  <tr> 
   <td>Liste des éléments récents</td> 
   <td>Effacée</td> 
  </tr> 
  <tr> 
   <td>Liste des favoris</td> 
   <td>Non affectée</td> 
  </tr> 
  <tr> 
   <td>Préférences de l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Revient à la valeur par défaut du système</p> <p>Les notifications par e-mail reviennent aux valeurs par défaut du système. Les notifications par défaut sont répertoriées dans <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Notifications d’événements disponibles dans Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Onglets personnalisés définis par l’utilisateur ou l’utilisatrice</td> 
   <td>Supprimés</td> 
  </tr> 
  <tr> 
   <td>Options de navigation globale définies par l’utilisateur ou l’utilisatrice</td> 
   <td>Reviennent à la définition du modèle de disposition ou à la valeur par défaut du système si aucun modèle de disposition n’est attribué.</td> 
  </tr> 
 </tbody> 
</table>

## Réinitialiser les préférences de l’utilisateur ou de l’utilisatrice

{{step-1-to-setup}}

1. Sélectionnez **Connexion en tant que**.
1. Commencez à saisir le nom de l’utilisateur ou de l’utilisatrice dont vous souhaitez réinitialiser les préférences, puis cliquez sur son nom lorsqu’il apparaît dans la liste déroulante.
1. Sélectionnez **Se connecter**.
1. Si votre entreprise n’a pas été intégrée à l’expérience unifiée Adobe, procédez comme suit :

   * Dans le champ de l’URL en haut de votre navigateur web, ajoutez `/resetUser` après `workfront.com`.

     >[!NOTE]
     >
     >Ce champ est sensible à la casse. Le U doit être en majuscule et les autres caractères doivent être en minuscules. Par exemple :
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Si votre entreprise a été intégrée à l’expérience unifiée Adobe, procédez comme suit :

   * Dans le champ URL situé en haut de votre navigateur web, ajoutez `/resetUser` après `workfront`.

     >[!NOTE]
     >
     >Ce champ est sensible à la casse. Le U doit être en majuscule et les autres caractères doivent être en minuscules. Par exemple :
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Appuyez sur **Entrée**.
1. Pour réinitialiser toutes les préférences de l’utilisateur ou de l’utilisatrice, sélectionnez **Réinitialiser**.

   Ou

   Pour réinitialiser uniquement les onglets personnalisés, sélectionnez **Réinitialiser les onglets**.
