---
product-area: documents
navigation-topic: approvals
title: Détails de l’AppBuilder dans le document Workfront
description: Vous pouvez installer AppBuilder dans les Détails du document
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 74e0a85b-a8aa-4e39-9c2e-0f09957ebafa
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 1%

---

# Détails de l’AppBuilder dans le document Workfront

Vous pouvez installer AppBuilder dans les Détails du document.

## Conditions préalables

Vous devez disposer des éléments suivants :

* Un compte Workfront compatible IMS
* Une machine de développement avec le nœud v18 et npm

## Ajout de développeurs à Admin Console

>[!IMPORTANT]
>
>Assurez-vous d’avoir sélectionné la bonne organisation IMS pour toutes les étapes suivantes. Si vous appartenez à plusieurs organisations, il est possible de sélectionner la mauvaise. Assurez-vous que vous agissez sous la bonne organisation, qui est généralement répertoriée dans le coin supérieur droit.


1. Accédez à l’une des options suivantes :

* Étape : [https://stage.adminconsole.adobe.com/](https://stage.adminconsole.adobe.com/)
* Prod : [https://adminconsole.adobe.com/](https://adminconsole.adobe.com/)

1. Dans la section Utilisateurs , cliquez sur **Développeurs** > **Ajouter des développeurs**.

   ![Gérer les développeurs dans Admin Console](assets/manage-users-admin-console.png)

   >[!NOTE]
   >
   >Si vous ne voyez pas d’option pour gérer les développeurs, vous ne disposez pas d’un produit qui autorise l’accès en développement. Workfront ne fournit pas d’accès développeur, contrairement à AEM. Si vous ne le voyez pas, nous devrons trouver comment faire pour que Workfront soit inclus dans la liste des applications qui permettent aux développeurs.

1. Ajoutez l’e-mail de l’utilisateur. Il doit rechercher des utilisateurs existants qui ont déjà été ajoutés à partir d’Admin Console.

1. Ajoutez les produits nécessaires au profil de développeur, puis cliquez sur **Enregistrer**.

![Ajout d’un développeur](assets/add-developer.png)

## Obtenir l’accès à AppBuilder

Les entreprises doivent collaborer avec leurs gestionnaires de compte pour acheter AppBuilder. Le processus exact n’est pas compris, car nous n’avions pas besoin de le faire pour le PDC.

Si vous souhaitez tester l’intégration d’AppBuilder, vous pouvez demander une version d’essai gratuite pour votre organisation IMS ici :
[https://developer.adobe.com/app-builder/docs/overview/getting_access/#](https://developer.adobe.com/app-builder/docs/overview/getting_access/#)

J&#39;ai l&#39;impression que, même s&#39;il s&#39;agit d&#39;un essai gratuit de 30 jours, ils ne désactiveront pas le procès après cette période.

Si AppBuilder est correctement configuré, vous devriez voir « Créer un projet à partir d’un modèle » dans le cadre de la création d’un projet (qui est traité dans la section suivante).

## Créer un projet dans la console de développement

1. Cliquez sur **Créer un projet à partir d’un modèle**.

   >[!IMPORTANT]
   >
   >Si cette option n’apparaît pas, cela signifie que vous êtes mal configuré(e) dans l’Admin Console et que vous n’avez pas accès au catalogue de l’App Builder. Cette option s’affiche uniquement lorsque vous avez accès à AppBuilder.

   ![Créer un projet à partir d’un modèle](assets/create-from-template.png)

1. Sélectionnez **App Builder**.

1. Saisissez un **Titre du projet** et **Nom de l’application**. Les deux comportent des valeurs par défaut, mais il sera plus facile d’identifier le projet de votre choix ultérieurement si vous personnalisez la valeur.

   >[!NOTE]
   >
   >Il existe une option pour ajouter des espaces de travail supplémentaires à cette étape. Il nous a été suggéré de créer un espace de travail pour chaque développeur. Cela permet de séparer les secrets et les déploiements lors du fonctionnement des développeurs. Il est conseillé de nommer l’espace de travail par le nom du développeur qui l’utilise. L’interface de ligne de commande de l’AIO offre des options permettant de changer d’espace de travail. Nous en parlerons plus loin.


1. Laissez **Inclure le runtime** sélectionné.

1. Cliquer sur **Enregistrer**.

## Interface de ligne de commande d’Adobe IO (aio)

Adobe fournit une interface de ligne de commande open source qui peut être utilisée pour créer des applications App Builder. La documentation se trouve ici : [https://github.com/adobe/aio-cli](https://github.com/adobe/aio-cli) ainsi que les instructions Adobe App Builder [https://developer.adobe.com/app-builder/docs/getting_started/first_app/](https://developer.adobe.com/app-builder/docs/getting_started/first_app/).

1. Installation
   1. Pour installer l’outil (assurez-vous d’être sur le nœud v18), exécutez : `npm install -g @adobe/aio-cli `.

1. S’authentifier dans Terminal
   1. Lancez votre terminal et connectez-vous à l’AIO avec la commande : `aio login`.

1. Initialisation De L’Application
   1. Commencez à configurer votre application en exécutant : `aio app init example-app`.

1. Sélection de la configuration
   1. Sélectionnez ensuite votre organisation et votre projet dans les options fournies.\
      ![Sélectionner l’organisation](assets/select-org.png)
      ![Sélectionner un projet](assets/select-project.png)

1. Sélection et configuration de modèles
   1. Parcourez tous les modèles disponibles et choisissez le modèle **@adobe/aem-cf-editor-ui-ext-tpl** pour votre projet.

      ![Modèle de recherche](assets/search-template.png)
      ![Sélectionner le modèle](assets/select-template.png)

1. Définition De Votre Extension
   1. Nommez votre extension.
   1. Fournissez un résumé descriptif des fonctionnalités de votre extension.
   1. Sélectionnez un numéro de version initial pour commencer.
   1. Confirmez l’achèvement en sélectionnant **J’ai terminé**.

      ![Définir l’extension](assets/define-extension.png)

1. Accédez au dossier du projet
   1. Accéder au dossier src
   1. Renommez le dossier `aem-cf-editor-1` en `workfront-doc-details-1`.

1. Modifier les fichiers de configuration
   1. Ouvrez app.config.yaml.
   1. Mettez à jour la ligne de `aem/cf-editor/1` à `workfront/doc-details/1`.
   1. Ajustez le chemin d’inclusion de `src/aem-cf-editor-1/ext.config.yaml` à `src/workfront-doc-details-1/ext.config.yaml`.

1. Modifier le composant Enregistrement d’extension
   1. Ouvrez `src/workfront-doc-details-1/web-src/src/components/ExtensionRegistration.js`.
   1. Dans la section des méthodes , ajoutez un `secondaryNav` de fonction contenant un `getButtons` de fonction asynchrone.
   1. `getButtons` doit recevoir un objet avec la structure suivante :

      ```
          {
          docId: "String",  // Document ID
          docvId: "String", // Document version ID
          sharedContext: {
              hostname: "String",
              protocol: "String",
              auth: {
              imsOrgID: "String",    // Customer's IMS Org ID
              imsToken: "String",    // User's IMS token
              imsClientId: "String"
              }
          }
          }
      ```

1. Cette fonction renvoie un tableau d’objets de bouton qui apparaîtront dans la navigation :

   ```
       methods: {
       secondaryNav: {
           async getButtons({docId, docvId, sharedContext}) {
           return [
               { label: 'Registration', url: '/index.html' },
               { label: 'Review', url: '/index.html#review' }
           ];
           }
       }
       }
   ```

1. Configurer le routage de l&#39;application
   1. Ouvrez votre fichier App.js et configurez les itinéraires pour inclure les fonctionnalités nouvellement développées. Vous devrez configurer des itinéraires pour la vue par défaut et pour toutes les vues supplémentaires telles que la page de révision. Voici comment définir ces itinéraires :

      ```
          <Route index element={<ExtensionRegistration />} />
          <Route exact path="index.html" element={<ExtensionRegistration />} />
          <Route exact path="review" element={<Review />} />
      ```

1. Accéder aux détails du document
   1. Mettez en œuvre la fonction fournie `document.getDocumentDetails` dans votre application pour récupérer les détails essentiels des documents. Cette fonction récupère un objet contenant des `docId` et des `docvId`, ainsi qu’un objet `sharedContext` avec des détails d’`hostname`, de `protocol` et d’authentification. Assurez-vous que votre application gère correctement ces données.

1. Intégration de la récupération de données dans vos composants
   1. Ajoutez un nouveau composant au dossier de composants de votre application. Dans ce composant, établissez une connexion à Workfront pour récupérer les informations sur le document et les données d’authentification à l’aide de la connexion établie avec l’application hôte. Voici un exemple de la manière dont vous pouvez structurer votre composant pour gérer cette situation :

      ```
          import { useEffect, useState } from 'react';
          import { attach } from "@adobe/uix-guest";
          import { extensionId } from "./Constants";
      
          function Review() {
              const [conn, setConn] = useState();
      
              useEffect(() => {
              const iife = async () => {
                  // "attach" the guest application to the host. This creates a "tunnel" from the host app that allows data to be passed to the iframe running this app.
                  const connection = await attach({
                  id: extensionId,
                  });
                  setConn(connection);
              };
      
              iife();
              }, []);
      
              useEffect(() => {
                  if (conn) {
                      // Using the connection created above, grab the document details from the host tunnel.
                      conn?.host?.document?.getDocumentDetails().then(setDocDetails);
                      // Pull the auth tokens from the sharedContext (see host app for details)
                      setAuth(conn?.sharedContext?.get("auth"));
                      setHostname(conn?.sharedContext?.get("hostname"));
                      setProtocol(conn?.sharedContext?.get("protocol"));
                  }
              }, [conn]);
      
          return (<>Text</>);
          }
      
          export default Review;
      ```

## Configuration pour les projets AIO existants

1. Mettre à jour les fichiers de configuration
   1. Ouvrez `app.config.yaml`.
   1. Modifiez la configuration en mettant à jour la référence de `aem/cf-editor/1` à `workfront/doc-details/1`. Cet ajustement aligne les chemins d’accès aux fichiers sur la structure actuelle du projet.

1. Révision du composant Enregistrement d’extension
   1. Recherchez et ouvrez le fichier nommé `ExtensionRegistration.js`.
   1. Dans la section des méthodes , ajoutez un `secondaryNav` de fonction contenant un `getButtons` de fonction asynchrone.
   1. `getButtons` doit recevoir un objet avec la structure suivante :

      ```
          {
          docId: "String",  // Document ID
          docvId: "String", // Document version ID
          sharedContext: {
              hostname: "String",
              protocol: "String",
              auth: {
              imsOrgID: "String",    // Customer's IMS Org ID
              imsToken: "String",    // User's IMS token
              imsClientId: "String"
              }
          }
          }
      ```

1. Cette fonction renvoie un tableau d’objets de bouton qui apparaîtront dans la navigation :

   ```
       methods: {
       secondaryNav: {
           async getButtons({docId, docvId, sharedContext}) {
           return [
               { label: 'Registration', url: '/index.html' },
               { label: 'Review', url: '/index.html#review' }
           ];
           }
       }
       }
   ```

1. Configurer le routage de l&#39;application
   1. Ouvrez votre fichier `App.js` et configurez les itinéraires pour inclure les fonctionnalités nouvellement développées. Vous devrez configurer des itinéraires pour la vue par défaut et pour toutes les vues supplémentaires telles que la page de révision. Voici comment définir ces itinéraires :

      ```
          <Route index element={<ExtensionRegistration />} />
          <Route exact path="index.html" element={<ExtensionRegistration />} />
          <Route exact path="review" element={<Review />} />
      ```

1. Accéder aux détails du document
   1. Mettez en œuvre la fonction fournie `document.getDocumentDetails` dans votre application pour récupérer les détails essentiels des documents. Cette fonction récupère un objet contenant des `docId` et des `docvId`, ainsi qu’un objet `sharedContext` avec des détails d’`hostname`, de `protocol` et d’authentification. Assurez-vous que votre application gère correctement ces données.

1. Intégration de la récupération de données dans vos composants
   1. Ajoutez un nouveau composant au dossier de composants de votre application. Dans ce composant, établissez une connexion à Workfront pour récupérer les informations sur le document et les données d’authentification à l’aide de la connexion établie avec l’application hôte. Voici un exemple de la manière dont vous pouvez structurer votre composant pour gérer cette situation :

      ```
          import { useEffect, useState } from 'react';
          import { attach } from "@adobe/uix-guest";
          import { extensionId } from "./Constants";
      
          function Review() {
              const [conn, setConn] = useState();
      
              useEffect(() => {
              const iife = async () => {
                  // "attach" the guest application to the host. This creates a "tunnel" from the host app that allows data to be passed to the iframe running this app.
                  const connection = await attach({
                  id: extensionId,
                  });
                  setConn(connection);
              };
      
              iife();
              }, []);
      
              useEffect(() => {
                  if (conn) {
                      // Using the connection created above, grab the document details from the host tunnel.
                      conn?.host?.document?.getDocumentDetails().then(setDocDetails);
                      // Pull the auth tokens from the sharedContext (see host app for details)
                      setAuth(conn?.sharedContext?.get("auth"));
                      setHostname(conn?.sharedContext?.get("hostname"));
                      setProtocol(conn?.sharedContext?.get("protocol"));
                  }
              }, [conn]);
      
          return (<>Text</>);
          }
      
          export default Review;
      ```

## Publier des applications

>[!IMPORTANT]
>
>Assurez-vous que la bonne organisation IMS est sélectionnée pour chacune des étapes suivantes.

Pour qu’une application invitée soit chargée dans Workfront, elle doit être envoyée à l’espace de travail de production et soumise pour approbation.

1. Déployez l’application dans l’espace de travail de production.
   1. `aio app use -w Production `
   1. `aio app deploy `

1. Accédez à [https://developer-stage.adobe.com/](https://developer-stage.adobe.com/) ou [https://developer.adobe.com/](https://developer.adobe.com/).
   1. Cliquez sur **Console** dans le coin supérieur droit.

1. Recherchez le projet que vous avez utilisé pour créer l’application AppBuilder.

1. Sélectionnez le Workspace de production.
   ![Sélectionner l’espace de travail de production](assets/find-application.png)

1. Envoyez la demande pour examen privé (vous recevrez des avertissements indiquant que nous ne publions pas sur le marketplace d&#39;échange d&#39;applications, ce qui est correct).

1. Remplissez le formulaire (titre, description, icône et note au réviseur).
   ![Remplissez le formulaire pour une révision privée](assets/submission-details.png)

>[!IMPORTANT]
>
>Une fois la soumission effectuée, un administrateur système de l’organisation devra approuver la soumission.

## Valider l’envoi

1. En tant qu’administrateur système, accédez à [https://stage.exchange.adobe.com/](https://stage.exchange.adobe.com/) ou [https://exchange.adobe.com/](https://exchange.adobe.com/).

1. Cliquez sur **Gérer** > **Applications Experience Cloud**. Vous devriez voir les applications envoyées avec des options d’approbation/de rejet.
Une fois approuvées, les extensions d’application publiées doivent se charger automatiquement dans votre environnement Workfront.

   ![Envoi approuvé](assets/approve-submission.png)

## Aide supplémentaire

Adobe dispose d’une excellente documentation sur la prise en main de la création d’applications pour AppBuilder et leur déploiement.

Voici quelques liens utiles :

* [https://developer.adobe.com/app-builder/docs/getting_started/first_app/#4-bootstrapping-new-app-using-the-cli](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#4-bootstrapping-new-app-using-the-cli)

* [https://developer.adobe.com/uix/docs/guides/publication/](https://developer.adobe.com/uix/docs/guides/publication/)

* [https://developer.adobe.com/uix/docs/services/aem-cf-console-admin/extension-development/](https://developer.adobe.com/uix/docs/services/aem-cf-console-admin/extension-development/)

## Développement Local

Lors du développement de votre application App Builder pour Workfront, il se peut que vous ayez besoin de tester votre application dans Workfront sans la publier. Heureusement, nous avons une solution à ce problème.

Dans votre application App Builder, vous pouvez lancer des `aio app run` de développement local. Vous obtiendrez alors une URL, généralement de type `https://localhost:9080`. Vous pouvez également exécuter `aio app deploy` pour obtenir un domaine Adobe statique. Veillez à noter ces URL pour une utilisation ultérieure.

Accédez ensuite à la page de détails du document spécifique que vous souhaitez développer dans votre navigateur. Ouvrez les outils de développement et accédez au stockage local pour workfront.com ou workfront.adobe.com. Ici, vous devez ajouter une entrée. Utilisez `appBuilderDocDetailsOverride` comme clé et l’URL App Builder mentionnée précédemment comme valeur.

Lors du rechargement de votre page, les boutons de votre application App Builder s’affichent. Cliquez sur ces boutons pour afficher votre application en action.
