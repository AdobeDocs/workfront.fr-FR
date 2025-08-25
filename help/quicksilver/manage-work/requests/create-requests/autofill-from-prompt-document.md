---
title: Remplir automatiquement une demande à l’aide d’invites ou de documents
content-type: reference
description: Vous pouvez utiliser l’IA pour remplir automatiquement les champs de requête en saisissant une invite ou en fournissant un document.
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 12%

---

# Remplir automatiquement une demande à l’aide d’invites ou de documents

>[!NOTE]
>
>* Cette fonctionnalité sera disponible en version Beta ouverte selon le planning suivant :
>
>   * Version mensuelle : 11 septembre 2025
>   * Version trimestrielle : 16 octobre 2025
>
>* Pour utiliser cette fonctionnalité, votre entreprise doit répondre aux exigences requises pour utiliser l’assistant Workfront AI. Pour plus d’informations, consultez [Conditions préalables pour l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

L’IA peut vous aider à remplir automatiquement les champs de requête en fonction d’une invite que vous saisissez. Il peut également remplir des champs basés sur du texte, tels que des e-mails ou des documents chargés. Vous pouvez approuver ou rejeter ces suggestions avant d’envoyer la demande.

Le remplissage automatique ne remplace aucun champ que vous avez déjà renseigné.

Les utilisateurs ne reçoivent pas de suggestions de données auxquelles ils n’ont pas accès autrement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouvelle : contributeur ou supérieure</p>
   Ou
   <p>Actuelle : demande ou supérieure</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p>  </td> 
  </tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td><p>Accès à l’ajout de demandes à une file d’attente</p> <p>Autorisation en affichage ou supérieure sur la demande existante</p> <p>Pour plus d’informations sur la configuration d’une file d’attente des demandes, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Créer une file d’attente des demandes</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Pour remplir automatiquement les demandes à l’aide d’une invite ou d’un document, **toutes** les conditions suivantes doivent être remplies :

* Votre entreprise doit utiliser Adobe IMS (système Identity Management)
* L’expérience unifiée Adobe doit être activée
* Votre organisation doit disposer d’un plan Select, Prime ou Ultimate Workfront
* Adobe doit disposer d’un contrat Adobe Gen AI signé dans le fichier .

  Pour plus d’informations sur la signature du contrat, consultez [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) dans l’article Présentation de l’assistant AI.
* L’assistant AI doit être activé dans les paramètres système de votre entreprise. Cette opération est gérée par votre administrateur Workfront.

  Pour plus d’informations sur l’activation de l’assistant AI dans les paramètres système, voir [Activer ou désactiver l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

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
1. Pour chaque suggestion de champ, sélectionnez **Accepter** ou **Rejeter** pour ce champ.

   ![Accepter ou refuser la suggestion](assets/accept-reject-suggestion.png)

   Ou

   Sélectionnez **Accepter tout** ou **Rejeter tout** en haut de la page pour accepter ou rejeter toutes les suggestions.

   >[!NOTE]
   >
   >Toute suggestion non révisée sera automatiquement acceptée lorsque vous soumettrez la demande.

## Obtenir des suggestions basées sur un document que vous téléchargez

Le remplissage automatique peut suggérer des valeurs de champ en fonction d’un document que vous téléchargez.

Ce type de suggestion vérifie également les demandes précédentes pour des contextes similaires. Par exemple, si l’invite indique que la demande concerne un certain client, Workfront peut localiser et saisir automatiquement l’adresse de facturation de ce client, en fonction des demandes précédentes.

### Mécanismes de sécurisation du chargement de document

#### Types de fichier pris en charge

Les types de fichiers pris en charge sont les suivants :

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
<li>CSV</li>
<li>DOC</li>
<li>DOCX</li>
<li>GIF</li>
<li>JPEG</li>
<li>JPEG</li>
</ul>
</td>
<td>
<ul>
<li>ODP</li>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
</ul>
</td>
<td>
<ul>
<li>PPTX</li>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>XLS</li>
<li>XLSX</li>
</ul>
</td>
</tr>
</table>

#### Taille de fichier prise en charge

La taille de chaque fichier peut atteindre 100 Mo

#### Nombre de fichiers

Vous pouvez charger jusqu’à 50 fichiers (pages, diapositives ou feuilles).

>[!IMPORTANT]
>
>Les documents sont convertis en une série d’images, chacune d’elles étant considérée comme un fichier distinct.
>
>Par exemple, vous pouvez charger un document PowerPoint contenant 50 diapositives ou 5 documents Word de 10 pages chacun.

#### Types de champ pris en charge

Les types de champs Workfront affectent la possibilité de remplir automatiquement un champ donné.

<table>
<tr>
<td><b>Pris en charge </b><br> le remplissage automatique peut remplir</td>
<td><b>Non pris en charge</b> <br>le remplissage automatique ne se remplit pas</td>
</tr>
<tr>
<td>
<ul>
<li>Texte sur une seule ligne</li>
<li>Zone de texte ou paragraphe</li>
<li>Champ de date</li>
<li>Case à cocher</li>
<li>Cases d’option</li>
<li>Listes déroulantes à sélection unique et multiple</li>
</ul>
</td>
<td><li>Frappe continue</li>
<li>Recherche externe</li>
<li>Recherche interne</li>
<li>Référence</li>
<li>Champs incorporés WF Planning</li>
</ul>
</td>
</tr>
</table>

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
1. Pour chaque suggestion de champ, sélectionnez **Accepter** ou **Rejeter** pour ce champ.

   ![Accepter ou refuser la suggestion](assets/accept-reject-suggestion.png)

   Ou

   Sélectionnez **Accepter tout** ou **Rejeter tout** en haut de la page pour accepter ou rejeter toutes les suggestions.

   >[!NOTE]
   >
   >Toute suggestion non révisée sera automatiquement acceptée lorsque vous soumettrez la demande.

## Dépannage

Si vous n’obtenez pas les suggestions attendues, cela peut être dû à l’un des problèmes suivants :

* Vous devez disposer d’au moins un mois de données de requête dans le système avant de pouvoir suggérer des valeurs de champ à partir de requêtes précédentes.
* Vous n’avez peut-être pas suivi les mécanismes de sécurisation de chargement de document lors du chargement d’un document à partir duquel extraire des suggestions. Pour plus d’informations, consultez la section [Mécanismes de sécurisation de chargement de document](#document-upload-guardrails) dans cet article.
