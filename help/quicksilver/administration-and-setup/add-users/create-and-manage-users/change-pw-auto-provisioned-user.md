---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Modification du mot de passe d’un utilisateur muni d’un profil d’approvisionnement automatique
description: Nous vous recommandons de remplacer le nom d’utilisateur d’un nouvel utilisateur par son adresse électronique Workfront, puis de lui permettre de modifier son mot de passe.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 94%

---

# Modifier le mot de passe d’un utilisateur ou d’une utilisatrice ayant un profil auto-alloué

Lorsque vous créez des utilisateurs et utilisatrices par le biais de l’approvisionnement automatique, Adobe Workfront leur attribue un GUID (identifiant unique global) comme nom d’utilisateur ou d’utilisatrice. Un GUID est une chaîne unique de chiffres et de lettres aléatoires, par exemple, *5489cb430012526e1ea635e8c29f377f*.

Souvent, lorsqu’une nouvelle personne tente de modifier son mot de passe temporaire, elle saisit son adresse e-mail comme nom d’utilisateur ou d’utilisatrice et reçoit un message d’erreur pour un nom d’utilisateur ou d’utilisatrice incorrect. Pour que la personne puisse modifier son mot de passe, elle doit saisir son nom d’utilisateur ou d’utilisatrice attribué par le système, qui est un GUID.

Comme les noms d’utilisateur ou d’utilisatrice GUID peuvent être difficiles à utiliser, nous vous recommandons d’abord de remplacer le nom de l’utilisateur ou de l’utilisatrice par son adresse e-mail Workfront, puis de lui permettre de modifier son mot de passe.

>[!TIP]
>
>Vous pouvez trouver le GUID d’une personne de la manière suivante :
>
>* Accédez au profil de la personne et copiez le GUID à partir de l’URL de votre navigateur.
>
>  Par exemple, dans l’URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`, vous copiez la chaîne de chiffres et de lettres entre les deux dernières barres obliques : `61941ab1000af22d7104628efa1c738b`.
>
>  Pour plus d’informations, voir [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Créez un rapport sur les utilisateurs ou utilisatrices avec une colonne Utilisateur ou utilisatrice > GUID. Pour plus d’informations, voir [Créer un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Interrogez l’API Workfront.
>

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Modifier le mot de passe d’un utilisateur ou d’une utilisatrice ayant un profil auto-alloué

1. Déterminez le nom d’utilisateur ou d’utilisatrice GUID d’une personne en transmettant une requête API, comme illustré dans l’exemple suivant :

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` où *`<domain>`* correspond au domaine de votre société et *`<ID of User>`* à l’ID Workfront de la personne.

   Vous recevez une réponse similaire à celle-ci :

   ![](assets/get-guid.png)

   Le retour de « username » est le GUID de la personne.

1. En utilisant le GUID comme nom d’utilisateur ou d’utilisatrice, modifiez le mot de passe de la personne.

   Pour plus d’informations sur la modification de votre mot de passe, voir [Réinitialiser votre mot de passe](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Si votre entreprise utilise un système d’authentification unique, seul un administrateur ou une administratrice système Workfront peut modifier le mot de passe d’une personne. Pour plus d’informations, voir [Vue d’ensemble de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

1. Une fois la personne connectée à Workfront, accédez à :

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. Dans la zone **Votre adresse e-mail de connexion**, vérifiez l’adresse e-mail de la personne, puis cliquez sur **Mettre à jour le compte**.

   ![](assets/guidusername-350x272.png)

   Le nom d’utilisateur ou d’utilisatrice de la personne est remplacé par son adresse e-mail Workfront.

>[!TIP]
>
>Pour rechercher l’ID d’une personne :
>
>1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Utilisateurs et utilisatrices** ![](assets/users-icon-in-main-menu.png).
>
>1. Sélectionnez la personne.
>
>   La page de profil de la personne s’ouvre et son ID s’affiche dans l’URL.
>
