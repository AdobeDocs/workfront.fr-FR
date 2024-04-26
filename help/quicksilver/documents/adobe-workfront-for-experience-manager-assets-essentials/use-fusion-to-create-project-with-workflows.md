---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilisation de Workfront Fusion pour créer un projet Workfront contenant des workflows Adobe Experience Manager
description: Si vous créez un projet via Workfront Fusion et que vous souhaitez inclure des processus Adobe Experience Manager sur le projet, vous devez utiliser une configuration de module Fusion spécifique, décrite dans cet article.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 1677ed676a5ccb4f519cc81bf3b31cc90b8326b4
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 2%

---

# Utilisation de Workfront Fusion pour convertir un problème Workfront en projet qui comprend des workflows Adobe Experience Manager

Si vous créez un projet via Workfront Fusion et que vous souhaitez inclure des processus Adobe Experience Manager sur le projet, vous devez utiliser une configuration de module Fusion spécifique, décrite dans cet article.

>[!NOTE]
>
>Les workflows sont disponibles uniquement dans une intégration Adobe Experience Manager as a Cloud Service. Ils ne sont pas disponibles dans les intégrations avec Adobe Experience Manager Assets Essentials.


## Conditions d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>Formule Adobe Workfront*</strong>
   </td>
   <td>N’importe quelle
   </td>
  </tr>
  <tr>
   <td><strong>Licences Adobe Workfront*</strong>
   </td>
   <td>Requête ou supérieure
   </td>
  </tr>
  <tr>
   <td><strong>Produit</strong>
   </td>
   <td><b>Adobe Experience Manager<b>:
   <ul>
   <li>
   <p>Vous devez disposer d’Experience Manager Assets as a Cloud Service ou d’Assets Essentials, et vous devez être ajouté au produit en tant qu’utilisateur dans le Admin Console.</p>
   </li
   ><li>
   <p>Vous devez disposer d’un accès en écriture au référentiel dans Adobe Experience Manager.</p>
   </li>
   </ul>
  <b>Workfront Fusion</b>:<p>Nouveau :</p>
   <ul>
   <li>
   <p>Sélectionnez ou forfait Workfront Prime : votre entreprise doit acheter Adobe Workfront Fusion.</p>
   </li>
   <li> 
   <p>Formule Workfront ultime : Workfront Fusion est incluse.</p>
   </li>
   </ul>
   <p>Ou</p>
   <p>Actuel : votre entreprise doit acheter Adobe Workfront Fusion.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Paramétrages du niveau d'accès*</strong>
   </td>
   <td>Modifier l’accès aux documents
<p>
<strong>Remarque : </strong>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <strong>Créer ou modifier les niveaux d’accès personnalisés</strong>.
   </td>
  </tr>
</table>

## Conditions préalables

Avant de commencer,

* Votre administrateur Workfront doit configurer des workflows dans une intégration Adobe Experience Manager. Pour plus d’informations, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* Un modèle de projet doit être configuré avec un workflow de dossier lié à l’intégration Adobe Experience Manager.
* Vous devez avoir créé une application OAuth dans Workfront pour configurer la connexion pour ce module.

  Pour obtenir des instructions, voir [Création d’une application OAuth](#create-an-oauth-application) dans cet article.

## Configuration des modules

Dans Workfront Fusion, si vous souhaitez créer un projet qui comprend des workflows Adobe Experience Manager, vous devez utiliser le module Workfront > Divers événements.

1. Ajoutez la variable **Workfront** > **Diverses actions** à votre scénario.
1. Dans le **Connexion** , sélectionnez la connexion Workfront qui se connecte au compte que ce module utilisera.

   Pour plus d’informations sur la création d’une connexion, voir [Connexion [!DNL Workfront] to [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) dans l’article Modules Workfront .

   Pour plus d’informations sur la création de l’ID client et du secret client, vous devez créer une connexion, voir [Création d’une application OAuth](#create-an-oauth-application) dans cet article.

1. Dans le **Type d’enregistrement** champ, sélectionnez `Issue`.
1. Dans le **Action** champ, sélectionnez `convertToProject`.
1. Dans le **ID** , saisissez ou mappez l’identifiant du problème que vous convertissez en projet.
1. Activer **Afficher les paramètres avancés**.
1. Faites défiler l’écran jusqu’au bas du module et recherchez la variable **Projet (collection avancée)** champ .
1. Collez le texte suivant dans le **Projet (collection avancée)** champ .

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Remplacer `Folder tree ID here` avec les ID de dossier.

   Pour localiser les ID d’arborescence de dossiers, voir [Localisation des identifiants d’arborescence de dossiers](#locate-folder-tree-ids) dans cet article.

   Pour utiliser plusieurs arborescences de dossiers, séparez les identifiants par une virgule :

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Remplacer `New project name here` avec le nom du nouveau projet.
1. Remplacer `Template ID here` avec l’identifiant du modèle que vous utilisez pour le nouveau projet.

   Vous pouvez mapper l’identifiant du modèle à partir d’un module précédent (tel qu’un module Workfront > Recherche) ou le localiser dans l’URL de la page du modèle dans Workfront.

1. Cliquez sur **OK** pour enregistrer la configuration du module.

## Localisation des identifiants d’arborescence de dossiers

Pour localiser les ID d’arborescence de dossiers :

>[!NOTE]
>
>Ces instructions utilisent le navigateur Chrome.

1. Dans Workfront, ouvrez le modèle que vous souhaitez utiliser pour ce projet. Ce modèle doit inclure la configuration Adobe Experience Manager que vous souhaitez utiliser pour le projet.
1. Ouvrez les outils de développement de votre navigateur.
1. Ouvrez le **Réseau** dans les outils de développement.
1. Dans le **Filtrer** zone, saisissez `object-workflow`.
1. Dans la colonne Nom , cliquez sur l’ID alphanumérique qui s’affiche.

   ![Localisation de l’ID de dossier 1](assets/finding-folder-id-1.png)

1. Cliquez sur le bouton **Aperçu** à droite de l’ID alphanumérique.
1. Ouvrez les sections réduites suivantes :
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Chaque arborescence de dossiers est représentée par un nombre. 0 (zéro) représente le premier dossier de la liste, 1 le second, etc. Si le modèle n’inclut qu’une seule arborescence de dossiers, il est égal à 0.

1. Ouvrez l’arborescence de dossiers que vous souhaitez utiliser pour le nouveau projet. Prenez note de la `_id` valeur du champ. Si vous souhaitez utiliser plusieurs arborescences de dossiers, notez toutes les `_id` valeurs de champ pour les arborescences de dossiers que vous souhaitez utiliser.

   ![Localisation de l’ID de dossier 2](assets/finding-folder-id-2.png)

   Voici les `aemNativeFolderTreeIDs`  valeurs que vous devez entrer dans la variable **Projet (collection avancée)** dans le champ **Workfront** > **Actions diverses** Module de fusion.

## Création d’une application OAuth

Vous devez configurer une application OAuth dans Workfront pour la connexion de ce module. Vous ne devez le faire qu’une seule fois pour une connexion Workfront donnée dans Fusion.

1. Dans Workfront, commencez à créer une application OAuth, comme décrit dans la section [Création d’une application OAuth2 à l’aide des informations d’identification de l’utilisateur (flux de code d’autorisation)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) dans l’article Créer des applications OAuth2 pour [!DNL Workfront] intégrations.
1. Copiez l’identifiant du client et le secret du client vers un emplacement sécurisé.
1. Dans le **URI de redirection** , saisissez ce qui suit :

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Cliquer sur **Enregistrer**.

Vous utiliserez cet identifiant client et ce secret client lors de la configuration de la connexion du module dans Fusion.

Pour plus d’informations sur la création d’une connexion, voir [Connexion [!DNL Workfront] to [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) dans l’article Modules Workfront .

