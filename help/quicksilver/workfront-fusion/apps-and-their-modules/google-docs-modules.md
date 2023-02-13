---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Documents Google
description: La fusion Adobe Workfront [!DNL Google Docs] Les modules vous permettent de surveiller, créer, modifier et récupérer des documents dans vos [!DNL Google Docs] et [!DNL Google Docs] (pour les utilisateurs de [!DNL G Suite]).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '4042'
ht-degree: 0%

---

# [!DNL Google Docs] modules

Le [!DNL Adobe Workfront Fusion] [!DNL Google Docs] Les modules vous permettent de surveiller, créer, modifier et récupérer des documents dans vos [!DNL Google Docs] et [!DNL Google Docs] (pour [!DNL G Suite] utilisateurs).

Pour utiliser [!DNL Google Docs] avec [!DNL Adobe Workfront Fusion], il est nécessaire d’avoir une [!DNL Google] compte . Si vous n’avez pas de [!DNL Google] vous pouvez toutefois en créer un à l’adresse [!DNL Google] Page d’aide du compte.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr>
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Google Docs] , vous devez disposer d’un compte Google.

## [!DNL Google Docs] modules et leurs champs

Lorsque vous configurez [!DNL Google Docs] modules, [!UICONTROL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Google Docs] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Document

* [[!UICONTROL Surveiller les documents]](#watch-documents)
* [[!UICONTROL Lister des documents]](#list-documents)
* [[!UICONTROL Obtention du contenu d’un document]](#get-content-of-a-document)
* [[!UICONTROL Création d’un document]](#create-a-document)
* [[!UICONTROL Création d’un document à partir d’un modèle]](#create-a-document-from-a-template)
* [[!UICONTROL Insertion d’un paragraphe à un document]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL Insertion d’une image dans un document]](#insert-an-image-to-a-document)
* [[!UICONTROL Remplacement d’une image par une nouvelle image]](#replace-an-image-with-a-new-image)
* [[!UICONTROL Remplacer le texte d’un document]](#replace-text-in-a-document)
* [[!UICONTROL Téléchargement d’un document]](#download-a-document)
* [[!UICONTROL Suppression d’un document]](#delete-a-document)

#### [!UICONTROL Surveiller les documents]

Ce module de déclenchement renvoie les détails du document lorsqu’un nouveau document est créé ou modifié dans le dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents de contrôle]</td> 
   <td> <p style="color: #000000;">Indiquez si vous souhaitez regarder les documents créés ([!UICONTROL Par date de création]) ou modifiés ([!UICONTROL Par date de modification]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur à surveiller.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier à surveiller pour les documents créés ou modifiés.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier à surveiller pour les documents créés ou modifiés.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé à regarder.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Shared Drive] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Définissez le nombre maximal de documents que Workfront Fusion renvoie dans un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lister des documents]

Ce module d’action récupère une liste de documents du dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur à partir duquel vous souhaitez répertorier les documents.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez répertorier les documents.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez répertorier les documents.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé à partir duquel vous souhaitez répertorier les documents.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td> <p>Définition du nombre maximal de documents [!DNL Workfront Fusion] renvoie un cycle d'exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention du contenu d’un document]

Ce module d’action récupère un document spécifié.

Vous devrez peut-être étendre vos autorisations.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtention du contenu d’un document]</td> 
   <td> <p>Choisissez si vous souhaitez mapper l’ID du document ou sélectionnez le document manuellement dans le menu déroulant.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur contenant le document que vous souhaitez récupérer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier contenant le document que vous souhaitez récupérer.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier contenant le document que vous souhaitez récupérer.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé qui contient le document que vous souhaitez récupérer.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Sélectionnez l’objet à renvoyer dans la sortie du module.</p> 
    <ul> 
     <li>[!UICONTROL Image] (par défaut)</li> 
     <li>[!UICONTROL Dessin]</li> 
     <li>[!UICONTROL Graphique]</li> 
    </ul> <p>Note:  <p>Pour effectuer un mappage supplémentaire de ces objets, utilisez la valeur [!UICONTROL Inline Objects Array] dans la sortie de ce module (au lieu de [!UICONTROL inlineObjects]).</p> <p>Les objets [!UICONTROL Inline Objects Array] sont triés dans l’ordre dans lequel ils apparaissent dans le document. Cela facilitera le traitement.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création d’un document]

Ce module d’action permet de créer un nouveau document dans le dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez le nom du document.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td> <p>Saisissez le contenu du document. HTML est pris en charge.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel vous souhaitez créer un document.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez créer un document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez créer un document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel vous souhaitez créer un document.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Insérer un en-tête]</td> 
   <td> <p> Activez cette option pour insérer l’en-tête dans le document, puis saisissez ou mappez le texte de l’en-tête.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Insérer un pied de page] </td> 
   <td> <p>Activez cette option pour insérer le pied de page dans le document, puis saisissez ou mappez le texte de l’en-tête.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création d’un document à partir d’un modèle]

Ce module d’action crée une copie d’un document de modèle existant et remplace toutes les balises. Ce module permet également aux utilisateurs de remplacer les images par de nouvelles images par URL.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Créer un document à partir d’un modèle]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par Mappage]</strong> <br>Sélectionnez cette option pour mapper le modèle de document.</li> 
     <li><strong>[!UICONTROL Par Liste Déroulante]</strong> <br>Sélectionnez cette option pour sélectionner le modèle de document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve votre modèle. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve votre modèle.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve votre modèle.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé où se trouve votre modèle.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Saisissez les valeurs qui seront saisies au lieu des variables dans le nouveau document.</p> 
    <ul> 
     <li><strong>[!UICONTROL Balises]</strong> <br>Saisissez les balises contenues dans le modèle de document. Ne pas utiliser <code>&#123;&#123;&#125;&#125;</code>. Exemple : use <code>name</code> au lieu de <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Valeur remplacée]</strong><br>Saisissez la valeur de la balise .</li> 
    </ul> <p>Par exemple, la fonction<code> &#123;&#123;name&#125;&#125;</code> dans le document source s’affiche comme champ de nom, où la valeur peut être insérée, par exemple <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Remplacement d’images]</p> </td> 
   <td> <p>Saisissez le lien vers l’[!UICONTROL ID d’objet image] et l’[!UICONTROL URL d’image] qui remplaceront l’image actuelle.</p> <p>Remarque : Vous pouvez récupérer les ID d’image à l’aide du module [!UICONTROL Obtenir un document] , où les ID sont contenus dans le tableau [!UICONTROL Tableau d’objets en ligne].</p> <p>Nous vous recommandons d’ajouter du texte ALT aux images de votre [!DNL Google] document. </p> <p>Pour ajouter un texte ALT à la variable [!DNL Google Docs] image :</p> 
    <ol> 
     <li value="1">Cliquez avec le bouton droit sur l’image.</li> 
     <li value="2">Sélectionnez l’option [!UICONTROL ALT text] .</li> 
     <li value="3">Saisissez le [!UICONTROL ALT texte] dans le champ [!UICONTROL Titre] et cliquez sur [!UICONTROL OK].</li> 
    </ol> <p>Une fois le texte ALT ajouté à l’image, il est affiché entre parenthèses dans le nom du champ.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>Saisissez le nom du nouveau document.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve votre modèle. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez créer le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez créer le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel vous souhaitez créer le document.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insertion d’un paragraphe à un document]

Ce module d’action ajoute ou insère un nouveau paragraphe dans un document existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sélectionner un document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par Mappage]</strong> <br>Sélectionnez cette option pour mapper le document.</li> 
     <li><strong>[!UICONTROL Par Liste Déroulante]</strong> <br> Sélectionnez cette option pour sélectionner le document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document auquel vous souhaitez ajouter un paragraphe. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter un paragraphe, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter un paragraphe, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document auquel vous souhaitez ajouter un paragraphe, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Insérer un paragraphe]</p> </td> 
   <td> <p>Sélectionnez le mode d’insertion du nouveau texte dans le document.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Par spécification de l’emplacement]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Par index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Saisissez le numéro de l'index dans lequel vous souhaitez insérer votre texte. Vous pouvez utiliser le module [!UICONTROL Obtenir un document] pour récupérer le numéro d’index.</p> <p>Pour afficher tous les caractères (y compris les caractères masqués) du document, vous pouvez utiliser le module complémentaire [!UICONTROL Afficher]. Le module complémentaire se trouve sous [!UICONTROL Modules complémentaires] &gt; [!UICONTROL Obtenir des modules complémentaires]. Recherchez [!UICONTROL Show] et installez le module complémentaire [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Texte inséré]</strong> </p> <p>Saisissez le texte à insérer dans le document.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Par identifiant de segment]</strong> </p> <p>Sélectionnez l'en-tête et le pied de page auxquels vous souhaitez insérer le contenu texte et saisissez le texte à insérer dans les champs correspondants.</p> <p>Si l’en-tête ou le pied de page contient déjà du texte, ce dernier est ajouté avant le texte existant.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL En ajoutant au corps du document]</strong> </p> <p>Ajoute le texte saisi à la fin du contenu du corps du document.</p> <p>Le style du nouveau paragraphe sera copié à partir du paragraphe à l’index d’insertion actuel, y compris les listes et les puces.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL En ajoutant à la fin du segment (en-tête et pied de page)]</strong> </p> <p>Sélectionnez l'en-tête et le pied de page auxquels vous souhaitez insérer le contenu texte et saisissez le texte à insérer dans les champs correspondants.</p> <p>Si l’en-tête ou le pied de page contient déjà du texte, ce dernier est ajouté après le texte existant.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texte annexé]</td> 
   <td>Saisissez ou mappez le texte à ajouter au document.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insertion d’une image dans un document]

Ce module d’action insère une image de l’URL vers le document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sélectionner un document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par Mappage]</strong> <br>Sélectionnez cette option pour mapper le modèle de document.</li> 
     <li><strong>[!UICONTROL Par Liste Déroulante]</strong> <br> Sélectionnez cette option pour sélectionner le document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document auquel vous souhaitez ajouter une image. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter une image, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter une image, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document auquel vous souhaitez ajouter une image, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Insérer une image]</p> </td> 
   <td> <p>Sélectionnez le mode d’insertion de la nouvelle image dans le document.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Par spécification de l’emplacement]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Par index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Saisissez le numéro de l'index dans lequel vous souhaitez insérer votre image. Vous pouvez utiliser le module [!UICONTROL Obtenir un document] pour récupérer le [!UICONTROL Numéro d’index].</p> <p>Pour afficher tous les caractères (y compris les caractères masqués) du document, vous pouvez utiliser le module complémentaire [!UICONTROL Afficher]. Le module complémentaire se trouve sous [!UICONTROL Modules complémentaires] &gt; [!UICONTROL Obtenir des modules complémentaires]. Recherchez [!UICONTROL Show] et installez le module complémentaire [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Image URL]</strong> </p> <p>Saisissez l'URL de l'image à insérer dans le document.</p> <p>La taille d’image maximale est de 50 Mo. Ne doit pas dépasser 25 mégapixels. Seul le format PNG, JPEG ou GIF est pris en charge.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Par identifiant de segment]</strong> </p> <p>Sélectionnez l’en-tête et le pied de page auxquels vous souhaitez insérer l’image et saisissez l’URL de l’image dans les champs correspondants.</p> <p>La taille d’image maximale est de 50 Mo. L’image ne doit pas dépasser 25 mégapixels. Seul le format PNG, JPEG ou GIF est pris en charge.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL En ajoutant au corps du document]</strong> </p> <p>Ajoute une image spécifique à la fin du contenu du corps du document.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL En ajoutant à la fin du segment (en-tête et pied de page)]</strong> </p> <p>Sélectionnez l’en-tête et le pied de page auxquels vous souhaitez insérer une image et saisissez l’URL de l’image à insérer dans les champs correspondants.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ampleur de la hauteur en points/longitude en points]</p> </td> 
   <td> <p>Définissez la taille de l’image insérée. Les proportions seront conservées.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remplacement d’une image par une nouvelle image]

Ce module d’action remplace une image existante. Les proportions de l’image d’origine seront conservées.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sélectionner un document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par Mappage]</strong> <br>Sélectionnez cette option pour mapper le modèle de document.</li> 
     <li><strong>[!UICONTROL Par Liste Déroulante]</strong> <br> Sélectionnez cette option pour sélectionner le document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document à remplacer par une image. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à remplacer par une image, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à remplacer par une image, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document à remplacer par une image, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Image URL]</p> </td> 
   <td> <p>Saisissez ou mappez l’URL de la nouvelle image qui remplacera l’image existante.</p> <p>Les images sont répertoriées dans l’ordre dans lequel elles apparaissent dans le document. Par exemple : <code>Body: Image No. 1</code> est la première image du document.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remplacer le texte d’un document]

Ce module d’action remplace le texte dans un document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sélectionner un document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par Mappage]</strong> <br>Sélectionnez cette option pour mapper le modèle de document.</li> 
     <li><strong>[!UICONTROL Par Liste Déroulante]</strong> <br> Sélectionnez cette option pour sélectionner le document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document auquel vous souhaitez ajouter du texte. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter du texte, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter du texte, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document auquel vous souhaitez ajouter du texte, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Remplacer un texte]</p> </td> 
   <td> <p>Ajoutez chaque texte à remplacer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ancien texte à remplacer]</strong> </p> <p>Saisissez le texte à remplacer.</p> </li> 
     <li> <p><strong>[!UICONTROL Nouveau texte à insérer]</strong> </p> <p>Saisissez le nouveau texte.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Téléchargement d’un document]

Ce module d’action convertit et télécharge le document sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document à télécharger.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à télécharger, puis sélectionnez-le.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à télécharger, puis sélectionnez-le.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document à télécharger, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Sélectionnez le format de fichier cible du document téléchargé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un document]

Ce module d’action supprime un document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document que vous souhaitez supprimer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à supprimer, puis sélectionnez-le.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à supprimer, puis sélectionnez-le.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document à supprimer, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared Drive]</td> 
   <td> <p>Sélectionnez le lecteur contenant le document à télécharger, puis sélectionnez un document. Cette option est disponible si vous avez sélectionné [!DNL Google Docs] dans le champ [!UICONTROL Choisir un lecteur] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID du document]</td> 
   <td> <p> Sélectionnez ou mappez le document dans lequel vous souhaitez remplacer une ou plusieurs images.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

* [[!UICONTROL Lancer un appel API]](#make-an-api-call)
* [[!UICONTROL Activer la sélection de tous les liens d’un document]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL Lancer un appel API]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Saisissez un chemin relatif à <code>https://docs.googleapis.com/</code>. Exemple: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Saisissez la chaîne de requête de requête de requête.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** L’appel API suivant récupère les détails du document spécifié dans vos documents Google :

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Méthode:**

[!UICONTROL GET]

![](assets/api-call-example.png)

Vous trouverez des détails sur le document récupéré dans la sortie du module sous [!UICONTROL Bundle] > [!UICONTROL Corps].

![](assets/api-output.png)

#### [!UICONTROL Activer la sélection de tous les liens d’un document]

Ce module d’action recherche tous les liens du document et permet de les cliquer.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Créer tous les liens dans un document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par Mappage]</strong> <br>Sélectionnez cette option pour mapper le modèle de document.</li> 
     <li><strong>[!UICONTROL Par Liste Déroulante]</strong> <br> Sélectionnez cette option pour sélectionner le document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document sur lequel vous souhaitez que les liens puissent faire l’objet d’un clic. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document sur lequel vous souhaitez que les liens puissent faire l’objet d’un clic, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document sur lequel vous souhaitez que les liens puissent faire l’objet d’un clic, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible pour [!DNL G Suite] utilisateurs uniquement)</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document sur lequel vous souhaitez que les liens puissent faire l’objet d’un clic, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné la variable [!DNL Google Docs] dans ce champ et que vous n’êtes pas une [!DNL G Suite] utilisateur, l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared Drive]</td> 
   <td> <p>Sélectionnez le lecteur contenant le document dans lequel vous souhaitez mettre à jour les liens, puis sélectionnez un document. Cette option est disponible si vous avez sélectionné [!DNL Google Docs] dans le champ [!UICONTROL Choisir un lecteur].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID du document]</td> 
   <td> <p> Sélectionnez ou mappez le document dans lequel vous souhaitez mettre à jour les liens.</p> </td> 
  </tr> 
 </tbody> 
</table>
