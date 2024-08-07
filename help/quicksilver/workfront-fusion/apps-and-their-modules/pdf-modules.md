---
title: Services Adobe PDF
description: Services Adobe PDF
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: ba161761acfc57e271f8593f534a5f7510187559
workflow-type: tm+mt
source-wordcount: '3719'
ht-degree: 26%

---

# [!DNL Adobe PDF Services]

Avec [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services], vous pouvez extraire des données d’un fichier de PDF ou générer un nouveau fichier de PDF à partir des données que vous fournissez. En outre, vous pouvez convertir divers types de fichiers en PDF ou en PDF en d’autres types de fichiers. Les services de PDF vous permettent également de combiner, de compresser ou de lire des métadonnées pour un fichier de PDF, ainsi que de contrôler la protection par mot de passe du fichier.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

Pour plus d’informations sur l’API utilisée pour les services de PDF, voir [ Adobe Document Generation API](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## Considérations de sécurité lors de l’utilisation de [!DNL Adobe PDF Services]

<!--

* [You do not need an [!DNL Adobe] account](#you-do-not-need-an-adobe-account) 
* [[!DNL Workfront Fusion] does not store your files](#workfront-fusion-does-not-store-your-files)

### You do not need an [!DNL Adobe] account 

Because [!DNL Workfront Fusion] is part of the [!DNL Adobe] product suite, you don't need a separate [!DNL Adobe] account to use these tools. Each tool accesses [!DNL Adobe] PDF functionality without using a connection.

Although [!DNL Workfront Fusion] does not require an [!DNL Adobe] account to use the PDF Services, the modules do require a connection. There are no credentials involved in this connection, and you provide only a name for the connection itself.

### [!DNL Workfront Fusion] does not store your files 

-->

[!DNL Adobe PDF Services] peut lire, convertir ou modifier vos fichiers, mais [!DNL Adobe] et [!DNL Workfront Fusion] ne stockent pas vos fichiers ou données. Cela signifie que :

* Vous conservez le contrôle de vos fichiers, y compris leur sécurité.
* Vous n’avez pas besoin d’un compte de stockage [!UICONTROL Adobe] ou de stockage dans le cloud pour utiliser les services PDF.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour créer un serveur à serveur OAuth, vous devez ajouter l’API Adobe PDF Services à votre console de développement Adobe. Lors de l’ajout de l’API, sélectionnez l’option Serveur à serveur OAuth.

Pour plus d’informations, voir [Ajout d’une API au projet à l’aide d’OAuth](https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/) dans la documentation destinée aux développeurs Adobe.

## Créer une connexion à [!DNL Adobe PDF Services]

Pour créer une connexion pour vos modules [!DNL Adobe PDF Services] :

1. Dans un module [!DNL Adobe PDF Services], cliquez sur **[!UICONTROL Ajouter]** en regard de la zone Connexion.

1. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection type]</td>
          <td>
            <p>Indiquez si vous souhaitez créer une connexion serveur à serveur ou une connexion JWT.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Nommez cette connexion.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>Saisissez votre [!DNL Adobe] [!UICONTROL ID client]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].<p>Pour plus d’informations sur la localisation des informations d’identification, voir <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credentials</a> dans la documentation destinée aux développeurs Adobe.</p></td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Entrez votre [0} [!UICONTROL Client Secret]. [!DNL Adobe] Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].<p>Pour plus d’informations sur la localisation des informations d’identification, voir <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credentials</a> dans la documentation destinée aux développeurs Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID du compte technique] (JWT uniquement)</td>
          <td>Saisissez votre [!DNL Adobe] [!UICONTROL ID de compte technique]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].<p>Pour plus d’informations sur la localisation des informations d’identification, voir <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credentials</a> dans la documentation destinée aux développeurs Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID d’organisation] (JWT uniquement)</td>
          <td>Saisissez votre [!DNL Adobe] [!UICONTROL ID d’organisation]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].<p>Pour plus d’informations sur la localisation des informations d’identification, voir <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credentials</a> dans la documentation destinée aux développeurs Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta-scopes] (JWT uniquement)</td>
          <td>
            Saisissez les portées de métadonnées nécessaires à la connexion.
          </td>
        </tr>
       </tbody>
    </table>
1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.


## Modules [!DNL Adobe PDF Services] et leurs champs

Lorsque vous configurez [!DNL PDF Services], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de cela, des champs supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Générer un document]](#generate-document)
* [[!UICONTROL Extract Text / Table]](#extract-text--table)
* [[!UICONTROL Combiner des fichiers de PDF]](#combine-pdf-files)
* [[!UICONTROL Compresser des fichiers de PDF]](#compress-pdf-files)
* [[!UICONTROL Convertir le document en fichier de PDF]](#convert-document-to-pdf-file)
* [[!UICONTROL Convertir l’HTML en fichier de PDF]](#convert-html-to-pdf-file)
* [[!UICONTROL Convertir une image en fichier PDF]](#convert-image-to-pdf-file)
* [[!UICONTROL Convertir le PDF en document]](#convert-pdf-to-document)
* [[!UICONTROL Convertir le PDF en image]](#convert-pdf-to-image)
* [[!UICONTROL Linearize a PDF file]](#linearize-a-pdf-file)
* [[!UICONTROL OCR pour le fichier de PDF]](#ocr-for-pdf-file)
* [[!UICONTROL Manipulation de page]](#page-manipulation)
* [[!UICONTROL Balise automatique d’accessibilité du PDF]](#pdf-accessibility-auto-tag)
* [[!UICONTROL Propriétés de fichier PDF]](#pdf-file-properties)
* [[!UICONTROL Fichier de PDF Protect]](#protect-pdf-file)
* [[!UICONTROL  Supprimer la protection d’un fichier de PDF]](#remove-protection-of-a-pdf-file)
* [Partage d’un fichier de PDF](#split-a-pdf-file)

### [!UICONTROL Générer un document]

Le module [!UICONTROL Générer un document] est un moyen puissant de créer un PDF contenant les données que vous sélectionnez. Vous pouvez le formater à l’aide d’un modèle [!DNL Microsoft Word] ou en fournissant des données au format JSON.

Pour plus d’informations sur la fonctionnalité [!UICONTROL [!DNL Adobe PDF Services] Generate document], consultez la [Présentation de la génération de documents](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) dans la documentation [!DNL Adobe Document Services].

* [ Utilisez le module [!UICONTROL Générer le document] avec un  [!DNL Microsoft Word] modèle](#use-the-generate-document-module-with-a-microsoft-word-template)
* [Utilisation du module [!UICONTROL Générer le document] avec JSON](#use-the-generate-document-module-with-json)

#### Utilisation du module [!UICONTROL Générer le document] avec un modèle [!DNL Microsoft Word]

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

Pour utiliser le module [!UICONTROL Générer le document] avec un modèle [!UICONTROL Microsoft Word], vous devez d’abord créer le modèle. Pour obtenir des instructions, recherchez &quot;Créer un modèle&quot; dans la documentation [!DNL Microsoft Office].

Renseignez les champs du module [!UICONTROL Générer le document] comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source File]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> <p>Ce fichier source est le modèle [!DNL Microsoft Word ] que le module utilise pour générer le nouveau PDF.</p> <p>Nous vous recommandons de créer un projet dans [!DNL Workfront] pour les modèles [!DNL Microsoft Word] que vous utilisez dans [!DNL Workfront Fusion]. Vous pouvez ensuite utiliser le module [!DNL Workfront] &gt; [!UICONTROL Télécharger le document] pour extraire le modèle approprié dans votre scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p>Sélectionnez le format du document généré.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Données à fusionner]</td> 
   <td> <p>Pour chaque balise de valeur de votre modèle que vous souhaitez remplacer par du texte, renseignez les éléments suivants :</p> 
    <ul> 
     <li> <p>[!UICONTROL Key]</p> <p>Entrez une clé. Dans le modèle, la clé correspond au texte affiché dans la balise value. Par exemple, si vous souhaitez placer du texte dans la balise de valeur <code>&#123;&#123;name&#125;&#125;</code>, saisissez <code>name </code> dans le champ de clé.</p> </li> 
     <li> <p>Type de valeur</p> <p>Indiquez si les données du champ de valeur sont une valeur, un objet ou un tableau d’objets.</p> </li> 
     <li> <p>[!UICONTROL Value]</p> <p>Saisissez ou mappez le texte que vous souhaitez afficher dans le document généré à la place de la balise value.</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Utilisation du module [!UICONTROL Générer le document] avec JSON

Pour utiliser le module [!UICONTROL  Generate document] avec JSON, renseignez les champs comme suit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source File]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p>Sélectionnez le format du document généré.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Données à fusionner]</td> 
   <td> <p>Pour utiliser JSON dans ce module, vous devez activer le mappage sur ce champ.</p> <p>Saisissez ou mappez le fichier JSON à partir duquel générer le document. </p> <p>Vous pouvez saisir directement JSON dans ce champ ou mapper la sortie JSON à partir d’un module JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extract Text / Table]

Ce module d’action vous permet d’extraire des données d’un fichier de PDF. Le module génère des éléments de texte individuels, tels qu’un paragraphe ou le texte dans une seule cellule d’un tableau.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Éléments qui doivent être extraits au format JSON]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Texte]</p> </li> 
     <li> <p>[!UICONTROL Tableaux]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Extraire les cadres de sélection ?]</td> 
   <td>Activez cette option pour extraire les données relatives au cadre de sélection du texte.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inclure les informations de style pour la sortie ?]</td> 
   <td>Activez cette option pour ajouter des informations de style au JSON de sortie.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Combiner des fichiers de PDF]

Ce module d’action prend plusieurs fichiers de PDF et les combine dans un seul fichier de PDF. Par exemple, ce module peut combiner tous les documents d’un projet [!UICONTROL Workfront] en un seul PDF à la fin du projet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents]</td> 
   <td> <p>Vous pouvez utiliser un module d’agrégation pour rassembler des documents dans un PDF, ou vous pouvez ajouter les documents manuellement. </p> <p>Nous vous recommandons d’utiliser un module [!UICONTROL Array Aggregator] pour agréger la sortie d’un module précédent. En utilisant un agrégateur, vous n’avez pas besoin de connaître les noms, emplacements ou nombres de fichiers à combiner. L’utilisation d’un agrégateur est donc beaucoup plus flexible et évolutive que la saisie manuelle des documents à combiner.</p> <p>Pour utiliser le module de fichiers [!UICONTROL Combiner le PDF] avec un agrégateur, vous devez activer le mappage sur le champ [!UICONTROL Documents] . </p> <p>Dans cet exemple, le module [!UICONTROL Read Related Records] identifie les documents associés à un projet et le module [!UICONTROL Download Documents] les télécharge chacun. Tous les PDF sont agrégés dans un tableau, qui est transmis dans le module de fichiers [!UICONTROL Combiner le PDF] .</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>Vous pouvez également saisir des documents manuellement.</p> <p>Pour chaque document à inclure dans le PDF combiné :</p> 
    <ol> 
     <li value="1"> <p>Cliquez sur [!UICONTROL Ajouter un document] .</p> </li> 
     <li value="2"> <p>Dans le champ [!UICONTROL Fichier Source] , sélectionnez le module qui génère le document que vous souhaitez inclure ou mappez le nom et les données du fichier source. </p> </li> 
     <li value="3"> <p>(Facultatif) Si vous souhaitez inclure uniquement certaines pages du fichier source, pour chaque plage de pages à ajouter, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong> dans le champ [!UICONTROL Pages], puis saisissez les première et dernière pages de la plage de pages à inclure, et cliquez sur <strong>[!UICONTROL Ajouter]</strong>. Vous pouvez inclure plusieurs plages de pages à partir d’un seul document.</p> </li> 
     <li value="4"> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Compresser des fichiers de PDF]

Ce module d’action prend un fichier de PDF et le compresse. Cela peut s’avérer utile pour économiser la bande passante ou la mémoire.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> <p>Le fichier source doit être au format PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Niveau de compression]</td> 
   <td>Sélectionnez le niveau de compression à utiliser.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir le document en fichier de PDF]

Cet outil convertit un document en fichier de PDF. Le fichier source doit être l’un des formats de document suivants :

* DOC
* XLS
* PPT
* TXT
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> <p>Le fichier source doit se présenter sous l’un des formats suivants :</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td> <p>Sélectionnez la langue par défaut du document source. Cela permet au module de sélectionner une police appropriée, si elle n’est pas incluse dans le fichier source.</p> <p>Choisissez l’une des langues suivantes :</p> 
    <ul> 
     <li> <p>en-US (par défaut) : anglais (États-Unis d’Amérique)</p> </li> 
     <li> <p>ca-ES : catalan (Espagne)</p> </li> 
     <li> <p>cs-CZ : Tchèque (République tchèque)</p> </li> 
     <li> <p>da-DK : Danois (Danemark)</p> </li> 
     <li> <p>de-DE : Allemand (Allemagne)</p> </li> 
     <li> <p>en-AE : anglais (Émirats arabes unis)</p> </li> 
     <li> <p>en-GB : anglais (Royaume-Uni)</p> </li> 
     <li> <p>en-IL : anglais (Israël)</p> </li> 
     <li> <p>en-US : anglais (États-Unis d’Amérique)</p> </li> 
     <li> <p>es-ES : Espagnol (Espagne)</p> </li> 
     <li> <p>es-MX : Espagnol (Mexique)</p> </li> 
     <li> <p>eu-ES : basque (Espagne)</p> </li> 
     <li> <p>fi-FI : Finnois (Finlande)</p> </li> 
     <li> <p>fr-CA : Français (Canada)</p> </li> 
     <li> <p>fr-FR : Français (France)</p> </li> 
     <li> <p>fr-MA : Français (Maroc)</p> </li> 
     <li> <p>hr-HR : Croate (Croatie)</p> </li> 
     <li> <p>hu-HU : hongrois (Hongrie)</p> </li> 
     <li> <p>it-IT : Italien (Italie)</p> </li> 
     <li> <p>ja-JP : japonais (Japon)</p> </li> 
     <li> <p>kr-KR : Coréen (Corée du Sud)</p> </li> 
     <li> <p>nb-NO : Norvégien Bokmål (Norvège)</p> </li> 
     <li> <p>nl-NL : Néerlandais (Pays-Bas)</p> </li> 
     <li> <p>pl-PL : polonais (Pologne)</p> </li> 
     <li> <p>pt-BR : Portugais (Brésil)</p> </li> 
     <li> <p>pt-PT : Portugais (Portugal)</p> </li> 
     <li> <p>roRO : roumain (Roumanie)</p> </li> 
     <li> <p>ru-RU : russe (Russie)</p> </li> 
     <li> <p>sk-SK : slovaque (Slovaquie)</p> </li> 
     <li> <p>sl-SI : Slovène (Slovénie)</p> </li> 
     <li> <p>sv-SE : suédois (Suède)</p> </li> 
     <li> <p>tr-TR : Turc (Turquie)</p> </li> 
     <li> <p>uk-UA : ukrainien (Ukraine)</p> </li> 
     <li> <p>zh-CN : Chinois (Chine continentale)</p> </li> 
     <li> <p>zh-TW : Chinois (Taïwan)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir l’HTML en fichier de PDF]

Cet outil convertit un fichier HTML en fichier PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> <p>Important : Le fichier Source doit être au format HTML ou ZIP. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>Si votre HTML fait référence à des variables JavaScript, vous pouvez inclure ces variables ici. </p> <p>Pour chaque variable, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong> et incluez la clé et la valeur de la variable.</p> <p>Remarque :   
     <ul> 
      <li> <p>Lors de la création d’un PDF à partir d’un fichier ZIP, le document source doit inclure un élément de script tel que : <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>Lors de la création d’un PDF à partir d’une URL, le contenu de cet objet JSON est injecté dans la machine virtuelle du navigateur avant le rendu de la page. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inclure l’en-tête et le pied de page]</td> 
   <td> <p>Activez cette option pour créer des en-têtes et des pieds de page pour le document du PDF.</p> 
    <ul> 
     <li> <p>L’en-tête comprend une date et le titre du document.</p> </li> 
     <li> <p>Le pied de page comprend le nom du fichier et un numéro de page.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Largeur de la page]</td> 
   <td>Saisissez la largeur du papier, en pouces. Le module utilise ces informations pour formater les pages dans le fichier de PDF créé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hauteur de la page]</td> 
   <td>Saisissez la hauteur du papier, en pouces. Le module utilise ces informations pour formater les pages dans le fichier de PDF créé.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir une image en fichier PDF]

Cet outil convertit une image en fichier PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et le fichier image du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir le PDF en document]

Cet outil convertit un fichier de PDF en document. Vous pouvez sélectionner l’un des formats suivants pour le fichier de sortie.

* DOC
* DOCX
* PPTX
* XLSX
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> <p>Le fichier source doit être au format PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Files Format]</td> 
   <td> <p>Sélectionnez le format de sortie des fichiers :</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>DOCX</p> </li> 
     <li> <p>PPTX</p> </li> 
     <li> <p>XLSX</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir le PDF en image]

Cet outil convertit un PDF en image au format PNG ou JPEG, qui est ensuite généré sous la forme d’un ZIP. Le PDF est converti en une image par page et chaque image se termine par le numéro de page. Les fichiers image sont ensuite combinés dans un fichier ZIP.

Par exemple, un fichier appelé &quot;TestFile&quot; de 8 pages produirait 8 images, appelées &quot;TestFile_1&quot; par &quot;TestFile_8&quot;. La sortie du module est un fichier ZIP contenant les 8 images.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> <p>Le fichier source doit être au format PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Files Format]</td> 
   <td> <p>Sélectionnez le format de sortie des fichiers :</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Linearize a PDF file]

Cet outil linéarise un document de PDF pour créer un document de PDF optimisé pour le web. Un document de PDF linéarisé peut être affiché page par page sans avoir à télécharger l’intégralité du document.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL OCR pour le fichier de PDF]

Cet outil exécute la reconnaissance optique des caractères (OCR) sur un fichier et produit un PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type OCR]</td> 
   <td> 
    <ul> 
     <li> <p>Le type [!UICONTROL Image d’origine modifiée] permet de s’assurer que le texte peut faire l’objet d’une recherche et peut être sélectionné, mais modifie l’image d’origine pendant le processus de nettoyage (par exemple, il la déforme) avant de placer un calque de texte invisible dessus. Ce type supprime les artefacts indésirables et peut générer un document plus lisible dans certains scénarios. </p> </li> 
     <li> <p>Le type [!UICONTROL Image d’origine non modifiée] incruste également un calque de texte indexable sur l’image d’origine, mais dans ce cas, l’image d’origine reste inchangée. Ce type produit une fidélité maximale à l’image originale.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Sélectionnez la langue de ce document.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Manipulation de page]

Ce module vous permet de faire pivoter ou supprimer des pages de manière sélective dans un document PDF. Par exemple, vous pouvez passer de la vue portrait à la vue paysage ou supprimer certaines pages du document du PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> <p>Sélectionnez l’action que vous souhaitez effectuer sur le fichier.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Supprimer]</b> </p> <p>Sélectionnez cette option pour supprimer des pages du document.</p> </li> 
     <li> <p><b>[!UICONTROL Rotation]</b> </p> <p>Sélectionnez cette option pour faire pivoter les pages, puis saisissez l’angle, en degrés dans le sens des aiguilles d’une montre, selon lequel vous souhaitez faire pivoter les pages du document par rapport à leur orientation de départ.</p> <p>Pour passer d’un portrait à un paysage, ou inversement, faites pivoter la page de 90 ou 270 degrés.</p> <p>Si une page est à l’envers, faites-la pivoter de 180 degrés.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pages]</td> 
   <td> <p>Pour chaque plage de pages à supprimer, cliquez sur <strong>[!UICONTROL Ajouter]</strong>, puis saisissez la première et la dernière page de la plage. </p> <p>Remarque :   
     <ul> 
      <li> <p>Vous pouvez utiliser des nombres négatifs pour effectuer un comptage à partir de la fin du document. La dernière page d’un document est -1, la deuxième à la dernière page est -2, etc.</p> </li> 
      <li> <p>Pour supprimer une seule page, définissez le même numéro de page que le début et la fin de la plage.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit utiliser au cours de chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Balise automatique d’accessibilité du PDF]

Ce module d’action crée un PDF balisé pour les cas d’utilisation de l’accessibilité. Il crée également un rapport Excel Microsoft facultatif qui répertorie les problèmes et suggère des correctifs.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maj d’en-têtes]</td> 
   <td> <p>Activez cette option pour modifier les en-têtes du document.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Générer un rapport]</b> </p> <p>Activez cette option pour générer un rapport qui répertorie les problèmes d’accessibilité dans le PDF, ainsi que leur emplacement, et fournit des suggestions sur la manière de les résoudre.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Propriétés de fichier PDF]

Cet outil extrait des informations de base sur le document, telles que :

* Nombre de pages
* Version du PDF
* Si le fichier est chiffré
* Si le fichier est linéarisé
* Si le fichier contient des fichiers incorporés

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Fichier de PDF Protect]

Cet outil sécurise un document de PDF avec un mot de passe utilisateur ou propriétaire. Il définit également des restrictions sur certaines fonctionnalités telles que l’impression, la modification et la copie dans le document du PDF. Vous sélectionnez le type de contenu à chiffrer et l’algorithme de cryptage.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> <p>Le fichier source doit être au format PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de protection par mot de passe]</td> 
   <td> <p>Activez cette option pour utiliser des mots de passe pour chiffrer le document du PDF d’entrée. Si vous activez cette option, vous devez spécifier et saisir une valeur pour l’une des options suivantes, ou les deux : </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>Chaque mot de passe peut contenir jusqu’à 128 caractères.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Algorithme de chiffrement]</td> 
   <td> <p>Sélectionnez l’algorithme de chiffrement. </p> 
    <ul> 
     <li> <p>[!UICONTROL Cryptage AES-128]</p> <p>Le mot de passe prend uniquement en charge les caractères LATIN-I. </p> </li> 
     <li> <p>[!UICONTROL Cryptage AES-256]</p> <p>Le mot de passe prend en charge le jeu de caractères Unicode</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenu à chiffrer]</td> 
   <td> <p>Sélectionnez le type de contenu à crypter.</p> 
    <ul> 
     <li> <p>[!UICONTROL Tout contenu]</p> </li> 
     <li> <p>[!UICONTROL Tout le contenu, à l’exception des métadonnées]</p> </li> 
     <li> <p>[!UICONTROL Uniquement les données incorporées] </p> </li> 
    </ul> <p>La sélection de "[!UICONTROL Uniquement les données incorporées]" rend les autorisations d’accès fournies inefficaces.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permissions]</td> 
   <td> <p>Sélectionnez les autorisations à inclure pour permettre l’impression, la modification ou la copie de contenu.</p> <p>Les paramètres d’autorisation ne sont utilisés que si le paramètre [!UICONTROL ownerPassword] est défini dans le champ [!UICONTROL Type de protection par mot de passe] .</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL  Supprimer la protection d’un fichier de PDF]

Cet outil supprime la sécurité (protection par mot de passe) d’un document de PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> <p>Le fichier source doit être au format PDF.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Password]</td> 
   <td>Saisissez le mot de passe qui protège actuellement le fichier.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Partage d’un fichier de PDF]

Ce module d’action divise un document de PDF en plusieurs documents plus petits. Vous indiquez s’il faut le fractionner en fonction du nombre de fichiers, de pages par fichier ou de plages de pages.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> <p>Le fichier source doit être au format PDF.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Option de fractionnement]</td> 
   <td>Sélectionnez le mode de partage du fichier. 
   <ul>
   <li><p><b>Plages de page</b></p><p>Pour chaque plage de pages que vous souhaitez diviser en un document distinct, cliquez sur <b>Ajouter</b> et saisissez la page sur laquelle vous souhaitez commencer et la page sur laquelle vous souhaitez terminer.</p></li>
   <li><p><b>Nombre de pages</b></p><p>Saisissez le nombre de pages à inclure dans les nouveaux documents.</p></li>
   <li><p><b>Nombre de fichiers</b></p><p>Saisissez le nombre de fichiers de taille égale dans lesquels vous souhaitez fractionner le document.</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

## Effectuer un appel API personnalisé

Ce module d’action est une requête HTTP personnalisée à l’API PDF Services.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Sélectionnez la connexion à utiliser pour ce module.</p> Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe PDF Services], voir <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Créer la connexion à [!DNL Adobe PDF Services]</a> dans cet article. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> Entrez un chemin relatif ou une URL. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute automatiquement les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Pour chaque champ à ajouter à l’appel API, cliquez sur <b>Ajouter un élément</b> et saisissez la clé et la valeur facultative du champ.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

