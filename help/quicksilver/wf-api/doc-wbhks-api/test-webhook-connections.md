---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Tester les connexions Webhook
description: Tester les connexions Webhook
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 1%

---


# Tester les connexions Webhook

Pour vérifier que l’implémentation de webhook de votre document fonctionne correctement, exécutez les tests manuels décrits dans cette section. Ces étapes passent par l’interface web d’Adobe Workfront et atteignent indirectement les points de terminaison de votre implémentation de webhook.

## Conditions préalables

Les conditions préalables suivantes sont requises pour exécuter les tests :

* un compte Workfront avec la fonction Advanced Document Management (ADM) activée ;

* Un utilisateur Workfront pour ce compte avec les droits d’administrateur système

* Une instance Webhook de document avec des points de terminaison HTTP accessibles par Workfront

Ces tests supposent également que votre instance Document Webhook est enregistrée. (Vous pouvez enregistrer votre instance dans Workfront sous Configuration > Documents > Intégrations personnalisées.)

**Test 1 : Configuration du service Document Webhook pour un utilisateur**

Teste l’URL d’authentification et l’URL du point de terminaison du jeton pour les fournisseurs WebHook basés sur OAuth.

1. Dans Workfront, accédez à la page Documents principale en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Cliquez sur la liste déroulante Ajouter des documents et sélectionnez votre service Document Webhook sous Ajouter un service.
1. (Services OAuth uniquement) Une fois l’étape précédente terminée, la page d’authentification OAuth2 de votre service s’affiche dans une fenêtre contextuelle. (Remarque : vous pouvez être invité à vous connecter d’abord à votre service.) Sur la page d’authentification, accordez à Workfront l’accès au compte de l’utilisateur en cliquant sur le bouton Approbation ou Autoriser .
1. Vérifiez que votre service a été ajouté à la liste déroulante Ajouter des documents . Si vous ne le voyez pas initialement, essayez d’actualiser votre navigateur.

**Test 2 : liez un document dans Workfront Tests les points de terminaison suivants : /files, /metadata**

1. Dans Workfront, accédez à la page Documents principale en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Sélectionnez votre service Document Webhook sous Ajouter des documents.
1. Dans le modal, parcourez la structure de dossiers.
1. Vérifiez que vous pouvez parcourir la structure de dossiers.
1. Sélection et liaison d’un document à Workfront

**Test 3 : Accédez à un document dans le système de gestion de contenu**

Teste les points de terminaison suivants : /metadata (en particulier viewLink)

1. Liaison d’un document à Workfront
1. Sélectionnez le document et cliquez sur le lien Ouvrir .
1. Vérifiez que le document s’ouvre dans un nouvel onglet.

**Test 4 : Accédez à un document dans le système de gestion de contenu (avec connexion)**

Teste les points de terminaison suivants : /metadata (en particulier viewLink)

1. Assurez-vous d’être déconnecté du système de gestion de contenu.
1. Liez un document à Workfront.
1. Sélectionnez le document et cliquez sur le lien Ouvrir .
1. Vérifiez que l’écran de connexion du système de gestion de contenu se charge dans un nouvel onglet.
1. Connectez-vous et vérifiez que vous êtes connecté au document.

**Test 5 : Téléchargez le document à partir du système de gestion de contenu**

Teste les points de terminaison suivants (en particulier le lien de téléchargement) : /metadata 

1. Liez un document à Workfront.
1. Sélectionnez le document et cliquez sur le lien Télécharger .
1. Vérifiez que le téléchargement commence.

**Test 6 : Recherche de contenu**

Teste les points de terminaison suivants : /search

1. Dans Workfront, accédez à la page Documents principale en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Sélectionnez votre service Document Webhook sous Ajouter des documents.
1. Dans le modal, effectuez une recherche.
1. Vérifiez que les résultats de la recherche sont corrects.

**Test 7 : envoyer un document de Workfront vers le système de gestion de contenu**

Teste les points de terminaison suivants : /files, /uploadInit, /upload

1. Dans Workfront, accédez à la page Documents principale en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Téléchargement d’un document vers Workfront à partir de votre ordinateur
1. Accédez à la page des détails du document.
1. Dans la liste déroulante Actions de document , sélectionnez votre service Document Webhook sous Envoyer à...
1. Accédez au dossier de destination de votre choix et cliquez sur le bouton Enregistrer .
1. Vérifiez que le document est téléchargé au bon emplacement dans le système de gestion de contenu.

**Test 8 : Afficher les miniatures dans Workfront**

Teste les points de terminaison suivants : /thumbnail

1. Liez un document à Workfront.
1. Sélectionnez le document dans la liste.
1. Vérifiez que la miniature s’affiche dans le panneau de droite.

**Test 9 : obtenir les octets de contenu**

Teste les points de terminaison suivants : /download

1. Liez un document à Workfront.
1. Accédez à la page des détails du document.
1. Envoyez le document à Workfront en sélectionnant Actions du document > Envoyer à... > Workfront. Une nouvelle version de document est alors créée dans Workfront.
1. Téléchargez le document à partir de Workfront en cliquant sur le lien Télécharger .

**Test 10 : Actualiser le jeton d’accès (fournisseurs OAuth2 Webhook uniquement)**

Teste les points de terminaison suivants : URL du point de terminaison du jeton

1. Configuration d’un service Document Webhook pour un utilisateur
1. Invalidez le jeton d’accès de l’utilisateur par 1 ) en attendant son expiration ou 2) en l’invalidant manuellement dans le système externe.
1. Actualisez le jeton d’accès dans Workfront. Vous pouvez le faire, par exemple, en liant un document à Workfront. Vous savez que le jeton d’accès s’est correctement actualisé si vous avez pu accéder à un document et le lier.

>[!NOTE]
>
>Actuellement, l’option Envoyer à... n’est pas disponible pour les documents liés. Cela sera ajouté par Workfront. Vous pouvez tester le point de terminaison /download en appuyant manuellement sur le point de terminaison à l’aide d’un client REST, tel que Postman. Vous pouvez également tester le point de terminaison /download en générant un BAT numérique. Pour l’activer, contactez Workfront.
