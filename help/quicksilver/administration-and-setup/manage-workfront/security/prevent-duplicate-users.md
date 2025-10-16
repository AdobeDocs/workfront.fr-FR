---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Empêcher les utilisateurs en double
description: Lors de la création d’un utilisateur ou d’une utilisatrice dans Adobe Workfront, vous ne pouvez plus utiliser une adresse e-mail déjà utilisée par un autre utilisateur ou une autre utilisatrice, même si l’adresse e-mail varie selon la casse (par exemple, JohnDoe@example.com et johndoe@example.com). En outre, pour se préparer à de futures améliorations en matière d’authentification, il faut s’assurer que tous les utilisateurs et toutes les utilisatrices disposent d’une adresse e-mail unique dans une instance de Workfront.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 98%

---

# Empêcher les doublons d’utilisateurs et d’utilisatrices

Lors de la création d’un utilisateur ou d’une utilisatrice dans Adobe Workfront, vous ne pouvez plus utiliser une adresse e-mail déjà utilisée par un autre utilisateur ou une autre utilisatrice, même si l’adresse e-mail varie selon la casse (par exemple, JohnDoe@example.com et johndoe@example.com). En outre, pour se préparer à de futures améliorations en matière d’authentification, il faut s’assurer que tous les utilisateurs et toutes les utilisatrices disposent d’une adresse e-mail unique dans une instance de Workfront.

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

## Créer des utilisateurs et utilisatrices avec des adresses e-mail uniques

À partir de la version 2019.4, lors de la création d’un utilisateur ou d’une utilisatrice dans Workfront, vous ne pouvez plus utiliser une adresse e-mail déjà utilisée par un autre utilisateur ou une autre utilisatrice, même si la casse des adresses e-mail est différente. Par exemple, vous ne pouvez pas créer un utilisateur ou une utilisatrice avec l’adresse e-mail JohnDoe@example.com si un autre utilisateur ou une autre utilisatrice a l’adresse e-mail johndoe@example.com.

## Mettre à jour les adresses e-mail des utilisateurs et utilisatrices existants dans votre instance Workfront

En tant qu’administrateur ou administratrice Workfront, vous devez mettre à jour les utilisateurs et utilisatrices existants dont les adresses e-mail correspondent, mais ont une casse différente.
Pour corriger les adresses e-mail dupliquées dans une instance de Workfront, procédez comme suit :

1. Examinez les éventuels doublons de personnes et décidez celles qui ne sont plus nécessaires.

   {{step-1-to-users}}

   1. Dans le menu **Filtre**, sélectionnez **Tout**.

   1. Dans le menu **Afficher**, sélectionnez **Identifiant d’utilisateur ou d’utilisatrice**.

   1. Dans le menu **Regroupement**, sélectionnez **Rien**.

   1. Personnalisez l’affichage de la vue Identifiant d’utilisateur ou d’utilisatrice.

      1. Cliquez sur **Vue** > **Personnaliser la vue**.

      1. Remplacez la colonne **ID** par la colonne **Adresse e-mail**.

      1. Renommez la vue et enregistrez-la.

   1. Créez un regroupement.

      1. Cliquez sur **Regroupement** > **Nouveau regroupement**.

      1. Cliquez sur **Basculer en mode texte** dans le coin supérieur droit de la page.
      1. Collez le code suivant en mode texte :

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. Renommez le regroupement et enregistrez-le.

1. Effectuez l’une des opérations suivantes :

   * (Méthode préférée) Ajoutez une adresse + à l’adresse e-mail de l’utilisateur ou de l’utilisatrice pour chaque compte supplémentaire.

     Choisissez cette option si un seul utilisateur ou une seule utilisatrice de votre organisation a besoin d’accéder à plus d’un compte. Si Plus Addressing n’est pas pris en charge par votre fournisseur de messagerie, vous devez fournir un compte de messagerie distinct pour chaque compte Workfront.

     Par exemple, John Doe peut avoir un compte d’utilisateur pour son utilisation quotidienne et un autre à des fins de test :

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * Modifiez le domaine pour utiliser un faux domaine en ajoutant le texte suivant à l’adresse e-mail :

     `.inactive`

     Par exemple, John Doe pourrait avoir les domaines suivants : (ceux-ci doivent être uniques).

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     Vous ne pouvez plus vous connecter à ces comptes, car la réinitialisation du mot de passe nécessite une adresse e-mail valide. Ces comptes sont uniquement accessibles à l’aide de la fonction « Connexion en tant que ».

   * Supprimer les utilisateurs et utilisatrices inutiles

     >[!IMPORTANT]
     >
     >Choisissez cette option uniquement pour les comptes qui ont été créés par erreur ou à des fins de test. Cette option n’est généralement utilisée que pour les comptes ayant zéro connexion ou bien une connexion erronée. Les comptes qui ont régulièrement été utilisés ne doivent jamais être supprimés.

Workfront vous informera et vous communiquera une chronologie s’il est découvert que des utilisateurs et des utilisatrices de la même instance ont des adresses e-mail qui ne diffèrent que par la casse des lettres.
