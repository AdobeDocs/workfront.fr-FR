---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Empêcher les utilisateurs en double
description: Lors de la création d’un nouvel utilisateur dans Adobe Workfront, vous ne pouvez plus utiliser d’adresse électronique déjà utilisée par un autre utilisateur, même si l’adresse électronique varie selon le cas (par exemple, JohnDoe@example.com et johndoe@example.com). En outre, pour préparer les futures améliorations de l’authentification, assurez-vous que tous les utilisateurs disposent d’adresses électroniques uniques dans une instance Workfront.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 13%

---

# Empêcher les doublons d’utilisateurs et d’utilisatrices

Lors de la création d’un nouvel utilisateur dans Adobe Workfront, vous ne pouvez plus utiliser d’adresse électronique déjà utilisée par un autre utilisateur, même si l’adresse électronique varie selon le cas (par exemple, JohnDoe@example.com et johndoe@example.com). En outre, pour préparer les futures améliorations de l’authentification, assurez-vous que tous les utilisateurs disposent d’adresses électroniques uniques dans une instance Workfront.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Créer des utilisateurs avec des adresses électroniques uniques

À partir de la version 2019.4, lors de la création d’un nouvel utilisateur dans Workfront, vous ne pouvez plus utiliser d’adresse électronique déjà utilisée par un autre utilisateur, même si l’adresse électronique varie selon le cas. Par exemple, vous ne pouvez pas créer un utilisateur avec l’adresse électronique JohnDoe@example.com si un autre utilisateur a l’adresse électronique johndoe@example.com.

## Mettre à jour les adresses électroniques des utilisateurs existants dans votre instance Workfront

En tant qu’administrateur de Workfront, vous devez mettre à jour les utilisateurs existants qui possèdent des adresses électroniques correspondantes qui ne diffèrent que par la casse.
Pour corriger les adresses électroniques en double dans une instance Workfront :

1. Examinez les utilisateurs en double et décidez quel utilisateur n’est plus nécessaire.

   {{step-1-to-users}}

   1. Dans le menu **Filter**, sélectionnez **All**.

   1. Dans le menu **View**, sélectionnez **User Login**.

   1. Dans le menu **Groupement**, sélectionnez **Rien**.

   1. Personnalisez la vue de connexion de l’utilisateur.

      1. Cliquez sur **Affichage** > **Personnaliser la vue**.

      1. Remplacez la colonne **ID** par la colonne **Adresse électronique**.

      1. Renommez la vue et enregistrez-la.

   1. Créez un groupement.

      1. Cliquez sur **Groupement** > **Nouveau groupement**.

      1. Cliquez sur **Passer en mode Texte** dans le coin supérieur droit de la page.
      1. Collez le code de mode Texte suivant :

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. Renommez le Groupement et enregistrez-le.

1. Effectuez l’une des opérations suivantes :

   * (Méthode préférée) Ajoutez une adresse + à l’adresse électronique de l’utilisateur pour chaque compte supplémentaire.

     Sélectionnez cette option si un utilisateur unique de votre entreprise doit accéder à plus d’un compte utilisateur. Si l’adressage plus n’est pas pris en charge par votre fournisseur de messagerie, vous devez fournir un compte de messagerie distinct pour chaque compte Workfront.

     Par exemple, John Doe peut avoir un compte utilisateur pour son compte d’utilisation quotidienne et un autre pour l’utilisation à des fins de test :

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * Modifiez le domaine pour utiliser un faux domaine en ajoutant le texte suivant à l’adresse électronique :

     `.inactive`

     Par exemple, John Doe peut avoir les domaines suivants : (Ils doivent être uniques.)

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     Vous ne pouvez plus vous connecter à ces comptes, car les réinitialisations de mot de passe nécessitent une adresse électronique valide. Ces comptes sont accessibles uniquement à l’aide de la fonction Se connecter en tant que .

   * Suppression des utilisateurs inutiles

     >[!IMPORTANT]
     >
     >Choisissez cette option uniquement pour les comptes créés par erreur ou pour les comptes de test. Cette option est généralement effectuée uniquement pour les comptes dont la connexion est nulle ou une erreur. Les comptes qui ont été régulièrement utilisés ne doivent jamais être supprimés.

Si des utilisateurs d’une instance Workfront ont des adresses électroniques correspondantes qui ne diffèrent que par la casse, Workfront vous contactera avec des informations supplémentaires et une chronologie du moment où celles-ci doivent être mises à jour.
