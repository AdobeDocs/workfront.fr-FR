---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Tester les connexions de webhook
description: Tester les connexions de webhook
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 100%

---


# Tester les connexions de webhook

Pour vérifier que votre implémentation de Document Webhook fonctionne correctement, exécutez les tests manuels de cette section. Ces étapes passent par l’interface web d’Adobe Workfront et accèdent indirectement aux points d’entrée de votre implémentation webhook.

## Conditions préalables

Les conditions préalables suivantes sont requises pour exécuter les tests :

* Un compte Workfront avec la gestion avancée des documents (ADM) activée.

* Un utilisateur ou une utilisatrice Workfront pour ce compte disposant des droits d’administration système.

* Une instance de Document Webhook avec des points d’entrée HTTP accessibles par Workfront.

Ces tests supposent également que votre instance Document Webhook est enregistrée. (Vous pouvez enregistrer votre instance dans Workfront dans Configuration > Documents > Intégrations personnalisées.)

**Test 1 : mettre en place le service Document Webhook pour un utilisateur ou une utilisatrice**

Teste l’URL d’authentification et l’URL du point d’entrée du jeton pour les fournisseurs de webhooks basés sur OAuth.

1. Dans Workfront, accédez à la page principale des documents en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Cliquez sur le menu déroulant Ajouter des documents et sélectionnez votre service Document Webhook dans Ajouter un service.
1. (Services OAuth uniquement) Après avoir effectué l’étape précédente, vous verrez la page d’authentification OAuth2 de votre service s’afficher dans une fenêtre contextuelle. (Remarque : il se peut que vous receviez d’abord une invitation à vous connecter à votre service.) Sur la page d’authentification, accordez à Workfront l’accès au compte de l’utilisateur ou de l’utilisatrice en cliquant sur le bouton Approuver ou autoriser.
1. Vérifiez que votre service a été ajouté au menu déroulant Ajouter des documents. Si en premier lieu vous ne le voyez pas, essayez d’actualiser votre navigateur.

**Test 2 : lier un document dans Workfront Teste les points d’entrée suivants : /files, /metadata.**

1. Dans Workfront, accédez à la page principale des documents en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Sélectionnez votre service Document Webhook dans Ajouter des documents.
1. Dans la fenêtre modale, naviguez dans la structure des dossiers.
1. Vérifiez que vous pouvez naviguer dans la structure des dossiers.
1. Sélectionner et lier un document dans Workfront

**Test 3 : naviguer jusqu’à un document dans le système de gestion de contenu**

Teste les points d’entrée suivants : /metadata (en particulier le viewLink).

1. Lier un document dans Workfront
1. Sélectionnez le document et cliquez sur le lien Ouvrir.
1. Vérifiez que le document s’ouvre dans un nouvel onglet.

**Test 4 : naviguer jusqu’à un document dans le système de gestion de contenu (avec une connexion active)**

Teste les points d’entrée suivants : /metadata (en particulier le viewLink).

1. Vérifiez que votre connexion au système de gestion de contenu n’est pas effective.
1. Liez un document dans Workfront.
1. Sélectionnez le document et cliquez sur le lien Ouvrir.
1. Vérifiez que l’écran de connexion du système de gestion de contenu se charge dans un nouvel onglet.
1. Connectez-vous et vérifiez que cela vous dirige bien vers le document.

**Test 5 : télécharger le document à partir du système de gestion de contenu**

Teste les points d’entrée suivants (en particulier le lien de téléchargement) : /metadata.

1. Liez un document dans Workfront.
1. Sélectionnez le document et cliquez sur le lien Télécharger.
1. Vérifiez que le téléchargement commence.

**Test 6 : rechercher du contenu**

Teste les points d’entrée suivants : /search.

1. Dans Workfront, accédez à la page principale des documents en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Sélectionnez votre service Document Webhook dans Ajouter des documents.
1. Dans la fenêtre modale, effectuez une recherche.
1. Vérifiez que les résultats de la recherche sont corrects.

**Test 7 : envoyer un document à partir de Workfront vers un système de gestion de contenu**

Teste les points d’entrée suivants : /files, /uploadInit, /upload.

1. Dans Workfront, accédez à la page principale des documents en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Chargez un document dans Workfront à partir de votre ordinateur.
1. Accédez à la page des détails du document.
1. Dans le menu déroulant Actions du document, sélectionnez votre service Document Webhook dans Envoyer à...
1. Accédez au dossier de destination souhaité et cliquez sur le bouton Enregistrer.
1. Vérifiez que le document est chargé au bon endroit dans le système de gestion de contenu.

**Test 8 : afficher les vignettes dans Workfront**

Teste les points d’entrée suivants : /thumbnail.

1. Liez un document dans Workfront.
1. Sélectionnez le document dans la liste.
1. Vérifiez que la vignette apparaît dans le panneau de droite.

**Test 9 : obtenir les octets du contenu**

Teste les points d’entrée suivants : /download.

1. Liez un document dans Workfront.
1. Accédez à la page des détails du document.
1. Envoyez le document à Workfront en sélectionnant Actions du document > Envoyer à... > Workfront. Cela crée une nouvelle version du document dans Workfront.
1. Téléchargez le document à partir de Workfront en cliquant sur le lien Télécharger.

**Test 10 : actualiser le jeton d’accès (fournisseurs de webhooks OAuth2 uniquement)**

Teste les points d’entrée suivants : URL du point d’entrée de jeton.

1. Mettre à disposition un service Document Webhook pour un utilisateur ou une utilisatrice
1. Invalidez le jeton d’accès de l’utilisateur ou de l’utilisatrice soit 1) en attendant que le délai d’expiration soit écoulé, soit 2) en l’invalidant manuellement dans le système externe.
1. Actualisez le jeton d’accès dans Workfront. Vous pouvez le faire, par exemple, en liant un document dans Workfront. Vous savez que le jeton d’accès a été actualisé si vous avez été en mesure de naviguer jusqu’à un document et le lier.

>[!NOTE]
>
>Actuellement, la fonction Envoyer à... n’est pas disponible pour les documents liés. Elle sera ajoutée par l’équipe Workfront. Vous pouvez tester le point d’entrée /download en accédant manuellement au point d’entrée à l’aide d’un client REST, tel que Postman. Il est également possible de tester le point d’entrée /download en générant une épreuve numérique. Pour activer la relecture numérique, contactez l’équipe Workfront.
