---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurer des politiques de mot de passe pour l’authentification
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer les options de politiques de mot de passe pour personnaliser l’expérience d’authentification de votre système Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 99%

---

# Configurer des politiques de mot de passe pour l’authentification

{{important-admin-console-onboard}}

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer les options de politiques de mot de passe pour personnaliser l’expérience d’authentification de votre système Workfront.

Nous vous recommandons de configurer les préférences d’authentification lors de l’implémentation de Workfront et de ne les modifier qu’occasionnellement par la suite.

Les améliorations des fonctionnalités de gestion des mots de passe seront bientôt disponibles ou le sont déjà pour votre entreprise. Utilisez l’une des sections suivantes, selon que votre entreprise a accès ou non à la nouvelle expérience d’authentification.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer l’authentification (disponible pour toute la clientèle) {#configure-authentication-available-for-all-customers}

Les options d’authentification s’affichent pour toute la clientèle. Les améliorations des fonctionnalités de gestion des mots de passe seront bientôt disponibles ou le sont déjà pour votre entreprise, comme décrit dans la section [Configurer l’authentification améliorée](#configure-enhanced-authentication-coming-soon) de cet article.

Pour configurer les préférences d’authentification :

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Authentification**.

1. Sélectionnez l’un des champs suivants pour définir les paramètres d’authentification de votre entreprise :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Forcer les utilisateurs et utilisatrices à réinitialiser leur mot de passe tous les <em>&lt;value&gt;</em> jours</td> 
      <td>Ceci établit le délai de réinitialisation des mots de passe Workfront. Cette option est désactivée par défaut. Lorsque vous l’activez, vous pouvez choisir entre 30, 60, 90, 120, 180 jours. La valeur par défaut est de 30 jours.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ne pas autoriser les utilisateurs et utilisatrices à définir un mot de passe identique à l’un des <em>&lt;value&gt;</em> derniers mots de passe utilisés.</td> 
      <td> <p>Ce champ interdit aux utilisateurs et utilisatrices de réutiliser des mots de passe pendant un nombre défini de réinitialisations. Par défaut, ce champ est désactivé. Lorsque vous l’activez, vous pouvez définir cette valeur sur 5, 10 ou 15 réinitialisations avant de pouvoir réutiliser un mot de passe.</p> <p>Lorsque cette option est sélectionnée, les utilisateurs et utilisatrices ne peuvent pas réinitialiser leurs mots de passe plus d’une fois par jour.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Si une personne saisit un mot de passe incorrect cinq fois de suite, le compte sera bloqué pendant <em>&lt;value&gt;</em> minutes : </td> 
      <td> <p>Sélectionnez la durée pendant laquelle le compte Workfront sera bloqué si une personne saisit un mot de passe incorrect cinq fois de suite. Par défaut, cette option est activée et le temps d’attente est de 10 minutes. Vous pouvez bloquer des comptes pendant 10 minutes, 30 minutes, 1 heure, 8 heures ou 24 heures. </p> <p>La réinitialisation manuelle du mot de passe de l’utilisateur ou de l’utilisatrice remplace cette valeur d’attente par défaut. <br>Les utilisateurs et utilisatrices peuvent réinitialiser leurs propres mots de passe lorsqu’ils sont bloqués via l’écran de connexion. Pour plus d’informations sur les façons de réinitialiser le mot de passe en cas d’oubli, voir <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Réinitialiser votre mot de passe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Les mots de passe doivent contenir au moins <em>&lt;value&gt;</em> types de caractères différents :</td> 
      <td> <p>Détermine le niveau de sécurité des mots de passe d’utilisateur ou d’utilisatrice requis en vous permettant de sélectionner les différents types de caractères requis dans les mots de passe.</p> <p>Un mot du dictionnaire reconnaissable ne peut pas être utilisé comme mot de passe.<br>Par défaut, Workfront exige d’inclure au moins 2 des types de caractères suivants dans les mots de passe (vous pouvez également exiger 3 de ces types de caractères pour un mot de passe valide) : </p> 
       <ul> 
        <li>Majuscules</li> 
        <li>Minuscules</li> 
        <li>Nombres</li> 
        <li>Symboles</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

## Configurer l’authentification améliorée{#configure-enhanced-authentication-coming-soon}

Cette section décrit l’expérience d’authentification améliorée, qui n’est peut-être pas encore disponible pour votre organisation. Si votre organisation n’a pas été migrée vers la nouvelle expérience d’authentification, vous devez configurer les paramètres d’authentification, comme décrit dans la section [Configurer l’authentification (disponible pour tous les clientes et clients)](#configure-authentication-available-for-all-customers).

Pour configurer les préférences d’authentification améliorée, procédez comme suit :

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Authentification améliorée**.
1. Dans la zone **Longueur du mot de passe**, saisissez le nombre minimum de caractères requis pour un mot de passe valide.

   Workfront requiert au moins 6 caractères.

1. (Facultatif) Dans la section **Exigences de mot de passe**, sélectionnez les types de caractères requis dans les mots de passe de l’utilisateur ou de l’utilisatrice.

   Vous pouvez augmenter la force des mots de passe de l’utilisateur ou de l’utilisatrice en exigeant n’importe quel type de caractères ou tous les types de caractères dans la section Exigence de mot de passe. Les options disponibles sont les suivantes :

   | Lettres minuscules | Requiert au moins une lettre minuscule. |
   |---|---|
   | Lettres majuscules | Requiert au moins une lettre majuscule. |
   | Nombres | Requiert au moins un nombre. |
   | Caractères spéciaux | Requiert au moins un caractère spécial. |

   {style="table-layout:auto"}

1. Cliquer sur **Enregistrer**.
