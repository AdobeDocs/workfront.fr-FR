---
title: Création d’applications personnalisées pour Workfront avec Adobe App Builder
description: Les extensions d’interface d’utilisation de Workfront, optimisées par Adobe App Builder, permettent aux clientes et clients et aux partenaires de créer des expériences d’utilisation personnalisées.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ed75053-8199-474c-afb4-fa9bbd3750f8
source-git-commit: a4e715d5212c3c166ce6ed995b327eb2b7198123
workflow-type: tm+mt
source-wordcount: '1693'
ht-degree: 1%

---

# Création d’applications personnalisées pour Workfront avec Adobe App Builder

Les extensions d’interface utilisateur de Workfront, optimisées par Adobe App Builder, permettent aux clients et aux partenaires de créer des expériences utilisateur personnalisées. Ces outils améliorent l’efficacité, offrent des expériences connectées transparentes, améliorent considérablement la satisfaction des utilisateurs et aident les entreprises à réaliser leur vision unique.

Par exemple, sans les extensions de l’interface utilisateur de Workfront, un gestionnaire de projet peut avoir besoin de basculer entre Workfront et un système de suivi temporel distinct pour consigner les heures. Avec les extensions de l’interface utilisateur, le suivi du temps peut être intégré directement à l’expérience Workfront, ce qui simplifie les workflows et permet de gagner du temps. Vous pouvez également ajouter des composants personnalisés pour améliorer la convivialité, automatiser les tâches répétitives et améliorer la gestion de contenu grâce à des fonctionnalités telles que le balisage des métadonnées et les aperçus de contenu. Adobe App Builder offre également l’évolutivité et une gestion des identités (IMS) robuste, assurant ainsi une personnalisation sécurisée et efficace à n’importe quelle échelle.

Les extensions de l’interface utilisateur de Workfront offrent plusieurs avantages clés :

* Personnalisation précise : les interfaces logicielles standard ne répondent souvent pas à tous les besoins de l’entreprise. Les extensions d’interface utilisateur permettent aux développeurs de modifier et d’étendre l’interface utilisateur par défaut pour répondre à des besoins professionnels spécifiques.
* Intégration du système : les extensions d’interface utilisateur facilitent l’intégration d’autres systèmes en garantissant des workflows transparents et la cohérence des données.
* Évolutivité : au fur et à mesure que les entreprises se développent, des extensions d’interface utilisateur peuvent être développées pour ajouter de nouvelles fonctionnalités sans avoir besoin d’une refonte complète du système.
* Temps de développement réduit : les points d’extension et les outils préconfigurés réduisent considérablement le temps et les efforts nécessaires à l’implémentation de fonctionnalités personnalisées.
* Meilleure adoption par les utilisateurs : une expérience utilisateur optimisée peut considérablement stimuler l’adoption des logiciels. Les éléments d’interface utilisateur personnalisés conçus pour répondre aux préférences des utilisateurs peuvent améliorer les taux d’adoption et la satisfaction globale.
* Grâce aux extensions d’interface utilisateur de Workfront, les entreprises peuvent créer des expériences utilisateur personnalisées qui favorisent l’efficacité, l’intégration et la satisfaction des utilisateurs.

Une fois l’application créée dans Adobe App Builder, un administrateur ou une administratrice Workfront peut l’ajouter au menu principal de Workfront et au panneau de navigation de gauche à l’aide de modèles de disposition. Un utilisateur disposant du modèle de mise en page qui clique sur l’application verra l’application incorporée dans Workfront, au lieu de devoir l’ouvrir séparément.

Cet article décrit comment accéder à App Builder et utiliser un modèle pour créer une application.

Pour plus d’informations sur l’ajout d’une application personnalisée aux modèles de mise en page, voir [Personnaliser le menu principal à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) et [Personnaliser le panneau de gauche à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Conditions préalables

Vous devez disposer des éléments suivants :

* Un compte Workfront compatible IMS
* Une machine de développement avec le nœud v18 et npm
* Licence App Builder

## Accès à Adobe App Builder

Pour créer des extensions d’interface utilisateur, vous devez avoir accès à Adobe App Builder dans Adobe Developer Console.

Des instructions supplémentaires sont disponibles sur le site [Adobe Developer](https://developer.adobe.com/uix/docs/guides/get-access/).

### Ajout de développeurs au Adobe Admin Console

>[!IMPORTANT]
>
>Assurez-vous d’avoir sélectionné la bonne organisation IMS pour toutes les étapes suivantes. Si vous appartenez à plusieurs organisations, il est possible de sélectionner la mauvaise. Assurez-vous que vous agissez sous la bonne organisation, qui est généralement répertoriée dans le coin supérieur droit.

1. Accédez à Production : https://adminconsole.adobe.com/ .

1. Dans la section **Utilisateurs**, cliquez sur **Développeurs** > **Ajouter des développeurs**.

   ![ajout d’utilisateurs dans admin console](assets/manage-users-admin-console.png)

   >[!NOTE]
   >
   >Si vous ne voyez pas d’option permettant de gérer les développeurs, cela signifie que vous ne disposez pas d’un produit permettant aux développeurs d’y accéder.

1. Ajoutez l’e-mail de l’utilisateur. Il doit rechercher des utilisateurs existants qui ont déjà été ajoutés à partir d’Admin Console.

1. Ajoutez les produits nécessaires au profil de développeur et cliquez sur **Enregistrer**.\
   ![ajout de développeurs](assets/add-developer.png)

### Obtenir l’accès à App Builder

Les entreprises doivent collaborer avec leurs gestionnaires de compte pour acheter App Builder.

Si AppBuilder est correctement configuré, vous devriez voir Créer un projet à partir d’un modèle dans le cadre de la création d’un projet.

## Création d’un projet dans le Adobe Developer Console

Vous devez utiliser Adobe Developer Console pour créer votre extension d’interface utilisateur.

Des instructions supplémentaires sont disponibles sur le site [Adobe Developer](https://developer.adobe.com/uix/docs/guides/creating-project-in-dev-console/).

1. Connectez-vous au Adobe Developer Console à l’aide de votre Adobe ID.

1. Choisissez votre compte et votre profil ou organisation.

1. Cliquez sur **Créer un projet à partir d’un modèle** dans la zone Démarrage rapide, ou cliquez sur **Créer un projet > Projet à partir d’un modèle**.

   >[!IMPORTANT]
   >
   >Si vous ne voyez pas l’option permettant de créer un projet à partir d’un modèle, cela signifie que vous êtes mal configuré(e) dans l’Admin Console et que vous n’avez pas accès au catalogue de l’App Builder. Cette option s’affiche uniquement lorsque vous avez accès à AppBuilder.

   ![Créer à partir d’un modèle](assets/create-from-template.png)

1. Sélectionnez **App Builder**.

1. Saisissez un **Titre du projet** et **Nom de l’application**. Les deux comportent des valeurs par défaut, mais il sera plus facile d’identifier le projet souhaité ultérieurement si vous personnalisez la valeur.

1. Laissez **Inclure le runtime** sélectionné.

1. Cliquer sur **Enregistrer**.

## Utilisation de l’interface de ligne de commande d’Adobe IO (aio)

Adobe fournit une interface de ligne de commande open source que vous pouvez utiliser pour créer l’application App Builder.

Des instructions supplémentaires sont disponibles sur GitHub et sur le site d’Adobe Developer :

* https://github.com/adobe/aio-cli
* https://developer.adobe.com/app-builder/docs/getting_started/first_app/

1. Pour installer l’outil (assurez-vous d’être sur le nœud v18), exécutez : `npm install -g @adobe/aio-cli`.
1. Lancez votre terminal et connectez-vous à l’AIO avec la commande : `aio login`. Si vous rencontrez des problèmes lors de la connexion à l’organisation IMS appropriée, `aio login -f` à forcer une invite de connexion. Utilisez `aio where` pour voir quelle organisation vous êtes connecté à l’organisation IMS appropriée. pour plus d’informations, utilisez `aio config`.
1. Commencez à configurer votre application en exécutant : `aio app init example-app` à remplacer « example-app » par le nom de votre application. Si vous n’êtes pas sûr des noms d’application, vous pouvez voir une liste de noms d’application avec la commande `aio console project list`.
1. Sélectionnez votre organisation et votre projet dans les options fournies.
   ![résultat de la commande](assets/1-command-result.png)
   ![Sélectionner un projet](assets/2-select-a-project.png)

1. Parcourez tous les modèles disponibles et choisissez le **@adobe/workfront-ui-ext-tpl** pour votre projet.
   ![Choisir un modèle](assets/3-choose-template.png)
1. Sélectionnez et saisissez le nom du projet que vous avez créé dans le Adobe Developer Console.
   ![sélectionnez et saisissez le nom du projet](assets/4-select-and-enter-project-name.png)

1. Répondez aux invites de l&#39;application :

   * Nommez l’extension.
   * Fournissez un résumé descriptif des fonctionnalités de l’extension.
   * Sélectionnez un numéro de version initial pour commencer.
   * Le modèle crée le code d’un bouton de navigation principal si vous sélectionnez Ajouter un bouton personnalisé à l’élément de menu principal lorsque vous êtes invité à indiquer « Que souhaitez-vous faire ensuite ? ».

   ![sélectionnez terminé](assets/5-select-done.png)

1. Confirmez l’achèvement en sélectionnant J’ai terminé. La génération du code à partir du modèle est en cours.
   ![génération en cours](assets/6-generation-in-process.png)
1. Patientez jusqu’à ce qu’un message indiquant que l’initialisation de l’application est terminée s’affiche. Vous pouvez ensuite ouvrir le projet dans un IDE (Visual Studio Code est recommandé) et accéder au dossier src.

   Pour plus d’informations sur les dossiers et fichiers de votre projet, consultez le [site du développeur Adobe](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#5-anatomy-of-an-appbuilder-application).

## Création des extensions dans VSCode

La configuration du fichier App.js est requise pour activer la navigation via le menu principal de Workfront ou la navigation secondaire (panneau de gauche).

La configuration du fichier ExtensionRegistration.js est requise pour afficher les extensions dans les modèles de disposition Workfront.

Les exemples suivants vous montrent comment ajouter des applications personnalisées au menu principal de Workfront et au panneau de gauche d’un objet à l’aide des extensions de l’interface utilisateur.

### Configuration d’ExtensionRegistration.js

Pour autoriser les applications personnalisées dans le menu principal de Workfront :

1. Accédez à ExtensionRegistration.js.

Dans la fonction ExtensionRegistration, vous devriez voir le code suivant. Ce code a été créé pour vous par le modèle. Ce code peut être ajouté pour créer des éléments de menu supplémentaires. Veillez à remplacer les identifiants et les URL.

    «
    mainMenu: &lbrace;
    
    getItems() &lbrace;
    
    return &lbrack;
    
    &lbrace;
    
    id: &#39;main-menu-label&#39;,
    
    url: &#39;/index.html#/main-menu-label&#39;,
    
    label: &#39;Main menu label&#39;,
    
    icon: icon1,
    
    &rbrace;,
    
    &rbrack;;
    
    &rbrace;,
    
    &rbrace;
    «

1. Ajoutez le fragment de code suivant :
   ![](assets/7-extension-registration-step1-from-sam.png) de fragment de code
Cet exemple illustre un élément du menu principal. Vous devez mettre à jour l’identifiant, le libellé, l’icône et l’URL vers les noms corrects pour votre application. Lors de l’ajout de plusieurs éléments, assurez-vous que l’identifiant est unique.

1. Enregistrez votre travail.

### Autoriser les applications personnalisées dans la navigation du panneau de gauche de Workfront

Pour autoriser les applications personnalisées dans le volet de navigation de gauche de Workfront, procédez comme suit :

1. Accédez à ExtensionRegistration.js.
1. Dans la fonction ExtensionRegistration, ajoutez le fragment de code suivant :

   ```
   secondaryNav: {  
   
   TASK: {  
   
       getItems() {       return [         {           id: "TASK", 
   
   label: "My TASK",           icon: metricsIcon,           url: "/myTask",  
   
           },  
   
       ];  
   
       },  
   
   },  
   
   },  
   ```

   ![enregistrement de l’extension](assets/8-extension-registration-file-step2.png)

   * Cet exemple montre un élément de navigation du panneau de gauche appelé Ma tâche. Vous devez mettre à jour l’identifiant, le libellé, l’icône et l’URL vers les noms corrects pour votre application.

   * Cet exemple montre un élément de navigation du panneau de gauche pour le type d&#39;objet Projet. Vous devez créer ces éléments séparément pour chaque objet pour lequel ils sont pris en charge dans Workfront. Les objets suivants sont disponibles : projet, tâche, problème, portefeuille et programme.

1. Enregistrez votre travail.

### Configuration d’App.js

1. Accédez à App.js.

1. Le modèle fournit un itinéraire pour une option de menu principal. Un itinéraire définit le mappage entre les chemins d’URL et les composants rendus pour ces chemins. Pour ajouter un itinéraire, utilisez le fragment de code suivant, veillez à remplacer le chemin et l’élément exacts par les vôtres.

   ```
       <Route 
   
               exact path="custom-application" 
   
               element={<Customapplication />} 
   
           /> 
   ```

   ![ exemple de code ](assets/9-app-file-step-1-from-sam.png)
1. Enregistrez votre travail.

Pour plus d’informations sur le développement et l’exécution de l’application, consultez le [site du développeur Adobe](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#6developing-the-application).

## Contexte partagé

Le contexte partagé est utilisé pour partager des données de Workfront vers une extension d’interface utilisateur. Les données disponibles via le contexte partagé comprennent les données utilisateur et le contexte de l’application.


### l’utilisateur ou de l’utilisatrice

Les extensions d’interface utilisateur de Workfront partagent des données utilisateur. L’objet utilisateur disponible via le contexte partagé comprend un ID utilisateur Workfront et l’adresse électronique de l’utilisateur.

`user = (conn?.sharedContext?.get("user")); // {ID: '1', email: 'test@aaa.com'} userID = user.ID userEmail = user.email `

### Contexte applicatif

Lors de l’ajout d’une application personnalisée à l’aide d’un point d’extension de navigation Secondaire, il est courant que l’application personnalisée utilise des données contextuelles comme un identifiant de projet ou de document. Pour ces données, le contexte partagé comprend un code objet et un ID objet.

Voici un exemple d&#39;obtention du contexte applicatif pour les documents :

`context = conn?.sharedContext; // Using the connection created above, grab the document details from the host tunnel. // conn?.host?.document?.getDocumentDetails().then(setDocDetails); `

## Tester l’application dans Workfront

Lors du développement de votre application App Builder pour Workfront, vous devrez peut-être tester votre application dans Workfront sans la publier.

Dans votre application App Builder, vous pouvez lancer des `aio app run` de développement local. Vous obtiendrez alors une URL, généralement de type `https://localhost:9080`. Vous pouvez également exécuter `aio app deploy` pour obtenir un domaine Adobe statique. Veillez à noter ces URL pour une utilisation ultérieure.

Ensuite, accédez à la page spécifique sur laquelle vous souhaitez développer dans votre navigateur. Ouvrez les outils de développement et accédez au stockage local pour workfront.com ou workfront.adobe.com. Ici, vous devez ajouter une entrée. Utilisez `extensionOverride` comme clé et l’URL App Builder mentionnée précédemment comme valeur.

Si la configuration a été correctement effectuée, les boutons de votre application App Builder s’affichent lorsque vous rechargez la page du modèle de mise en page dans Workfront. Ajoutez les boutons d’application au menu principal et au panneau de gauche d’un objet et vérifiez qu’ils s’affichent correctement dans ces zones.

Des instructions supplémentaires sont disponibles sur le site du développeur d’Adobe, à l’aide d’un exemple d’AEM : https://developer.adobe.com/uix/docs/guides/preview-extension-locally/

## Publier les demandes et approuver l&#39;envoi

Pour publier la demande et l&#39;approuver, suivez les instructions figurant sur le site du développeur d&#39;Adobe [&#128279;](https://developer.adobe.com/uix/docs/guides/publication/).
