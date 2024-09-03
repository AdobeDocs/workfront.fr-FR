---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Sauvegarder vos données  [!DNL Workfront Proof]
description: Vous pouvez demander une sauvegarde de toutes vos données sur  [!DNL Workfront Proof]  en utilisant la fonction de sauvegarde.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 100%

---

# Sauvegarder vos données [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

## Présentation des sauvegardes

Vous pouvez demander une sauvegarde de toutes vos données dans [!DNL Workfront Proof] en utilisant la fonction de sauvegarde.

La sauvegarde est remise sous la forme d’un fichier .zip. Il comprend une exportation XML de toutes vos données (y compris les commentaires et les réponses pour toutes les versions de toutes les épreuves). Cependant, il n’inclut pas les fichiers originaux que vous avez téléchargés en tant qu’épreuves.

Chaque fichier .zip de sauvegarde créé pour que vous le téléchargiez a un nom de fichier unique, par exemple :

9789_05_05_2011_61703.zip

Le nom de fichier de cet exemple fournit les informations suivantes :

* 9789 est l’identifiant de votre compte [!DNL Workfront Proof].
* 05_05_2011 est la date de création, le 5 mai 2011.
* 61703 est un numéro aléatoire attribué par le système.

Cette convention de nommage vous permet de stocker facilement tous vos fichiers .zip de sauvegarde à un seul endroit sur votre ordinateur et de savoir exactement quand chaque sauvegarde a été créée pour vous.

La fonction [!UICONTROL Sauvegarde] vous permet de décider de l’utilisation de vos ressources :

* Vous permet de libérer de l’espace de stockage sans perdre vos épreuves actives ou archivées. Vous pouvez demander une sauvegarde, supprimer les épreuves, puis [Restaurer et vider la corbeille dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).
* Vous permet d’accéder à tous les fichiers que vous avez initialement chargés sur [!DNL Workfront] Proof. Vous pouvez les télécharger à l&#39;aide de la fonction [!UICONTROL Télécharger le fichier original] avant de supprimer les épreuves.

>[!NOTE]
>
>Les points suivants doivent être pris en compte lors de l’utilisation des sauvegardes :
>
>* Les sauvegardes sont disponibles sur les plans Entreprise et Illimité. Veuillez contacter notre [équipe de vente](mailto:sales@proofhq.com) pour obtenir un devis.
>* Le type d’encodage des données est défini par défaut sur UTF-8 et nous recommandons ce paramètre. Il s’agit du type d’encodage le plus couramment utilisé par les applications Internet.
>* Vous ne pouvez demander qu’une seule [!DNL backup] à la fois. Lorsque votre fichier .zip de sauvegarde est en cours de traitement, le lien Demander une nouvelle sauvegarde dans l’onglet Sauvegardes n’apparaît pas et le message affiché reste inchangé. Pour plus d’informations sur la demande de sauvegarde, voir [Demander une nouvelle sauvegarde des données de  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md).
>



## Sauvegarder vos données

1. Cliquez sur **[!UICONTROL Paramètres du compte]** dans le coin supérieur droit de l’interface [!DNL Workfront Proof]. (1)
1. Cliquez sur l&#39;onglet **[!UICONTROL Sauvegardes]**. (2)
1. Cliquez sur le lien **[!UICONTROL Demander une nouvelle sauvegarde]** (3).

Lorsque la sauvegarde est prête, le processus suivant se produit :

* Vous recevez un e-mail de [!DNL Workfront Proof] vous en informant (« Votre sauvegarde [!DNL Workfront Proof] est prête »). L’e-mail contient un lien de téléchargement pour vos données de sauvegarde.
* L’onglet de sauvegarde des [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) affiche un lien de téléchargement pour vos données de sauvegarde.
* Le lien Demander une nouvelle sauvegarde (3) réapparaît dans l’onglet Sauvegardes.

Vos données sont prêtes à être téléchargées sous forme de fichier zip. Vous pouvez télécharger le fichier .zip de sauvegarde soit à partir de l’e-mail de notification, soit dans les [!UICONTROL paramètres du compte], comme décrit dans les sections suivantes :

* [Télécharger votre fichier .zip de sauvegarde à partir de votre notification par e-mail](#downloading-your-backup-zip-file-from-your-email-notification)
* [Télécharger le fichier .zip de sauvegarde à partir des paramètres du compte](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## Télécharger votre fichier .zip de sauvegarde à partir de votre notification par e-mail {#downloading-your-backup-zip-file-from-your-email-notification}

Lorsque votre fichier .zip de sauvegarde est prêt à être téléchargé, vous recevez un e-mailde [!DNL Workfront Proof] dont l’objet est « Votre sauvegarde [!DNL Workfront Proof] est prête ».

Pour télécharger le fichier .zip de sauvegarde à partir de l’e-mail :

1. Cliquez sur le lien de téléchargement contenu dans l’e-mail.\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   Si votre connexion à [!DNL Workfront Proof] n’est pas actuellement effective, une nouvelle fenêtre de navigateur s’ouvre et affiche la page de connexion.

## Télécharger le fichier .zip de sauvegarde à partir des paramètres du compte {#downloading-your-backup-zip-file-from-the-account-settings}

Lorsque votre fichier .zip de sauvegarde est prêt à être téléchargé, l’onglet [!UICONTROL Sauvegarde] l’indique en affichant un lien de téléchargement. En outre, le lien [!UICONTROL Demander une nouvelle sauvegarde] apparaît à nouveau.

1. Cliquez sur **[!UICONTROL Paramètres du compte]** dans le coin supérieur droit de l’interface [!DNL Workfront Proof]. (1)
1. Cliquez sur l&#39;onglet **[!UICONTROL Sauvegardes]**. (2)\
   Si aucune personne de votre compte n’a demandé de sauvegarde, l’onglet [!UICONTROL Sauvegardes] indique que vous n’avez pas de sauvegardes. Si une personne a demandé une sauvegarde, l’onglet affiche la date de création et le lien de téléchargement de la dernière sauvegarde.

1. Cliquez sur le lien **[!UICONTROL Télécharger la sauvegarde]**. (3)\
   ![Download_Backup.png](assets/download-backup-350x167.png) Un écran de téléchargement de fichier s’affiche, vous demandant si vous souhaitez ouvrir ou enregistrer le fichier de téléchargement.

1. Cliquez sur **[!UICONTROL Enregistrer]**, puis sélectionnez l’emplacement sur votre ordinateur où vous souhaitez enregistrer le fichier .zip de sauvegarde.\
   Le message indiquant la date de votre dernière sauvegarde reste affiché au bas de la page [!UICONTROL Sauvegarde] jusqu’à la prochaine demande de sauvegarde. Le lien Télécharger la sauvegarde s’applique à cette dernière sauvegarde. Lorsque le lien [!UICONTROL Demander une nouvelle sauvegarde] s’affiche, vous pouvez cliquer dessus pour demander une nouvelle sauvegarde.

## Comprendre les fichiers de votre fichier .zip de sauvegarde

Votre fichier .zip de sauvegarde contient sept fichiers CSV (valeurs séparées par des virgules ou délimitées par des virgules) qui contiennent des informations sur vos épreuves actives et archivées jusqu’au moment où vos données ont été sauvegardées :

* comments.csv : comprend les commentaires sur les épreuves.
* comment_replies.csv : comprend les réponses aux commentaires sur les épreuves. organisation.csv : comprend l’identifiant numérique et le nom de votre organisation (votre compte).
* contacts.csv : comprend l’identifiant numérique, le nom et l’organisation de chaque contact.
* files.csv : comprend les informations de la page Détails de l’épreuve ou de la page Détails du fichier sur les épreuves ou les fichiers chargés vers [!DNL Workfront Proof].
* recipients.csv : comprend l’identifiant numérique, le rôle et les décisions de chaque personne désignée comme réviseur ou réviseuse, réviseur et approbateur ou réviseuse et approbatrice, etc., lorsque les épreuves sont chargées pour révision sur [!DNL Workfront Proof].
* users.csv : comprend les identifiants numériques et les noms de toutes les personnes du compte.

Vous pouvez extraire ces fichiers du fichier .zip de sauvegarde à l’aide de l’utilitaire zip que vous utilisez, puis les stocker à l’emplacement de votre choix sur votre ordinateur. Après avoir enregistré le fichier zip et extrait les différents fichiers CSV, vous pouvez manipuler les informations comme vous le souhaitez pour vos archives internes.

Chaque fichier .zip de sauvegarde créé à votre demande porte un nom distinct qui inclut la date de création de la sauvegarde, mais les fichiers CSV inclus dans chaque fichier .zip de sauvegarde portent toujours les mêmes noms. Vous pouvez utiliser l’une des méthodes suivantes pour vous assurer que vos fichiers de sauvegarde sont distincts les uns des autres :

* Créez un nouveau dossier pour chaque fichier .zip de sauvegarde et les fichiers CSV que vous en extrayez.
* Renommez chaque fichier CSV individuel pour inclure la date de sauvegarde lorsque vous l’extrayez du fichier zip.

>[!NOTE]
>
>Si [!DNL Microsoft Excel] est installé sur votre ordinateur, votre utilitaire d’extraction peut répertorier le type de fichier des différents fichiers CSV comme Fichier de valeurs séparées par des virgules [!DNL Microsoft Office Excel]. Vous pouvez ouvrir un fichier CSV extrait à l’aide d’[!DNL Excel] et enregistrer le fichier en tant que classeur [!DNL Excel] (&#42;.xlsx) ou tout autre type de fichier.
