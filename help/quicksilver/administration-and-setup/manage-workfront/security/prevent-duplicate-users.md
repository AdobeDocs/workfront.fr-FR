---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Prévention des doublons d’utilisateurs
description: Lors de la création d’un nouvel utilisateur dans Adobe Workfront, vous ne pouvez plus utiliser d’adresse électronique déjà utilisée par un autre utilisateur, même si l’adresse électronique varie selon le cas (par exemple, JohnDoe@example.com et johndoe@example.com). En outre, pour préparer les futures améliorations de l’authentification, assurez-vous que tous les utilisateurs disposent d’adresses électroniques uniques dans une instance Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6f5b9e7638a85eca16d722cec6185cd5ed755eca
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Prévention des doublons d’utilisateurs

Lors de la création d’un nouvel utilisateur dans Adobe Workfront, vous ne pouvez plus utiliser d’adresse électronique déjà utilisée par un autre utilisateur, même si l’adresse électronique varie selon le cas (par exemple, JohnDoe@example.com et johndoe@example.com). En outre, pour préparer les futures améliorations de l’authentification, assurez-vous que tous les utilisateurs disposent d’adresses électroniques uniques dans une instance Workfront.

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
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Présentation

<!--WRITER
<iframe class="vimeo-player_0" src="assets/371505632?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>
-->

[Regardez une démonstration vidéo de cette fonctionnalité.](https://vimeo.com/371505632/2e6938ce06)

## Créer des utilisateurs avec des adresses électroniques uniques

À partir de la version 2019.4, lors de la création d’un nouvel utilisateur dans Workfront, vous ne pouvez plus utiliser d’adresse électronique déjà utilisée par un autre utilisateur, même si l’adresse électronique varie selon le cas. Par exemple, vous ne pouvez pas créer un utilisateur avec l’adresse électronique JohnDoe@example.com si un autre utilisateur a l’adresse électronique johndoe@example.com.

## Mettre à jour les adresses électroniques des utilisateurs existants dans votre instance Workfront

En tant qu’administrateur de Workfront, vous devez mettre à jour les utilisateurs existants qui possèdent des adresses électroniques correspondantes qui ne diffèrent que par la casse.
Pour corriger les adresses électroniques en double dans une instance Workfront :

1. Examinez les utilisateurs en double et décidez quel utilisateur n’est plus nécessaire.

   1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **Utilisateurs**. ![](assets/users-icon-in-main-menu.png)

   1. Dans le **Filtrer** menu, sélectionnez **Tous**.

   1. Dans le **Affichage** menu, sélectionnez **Connexion utilisateur**.

   1. Dans le **Regroupement** menu, sélectionnez **Rien**.

   1. Personnalisez la vue de connexion de l’utilisateur.

      1. Cliquez sur **Affichage** > **Vue Personnaliser**.

      1. Remplacez la variable **ID** avec la colonne **Adresse électronique** colonne .

      1. Renommez la vue et enregistrez-la.
   1. Créez un groupement.

      1. Cliquez sur **Regroupement** > **Nouveau groupement**.

      1. Cliquez sur **Passer en mode Texte** dans le coin supérieur droit de la page.
      1. Collez le code de mode Texte suivant :

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. Renommez le Groupement et enregistrez-le.



1. Effectuez l’une des opérations suivantes :

   * (Méthode préférée) Ajoutez une adresse + à l’adresse électronique de l’utilisateur pour chaque compte supplémentaire.

      Sélectionnez cette option si un utilisateur unique de votre entreprise doit accéder à plus d’un compte utilisateur. Si l’adressage plus n’est pas pris en charge par votre fournisseur de messagerie, vous devez fournir un compte de messagerie distinct pour chaque compte Workfront.

      Par exemple, John Doe peut avoir un compte d’utilisateur pour son compte d’utilisation quotidienne et un compte à utiliser à des fins de test :

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * Modifiez le domaine pour utiliser un faux domaine en ajoutant le texte suivant à l’adresse électronique :

      `.inactive`

      Par exemple, John Doe peut avoir les domaines suivants : (Elles doivent être uniques.)

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      Vous ne pouvez plus vous connecter à ces comptes, car les réinitialisations de mot de passe nécessitent une adresse électronique valide. Ces comptes sont accessibles uniquement à l’aide de la fonction Se connecter en tant que .

   * Suppression des utilisateurs inutiles

      >[!IMPORTANT]
      >
      >Choisissez cette option uniquement pour les comptes créés par erreur ou pour les comptes de test. Cette option est généralement effectuée uniquement pour les comptes dont la connexion est nulle ou une erreur. Les comptes qui ont été régulièrement utilisés ne doivent jamais être supprimés.



Si des utilisateurs d’une instance Workfront ont des adresses électroniques correspondantes qui ne diffèrent que par la casse, Workfront vous contactera avec des informations supplémentaires et une chronologie du moment où celles-ci doivent être mises à jour.
