---
title: Octroi de l’accès aux autorisations de marque
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer les autorisations de marque en créant un groupe d’utilisateurs dans Admin Console et en attribuant le profil de produit Gestionnaire système GenStudio .
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 727efbd6-79b4-42c5-bfa2-e5350f30ff23
source-git-commit: f74c567505dbdf6b2d1d8a85a62ba40d919be7b3
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 9%

---

# Octroi de l’accès aux autorisations de marque

{{highlighted-preview-article-level}}

Les utilisateurs se voient accorder les autorisations de création, de modification et de publication de marque des responsables système d’Adobe GenStudio lorsqu’ils sont ajoutés à un groupe d’utilisateurs.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations Admin Console</td> 
   <td> <p>Vous devez être un administrateur système dans Adobe Admin Console.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions

* Les approbations unifiées doivent être activées pour votre instance Workfront.

* Votre organisation doit disposer de GenStudio Foundation.
   * Content Reviewer dans Workfront fournit les fonctionnalités disponibles dans GenStudio Foundation pour les workflows de révision et d’approbation de ressources. Vous n’avez pas besoin d’accéder directement à GenStudio Foundation pour terminer votre travail. Votre accès à la fonctionnalité GenStudio Foundation par l’intermédiaire de l’analyseur de contenu est soumis aux conditions de votre contrat Workfront.
* Adobe doit disposer d’un contrat Adobe Gen AI signé dans ce fichier.
Pour plus d’informations sur la signature du contrat, voir [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## &#x200B;1. Configuration des autorisations de marque dans Admin Console

### Étape 1 : créer un groupe d’utilisateurs

Créez un groupe d’utilisateurs dans Admin Console pour gérer les autorisations de création et de modification de marques.

### Étape 2 : affecter un profil de produit au groupe d’utilisateurs

Le droit associé au profil affecté donne à tous les utilisateurs de ce groupe les autorisations de marques GenStudio (création, mise à jour et suppression de marques).

Pour attribuer un profil :

1. Accédez au groupe d’utilisateurs nouvellement créé.
1. Cliquez sur l’onglet **Profils de produit attribués**.
1. Cliquez sur **Attribuer un profil**.
1. Dans la fenêtre contextuelle, sélectionnez **&#x200B;**&#x200B;dans la liste de produits, puis cliquez sur **Appliquer**.
1. Sélectionnez le profil **Éditeurs Adobe GenStudio Foundation**.
1. Cliquez sur **Appliquer**.
1. Cliquez sur **Enregistrer**.

### Étape 3 : ajouter des utilisateurs au groupe d’utilisateurs

Pour attribuer aux utilisateurs des autorisations de création, de modification et de publication de marques, ajoutez-les au groupe d’utilisateurs .

>[!NOTE]
>
>Vous devez ajouter au moins un utilisateur avant d’ajouter le groupe à un projet, comme décrit à l’étape 4.

Pour ajouter des utilisateurs :

1. Accédez à **&#x200B;**&#x200B;> **Utilisateurs** > **Groupes d’utilisateurs**.
1. Sélectionnez votre groupe d’utilisateurs.
1. Ajoutez des utilisateurs par nom d’utilisateur ou adresse électronique.
1. Effectuez un choix parmi les correspondances suggérées pour les utilisateurs existants.

### Étape 4 : créer un projet Marques

Un projet fournit un emplacement de stockage où les utilisateurs peuvent enregistrer les ressources de la marque.

Pour créer un projet :

1. Accédez à l’onglet **Stockage** dans Admin Console.
1. Cliquez sur **Projets**.
1. Cliquez sur **Créer un projet**.
1. Dans la fenêtre contextuelle, saisissez le nom du projet : **Marques**.

   >[!IMPORTANT]
   >
   >Saisissez le nom du projet exactement comme indiqué. N’ajoutez pas d’espaces supplémentaires et ne modifiez pas la casse.

1. Cliquez sur **Créer**.

### Étape 5 : inviter le groupe d’utilisateurs au projet

Ajoutez le groupe d’utilisateurs au projet Marques afin qu’ils puissent accéder aux ressources et les gérer.

1. Dans la fenêtre contextuelle **Inviter au projet** ajoutez le groupe d’utilisateurs que vous avez créé.
1. Sélectionnez **Peut modifier** autorisations.
1. Cliquez sur **Inviter**.

### Résultat

Les utilisateurs du groupe disposent désormais des autorisations nécessaires pour créer, modifier et publier des ressources de marque dans Workfront.

## &#x200B;2. Accorder l’accès à Marques dans les niveaux d’accès Workfront

Vous devez suivre toutes les étapes de la section précédente avant d’accorder l’accès à des utilisateurs individuels pour les niveaux d’accès Marques dans Workfront .

>[!IMPORTANT]
>
>* Seuls les utilisateurs affectés au groupe d’utilisateurs avec le profil de produit Gestionnaire système GenStudio dans Admin Console peuvent créer, modifier et publier des marques dans Workfront, même si d’autres utilisateurs ont accès aux marques activées dans leurs paramètres de niveau d’accès.
>* Les utilisateurs ajoutés au niveau d’accès avec un accès aux marques activé mais non ajoutés au groupe d’utilisateurs dans l’Admin Console peuvent uniquement afficher les marques.


Pour accorder l’accès aux marques dans les niveaux d’accès Workfront :

{{step-1-to-setup}}

1. Cliquez sur **Niveaux d’accès** dans le panneau de gauche.
1. Recherchez le niveau d’accès à modifier, puis cliquez sur l’icône de modification ![icône de modification](assets/edit-icon.png) pour le modifier.

   Ou

   Cliquez sur **Nouveau niveau d&#39;accès** pour créer un nouveau niveau d&#39;accès. Pour plus d&#39;informations sur la création de niveaux d&#39;accès, voir [Créer ou modifier des niveaux d&#39;accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Faites défiler jusqu’à **Définir des restrictions supplémentaires**, puis sélectionnez **Autoriser les utilisateurs à accéder à Marques**.
   ![paramètre autoriser l’accès aux marques](assets/access-for-brands.png)
1. Cliquez sur **Enregistrer**.

Une fois que vous avez configuré les marques, vous pouvez créer un réviseur de contenu pour réviser les ressources en fonction des directives de la marque dans le workflow de révision et d’approbation. Pour plus d’informations, voir [Configuration des collaborateurs d’IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).
