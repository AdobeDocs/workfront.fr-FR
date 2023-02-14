---
filename: microsoft-word-templates-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules de modèle Microsoft Word
description: Dans un scénario de fusion Adobe Workfront, vous pouvez automatiser les workflows qui utilisent des modèles Microsoft Word et les connecter à plusieurs applications et services tiers.
author: Becky
source-git-commit: 43b64d1371438909063d2ac81cccb90b97179dfc
workflow-type: tm+mt
source-wordcount: '1286'
ht-degree: 0%

---


# [!DNL Microsoft Word Template] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft Word Templates], ainsi que de la connecter à plusieurs applications et services tiers.

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
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> 
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Miscrosoft Word Templates] avec [!DNL Adobe Workfront Fusion], une [!DNL Office 365] compte . Vous pouvez en créer un à l’adresse www.office.com.

## Utilisation [!DNL Microsoft Word Templates] modules

Vous pouvez utiliser une [!DNL Microsoft Word Template] pour fusionner les données de plusieurs services web en un [!DNL Microsoft Word] document.

Par exemple, vous pouvez utiliser [!DNL Microsoft Word] modèle :

![](assets/word-template-before-filled-350x62.png)

Pour créer ce document :

![](assets/word-template-exampled-filled-350x85.png)

## À propos des balises de valeur

A [!DNL Microsoft Word] modèle est normal [!DNL Microsoft Word] document (fichier .docx) avec des balises spéciales dans son texte qui déterminent où et comment fusionner ou remplir des données. Il existe trois types de balises :

* [Balise de valeur simple](#simple-value-tag)
* [Balise de condition](#condition-tag)
* [Balise de boucle](#loop-tag)

### Balise de valeur simple {#simple-value-tag}

Une balise de valeur simple est simplement remplacée par une valeur correspondante. Le nom de la balise correspond au [!UICONTROL Clé] la valeur du champ, placée entre accolades doubles ; par exemple,


<pre>&#123;&#123;name&#125;&#125;</pre>


.

**Exemple :** Pour créer un document qui indique &quot;Bonjour, Piotr !&quot;, vous pouvez utiliser un [!DNL Microsoft Word Template] pour créer le modèle suivant :

<pre>&gt; Bonjour &#123;&#123;name&#125;&#125;!</pre>

Pour ce faire, vous devez configurer le module comme suit :

![](assets/word-template-simple-value-350x286.png)

### Balise de condition {#condition-tag}

Vous pouvez utiliser une balise de condition pour renvoyer à la ligne le texte qui doit être rendu uniquement lorsque certaines conditions sont remplies. Pour renvoyer le texte à la ligne, placez-le entre les balises de condition d’ouverture et de fermeture, telles que &quot;hasPhone&quot; si la condition indique si les données incluent ou non un numéro de téléphone. Le nom d’une balise d’ouverture est précédé d’un signe de hachage #, le nom d’une balise de fermeture est précédé d’une barre oblique /, comme illustré dans l’exemple ci-dessous.

**Exemple :** Pour produire un document qui comprend le numéro de téléphone d’un client si les données d’entrée incluent un numéro de téléphone, mais pas d’adresse électronique, vous pouvez utiliser une [!DNL Microsoft Word Template] et créez le modèle suivant :
<pre>> &#123;&#123;#hasPhone&#125;&#125;Téléphone : &#123;&#123;phone&#125;&#125; &#123;&#123;/hasPhone&#125;&#125;</pre><pre>> &#123;&#123;#hasEmail&#125;&#125;Courriel : &#123;&#123;email&#125;&#125; &#123;&#123;/hasEmail&#125;&#125;</pre>Pour ce faire, vous devez configurer le module comme suit :

![](assets/word-template-conditional-350x501.png)

Dans le document, le numéro de téléphone se présente comme suit :
<pre>&gt; Téléphone : 4445551234</pre>

### Balise de boucle {#loop-tag}

Vous pouvez utiliser une balise de boucle, également appelée balise de section, pour répéter une section de texte. Entourez le texte en le plaçant entre les balises de boucle d’ouverture et de fermeture. Le nom d’une balise d’ouverture est précédé d’un signe de hachage #; le nom d’une balise de fermeture est précédé d’une barre oblique /.

* [Balise de boucle avec remplissage d’un module de document](#loop-tag-with-fill-out-a-document-module)

<!-- [Loop tag with Fill a document with a batch of data module](#loop-tag-with-fill-a-document-with-a-batch-of-data-module)-->

#### Balise de boucle avec remplissage d’un module de document {#loop-tag-with-fill-out-a-document-module}

**Exemple :** Pour produire un document qui répertorie le nom et le numéro de téléphone de chaque contact dans une liste de clients, vous pouvez utiliser une [!DNL Microsoft Word Template] et créez le modèle suivant :

<pre>> &#123;&#123;#contact&#125;&#125;</pre><pre>>     &#123;&#123;name&#125;&#125;, &#123;&#123;phone&#125;&#125;</pre><pre>> &#123;&#123;/contact&#125;&#125;</pre>

Pour ce faire, vous devez configurer le module comme suit :


![](assets/word-template-fill-out-a-document-350x732.png)

Le module crée le document suivant :

```
> Jan Toman, 4445551234
> Eduard Salo, 4445552345
```

<!--

#### Loop tag with Fill a document with a batch of data module {#loop-tag-with-fill-a-document-with-a-batch-of-data-module}

**Example:** You can export Google contacts into a table that you create using loop tags.

The first module loads the template. The next module retrieves all contacts from the group you specify in [!DNL Google Contacts]. The aggregator module aggregates all values retrieved from Google Contacts and merges them into the template. And the last module saves the filled template to the desired location.

![](assets/word-template-batch-scenario-350x124.png)

You could use this scenario with the following template:

![](assets/word-template-batch-template-350x26.png)

To do this, you would set up the module as follows:

![](assets/word-template-batch-module-setup-350x323.png)

The module would create the following document:

![](assets/word-template-batch-document-350x46.png)
-->

## [!DNL Microsoft Word Template] modules

Ces modules ne nécessitent pas de connexion.

* [Remplissage d’un document](#fill-out-a-document)
* [Remplir un document avec un lot de données](#fill-a-document-with-a-batch-of-data)

### [!UICONTROL Remplissage d’un document] {#fill-out-a-document}

Ce module du transformateur permet de remplir un document avec les données que vous indiquez. Il peut être utilisé avec des balises de valeurs simples, des balises conditionnelles ou des balises de boucle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Délimiteur de début du texte remplacé]</td> 
   <td> <p>Saisissez le ou les caractères que vous souhaitez marquer au début du texte remplacé. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>Entrée <code>[[</code> si vous souhaitez remplacer un texte similaire à celui-ci : <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Délimiteur de fin du texte remplacé]</p> </td> 
   <td> <p>Saisissez le ou les caractères que vous souhaitez marquer la fin du texte remplacé. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>Entrée <code>]]</code> si vous souhaitez remplacer un texte similaire à celui-ci : <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fichier source]</td> 
   <td> <p> Mappez le fichier que vous souhaitez charger à partir du module précédent (par exemple, HTTP &gt; Obtenir un fichier ou un Dropbox &gt; Obtenir un module de fichier). Vous pouvez également saisir le fichier de données manuellement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du fichier rempli]</td> 
   <td>Saisissez un nom de fichier (extension incluse) pour le fichier de sortie cible.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source de données]</td> 
   <td> <p>Sélectionnez une option pour indiquer si les données que vous utilisez proviennent d’un formulaire ou d’une collecte de données brutes (données informatiques non traitées).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Il doit s’agir d’un tableau de collections dans lequel :</p> 
    <ul> 
     <li>Chaque collection correspond à une entrée de données et contient un élément . <code>entry</code></li> 
     <li>Élément <code>entry </code>contient une collection de la variable <code>key </code>et <code>value</code></li> 
     <li>Élément <code>key </code>contient le nom de la balise.</li> 
     <li>item <code>value </code>contient la valeur de la balise.</li> 
    </ul> 
    <p>Pour ajouter une entrée :</p>
    <ol> 
     <li> Cliquez sur <b>[!UICONTROL Ajouter un élément]</b>. </li> 
     <li>Sélectionnez le type de valeur de l’entrée.</li> 
     <li>Ajoutez le nom et la valeur. Pour plus d’informations, voir l’exemple du type de valeur choisi dans cet article. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Balise de valeur simple</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Balise de condition</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Balise de boucle</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Remplir un document avec un lot de données] {#fill-a-document-with-a-batch-of-data}

Ce module d’agrégation est utile si vos entrées de données sont des lots distincts. Avec ce module, vous pouvez facilement configurer la structure requise pour le champ Valeur et mapper les éléments à chaque élément de valeur. Contrairement au module Remplir un document , le champ Valeurs du module Remplir un document avec un lot de données n’autorise qu’une seule entrée contenant des variables.

Vous pouvez également utiliser ce module si vos entrées de données sont fournies sous la forme d’un tableau, en utilisant la variable *Itérateur* pour transformer le contenu du tableau en une série de lots.

Les valeurs réelles sont créées et renseignées pour chaque lot entrant. Le modèle est généré une fois tous les lots d’entrée traités.

Ce module d&#39;agrégation est particulièrement utile pour créer des listes ou des rapports.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module source]</td> 
   <td>Sélectionnez le module source de votre texte.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Délimiteur de début du texte remplacé]</td> 
   <td> <p>Saisissez le ou les caractères que vous souhaitez marquer au début du texte remplacé. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>Entrée <code>[[</code> si vous souhaitez remplacer un texte similaire à celui-ci : <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Délimiteur de fin du texte remplacé]</p> </td> 
   <td> <p>Saisissez le ou les caractères que vous souhaitez marquer la fin du texte remplacé. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>Entrée <code>]]</code> si vous souhaitez remplacer un texte similaire à celui-ci : <code>[[replace_me]]</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groupe [!UICONTROL par]</td> 
   <td> Définissez une expression contenant un ou plusieurs éléments mappés. Les données agrégées sont séparées sous Groupes avec la même valeur d’expression. Chaque groupe génère en tant que lot distinct contenant une clé avec l’expression évaluée et le texte agrégé. Vous pouvez ainsi utiliser la clé comme filtre dans les modules suivants.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arrêter le traitement après une agrégation vide]</td> 
   <td>Activez cette option pour arrêter le traitement lorsqu’une agrégation ne contient aucun lot.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fichier source]</td> 
   <td> <p> Mappez le fichier que vous souhaitez charger à partir du module précédent (par exemple, HTTP &gt; Obtenir un fichier ou un Dropbox &gt; Obtenir un module de fichier). Vous pouvez également saisir le fichier de données manuellement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du fichier rempli]</td> 
   <td>Saisissez un nom de fichier (extension incluse) pour le fichier de sortie cible.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source de données]</td> 
   <td> <p>Sélectionnez une option pour indiquer si les données que vous utilisez proviennent d’un formulaire ou d’une collecte de données brutes (données informatiques non traitées).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Il doit s’agir d’un tableau de collections dans lequel :</p> 
    <ul> 
     <li>Chaque collection correspond à une entrée de données et contient un élément . <code>entry</code></li> 
     <li>Élément <code>entry </code>contient une collection de la variable <code>key </code>et <code>value</code></li> 
     <li>Élément <code>key </code>contient le nom de la balise.</li> 
     <li>item <code>value </code>contient la valeur de la balise.</li> 
    </ul> 
    <p>Pour ajouter une entrée :</p>
    <ol> 
     <li> Cliquez sur <b>[!UICONTROL Ajouter un élément]</b>. </li> 
     <li>Sélectionnez le type de valeur de l’entrée.</li> 
     <li>Ajoutez le nom et la valeur. Pour plus d’informations, voir l’exemple du type de valeur choisi dans cet article. 
      <ul> 
       <li><a href="#simple-value-tag" class="MCXref xref">Balise de valeur simple</a></li> 
       <li><a href="#condition-tag" class="MCXref xref">Balise de condition</a></li> 
       <li><a href="#loop-tag" class="MCXref xref">Balise de boucle</a></li> 
      </ul></li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

