---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Générer des épreuves dans  [!DNL Workfront Proof]
description: Workfront Proof vous permet de créer des épreuves à partir de documents ou de sites web et de les partager avec d’autres personnes.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: de23513976d7bc4fe34cbf7b007a41c3b9797347
workflow-type: tm+mt
source-wordcount: '1889'
ht-degree: 53%

---

# Générer des épreuves dans [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] vous permet de créer des épreuves à partir de documents ou de sites web et de les partager avec d’autres personnes. Les étapes suivantes décrivent les différentes options de configuration disponibles :

## Générer une épreuve à partir d’un document

1. Effectuez l’une des opérations suivantes pour ouvrir la page **[!UICONTROL Nouvelle épreuve]** :

   * Cliquez sur le bouton **[!UICONTROL Nouvelle épreuve]** dans le coin supérieur gauche d’une page.
   * Envoyer via Zone de dépôt (fonctionnalité Entreprise).

1. Pour corriger un ou plusieurs documents, ajoutez les documents à corriger de l’une des manières suivantes (répétez cette procédure pour ajouter plusieurs documents) :

   * Faites glisser un document de votre système de fichiers dans la zone de glisser-déposer de la zone **[!UICONTROL Ajouter des fichiers]**.
   * Dans la zone **[!UICONTROL Ajouter des fichiers]**, cliquez sur le lien **parcourir** pour rechercher et sélectionner le document à charger à partir du système de fichiers de votre station de travail.

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Pour corriger un site web, saisissez l’URL du site web dans la zone **[!UICONTROL Ajouter des fichiers]**, puis appuyez sur **[!UICONTROL Entrée]**. Répétez cette étape pour ajouter plusieurs sites web à l’épreuve.

   Pour plus d’informations sur la relecture de sites web, voir [Générer une épreuve pour une URL](#generate-a-proof-for-a-url).

   ![Site web de l’épreuve](assets/proof-website-350x65.png)

1. (Facultatif) Modifiez les noms des fichiers chargés :

   1. Dans la liste des documents, passez la souris sur le nom du document à modifier, puis cliquez sur l’icône **[!UICONTROL Modifier]**.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. Dans le champ **[!UICONTROL Nom de l’épreuve]**, spécifiez un nouveau nom, puis cliquez sur **[!UICONTROL Terminé]**.

   1. (Facultatif) Pour supprimer des fichiers du téléchargement, passez la souris sur le document à supprimer dans la liste de documents, puis cliquez sur l’icône **[!UICONTROL Supprimer]**.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Facultatif) Activez l’option **[!UICONTROL Combiner tous les fichiers compatibles en une seule épreuve]**.

      **Lorsque cette option est activée :** tous les fichiers et sites web statiques sont disponibles dans une seule épreuve et vous pouvez charger jusqu’à 50 fichiers à la fois.

      >[!NOTE]
      >
      >Les fichiers interactifs, y compris les vidéos et les sites web interactifs, ne peuvent pas être combinés en une seule épreuve.

      **Lorsque cette option est désactivée :** tous les documents et sites web sont générés sous la forme d’épreuves individuelles et vous pouvez charger jusqu’à 20 fichiers à la fois.

      Pour combiner tous les fichiers et sites web chargés dans une seule épreuve :

      1. Activez l’option **[!UICONTROL Combiner tous les fichiers compatibles en une seule épreuve]**.
      1. Dans le champ **[!UICONTROL Nom de l’épreuve]**, saisissez un nouveau nom pour l’épreuve combinée.
      1. Dans la zone **[!UICONTROL Ajouter des fichiers]**, réorganisez les fichiers inclus en les faisant glisser dans l’ordre souhaité. L’ordre des fichiers correspond à l’ordre des pages de l’épreuve combinée. Pour plus d’informations sur la création d’épreuves combinées, voir [Créer une épreuve de plusieurs pages](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Facultatif) Si vous souhaitez utiliser un workflow automatisé qui comprend plusieurs étapes, sélectionnez l’une des options suivantes dans la section **[!UICONTROL Workflow]** :

   * **De base :** sélectionnez cette option pour désigner les utilisateurs et utilisatrices qui doivent avoir accès à l’épreuve immédiatement après sa création. Vous pouvez également partager l’épreuve avec plusieurs utilisateurs et utilisatrices.

     Pour plus d’informations sur le partage d’une épreuve, voir [ Partager une épreuve dans  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatisé :** sélectionnez cette option pour gérer la révision et l’approbation du contenu lorsque vous disposez de processus de révision complexes, ou si vous envoyez régulièrement du contenu à des groupes de personnes identiques. Avec un workflow automatisé, le BAT passe d’une étape à l’autre jusqu’à l’approbation finale. Les utilisateurs concernés sont avertis à tout moment qu&#39;ils doivent donner leur accord.

     Pour plus d’informations sur la création d’un workflow automatisé, voir [Configurer une épreuve avec un workflow automatisé dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Indiquez si vous souhaitez envoyer des notifications par e-mail et un message personnalisé aux utilisateurs et utilisatrices que vous avez sélectionnés à l’étape précédente :

   * **Informer les personnes destinataires de cette épreuve :** sélectionnez cette option pour envoyer une notification par e-mail aux utilisateurs et utilisatrices. Lorsque l’option **[!UICONTROL Partage de base]** est sélectionnée dans la section **[!UICONTROL Workflow]**, une notification par e-mail est envoyée lorsque l’épreuve est créée. Lorsque l’option **[!UICONTROL Workflow automatisé]** est sélectionnée dans la section **[!UICONTROL Workflow]**, une notification par e-mail est envoyée lorsque l’épreuve passe à l’étape du workflow automatisé auquel la personne est associée.

   * **Ajouter un message personnalisé :** sélectionnez cette option pour inclure un message personnalisé dans la notification. Vous pouvez spécifier un objet et un corps de message. Le corps du message peut inclure une mise en forme en texte enrichi (gras, puces et liens hypertexte).

1. Sélectionnez l’un des paramètres d’épreuve suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exiger une connexion. Cette épreuve ne peut pas être partagée avec d'autres utilisateurs</td> 
      <td> <p>Lorsque cette option est sélectionnée :</p> 
       <ul> 
        <li>Les utilisateurs ne peuvent pas se connecter à l’épreuve pour l’afficher, sauf s’ils y ont été ajoutés.</li> 
        <li>Les abonnements ne peuvent pas être activés.</li> 
       </ul> 
       <p>Cette option est désactivée par défaut.</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger que les décisions soient signées de manière électronique</td> 
      <td><p>Lorsque cette option est sélectionnée, les utilisateurs doivent spécifier leur nom d’utilisateur et leur mot de passe au moment de prendre une décision concernant une épreuve.</p>
      <p>Cette option est désactivée par défaut.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’épreuve lorsque toutes les décisions requises sont prises.</td> 
      <td> <p>Lorsque ce paramètre est activé, l’état de l’épreuve est verrouillé une fois toutes les décisions prises. L’état passe automatiquement de déverrouillé à verrouillé lorsque la dernière personne chargée de l’approbation prend sa décision.</p> 
      <p>Cette option est désactivée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser le téléchargement du fichier original</td> 
      <td> <p><strong></strong> Lorsque cette option est sélectionnée, les réviseurs et réviseuses peuvent télécharger le fichier original à partir duquel l’épreuve a été créée.</p> <p>Si cette option est désélectionnée, l’icône Télécharger n’est pas visible.</p>
      <p>Cette option est activée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">autoriser le partage de l'épreuve via une URL publique ou un code intégré</td> 
      <td><p>Lorsque cette option est sélectionnée, l’épreuve peut être partagée via une URL publique ou un code intégré.</p>
       <p>Cette option est activée par défaut.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser l’abonnement à l’épreuve par une URL publique ou un code intégré</td> 
      <td> <p>Lorsque cette option est sélectionnée, les personnes qui n’ont pas été ajoutées au BAT peuvent s’abonner au BAT. La personne qui s’abonne à l’épreuve se voit attribuer le rôle et l’adresse e-mail que vous définissez dans les paramètres suivants :</p> 
       <ul> 
        <li><strong>Rôle de personne abonnée</strong> : rôle d’épreuve par défaut attribué à tous les réviseurs et réviseuses qui s’abonnent à l’épreuve.</li> 
        <li><strong>Paramètres d’alerte par e-mail pour les personnes abonnées</strong> : alerte par défaut affectée à tous les réviseurs et réviseuses qui s’abonnent à l’épreuve.</li> 
        <li> <p><strong>Accès à l’épreuve via un lien par e-mail requis pour</strong> : indiquez si la personne abonnée reçoit un e-mail avec un lien vers l’épreuve. Vous pouvez sélectionner <strong>Aucun e-mail</strong> (le lien par e-mail n’est pas obligatoire pour accéder au BAT), <strong>E-mail de notification du BAT uniquement</strong> (l’abonné reçoit un lien vers le BAT par e-mail sans vérification) ou <strong>E-mails de validation et de notification du BAT</strong> (l’abonné reçoit un lien vers le BAT par e-mail et doit cliquer sur le lien pour accéder à un BAT. Cette option a pour but de s’assurer que la personne a saisi une adresse e-mail correcte (à laquelle elle a accès).</p> <p>Remarque : si un workflow automatisé est associé aux épreuves, tous les abonnements génèrent des e-mails de confirmation à l’attention du propriétaire de l’épreuve afin qu’il puisse décider à quelle étape la personne doit être ajoutée.</p> </li> 
       </ul> 
        <p>Cette option est désactivée par défaut.</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Créer une épreuve]**. Workfront génère un BAT des documents ou sites web sélectionnés.

   Le délai de chargement d’un document varie en fonction de la taille et du type de fichier. La génération des fichiers plus volumineux prendra plus de temps. Vous pouvez quitter la page pendant que Workfront continue à générer votre fichier. La taille maximale du chargement de fichier est de 4 Go.

## Générer une épreuve statique avec une URL {#generate-a-proof-for-a-url}

Vous pouvez générer une épreuve statique à l’aide d’une URL de site web.

>[!NOTE]
>
>Vous ne pouvez générer une épreuve interactive pour une URL que si votre environnement [!DNL Workfront] est intégré à un compte Premium [!DNL Workfront Proof]. Si vous ne pouvez pas utiliser la relecture comme indiqué dans cette section, contactez votre administrateur Workfront.

1. Effectuez l’une des opérations suivantes pour ouvrir la page **[!UICONTROL Nouvelle épreuve]** :

   * Cliquez sur le bouton **[!UICONTROL Nouvelle épreuve]** dans le coin supérieur gauche d’une page.
   * Envoyer via Zone de dépôt (fonctionnalité Entreprise).

1. Sur la page **Nouvelle épreuve**, saisissez l’URL du site web à partir duquel vous souhaitez créer une épreuve dans la zone **[!UICONTROL Ajouter des fichiers]**, puis appuyez sur **[!UICONTROL Entrée]** ou **[!UICONTROL Retour]** sur votre clavier.

1. (Facultatif) Répétez ce processus pour ajouter plusieurs sites web à l’épreuve.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Dans la zone **[!UICONTROL Ajouter des fichiers]**, cliquez sur l’icône **Modifier** située à droite de l’URL pour ouvrir les détails du BAT du site web.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Saisissez un **[!UICONTROL Nom de l’épreuve]**. Par défaut, le nom de l’épreuve est identique à l’URL du site.

1. Sélectionnez l’une des options suivantes **[!UICONTROL Gérer le contenu du site]** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Capturer une copie d’écran</td> 
      <td>Crée une épreuve d’une image statique de la page d’accueil de l’URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interactif</td> 
      <td> <p>Crée une épreuve qui permet aux personnes réviseuses de parcourir le site, d’afficher des images en HTML5, des éléments Flash, etc.</p> <p>Pour créer une épreuve interactive, le site web doit être hébergé avec un protocole sécurisé (https). En outre, les sites web qui ne peuvent pas être incorporés dans un iframe ne peuvent pas être générés en tant que BAT interactif (les restrictions d’incorporation d’iframe sont contrôlées par le site web que vous essayez d’incorporer).</p> <p>Une fois l’épreuve initiale créée, ce paramètre ne peut plus être modifié lors de la création de versions ultérieures.</p> <p>Pour plus d’informations sur la relecture interactive, voir <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Générer une épreuve pour le contenu interactif</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résolution de la copie d’écran</td> 
      <td> <p>(Cette option n’est pas disponible pour les épreuves interactives.) Vous pouvez ajuster la résolution dans laquelle votre contenu s’affiche ou sélectionner plusieurs résolutions.</p> <p>Cela permet de vérifier l’épreuve afin de voir comment le contenu apparaîtra sur différents appareils, en fonction des différentes tailles de téléphones, tablettes ou moniteurs.</p> <p>Si vous sélectionnez plusieurs résolutions, une épreuve distincte est créée pour chaque résolution sélectionnée.</p> <p>Lorsqu’une épreuve est commentée, la résolution d’écran actuelle s’affiche automatiquement dans le commentaire, afin d’informer les autres personnes de la résolution à laquelle le commentaire est associé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rechercher des sous-pages</td> 
      <td>(Cette option n’est pas disponible pour les épreuves interactives.) Sélectionnez cette option pour parcourir les pages du site web. Vous pouvez développer le site web jusqu’à 2 niveaux de profondeur à partir de la page principale. Passez la souris sur une page pour afficher l’URL de la page et sélectionnez uniquement les pages à corriger. Chaque page sélectionnée est créée par défaut en tant qu’épreuve individuelle. Vous pouvez également activer l’option <strong>Combiner tous les fichiers compatibles en un seul BAT</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Configurez toutes les options de relecture avancées, telles que le partage de l’épreuve, l’ajout d’un workflow automatisé ou la configuration des paramètres d’accès et d’abonnement. Pour plus d’informations sur ces options, consultez les articles suivants :

   * [Partager une épreuve dans  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configurer une épreuve avec un workflow automatisé dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Configurer les paramètres d’accès et d’abonnement d’une épreuve](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Cliquez sur **[!UICONTROL Terminé]**.

1. Cliquez sur **[!UICONTROL Créer une épreuve]**.

## Générer une épreuve pour le contenu interactif {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

Pour plus d’informations sur le contenu interactif, voir [Vue d’ensemble des épreuves de contenu interactif](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Ajouter du contenu interactif en tant qu’URL](#add-interactive-content-as-a-url)
* [Ajouter du contenu interactif en tant que fichier ZIP](#add-interactive-content-as-a-zip-file)

### Ajouter du contenu interactif en tant qu’URL {#add-interactive-content-as-a-url}

Pour plus d’informations sur l’ajout d’une épreuve d’URL interactive, voir [Générer une épreuve pour une URL](#generate-a-proof-for-a-url).

### Ajouter du contenu interactif en tant que fichier ZIP {#add-interactive-content-as-a-zip-file}

1. Préparez votre contenu en créant un fichier compressé ZIP.

   Pour plus d’informations sur les spécifications des fichiers groupés .zip, voir [Présentation des épreuves de contenu interactif](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Effectuez l’une des opérations suivantes pour ouvrir la page **[!UICONTROL Nouvelle épreuve]** :

   * Cliquez sur le bouton **[!UICONTROL Nouvelle épreuve]** dans le coin supérieur gauche d’une page.
   * Envoyer via Zone de dépôt (fonctionnalité Entreprise).

1. Sur la page **[!UICONTROL Nouvelle épreuve]**, effectuez un glisser-déposer de votre bundle .zip interactif dans la zone **[!UICONTROL Ajouter des fichiers]**.

1. (Facultatif) Configurez toutes les options de relecture avancées, telles que le partage de l’épreuve, l’ajout d’un workflow automatisé ou la configuration des paramètres d’accès et d’abonnement. Pour plus d’informations sur ces options, consultez les articles suivants :

   * [Partager une épreuve dans  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configurer les paramètres d’accès et d’abonnement d’une épreuve](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Cliquez sur **[!UICONTROL Créer une épreuve]**. Workfront génère un BAT du fichier zip.

   Le délai de chargement d’un document varie en fonction de la taille du fichier compressé. Vous pouvez quitter la page pendant que Workfront continue à générer votre fichier. La taille maximale du chargement de fichier est de 4 Go.
