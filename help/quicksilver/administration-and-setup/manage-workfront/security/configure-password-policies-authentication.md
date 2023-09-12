---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configuration des stratégies de mot de passe pour l’authentification
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer les options de stratégie de mot de passe pour personnaliser l’expérience d’authentification de votre système Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 970cc86b00dc1afe0473ac3a387e7ce47e4a2433
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Configuration des stratégies de mot de passe pour l’authentification

{{important-admin-console-onboard}}

En tant qu’administrateur Adobe Workfront, vous pouvez configurer les options de stratégie de mot de passe pour personnaliser l’expérience d’authentification de votre système Workfront.

Nous vous recommandons de configurer les préférences d’authentification lors de l’implémentation de Workfront et de ne les revoir qu’occasionnellement par la suite.

Amélioration des fonctionnalités de gestion des mots de passe bientôt ou déjà disponibles pour votre entreprise. Utilisez l’une des sections suivantes, selon que votre entreprise a accès ou non à la nouvelle expérience d’authentification.

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
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurer l’authentification (disponible pour tous les clients) {#configure-authentication-available-for-all-customers}

Les options d’authentification s’affichent pour tous les clients. Amélioration des fonctionnalités de gestion des mots de passe bientôt ou déjà disponibles pour votre entreprise, comme décrit dans la section . [Configuration de l’authentification améliorée)](#configure-enhanced-authentication-coming-soon) dans cet article.

Pour configurer les préférences d’authentification :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Authentification**.

1. Sélectionnez l’un des champs suivants pour définir les paramètres d’authentification de votre entreprise :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Forcer les utilisateurs à réinitialiser leur mot de passe chaque <em>&lt;value&gt;</em> days</td> 
      <td>Cela établit la période pendant laquelle les utilisateurs peuvent réinitialiser leur mot de passe Workfront. Par défaut, cette option est désactivée. Lorsque vous l’activez, vous pouvez choisir entre 30, 60, 90, 120, 180 jours. La valeur par défaut est de 30 jours.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ne pas autoriser les utilisateurs à définir le même mot de passe que l’un de leurs précédents <em>&lt;value&gt;</em> mots de passe</td> 
      <td> <p>Ce champ interdit aux utilisateurs de réutiliser des mots de passe pour un nombre défini de réinitialisations. Par défaut, ce champ est désactivé. Lorsque vous l’activez, vous pouvez définir cette valeur sur 5, 10 ou 15 réinitialisations avant de pouvoir réutiliser un mot de passe.</p> <p>Lorsque cette option est sélectionnée, les utilisateurs ne peuvent pas réinitialiser leurs mots de passe plus d’une fois par jour.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Si un mot de passe incorrect est saisi cinq fois de suite, verrouillez le compte pour <em>&lt;value&gt;</em> minutes : </td> 
      <td> <p>Sélectionnez la durée pendant laquelle un utilisateur sera verrouillé de Workfront après avoir saisi un mot de passe incorrect cinq fois de suite. Par défaut, cette option est activée et le temps d’attente est de 10 minutes. Vous pouvez verrouiller des comptes pendant 10 minutes, 30 minutes, 1 heure, 8 heures ou 24 heures. </p> <p>La réinitialisation manuelle du mot de passe de l’utilisateur remplace cette valeur d’attente par défaut. <br>Les utilisateurs peuvent réinitialiser leurs propres mots de passe lorsqu’ils sont verrouillés via l’écran de connexion. Pour plus d’informations sur la façon dont ils peuvent réinitialiser leur mot de passe, s’ils l’ont oublié, voir <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Réinitialisation de votre mot de passe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Les mots de passe doivent contenir au moins <em>&lt;value&gt;</em> différents types de caractères :</td> 
      <td> <p>Détermine le nombre de mots de passe utilisateur requis en vous permettant de sélectionner les différents types de caractères requis dans vos mots de passe.</p> <p>Un mot de dictionnaire reconnaissable ne peut pas être utilisé comme mot de passe.<br>Par défaut, Workfront exige qu’au moins 2 des caractères suivants soient présents dans les mots de passe (vous pouvez également avoir besoin de 3 de ces caractères pour un mot de passe valide) : </p> 
       <ul> 
        <li>Caractères majuscules</li> 
        <li>Caractères minuscules</li> 
        <li>Nombres</li> 
        <li>Symboles</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

## Configuration de l’authentification améliorée{#configure-enhanced-authentication-coming-soon}

Cette section décrit l’expérience d’authentification améliorée, qui n’est peut-être pas encore disponible pour votre entreprise. Si votre entreprise n’a pas été migrée vers la nouvelle expérience d’authentification, vous devez configurer les paramètres d’authentification, comme décrit dans la section [Configurer l’authentification (disponible pour tous les clients)](#configure-authentication-available-for-all-customers).

Pour configurer les préférences d’authentification améliorées :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Authentification améliorée**.
1. Dans le **Longueur du mot de passe** saisissez le nombre minimum de caractères requis pour un mot de passe valide.

   Workfront requiert au moins 6 caractères.

1. (Facultatif) Dans la variable **Exigences en matière de mot de passe** , sélectionnez les types de caractères requis dans les mots de passe utilisateur.

   Vous pouvez augmenter la force des mots de passe utilisateur en exigeant n’importe quel type de caractères ou tous les types de caractères dans la section Exigence de mot de passe . Les options disponibles sont les suivantes :

   | Lettres minuscules | Requiert au moins une lettre minuscule |
   |---|---|
   | Lettres majuscules | Requiert au moins une lettre majuscule |
   | Nombres | Nécessiter au moins un nombre |
   | Caractères spéciaux | Requiert au moins un caractère spécial |

   {style="table-layout:auto"}

1. Cliquer sur **Enregistrer**.
