---
title: Réinitialiser les préférences d’un utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez réinitialiser ou supprimer les paramètres des préférences d’un utilisateur ou d’une utilisatrice pour tout utilisateur ou toute utilisatrice du système Workfront. Les utilisateurs et utilisatrices individuels peuvent également réinitialiser leurs propres préférences.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: f1fe1a2fe6e123d8a039e8d7e3547c0b0a8141df
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 78%

---

# Réinitialiser les préférences d’un utilisateur ou d’une utilisatrice

<!-- Audited: 12/2023 -->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez réinitialiser ou supprimer les paramètres des préférences d’un utilisateur ou d’une utilisatrice pour tout utilisateur ou toute utilisatrice du système Workfront.

Les utilisateurs et utilisatrices individuels peuvent également réinitialiser leurs propres préférences.

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
   <td>Administrateur ou administratrice système</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## À propos des paramètres affectés

Lorsque vous réinitialisez les préférences d’un utilisateur ou d’une utilisatrice, certaines préférences sont ramenées à la valeur par défaut du système, tandis que d’autres sont effacées ou supprimées :

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

| Préférence | Statut après la réinitialisation |
| --- | --- |
| Vues | Revient à la valeur par défaut du système <p>Les vues existantes ne sont pas supprimées. Vous pouvez les sélectionner à nouveau.</p> |
| Filtres | Revient à la valeur par défaut du système <p>Les filtres existants ne sont pas supprimés. Vous pouvez les sélectionner à nouveau.</p> |
| Regroupements | Revient à la valeur par défaut du système <p>Les regroupements existants ne sont pas supprimés. Vous pouvez les sélectionner à nouveau.</p> |
| Liste d&#39;éléments récents | Effacée |
| Liste des favoris | Non affectée |
| Préférences de l’utilisateur ou de l’utilisatrice | Revient à la valeur par défaut du système <p>Les notifications par e-mail reviennent aux valeurs par défaut du système. Les notifications par défaut sont répertoriées dans [Notifications d’événements disponibles dans Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |

## Réinitialiser les préférences de l’utilisateur ou de l’utilisatrice

{{step-1-to-setup}}

1. Sélectionnez **Connexion en tant que**.
1. Commencez à saisir le nom de l’utilisateur ou de l’utilisatrice dont vous souhaitez réinitialiser les préférences, puis cliquez sur son nom lorsqu’il apparaît dans la liste déroulante.
1. Sélectionnez **Se connecter**.
1. Si votre organisation n’a pas été intégrée à l’expérience unifiée Adobe, procédez comme suit :

   * Dans le champ de l’URL en haut de votre navigateur web, ajoutez `/resetUser` après `workfront.com`.

     >[!NOTE]
     >
     >Ce champ est sensible à la casse. Le U doit être en majuscule et les autres caractères doivent être en minuscules. Par exemple :
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Si votre organisation a été intégrée à l’expérience unifiée Adobe, procédez comme suit :

   * Dans le champ URL situé en haut de votre navigateur web, ajoutez le `/resetUser` après la `workfront`.

     >[!NOTE]
     >
     >Ce champ est sensible à la casse. Le U doit être en majuscule et les autres caractères doivent être en minuscules. Par exemple :
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Appuyez sur **Entrée**.

1. Pour réinitialiser toutes les préférences utilisateur, cliquez sur **Réinitialiser**.

   Ou

   Pour réinitialiser le volet de navigation de gauche de l’utilisateur à la configuration du modèle de mise en page d’origine, cliquez sur **Réinitialiser le volet de navigation de gauche**.
