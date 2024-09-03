---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Générer des épreuves dans  [!DNL Workfront Proof]
description: Workfront Proof vous permet de créer des épreuves à partir de documents ou de sites web et de les partager avec d’autres personnes.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '2253'
ht-degree: 100%

---

# Générer des épreuves dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] vous permet de créer des épreuves à partir de documents ou de sites web et de les partager avec d’autres personnes. Les étapes suivantes décrivent les différentes options de configuration disponibles :

## Générer une épreuve pour un document

1. Effectuez l’une des opérations suivantes pour commencer à créer une épreuve et afficher la page [!UICONTROL Nouvelle épreuve] :

   * Cliquez sur le bouton vert **[!UICONTROL Nouvelle épreuve]** dans le coin supérieur gauche d’une page.
   * Dans la zone **[!UICONTROL Tableau de bord]**, dans l’onglet **[!UICONTROL Vue d’ensemble]**, cliquez sur le lien **[!UICONTROL Nouvelle épreuve]**.

   * Envoyer via Zone de dépôt (fonctionnalité Entreprise).
   * La page **[!UICONTROL Nouvelle épreuve]** s’affiche.

1. Pour relire un ou plusieurs documents, ajoutez les documents à relire de l’une des façons suivantes (répétez cette procédure pour ajouter plusieurs documents à relire) :

   * Faites glisser un document de votre système de fichiers vers la zone de glisser-déposer dans la zone **[!UICONTROL Ajouter des fichiers]**.
   * Cliquez dans la zone de glisser-déposer de la zone **[!UICONTROL Ajouter des fichiers]**, puis naviguez pour rechercher et sélectionner le document à charger que vous souhaitez charger du système de fichiers sur votre poste de travail.

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Pour relire un ou plusieurs sites web, spécifiez l’URL du site web que vous souhaitez relire dans la zone **[!UICONTROL Ajouter des fichiers]**, puis appuyez sur **[!UICONTROL Entrée]**.

1. (Facultatif) Répétez cette procédure pour ajouter plusieurs sites web à relire.

   Pour plus d’informations sur la relecture de sites web, voir [Générer une épreuve pour une URL](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. (Facultatif) Modifiez les noms des fichiers chargés :

   1. Placez le pointeur de la souris sur le nom du document que vous souhaitez modifier dans la liste des documents de la zone **[!UICONTROL Ajouter des fichiers]**, puis cliquez sur l’icône **[!UICONTROL Modifier]**.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. Dans le champ **[!UICONTROL Nom de l’épreuve]**, spécifiez un nouveau nom, puis cliquez sur **[!UICONTROL Terminé]**.

   1. (Facultatif) Pour supprimer des fichiers du chargement, placez le pointeur de la souris sur le document que vous souhaitez supprimer dans la liste des documents de la zone **[!UICONTROL Ajouter des fichiers]**, puis cliquez sur l’icône **[!UICONTROL Supprimer]**.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Facultatif) Activez l’option **[!UICONTROL Combiner tous les fichiers compatibles dans une seule épreuve]**.

      **Lorsque cette option est activée :** tous les fichiers et sites web statiques sont disponibles dans une seule épreuve et vous pouvez charger jusqu’à 50 fichiers à la fois.

      >[!NOTE]
      >
      >Les fichiers interactifs, y compris les vidéos et les sites web interactifs, ne peuvent pas être combinés en une seule épreuve.

      **Lorsque cette option est désactivée :** tous les documents et sites web sont générés sous la forme d’épreuves individuelles et vous pouvez charger jusqu’à 20 fichiers à la fois.

      Pour combiner tous les fichiers et sites web chargés dans une seule épreuve :

      1. Activez l’option **[!UICONTROL Combiner tous les fichiers compatibles dans une seule épreuve]**.
      1. Dans le champ **[!UICONTROL Nom de l’épreuve]**, spécifiez un nouveau nom pour l’épreuve combinée.
      1. Dans la zone **[!UICONTROL Ajouter des fichiers]**, réorganisez les fichiers inclus en les faisant glisser dans l’ordre souhaité. L’ordre des fichiers correspond à l’ordre des pages de l’épreuve combinée. Pour plus d’informations sur la création d’épreuves combinées, voir [Créer une épreuve de plusieurs pages](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Facultatif) Si vous souhaitez utiliser un workflow automatisé qui comprend plusieurs étapes, sélectionnez l’une des options suivantes dans la section **[!UICONTROL Workflow]** :

   * **De base :** sélectionnez cette option pour désigner les utilisateurs et utilisatrices qui doivent avoir accès à l’épreuve immédiatement après sa création. Vous pouvez également partager l’épreuve avec plusieurs utilisateurs et utilisatrices.

     Pour plus d’informations sur le partage d’une épreuve, voir « Ajouter des utilisateurs et utilisatrices à une épreuve » dans [Partager une épreuve dans  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatisé :** sélectionnez cette option pour gérer la révision et l’approbation du contenu lorsque vous disposez de processus de révision complexes, ou si vous envoyez régulièrement du contenu à des groupes de personnes identiques. Avec le workflow automatisé, l’épreuve passe d’une étape à l’autre jusqu’à l’approbation finale. Les utilisateurs et utilisatrices concernés sont avertis lorsqu’ils sont tenus d’effectuer une approbation.

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
      <td role="rowheader">Connexion requise : l’épreuve ne peut être partagée qu’avec d’autres utilisateurs et utilisatrices.</td> 
      <td> <p><strong>Connexion requise : l’épreuve ne peut être partagée qu’avec d’autres utilisateurs et utilisatrices :</strong> lorsque cette option est sélectionnée, uniquement les utilisateurs et utilisatrices de [!DNL Workfront Proof] peuvent afficher l’épreuve.</p> <p>Cette option est désactivée par défaut ; toute personne disposant de l’URL peut afficher l’épreuve.</p> <p>Lorsque cette option est sélectionnée :</p> 
       <ul> 
        <li>Les utilisateurs et utilisatrices ne peuvent pas se connecter à l’épreuve à moins qu’ils n’aient été ajoutés à l’épreuve.</li> 
        <li>Les abonnements ne peuvent pas être activés.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Une seule décision requise pour cette épreuve</td> 
      <td> <p>Lorsque cette option est sélectionnée, la révision est terminée une fois que l’une des personnes décisionnaires a pris sa décision.</p> <p>Cette option est désactivée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger que les décisions soient signées de manière électronique</td> 
      <td>Les utilisateurs et utilisatrices doivent indiquer leur nom d’utilisateur ou d’utilisatrice et leur mot de passe au moment où ils prennent une décision sur une épreuve.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’épreuve lorsque toutes les décisions requises sont prises.</td> 
      <td> <p><strong></strong>Lorsque ce paramètre est activé, l’état de l’épreuve est verrouillé une fois que toutes les décisions sont prises. L’état passe automatiquement de déverrouillé à verrouillé lorsque la dernière personne chargée de l’approbation prend sa décision.</p> <p>Cette option est désactivée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Télécharger le fichier original</td> 
      <td> <p><strong></strong> Lorsque cette option est sélectionnée, les réviseurs et réviseuses peuvent télécharger le fichier original à partir duquel l’épreuve a été créée.</p> <p>Si cette option est désélectionnée, l’icône Télécharger n’est pas visible.<br>Cette option est activée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partager l’épreuve via une URL publique ou un code intégré</td> 
      <td>Lorsque cette option est sélectionnée, l’épreuve peut être partagée via une URL publique ou un code intégré.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">S’abonner à l’épreuve via une URL publique ou un code intégré</td> 
      <td> <p>Lorsque cette option est sélectionnée, les personnes qui n’ont pas été explicitement ajoutées à l’épreuve peuvent s’y abonner. La personne qui s’abonne à l’épreuve se voit attribuer le rôle et l’adresse e-mail que vous définissez dans les paramètres suivants :</p> 
       <ul> 
        <li><strong>Rôle de personne abonnée</strong> : rôle d’épreuve par défaut attribué à tous les réviseurs et réviseuses qui s’abonnent à l’épreuve.</li> 
        <li><strong>Paramètres d’alerte par e-mail pour les personnes abonnées</strong> : alerte par défaut affectée à tous les réviseurs et réviseuses qui s’abonnent à l’épreuve.</li> 
        <li> <p><strong>Accès à l’épreuve via un lien par e-mail requis pour</strong> : indiquez si la personne abonnée reçoit un e-mail avec un lien vers l’épreuve. Vous pouvez sélectionner <strong>Aucun e-mail</strong> (aucun lien par e-mail n’est nécessaire pour accéder à l’épreuve), <strong>E-mail de notification d’épreuve uniquement</strong> (la personne abonnée reçoit un lien vers l’épreuve par e-mail sans vérification), ou <strong>E-mails de validation et de notification d’épreuve</strong> (la personne abonnée reçoit un lien vers l’épreuve par e-mail et doit cliquer sur le lien pour accéder à une épreuve ; l’objectif de cette option est de s’assurer que la personne a saisi une adresse e-mail correcte à laquelle elle a accès).</p> <p>Remarque : si le workflow automatisé est joint aux épreuves, tous les abonnements génèrent des e-mails de confirmation à la personne propriétaire de l’épreuve, afin qu’elle puisse décider à quelle étape la personne doit être ajoutée.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Créer une épreuve]**.

   Workfront commence à générer une épreuve des documents ou des sites web sélectionnés. Selon la taille et le type du fichier, le délai de chargement d’un document varie. Faites preuve de patience, car la génération de fichiers volumineux prend plus de temps. Vous pouvez quitter la page. Workfront continue à générer votre fichier. La taille maximale du chargement de fichier est de 4 Go.

   Une fois l’épreuve générée, cliquez sur **[!UICONTROL Accéder à l’épreuve]** pour lancer l’outil de relecture.

   ![Screenshot_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   Le document apparaît dans l’outil de relecture.

   Les utilisateurs et utilisatrices qui n’ont pas la relecture activée sur leur compte peuvent toujours afficher le document et ajouter des commentaires à l’épreuve.

## Générer l’épreuve d’une URL {#generate-a-proof-for-a-url}

Vous pouvez générer l’épreuve d’une URL pour la première fois. Vous pouvez également générer une nouvelle version de l’épreuve d’une URL si une épreuve a déjà été générée.

>[!NOTE]
>
>Vous ne pouvez générer une épreuve interactive pour une URL que si votre environnement [!DNL Workfront] est intégré à un compte Premium [!DNL Workfront Proof]. Si vous ne pouvez pas utiliser la relecture comme décrit dans cette section, contactez votre administrateur ou administratrice système.

Pour générer l’épreuve d’une URL :

1. Effectuez l’une des opérations suivantes pour commencer à créer une épreuve et afficher la page [!UICONTROL Nouvelle épreuve] :

   * Cliquez sur le bouton vert **[!UICONTROL Nouvelle épreuve]** dans le coin supérieur gauche d’une page.
   * Dans la zone **[!UICONTROL Tableau de bord]**, dans l’onglet **[!UICONTROL Vue d’ensemble]**, cliquez sur le lien **[!UICONTROL Nouvelle épreuve]**.

   * Envoyer via Zone de dépôt (fonctionnalité Entreprise).

1. (Le cas échéant) Sur la page **[!UICONTROL Nouvelle épreuve]** qui s’affiche, pour créer une nouvelle version d’épreuve existante, procédez comme suit :

   1. Sélectionnez l’épreuve de l’URL où ajouter une nouvelle version.
   1. Cliquez sur le bouton **[!UICONTROL Nouvelle version]** en haut de la page.

      ![Screenshot_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. Dans la page Nouvelle version de l’épreuve qui s’affiche, spécifiez l’URL du site web à tester comme épreuve dans la zone **[!UICONTROL Ajouter des fichiers]**, puis appuyez sur **[!UICONTROL Entrée]**.

1. (Facultatif) Répétez cette procédure pour ajouter plusieurs sites web à relire.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Cliquez sur le site web dans la liste des documents de la zone **[!UICONTROL Ajouter des fichiers]**.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Spécifiez un **[!UICONTROL Nom de l’épreuve]** pour l’épreuve.

   Par défaut, le nom de l’épreuve est identique à l’URL du site.

1. Sélectionnez les options **[!UICONTROL Gérer le contenu du site]** :

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
      <td> <p>Crée une épreuve qui permet aux personnes réviseuses de parcourir le site, d’afficher des images en HTML5, des éléments Flash, etc.</p> <p>Pour créer une épreuve interactive, le site web doit être hébergé avec un protocole sécurisé (https). En outre, les sites web qui ne peuvent pas être incorporés dans un iframe ne peuvent pas être générés en tant qu’épreuve interactive (les restrictions d’intégration d’iframe sont contrôlées par le site web que vous tentez d’incorporer).</p> <p>Une fois l’épreuve initiale créée, ce paramètre ne peut plus être modifié lors de la création de versions ultérieures.</p> <p>Pour plus d’informations sur la relecture interactive, voir <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Générer une épreuve pour le contenu interactif</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résolution de la copie d’écran</td> 
      <td> <p>(Cette option n’est pas disponible pour les épreuves interactives.) Vous pouvez ajuster la résolution de votre contenu ou sélectionner plusieurs résolutions.</p> <p>Cela permet de vérifier l’épreuve afin de voir comment le contenu apparaîtra sur différents appareils, en fonction des différentes tailles de téléphones, tablettes ou moniteurs.</p> <p>Si vous sélectionnez plusieurs résolutions, une épreuve distincte est créée pour chaque résolution sélectionnée.</p> <p>Lorsqu’une épreuve est commentée, la résolution d’écran actuelle s’affiche automatiquement dans le commentaire, afin d’informer les autres personnes de la résolution à laquelle le commentaire est associé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rechercher des sous-pages</td> 
      <td>(Cette option n’est pas disponible pour les épreuves interactives.) Sélectionnez cette option pour parcourir les pages du site web. Vous pouvez développer le site web jusqu’à 2 niveaux de profondeur à partir de la page principale. Passez le pointeur sur une page pour en afficher l’URL. Sélectionnez uniquement les pages à relire. Chaque page sélectionnée est créée par défaut en tant qu’épreuve individuelle. Vous pouvez également activer la fonction <strong>Combiner en une seule épreuve</strong> pour combiner toutes les pages sélectionnées en une seule épreuve.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Configurez toutes les options de relecture avancées, telles que le partage de l’épreuve, l’ajout d’un workflow automatisé ou la configuration des paramètres d’accès et d’abonnement. Pour plus d’informations sur ces options, consultez les articles suivants :

   * [Partager une épreuve dans  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configurer une épreuve avec un workflow automatisé dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Configurer les paramètres d’accès et d’abonnement d’une épreuve](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Cliquez sur **[!UICONTROL Terminé]**.

   Si vous ajoutez une nouvelle version à une épreuve d’URL existante, toutes les options configurées sur l’épreuve d’origine ou la version précédente sont conservées dans cette version.

1. Cliquez sur **[!UICONTROL Créer une épreuve]**.

## Générer une épreuve pour le contenu interactif {#generate-a-proof-for-interactive-content}

Pour utiliser cette fonctionnalité, vous devez disposer d’un plan Pro Workfront ou supérieur. Pour plus d’informations sur les différents plans disponibles, voir [Plans Workfront](https://www.workfront.com/plans?lang=fr).

Pour plus d’informations sur le contenu interactif, voir [Vue d’ensemble des épreuves de contenu interactif](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Ajouter du contenu interactif en tant qu’URL](#add-interactive-content-as-a-url)
* [Ajouter du contenu interactif en tant que fichier ZIP](#add-interactive-content-as-a-zip-file)

### Ajouter du contenu interactif en tant qu’URL {#add-interactive-content-as-a-url}

Pour plus d’informations sur l’ajout d’une épreuve d’URL interactive, voir [Générer l’épreuve d’une URL](#generate-a-proof-for-a-url).

### Ajouter du contenu interactif en tant que fichier ZIP {#add-interactive-content-as-a-zip-file}

1. Préparez votre contenu en créant un fichier compressé ZIP.

   Pour plus d’informations sur les spécifications des fichiers compressés ZIP, voir [À propos de la préparation de contenu interactif dans un fichier ZIP pour la relecture](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) dans l’article [Vue d’ensemble des épreuves de contenu interactif](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Effectuez l’une des opérations suivantes pour commencer à créer une épreuve et afficher la page [!UICONTROL Nouvelle épreuve] :

   * Cliquez sur le bouton vert **[!UICONTROL Nouvelle épreuve]** dans le coin supérieur gauche d’une page.
   * Dans la zone **[!UICONTROL Tableau de bord]**, dans l’onglet **[!UICONTROL Vue d’ensemble]**, cliquez sur le lien **[!UICONTROL Nouvelle épreuve]**.

   * Envoyer via Zone de dépôt (fonctionnalité Entreprise).

1. Sur la page **[!UICONTROL Nouvelle épreuve]** qui s’affiche, faites glisser et déposez votre fichier compressé ZIP interactif dans la zone **[!UICONTROL Ajouter des fichiers]**.

1. (Facultatif) Configurez toutes les options de relecture avancées, telles que le partage de l’épreuve, l’ajout d’un workflow automatisé ou la configuration des paramètres d’accès et d’abonnement. Pour plus d’informations sur ces options, consultez les articles suivants :

   * [Partager une épreuve dans  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * dans l’article
   * [Configurer les paramètres d’accès et d’abonnement d’une épreuve](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Cliquez sur **[!UICONTROL Créer une épreuve]**.

   Workfront commence à générer une épreuve du fichier ZIP. Le délai de chargement du fichier compressé varie en fonction de sa taille. La génération de fichiers volumineux prend plus de temps. Vous pouvez quitter la page. Workfront continue à générer votre fichier. La taille maximale du chargement de fichier est de 4 Go.

   Une fois l’épreuve générée, vous pouvez cliquer sur le bouton **[!UICONTROL Accéder à l’épreuve]** qui apparaît pour l’ouvrir.
