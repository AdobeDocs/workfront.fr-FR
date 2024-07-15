---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Google Docs
description: Les modules Adobe Workfront Fusion  [!DNL Google Docs]  vous permettent de surveiller, créer, modifier et récupérer des documents dans vos  [!DNL Google Docs]  et  [!DNL Google Docs]  (pour les  [!DNL Google Workspace]  utilisateurs).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '4085'
ht-degree: 8%

---

# Modules [!DNL Google Docs]

Les modules [!DNL Adobe Workfront Fusion] [!DNL Google Docs] vous permettent de surveiller, créer, modifier et récupérer des documents dans vos [!DNL Google Docs] et [!DNL Google Docs] (pour les utilisateurs de [!DNL Google Workspace]).

Pour utiliser [!DNL Google Docs] avec [!DNL Adobe Workfront Fusion], il est nécessaire d&#39;avoir un compte [!DNL Google]. Si vous n&#39;avez pas encore de compte [!DNL Google], vous pouvez en créer un sur la page d&#39;aide du compte [!DNL Google].

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Pour utiliser les modules [!DNL Google Docs], vous devez disposer d’un compte Google.

## Modules [!DNL Google Docs] et leurs champs

Lorsque vous configurez [!DNL Google Docs] modules, [!UICONTROL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Google Docs] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Document

* [[!UICONTROL Surveiller les documents]](#watch-documents)
* [[!UICONTROL Liste de documents]](#list-documents)
* [[!UICONTROL Obtenir le contenu d’un document]](#get-content-of-a-document)
* [[!UICONTROL Créer un document]](#create-a-document)
* [[!UICONTROL Créer un document à partir d’un modèle]](#create-a-document-from-a-template)
* [[!UICONTROL Insérer un paragraphe dans un document]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL Insérer une image dans un document]](#insert-an-image-to-a-document)
* [[!UICONTROL Remplacer une image par une nouvelle image]](#replace-an-image-with-a-new-image)
* [[!UICONTROL Remplacer du texte dans un document]](#replace-text-in-a-document)
* [[!UICONTROL Télécharger un document]](#download-a-document)
* [[!UICONTROL Supprimer un document]](#delete-a-document)

#### [!UICONTROL Surveiller les documents]

Ce module de déclenchement renvoie les détails du document lorsqu’un nouveau document est créé ou modifié dans le dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents de contrôle]</td> 
   <td> <p style="color: #000000;">Indiquez si vous souhaitez regarder les documents créés ([!UICONTROL Par date de création]) ou modifiés ([!UICONTROL Par date de modification]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur à surveiller.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier à surveiller pour les documents créés ou modifiés.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier à surveiller pour les documents créés ou modifiés.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé à regarder.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Shared Drive] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Définissez le nombre maximal de documents que Workfront Fusion renvoie dans un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Liste de documents]

Ce module d’action récupère une liste de documents du dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur à partir duquel vous souhaitez répertorier les documents.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez répertorier les documents.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez répertorier les documents.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé à partir duquel vous souhaitez répertorier les documents.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Définissez le nombre maximal de retours de documents [!DNL Workfront Fusion] dans un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir le contenu d’un document]

Ce module d’action récupère un document spécifié.

Vous devrez peut-être étendre vos autorisations.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtention du contenu d’un document]</td> 
   <td> <p>Choisissez si vous souhaitez mapper l’ID du document ou sélectionnez le document manuellement dans le menu déroulant.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur contenant le document que vous souhaitez récupérer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier contenant le document que vous souhaitez récupérer.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier contenant le document que vous souhaitez récupérer.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé qui contient le document que vous souhaitez récupérer.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Sélectionnez l’objet à renvoyer dans la sortie du module.</p> 
    <ul> 
     <li>[!UICONTROL Image] (par défaut)</li> 
     <li>[!UICONTROL Dessin]</li> 
     <li>[!UICONTROL Graphique]</li> 
    </ul> <p>Remarque :  <p>Pour effectuer un mappage supplémentaire de ces objets, utilisez la valeur [!UICONTROL Inline Objects Array] dans la sortie de ce module (au lieu de [!UICONTROL inlineObjects]).</p> <p>Les objets [!UICONTROL Inline Objects Array] sont triés dans l’ordre dans lequel ils apparaissent dans le document. Cela facilitera le traitement.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un document]

Ce module d’action permet de créer un nouveau document dans le dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez créer un document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez créer un document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel vous souhaitez créer un document.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
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

#### [!UICONTROL Créer un document à partir d’un modèle]

Ce module d’action crée une copie d’un document de modèle existant et remplace toutes les balises. Ce module permet également aux utilisateurs de remplacer les images par de nouvelles images par URL.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Créer un document à partir d’un modèle]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par mappage]</strong> <br> Sélectionnez cette option pour mapper le modèle de document.</li> 
     <li><strong>[!UICONTROL Par liste déroulante]</strong> <br>Sélectionnez cette option pour choisir le modèle de document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve votre modèle. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve votre modèle.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve votre modèle.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé où se trouve votre modèle.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Saisissez les valeurs qui seront saisies au lieu des variables dans le nouveau document.</p> 
    <ul> 
     <li><strong>[!UICONTROL Balises]</strong> <br>Saisissez les balises contenues dans le modèle de document. N’utilisez pas <code>&#123;&#123;&#125;&#125;</code>. Exemple : utilisez <code>name</code> au lieu de <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Valeur remplacée]</strong><br>Saisissez la valeur de la balise.</li> 
    </ul> <p>Par exemple, la variable<code> &#123;&#123;name&#125;&#125;</code> du document source s’affiche comme champ de nom ici, où la valeur peut être insérée, par exemple <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Remplacement d’images]</p> </td> 
   <td> <p>Saisissez le lien vers l’[!UICONTROL ID d’objet image] et l’[!UICONTROL URL d’image] qui remplaceront l’image actuelle.</p> <p>Remarque : vous pouvez récupérer les ID d’image à l’aide du module [!UICONTROL Obtenir un document] , où les ID sont contenus dans le tableau [!UICONTROL Tableau d’objets en ligne].</p> <p>Nous vous recommandons d’ajouter du texte ALT aux images de votre document [!DNL Google]. </p> <p>Pour ajouter un texte ALT à l’image [!DNL Google Docs] :</p> 
    <ol> 
     <li value="1">Cliquez avec le bouton droit de la souris sur l’image.</li> 
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
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez créer le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel vous souhaitez créer le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel vous souhaitez créer le document.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insérer un paragraphe dans un document]

Ce module d’action ajoute ou insère un nouveau paragraphe dans un document existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sélectionner un document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par mappage]</strong> <br>Sélectionnez cette option pour mapper le document.</li> 
     <li><strong>[!UICONTROL Par liste déroulante]</strong> <br> Sélectionnez cette option pour choisir le document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document auquel vous souhaitez ajouter un paragraphe. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter un paragraphe, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter un paragraphe, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document auquel vous souhaitez ajouter un paragraphe, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
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
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Saisissez le numéro de l'index dans lequel vous souhaitez insérer votre texte. Vous pouvez utiliser le module [!UICONTROL Obtenir un document] pour récupérer le numéro de l’index.</p> <p>Pour afficher tous les caractères (y compris les caractères masqués) du document, vous pouvez utiliser le module complémentaire [!UICONTROL Afficher]. Le module complémentaire se trouve sous [!UICONTROL Modules complémentaires] &gt; [!UICONTROL Obtenir des modules complémentaires]. Recherchez [!UICONTROL Show] et installez le module complémentaire [!UICONTROL Show].</p> </li> 
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

#### [!UICONTROL Insérer une image dans un document]

Ce module d’action insère une image de l’URL vers le document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sélectionner un document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par mappage]</strong> <br> Sélectionnez cette option pour mapper le modèle de document.</li> 
     <li><strong>[!UICONTROL Par liste déroulante]</strong> <br> Sélectionnez cette option pour choisir le document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document auquel vous souhaitez ajouter une image. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter une image, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter une image, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document auquel vous souhaitez ajouter une image, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
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

#### [!UICONTROL Remplacer une image par une nouvelle image]

Ce module d’action remplace une image existante. Les proportions de l’image d’origine seront conservées.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sélectionner un document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par mappage]</strong> <br> Sélectionnez cette option pour mapper le modèle de document.</li> 
     <li><strong>[!UICONTROL Par liste déroulante]</strong> <br> Sélectionnez cette option pour choisir le document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document à remplacer par une image. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à remplacer par une image, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à remplacer par une image, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document à remplacer par une image, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Image URL]</p> </td> 
   <td> <p>Saisissez ou mappez l’URL de la nouvelle image qui remplacera l’image existante.</p> <p>Les images sont répertoriées dans l’ordre dans lequel elles apparaissent dans le document. Par exemple, <code>Body: Image No. 1</code> est la première image du document.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remplacer du texte dans un document]

Ce module d’action remplace le texte dans un document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sélectionner un document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par mappage]</strong> <br> Sélectionnez cette option pour mapper le modèle de document.</li> 
     <li><strong>[!UICONTROL Par liste déroulante]</strong> <br> Sélectionnez cette option pour choisir le document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document auquel vous souhaitez ajouter du texte. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter du texte, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document auquel vous souhaitez ajouter du texte, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document auquel vous souhaitez ajouter du texte, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
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

#### [!UICONTROL Télécharger un document]

Ce module d’action convertit et télécharge le document sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document à télécharger.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à télécharger, puis sélectionnez-le.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à télécharger, puis sélectionnez-le.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document à télécharger, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Sélectionnez le format de fichier cible du document téléchargé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un document]

Ce module d’action supprime un document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document que vous souhaitez supprimer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à supprimer, puis sélectionnez-le.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document à supprimer, puis sélectionnez-le.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document à supprimer, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared Drive]</td> 
   <td> <p>Sélectionnez le lecteur contenant le document à télécharger, puis sélectionnez un document. Cette option est disponible si vous avez sélectionné [!DNL Google Docs] dans le champ [!UICONTROL Choisir un lecteur] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Document ID]</td> 
   <td> <p> Sélectionnez ou mappez le document dans lequel vous souhaitez remplacer une ou plusieurs images.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)
* [[!UICONTROL  Faire en sorte que tous les liens d’un document puissent faire l’objet d’un clic]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL Effectuer un appel API]

Ce module d’action vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Saisissez un chemin relatif à <code>https://docs.googleapis.com/</code>. Exemple : <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Saisissez la chaîne de requête.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** L’appel API suivant récupère les détails du document spécifié dans vos documents Google :

**URL :**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Méthode :**

[!UICONTROL GET]

![](assets/api-call-example.png)

Vous trouverez des détails sur le document récupéré dans la sortie du module sous [!UICONTROL Bundle] > [!UICONTROL Body].

![](assets/api-output.png)

#### [!UICONTROL  Faire en sorte que tous les liens d’un document puissent faire l’objet d’un clic]

Ce module d’action recherche tous les liens du document et permet de les cliquer.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Google] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Créer tous les liens dans un document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Par mappage]</strong> <br> Sélectionnez cette option pour mapper le modèle de document.</li> 
     <li><strong>[!UICONTROL Par liste déroulante]</strong> <br> Sélectionnez cette option pour choisir le document dans le menu déroulant.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez le type de lecteur sur lequel se trouve le document sur lequel vous souhaitez que les liens puissent être cliqués. Cette option est disponible si vous avez sélectionné [!UICONTROL par liste déroulante] dans le champ précédent.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mon Lecteur]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document sur lequel vous souhaitez que les liens puissent faire l’objet d’un clic, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL Partagé Avec Moi]</strong> </p> <p>Sélectionnez le dossier dans lequel se trouve le document sur lequel vous souhaitez que les liens puissent faire l’objet d’un clic, puis sélectionnez le document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Lecteur partagé]</strong> (disponible uniquement pour les utilisateurs de [!DNL Google Workspace])</p> <p>Indiquez si vous souhaitez [!UICONTROL Utiliser l’accès administrateur de domaine]. Si vous sélectionnez [!UICONTROL Oui], la demande est émise en tant qu’administrateur de domaine, et tous les lecteurs partagés dans lesquels le demandeur est un administrateur sont renvoyés.</p> <p>Sélectionnez le lecteur partagé sur lequel se trouve le document sur lequel vous souhaitez que les liens puissent faire l’objet d’un clic, puis sélectionnez le document.</p> <p>Remarque : Si vous avez sélectionné l’option [!DNL Google Docs] dans ce champ et que vous n’êtes pas un utilisateur [!DNL Google Workspace], l’erreur <code>[400] Invalid Value</code> est renvoyée.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared Drive]</td> 
   <td> <p>Sélectionnez le lecteur contenant le document dans lequel vous souhaitez mettre à jour les liens, puis sélectionnez un document. Cette option est disponible si vous avez sélectionné [!DNL Google Docs] dans le champ [!UICONTROL Choisir un lecteur].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Document ID]</td> 
   <td> <p> Sélectionnez ou mappez le document dans lequel vous souhaitez mettre à jour les liens.</p> </td> 
  </tr> 
 </tbody> 
</table>
