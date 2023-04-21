---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Airtable
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
exl-id: 5d061b23-0a39-44e6-ac9b-0ef5ac7e9ab4
source-git-commit: 9460e14a66653eaf1856cdf5c1ab3213859f354a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Modules Airtable


Avec le [!DNL Airtable] connecteur pour [!DNL Adobe Workfront Fusion], vous pouvez démarrer un scénario en fonction des événements de votre [!DNL Airtable] créer, charger et mettre à jour des enregistrements, rechercher des enregistrements et effectuer des appels d’API personnalisés vers l’API Airtable.

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

Vous devez disposer d’un compte Airtable pour utiliser la fonctionnalité de cet article.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## Connexion d’Airtable à Workfront Fusion {#connect-airtable-to-workfront-fusion}

<!--

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
-->
1. Ouvrez Workfront Fusion et le **Création d’une connexion** de la boîte de dialogue du module souhaité.
1. Saisissez le nom de la connexion.
1. (Facultatif) Cliquez sur Afficher les paramètres avancés, puis saisissez votre ID client Airtable et votre secret client.
1. Cliquez sur le bouton **Continuer** pour créer la connexion et revenir au module.

## Modules Airtable et leurs champs

### Enregistrements

* [Création d’un enregistrement](#create-a-record)
* [Suppression d’un enregistrement](#delete-a-record)
* [Obtention d’un enregistrement](#get-a-record)
* [Enregistrements de recherche](#search-records)
* [Mettre à jour un enregistrement](#update-a-record)
* [Insérer un enregistrement](#upsert-a-record)
* [Surveillance des enregistrements](#watch-records)
* [Regarder les réponses](#watch-responses)
* [Effectuer un appel API](#make-an-api-call)

#### Création d’un enregistrement {#create-a-record}

Ce module d’action crée un nouvel enregistrement.

Vous indiquez les données que vous souhaitez voir contenues dans l’enregistrement et leur emplacement de stockage.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connexion </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte Airtable à Workfront Fusion, voir <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connexion d’Airtable à Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Sélectionnez la base à laquelle doit appartenir le nouvel enregistrement.</p> </td> 
  </tr> 
  <tr> 
   <td>Tableau </td> 
   <td> <p>Sélectionnez la table à laquelle doit appartenir le nouvel enregistrement.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Enregistrement</p> </td> 
   <td> <p>Saisissez les valeurs du nouvel enregistrement. Les champs disponibles dépendent du tableau que vous avez sélectionné.</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><strong>Emails</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Liens intelligents</td> 
   <td> <p>Activez cette option pour saisir des noms plutôt que des identifiants d’enregistrement pour les champs liés à une autre table. L'enregistrement est automatiquement créé dans la table liée en cas d'absence de correspondance.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Suppression d’un enregistrement {#delete-a-record}

Ce module d’action supprime un enregistrement particulier.

Vous spécifiez l’identifiant et les emplacements de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connexion </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte Airtable à Workfront Fusion, voir <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connexion d’Airtable à Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Sélectionnez la base contenant l’enregistrement que vous souhaitez supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>Tableau </td> 
   <td> <p>Sélectionnez la table contenant l'enregistrement à supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>Record ID</td> 
   <td> <p>Saisissez ou mappez l’identifiant Airtable unique de l’enregistrement que vous souhaitez que le module supprime. Vous pouvez récupérer l’ID, par exemple, à l’aide du module Enregistrements de recherche .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Obtention d’un enregistrement {#get-a-record}

Ce module d’action récupère les détails de l’enregistrement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connexion </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte Airtable à Workfront Fusion, voir <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connexion d’Airtable à Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Sélectionnez la base contenant la table avec l'enregistrement que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td>Tableau</td> 
   <td> <p> Sélectionnez la table contenant l'enregistrement pour lequel vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
  <tr> 
   <td>Record ID</td> 
   <td> <p> Saisissez ou mappez l’identifiant de l’enregistrement pour lequel vous souhaitez récupérer des détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Enregistrements de recherche {#search-records}

Ce module de recherche recherche recherche les enregistrements dans un objet d’Airtable correspondant à la requête que vous spécifiez.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connexion </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte Airtable à Workfront Fusion, voir <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connexion d’Airtable à Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Sélectionnez la base à rechercher pour les enregistrements.</p> </td> 
  </tr> 
  <tr> 
   <td>Tableau </td> 
   <td> <p>Sélectionnez la table à rechercher dans les enregistrements.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Formule</p> </td> 
   <td> <p>Formule de filtrage des enregistrements. La formule est évaluée pour chaque enregistrement et si le résultat n’est pas <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>ou <code>#Error!</code> l’enregistrement est inclus dans la réponse.</p> <p>Si elle est combinée avec la fonction <code>view</code>, seuls les enregistrements de cette vue qui correspondent à la formule sont renvoyés.</p> <p>Par exemple, pour inclure uniquement les enregistrements dont le nom n’est pas vide, transmettez :<code> NOT({Name} = '')</code></p> <p>Pour en savoir plus, recherchez des informations sur les références de champs de formule dans la documentation d’assistance sur la table.</p> </td> 
  </tr> 
  <tr> 
   <td>Trier </td> 
   <td> <p>Sélectionnez la direction du tri et le champ selon lequel vous souhaitez trier les résultats.</p> </td> 
  </tr> 
  <tr> 
   <td>Afficher </td> 
   <td> <p>Sélectionnez la vue dans laquelle vous souhaitez rechercher des enregistrements.</p> </td> 
  </tr> 
  <tr> 
   <td>Limite</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Mettre à jour un enregistrement {#update-a-record}

Ce module d’action met à jour un enregistrement particulier.

Vous indiquez l’identifiant de l’enregistrement et les nouvelles données que vous souhaitez qu’il contienne.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connexion </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte Airtable à Workfront Fusion, voir <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connexion d’Airtable à Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Sélectionnez la base contenant l'enregistrement que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>Tableau </td> 
   <td> <p>Sélectionnez la table contenant l'enregistrement que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>Record ID </td> 
   <td> <p>Saisissez ou mappez l’identifiant Airtable unique de l’enregistrement que vous souhaitez que le module soit mis à jour. Vous pouvez récupérer l’ID, par exemple, à l’aide du module Enregistrements de recherche .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Enregistrement</p> </td> 
   <td> <p>Saisissez les valeurs du nouvel enregistrement. Les champs disponibles dépendent de la table sélectionnée.</p> <!--<p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Liens intelligents</td> 
   <td> <p>Saisissez des noms plutôt que des identifiants d’enregistrement pour les champs liés à une autre table. L'enregistrement est automatiquement créé dans la table liée en cas d'absence de correspondance.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Mettre à jour un enregistrement

Ce module d’action met à jour ou insère un enregistrement particulier.

Vous indiquez l’identifiant de l’enregistrement et les nouvelles données que vous souhaitez qu’il contienne.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connexion </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte Airtable à Workfront Fusion, voir <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connexion d’Airtable à Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Sélectionnez la base contenant l'enregistrement que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>Tableau </td> 
   <td> <p>Sélectionnez la table contenant l'enregistrement que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>Record ID </td> 
   <td> <p>Si vous mettez à jour un enregistrement, saisissez ou mappez l’identifiant Airtable unique de l’enregistrement que vous souhaitez que le module soit mis à jour. Vous pouvez récupérer l’ID, par exemple, à l’aide du module Enregistrements de recherche .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Enregistrement</p> </td> 
   <td> <p>Saisissez les valeurs du nouvel enregistrement. Les champs disponibles dépendent de la table sélectionnée.</p> <!-- <p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Liens intelligents</td> 
   <td> <p>Saisissez des noms plutôt que des identifiants d’enregistrement pour les champs liés à une autre table. L'enregistrement est automatiquement créé dans la table liée en cas d'absence de correspondance.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Surveillance des enregistrements {#watch-records}

Ce module de déclenchement lance un scénario lorsqu’un enregistrement est créé ou mis à jour dans la table spécifiée.

>[!NOTE]
>
>Pour utiliser ce module, le champ Heure de création ou Heure de dernière modification doit être créé dans votre tableau.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connexion </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte Airtable à Workfront Fusion, voir <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connexion d’Airtable à Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Base </td> 
   <td> <p>Sélectionnez la base que vous souhaitez suivre pour de nouveaux enregistrements.</p> </td> 
  </tr> 
  <tr> 
   <td>Tableau </td> 
   <td> <p>Sélectionnez la table à surveiller pour les nouveaux enregistrements.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Configuration des déclencheurs</p> </td> 
   <td> <p>Champ Déclencheur</p> <p>A <code>Created Time</code> ou <code>Last Modified Time</code> champ utilisé pour trier les enregistrements. Si vous n’avez pas de <code>Created Time</code> ou <code>Last Modified Time</code> dans votre schéma, vous devez en créer un. </p> <p>Champ de libellé</p> <p>Champ utilisé comme libellé pour un enregistrement, par exemple, dans la boîte de dialogue Choisir où commencer .</p> </td> 
  </tr> 
  <tr> 
   <td>Limite</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit surveiller pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td>Afficher</td> 
   <td> <p>Sélectionnez la vue à utiliser.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Formule</p> </td> 
   <td> <p>Formule de filtrage des enregistrements. La formule est évaluée pour chaque enregistrement et si le résultat n’est pas <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>ou <code>#Error!</code> l’enregistrement est inclus dans la réponse.</p> <p>Si elle est combinée avec la fonction <code>view</code>, seuls les enregistrements de cette vue qui correspondent à la formule sont renvoyés.</p> <p>Par exemple, pour inclure uniquement les enregistrements dont le nom n’est pas vide, transmettez :<code> NOT({Name} = '')</code></p> <p>Pour en savoir plus, consultez les informations sur les références de champ de formule dans la documentation de l’assistance Airtable.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Regarder les réponses

Ce module de déclenchement lance un scénario lorsqu’un formulaire est envoyé.

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement pour le forfait Airtable Pro payant.

L’URL webhook doit être générée dans Workfront Fusion, puis ajoutée à la configuration de formulaire dans Airtable.

1. Ajoutez le module Watch New Responses à votre scénario Workfront Fusion.
1. Générez et copiez l’URL du webhook.

   Pour obtenir des instructions, voir [Triggers instantanés (webhooks) dans Adobe Workfront Fusion](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

1. Connectez-vous à votre compte Airtable.
1. Ouvrez la Base et le tableau à utiliser pour le formulaire et créez une vue de formulaire.
1. Définissez le formulaire selon vos besoins, faites défiler le formulaire vers le bas et activez l’option Rediriger vers l’URL après l’envoi du formulaire.
1. Saisissez l’URL Webhook générée à l’étape 2 de la boîte de dialogue affichée et ajoutez ?record_id={record_id} juste après l’URL webhook pour inclure l’ID d’enregistrement dans la sortie du module, puis cliquez sur Enregistrer. L’URL qui en résulte, par exemple, se présente comme suit :
1. Revenez à votre scénario de fusion Workfront et exécutez le module Watch Responses uniquement pour charger les champs d’Airtable et pour pouvoir mapper ces champs dans les autres modules.
1. Envoyez le formulaire dans Airtable, où l’option Rediriger vers l’URL après l’envoi du formulaire est activée et où l’URL Webhook est ajoutée (étape 6 ci-dessus).

   Le module Watch Responses est déclenché et les données souhaitées sont chargées.

1. Ajoutez le module Airtable > Get a Record juste après le module Airtable > Watch Responses et mappez le paramètre record_id au champ Record ID .

Désormais, chaque fois que le formulaire est envoyé, le module Watch Responses dans votre scénario Workfront Fusion est déclenché et le module Get a Record renvoie les détails du formulaire envoyé.

#### Effectuer un appel API

#### Appel API personnalisé

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL Airtable] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL Airtable] modules.

L’action est basée sur le type d’entité (type d’objet Allocadia) que vous spécifiez.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connexion</p> </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte Airtable à Workfront Fusion, voir <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Connexion d’Airtable à Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Saisissez un chemin relatif à <code>https://api.airtable.com/}</code>. Exemple: <code>v0/{base}/{table}</code> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">En-têtes</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Chaîne de requête</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’une clé et d’une valeur.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Corps</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
