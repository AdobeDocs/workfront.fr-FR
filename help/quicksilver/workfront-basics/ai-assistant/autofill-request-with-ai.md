---
title: Remplir automatiquement une demande à l’aide de l’IA
content-type: reference
description: Vous pouvez utiliser l’IA pour remplir automatiquement les champs de requête.
author: Becky
feature: Get Started with Workfront
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
source-git-commit: b0454d5fe3d866b30513cdea67d22c06c5efbfb3
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 3%

---

# Remplir automatiquement une demande à l’aide de l’IA

>[!NOTE]
>
>Cette fonctionnalité fait actuellement partie d’une version Beta fermée. Pour activer cette fonctionnalité, contactez `sargism@adobe.com`.
>
>Pour être éligible à la version Beta fermée, votre entreprise doit répondre aux conditions requises pour utiliser l’assistant Workfront AI. Pour plus d’informations, consultez [Conditions préalables pour l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

L’IA peut vous aider à remplir automatiquement les champs de requête. Il peut suggérer des valeurs de champ en fonction de requêtes précédentes ou les analyser à partir de texte tel que des e-mails ou des documents chargés.

Vous pouvez approuver ou rejeter ces suggestions avant d’envoyer la demande.

Le remplissage automatique ne remplace aucun champ que vous avez déjà renseigné.

Les utilisateurs ne reçoivent pas de suggestions de données auxquelles ils n’ont pas accès autrement.

## Obtention de suggestions lors du remplissage du formulaire

Le remplissage automatique peut suggérer des valeurs de champ lorsque vous remplissez le formulaire. Lorsque vous saisissez des valeurs dans les champs de requête, Workfront compare ces valeurs aux requêtes précédentes. Si la valeur saisie est étroitement corrélée à d’autres valeurs de champ dans des contextes similaires dans des requêtes précédentes, Workfront suggère ces valeurs.

Par exemple, si une clinique utilise toujours le même code de facturation, Workfront suggère ce code de facturation dans le champ approprié lorsque le nom de la clinique est saisi.

Pour utiliser des suggestions basées sur des requêtes précédentes :

1. Commencez à créer une demande.

   Pour obtenir des instructions, voir [Création et envoi de requêtes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Commencez à remplir les champs.

   Lorsque vous remplissez des champs, d’autres champs peuvent afficher des suggestions.

1. Pour chaque suggestion de champ, sélectionnez **Accepter** ou **Rejeter** sous ce champ.

   Ou

   Sélectionnez **Accepter tout** ou **Rejeter tout** en haut de la page pour accepter ou rejeter toutes les suggestions.

## Obtenir des suggestions à partir d’une invite de texte

Le remplissage automatique peut suggérer des valeurs de champ en fonction du texte, tel que les e-mails. Vous collez dans un bloc de texte et Workfront traite le texte pour suggérer des valeurs de champ en fonction du texte.

Par exemple, si l’e-mail inclut « L’échéance est le 1er juin » et que le formulaire de demande comporte un champ pour la date d’échéance, Workfront suggère le 1er juin pour cette valeur de champ.

Ce type de suggestion vérifie également les demandes précédentes pour des contextes similaires. Par exemple, si l’invite indique que la demande concerne un certain client, Workfront peut localiser et saisir automatiquement l’adresse de facturation de ce client, en fonction des demandes précédentes.

Vous pouvez coller du texte à appliquer à l’ensemble du formulaire ou à une seule section du formulaire.

Pour utiliser des suggestions basées sur une invite de texte collée :

1. Commencez à créer une demande.

   Pour obtenir des instructions, voir [Création et envoi de requêtes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Pour appliquer l’invite de texte à l’ensemble du formulaire, cliquez sur l’icône AI ![icône AI](assets/request-prompt-icon.png) sous le nom du formulaire.

   Ou

   Pour appliquer l’invite de texte à une seule section, cliquez sur l’icône AI ![icône AI](assets/request-prompt-icon.png) à côté du nom de la section.

1. Collez le texte dans la zone d’invite.
1. Cliquez sur **Remplir le formulaire**.

   Workfront génère des suggestions pour le formulaire.
1. Pour chaque suggestion de champ, sélectionnez **Accepter** ou **Rejeter** sous ce champ.

   Ou

   Sélectionnez **Accepter tout** ou **Rejeter tout** en haut de la page pour accepter ou rejeter toutes les suggestions.

## Obtenir des suggestions basées sur un document que vous téléchargez

Le remplissage automatique peut suggérer des valeurs de champ en fonction d’un document que vous téléchargez.

Ce type de suggestion vérifie également les demandes précédentes pour des contextes similaires. Par exemple, si l’invite indique que la demande concerne un certain client, Workfront peut localiser et saisir automatiquement l’adresse de facturation de ce client, en fonction des demandes précédentes.

### Mécanismes de sécurisation du chargement de document

#### Types de fichier pris en charge

Les types de fichiers pris en charge sont les suivants :

* BMP
* CSV
* DOC
* DOCX
* GIF
* JPEG
* JPG
* ODP
* ODS
* ODT
* PDF
* PNG
* PPT
* PPTX
* RTF
* TIFF
* TXT
* XLS
* XLSX

#### Taille de fichier prise en charge

La taille de chaque fichier peut atteindre 100 Mo

#### Nombre de fichiers

Vous pouvez charger jusqu’à 50 fichiers (pages, diapositives ou feuilles).

>[!IMPORTANT]
>
>Les documents sont convertis en une série d’images, chacune d’elles étant considérée comme un fichier distinct.
>
>Par exemple, vous pouvez charger un document PowerPoint contenant 50 diapositives ou 5 documents Word de 10 pages chacun.

#### Autres bonnes pratiques

Tenez compte des points suivants lors du chargement d’un document pour le remplissage automatique de la demande :

* Le remplissage automatique est actuellement optimisé pour l’alphabet latin.
* Nous vous recommandons d’utiliser une taille de texte de 8 points ou plus.
* Le remplissage automatique peut présenter des difficultés avec les images du document, telles que les images pivotées ou déformées, les graphiques, le comptage ou l&#39;utilisation de raisons spatiales sur des objets dans les images.
* Comme toujours, nous vous recommandons de vérifier l’exactitude des résultats avant d’envoyer la requête.

### Chargement d’un document pour remplir automatiquement une demande

Vous pouvez charger un document à appliquer à l’ensemble du formulaire ou à une seule section du formulaire.

1. Commencez à créer une demande.

   Pour obtenir des instructions, voir [Création et envoi de requêtes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Pour appliquer le document à l’ensemble du formulaire, cliquez sur l’icône AI ![icône AI](assets/request-prompt-icon.png) sous le nom du formulaire.

   Ou

   Pour appliquer le document à une seule section, cliquez sur l’icône AI ![icône AI](assets/request-prompt-icon.png) en regard du nom de la section.

1. Cliquez sur **Télécharger des fichiers**, puis sélectionnez le fichier dans le gestionnaire de fichiers.

   Ou

   Faites glisser le document de votre gestionnaire de fichiers vers la zone **Télécharger des fichiers pour remplir automatiquement les formulaires de demande**.
1. Cliquez sur **Remplir le formulaire** ou **Remplir la section**.

   Workfront génère des suggestions pour le formulaire.
1. Pour chaque suggestion de champ, sélectionnez **Accepter** ou **Rejeter** sous ce champ.

   Ou

   Sélectionnez **Accepter tout** ou **Rejeter tout** en haut de la page pour accepter ou rejeter toutes les suggestions.

## Dépannage

Si vous n’obtenez pas les suggestions attendues, cela peut être dû à l’un des problèmes suivants :

* Vous devez disposer d’au moins un mois de données de requête dans le système avant de pouvoir suggérer des valeurs de champ à partir de requêtes précédentes.
* Vous n’avez peut-être pas suivi les mécanismes de sécurisation de chargement de document lors du chargement d’un document à partir duquel extraire des suggestions. Pour plus d’informations, consultez la section [Mécanismes de sécurisation de chargement de document](#document-upload-guardrails) dans cet article.

