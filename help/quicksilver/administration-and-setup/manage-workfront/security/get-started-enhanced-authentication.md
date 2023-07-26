---
title: Présentation de l’authentification améliorée
description: Masqué de la recherche et du volet de navigation de gauche
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 3%

---

# Présentation de l’authentification améliorée

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront modifie la gestion système des utilisateurs et des mots de passe. Ces modifications seront appliquées par phases, appelées **Authentification améliorée** expérience. L’authentification améliorée offre aux utilisateurs une expérience de connexion plus cohérente et plus sécurisée pour tous les produits et services Workfront.

Le tableau suivant fournit des détails sur les fonctionnalités actuelles et futures :

>[!IMPORTANT]
>
>La plupart des clients utilisent actuellement l’authentification héritée et certains utilisent l’authentification améliorée 1.0.
> 
>Pour vérifier le type d’authentification que vous utilisez actuellement, accédez à *your_domain*.my.workfront.com/login. Si vous êtes redirigé vers /auth/login, vous utilisez l’authentification améliorée 1.0.
> 
>Si vous êtes redirigé vers https://login-a-xx.workfront.com/, où &quot;xx&quot; peut être États-Unis (États-Unis), UE (Europe) ou GCP (Google Cloud Platform) en fonction de votre emplacement/plateforme, alors vous utilisez l’authentification améliorée 2.0.
>
>Tous les clients passeront à l’authentification améliorée 2.0 d’ici la fin de 2021.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Fonctionnalité</strong> </p> </th> 
   <th><strong>Authentification héritée</strong> </th> 
   <th><strong>Authentification améliorée 1.0</strong> </th> 
   <th> <p>Authentification améliorée 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>Options de connexion</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Activer l’utilisation d’un seul nom d’utilisateur pour tous les produits et services Workfront, y compris la formation, l’assistance et autres</p> </td> 
   <td>non disponible</td> 
   <td> <p>non disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autoriser l’utilisation de la même adresse électronique sur les instances Workfront</p> </td> 
   <td> <p>✓</p> <p>Disponible à partir de la version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Disponible à partir de la version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Disponible à partir de la version 2019.3</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Les adresses électroniques ne sont pas sensibles à la casse</p> </td> 
   <td> <p>✓</p> <p>Disponible à partir de la version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Plusieurs utilisateurs ne peuvent pas avoir la même adresse électronique si l’adresse diffère uniquement par casse. </p> </td> 
   <td> <p>✓</p> <p>Plusieurs utilisateurs ne peuvent pas avoir la même adresse électronique si l’adresse diffère uniquement par casse. </p> <p>Les administrateurs de Workfront seront avertis à la fin de 2019 de commencer à corriger les adresses email en double.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Options de gestion des mots de passe</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Incorporation d’un courrier électronique de réinitialisation de mot de passe pour un utilisateur en tant qu’administrateur Workfront</p> </td> 
   <td> <p>non disponible </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Définition d’un mot de passe temporaire pour un utilisateur en tant qu’administrateur Workfront</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>Non planifié</p> <p>Cette fonctionnalité n’est pas une bonne pratique de sécurité</p> </td> 
   <td> <p>Non planifié</p> <p>Cette fonctionnalité n’est pas une bonne pratique de sécurité</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Exigences en matière de stratégie de mot de passe</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Obliger les utilisateurs à réinitialiser les mots de passe après une certaine période</p> </td> 
   <td>✓</td> 
   <td> <p>Non planifié</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Restreindre les utilisateurs à l’utilisation d’un mot de passe précédent </p> </td> 
   <td>✓</td> 
   <td>Non planifié </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Protection contre les tentatives de saisie de mot de passe incorrectes </p> </td> 
   <td> <p>✓ </p> <p>Verrouille le compte après 5 tentatives de saisie de mot de passe incorrectes. Le temps d’attente requis après l’enregistrement est configuré par l’administrateur Workfront.</p> </td> 
   <td> <p>✓</p> <p>Le temps d’attente augmente de manière exponentielle après chaque mot de passe incorrect consécutif en fonction des bonnes pratiques du secteur ; le temps requis n’est pas configurable par l’administrateur Workfront.</p> </td> 
   <td> <p>✓</p> <p>Utilise un algorithme de verrouillage qui bloque de manière proactive tout type de comportement suspect.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Requiert un mélange de minuscules, de majuscules, de nombres et de caractères spéciaux.</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>Plus grande flexibilité pour choisir des exigences spécifiques</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Définition d’une longueur minimale de mot de passe </p> </td> 
   <td> non disponible </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>Prise en charge du protocole de connexion unique</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Prend en charge les intégrations SSO conformes aux protocoles Principal Directory et LDAP</p> </td> 
   <td> ✓ </td> 
   <td> <p> Obsolète</p> <p>Les systèmes principale Directory, Azure et LDAP doivent utiliser SAML 2.0</p> </td> 
   <td> <p>Obsolète</p> <p>Les systèmes principale Directory, Azure et LDAP peuvent être configurés avec SAML 2.0 chiffré ou OpenID Connect.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Prend en charge les protocoles SSO conformes à SAML 2.0 </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Prend en charge les protocoles Open ID Connect</p> </td> 
   <td> <p>non disponible</p> </td> 
   <td> <p>non disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Configurez la page de connexion Workfront pour toujours rediriger vers la page de connexion du fournisseur d’identité. </p> </td> 
   <td> Activé par défaut et ne peut pas être désactivé</td> 
   <td> <p>✓</p> <p>L’administrateur de Workfront peut configurer la page de connexion pour qu’elle revienne à la page de connexion du fournisseur d’identité ou configurer un bouton ou des boutons de connexion.</p> </td> 
   <td> <p>✓</p> <p> Les administrateurs de Workfront peuvent configurer la page de connexion pour qu’elle revienne à la page de connexion du fournisseur d’identité ou configurer un bouton ou des boutons de connexion.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autoriser chaque instance à activer plusieurs fournisseurs d’authentification unique</p> </td> 
   <td> <p>S/O</p> </td> 
   <td> <p>Non planifié</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Prise en charge de l’environnement</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Un nom d’utilisateur et un mot de passe uniques pour les environnements d’aperçu</p> </td> 
   <td> <p>non disponible</p> </td> 
   <td> <p>non disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nom d’utilisateur et mot de passe uniques pour les environnements Sandbox</p> </td> 
   <td> <p>non disponible</p> </td> 
   <td> <p>non disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>
