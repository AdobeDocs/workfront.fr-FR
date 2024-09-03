---
title: Vue d’ensemble de l’authentification améliorée
description: Masqué dans la recherche et dans la navigation de gauche
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: bf8e6c2b8a45cf65840a2ac8b3c25d11266d49f9
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 100%

---

# Vue d’ensemble de l’authentification améliorée

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront modifie la gestion des utilisateurs et utilisatrices et des mots de passe. Ces modifications seront déployées dans une version progressive appelée l’expérience d’**authentification améliorée** L’authentification améliorée offre aux utilisateurs et utilisatrices une expérience de connexion plus cohérente et sécurisée sur tous les produits et services Workfront.

Le tableau suivant fournit des détails sur les fonctionnalités actuelles et futures :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Fonctionnalité</strong> </p> </th> 
   <th><strong>Authentification héritée</strong> </th> 
   <th><strong>Authentification améliorée 1.0</strong> </th> 
   <th> <p>Authentification améliorée 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>Options de connexion</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permettre l’utilisation d’un seul nom d’utilisateur ou d’utilisatrice pour tous les produits et services Workfront, y compris la formation, l’assistance, etc.</p> </td> 
   <td>Non disponible</td> 
   <td> <p>Non disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permettre l’utilisation de la même adresse e-mail dans les instances de Workfront</p> </td> 
   <td> <p>✓</p> <p>Disponible à partir de la version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Disponible à partir de la version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Disponible à partir de la version 2019.3</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Les adresses e-mail ne sont pas sensibles à la casse.</p> </td> 
   <td> <p>✓</p> <p>Disponible à partir de la version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Plusieurs utilisateurs et utilisatrices ne peuvent pas avoir la même adresse e-mail si celle-ci ne diffère que par la casse. </p> </td> 
   <td> <p>✓</p> <p>Plusieurs utilisateurs et utilisatrices ne peuvent pas avoir la même adresse e-mail si celle-ci ne diffère que par la casse. </p> <p>Les administrateurs et administratrices de Workfront seront informés vers la fin de l’année 2019 par rapport aux adresses e-mail en double à corriger.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Options de gestion des mots de passe</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Créer un e-mail de réinitialisation de mot de passe pour un utilisateur ou une utilisatrice en tant qu’administrateur ou administratrice de Workfront</p> </td> 
   <td> <p>Non disponible </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Définir un mot de passe temporaire pour un utilisateur ou une utilisatrice en tant qu’administrateur ou administratrice de Workfront</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>Non prévu</p> <p>Cette fonctionnalité n’est pas une bonne pratique en matière de sécurité.</p> </td> 
   <td> <p>Non prévu</p> <p>Cette fonctionnalité n’est pas une bonne pratique en matière de sécurité.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Exigences de la politique des mots de passe</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exiger des utilisateurs et utilisatrices qu’ils réinitialisent leurs mots de passe après un certain délai.</p> </td> 
   <td>✓</td> 
   <td> <p>Non prévu</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Interdire aux utilisateurs et utilisatrices d’utiliser un mot de passe antérieur </p> </td> 
   <td>✓</td> 
   <td>Non prévu </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Protéger contre les tentatives de saisie de mots de passe erronés </p> </td> 
   <td> <p>✓ </p> <p>Verrouille le compte après 5 tentatives incorrectes de saisie du mot de passe. Le temps d’attente nécessaire après le verrouillage est configuré par l’équipe d’administration Workfront.</p> </td> 
   <td> <p>✓</p> <p>Le temps d’attente augmente de manière exponentielle après chaque saisie de mot de passe incorrect successive sur la base des bonnes pratiques du secteur ; le temps requis n’est pas configurable par l’équipe d’administration Workfront.</p> </td> 
   <td> <p>✓</p> <p>Utilise un algorithme de verrouillage qui bloque de manière proactive divers comportements suspects.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exiger un mélange de minuscules, de majuscules, de chiffres et de caractères spéciaux</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>Augmenter la flexibilité du choix des exigences spécifiques</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Définir une longueur minimale pour le mot de passe </p> </td> 
   <td> Non disponible </td> 
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
   <td colspan="3"> <p><strong>Prise en charge du protocole d’authentification unique</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Prend en charge les intégrations SSO conformes aux protocoles Active Directory et LDAP.</p> </td> 
   <td> ✓</td> 
   <td> <p> Obsolète</p> <p>Les systèmes Active Directory, Azure et LDAP doivent utiliser SAML 2.0.</p> </td> 
   <td> <p>Obsolète</p> <p>Les systèmes Active Directory, Azure et LDAP peuvent être configurés avec SAML 2.0 chiffré ou OpenID Connect.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Prend en charge les protocoles SSO conformes à SAML 2.0.</p> </td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Prend en charge les protocoles OpenID Connect.</p> </td> 
   <td> <p>Non disponible</p> </td> 
   <td> <p>Non disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Configure la page de connexion Workfront pour qu’elle redirige toujours vers la page de connexion du fournisseur d’identité. </p> </td> 
   <td> Activé par défaut et ne peut être désactivé.</td> 
   <td> <p>✓</p> <p>L’équipe d’administration Workfront peut configurer la page de connexion pour qu’elle redirige vers la page de connexion du fournisseur d’identité, ou configurer un ou plusieurs boutons de connexion.</p> </td> 
   <td> <p>✓</p> <p> L’équipe d’administration Workfront peut configurer la page de connexion pour qu’elle redirige vers la page de connexion du fournisseur d’identité, ou configurer un ou plusieurs boutons de connexion.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permettre à chaque instance d’activer plusieurs fournisseurs SSO</p> </td> 
   <td> <p>S/O</p> </td> 
   <td> <p>Non prévu</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Prise en charge de l’environnement</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Un seul nom d’utilisateur ou d’utilisatrice et un seul mot de passe pour les environnements de prévisualisation</p> </td> 
   <td> <p>Non disponible</p> </td> 
   <td> <p>Non disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Un seul nom d’utilisateur ou d’utilisatrice et un seul mot de passe pour les environnements de sandbox</p> </td> 
   <td> <p>Non disponible</p> </td> 
   <td> <p>Non disponible</p> </td> 
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
