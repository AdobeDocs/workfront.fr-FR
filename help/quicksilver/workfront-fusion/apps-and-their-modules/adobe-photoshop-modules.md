---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Adobe Photoshop
description: Avec les modules Adobe Photoshop, vous pouvez lancer un scénario de fusion Adobe Workfront basé sur les événements de votre compte Adobe Photoshop, créer, lire ou mettre à jour des contrats et d’autres enregistrements, rechercher des enregistrements à l’aide de critères que vous avez définis et télécharger des documents.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: f20192ea-e363-4fba-8bd2-b1d50443918d
source-git-commit: 1de5018a13f1fbe4383ce9655bc3fe29612b1411
workflow-type: tm+mt
source-wordcount: '3966'
ht-degree: 18%

---

# Modules [!DNL Adobe Photoshop]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Photoshop] et les connecter à plusieurs applications et services tiers.


Si vous avez besoin d’instructions sur la création d’un scénario, voir [Création d’un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

+++**Développez pour afficher les exigences d’accès à la fonctionnalité de cet article.**

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
      <td>
        <p>[!UICONTROL Pro] ou un forfait supérieur</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td>
      <td >
        <p>[!UICONTROL Fusion Workfront pour l’automatisation et l’intégration du travail]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Produit</td>
      <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

&#42;&#42;Pour plus d’informations sur les [!DNL Adobe Workfront Fusion] licences, voir [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

+++

## Conditions préalables

Avant de pouvoir utiliser le connecteur [!DNL Adobe Photoshop], vous devez vous assurer que les conditions préalables suivantes sont remplies :

* Vous devez avoir un compte [!DNL Adobe Photoshop] actif.

## Créer une connexion à [!DNL Adobe Photoshop]

Pour créer une connexion pour vos modules [!DNL Adobe Photoshop] :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la zone Connexion.

1. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Nommez cette connexion.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Saisissez votre [!UICONTROL Adobe] [!UICONTROL ID client]. Vous pouvez le trouver dans la section de détails [!UICONTROL Credentials] de la variable [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Entrez votre [0} [!UICONTROL Client Secret]. [!DNL Adobe] Vous pouvez le trouver dans la section de détails [!UICONTROL Credentials] de la variable [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID du compte technique]</td>
        <td>Saisissez votre [!DNL Adobe] [!UICONTROL ID de compte technique]. Vous pouvez le trouver dans la section de détails [!UICONTROL Credentials] de la variable [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID d’organisation]</td>
        <td>Saisissez votre [!DNL Adobe] [!UICONTROL ID d’organisation]. Vous pouvez le trouver dans la section de détails [!UICONTROL Credentials] de la variable [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Clé privée]</td>
        <td>
          <p>Entrez la clé privée qui a été générée lors de la création de vos informations d’identification dans le [!DNL Adobe Developer Console]. </p>
          <p>Pour extraire votre clé privée ou votre certificat :</p>
          <ol>
            <li value="1">
              <p>Cliquez sur <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Sélectionnez le type de fichier que vous extrayez.</p>
            </li>
            <li value="3">
              <p>Sélectionnez le fichier contenant la clé privée ou le certificat.</p>
            </li>
            <li value="4">
              <p>Saisissez le mot de passe du fichier.</p>
            </li>
            <li value="5">
              <p>Cliquez sur <b>Enregistrer</b> pour extraire le fichier et revenir à la configuration de la connexion[!UICONTROL ].</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.

## Modules [!DNL Adobe Photoshop] et leurs champs

Lorsque vous configurez des modules [!DNL Adobe Photoshop], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Adobe Photoshop] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Appliquer les modifications Photoshop](#apply-psd-edits)
* [Corrigez automatiquement une image](#auto-color-correct-an-image)
* [Convertir le format d&#39;image](#convert-image-format)
* [Création d’un masque](#create-a-mask)
* [Création d’un PSD](#create-a-new-psd)
* [Modifier des calques de texte](#edit-text-layers)
* [Exécuter le flou de profondeur](#execute-depth-blur)
* [Exécution d’actions Photoshop](#execute-photoshop-actions)
* [Exécuter les actions Photoshop (JSON)](#execute-photoshop-actions-json)
* [Exécuter le recadrage de produit](#execute-product-crop)
* [Obtention des informations sur le calque](#get-layer-info)
* [Effectuer un appel API personnalisé](#make-a-custom-api-call)
* [Suppression de l’arrière-plan](#remove-background)
* [Remplacement d’un objet dynamique](#replace-a-smart-object)
* [Redimensionner une image](#resize-an-image)
* [Application d’un filigrane à une image](#watermark-an-image)

### Appliquer les modifications de PSD

Ce module d’action applique diverses modifications au niveau du document et du calque.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez modifier est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (entrée) Emplacement du fichier]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier à modifier. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options &gt; Document &gt; Taille de l’image) Hauteur]</p>
      </td>
      <td> Saisissez ou mappez la hauteur de l’image en pixels. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options &gt; Document &gt; Taille de l’image) Largeur]</p>
      </td>
      <td> Saisissez ou mappez la largeur de l’image en pixels. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options &gt; Document &gt; Taille de la zone de travail) Haut]</p>
      </td>
   <td> Saisissez ou mappez, en pixels, la coordonnée y du coin supérieur gauche du document. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options &gt; Document &gt; Taille de la zone de travail) Bas]</p>
      </td>
   <td> Saisissez ou mappez, en pixels, la coordonnée y du coin inférieur droit du document. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options &gt; Document &gt; Taille de la zone de travail à gauche)]</p>
      </td>
   <td> Saisissez ou mappez, en pixels, la coordonnée x du coin supérieur gauche du document. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options &gt; Document &gt; Taille de la zone de travail à droite)]</p>
      </td>
   <td> Saisissez ou mappez, en pixels, la coordonnée x du coin inférieur droit du document. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options &gt; Rognage du document)]</p>
      </td>
   <td> Sélectionnez Pixels transparents pour baser le rognage sur les pixels transparents de l’image. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options) Police par défaut]</p>
      </td>
   <td> Saisissez le nom complet du postscript de la police à utiliser comme valeur par défaut globale pour le document. Cette police sera utilisée pour tout calque de texte qui comporte une police manquante et aucune autre police n’a été spécifiquement fournie pour ce calque. Si cette police est manquante, l’option indiquée dans Gérer les polices manquantes prend effet. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options) Polices]</p>
      </td>
   <td> Pour chaque police dont le document a besoin, cliquez sur Ajouter un élément et saisissez l’emplacement de stockage et l’emplacement de fichier de la police. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options) Gérer les polices manquantes]</p>
      </td>
   <td> Sélectionnez l’action à effectuer en cas d’absence d’une ou de plusieurs polices dans le document. <ul><li><code>fail</code>: la tâche échoue et l’état est défini sur échec, avec les détails de l’erreur fournis dans la section détails de l’état.</li><li><code>useDefault</code>: la tâche réussira, cependant, toutes les polices manquantes seront remplacées par ArialMT par défaut.</li></ul></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options) Calques]</p>
      </td>
   <td> Pour chaque calque à ajouter, cliquez sur Ajouter un élément et renseignez les détails du calque. <p>Pour plus d’informations sur les options de calque, voir <a href="https://developer.adobe.com/firefly-services/docs/photoshop/api/photoshop_applyPsdEdits/">Appliquer les modifications de PSD</a> dans la documentation Adobe Photoshop.  </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Outputs]</td>
      <td>
        <p>Pour chaque fichier converti que vous souhaitez créer, cliquez sur Ajouter un élément et saisissez le stockage, l’emplacement et le type, comme indiqué dans ce tableau.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers où le nouveau fichier doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output Type)]</p>
      </td>
   <td>Sélectionnez le type de fichier dans lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">Remplacement de [!UICONTROL (sortie)]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà. Cela s’applique uniquement aux fichiers dans le stockage Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>



### Corrigez automatiquement une image

Ce module d’action corrige automatiquement la couleur de l’image spécifiée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez corriger par couleur est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (entrée) Emplacement du fichier]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier dont vous souhaitez corriger les couleurs. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers où le nouveau fichier doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output Type)]</p>
      </td>
   <td>Sélectionnez le type de fichier dans lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">Remplacement de [!UICONTROL (sortie)]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà. Cela s’applique uniquement aux fichiers dans le stockage Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>


### Convertir le format d&#39;image

Ce module d’action convertit un fichier en JPEG, PNG, PSD ou TIFF.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier dont vous souhaitez supprimer l’arrière-plan est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (entrée) Emplacement du fichier]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier duquel vous souhaitez supprimer l’arrière-plan. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Outputs]</td>
      <td>
        <p>Pour chaque fichier converti que vous souhaitez créer, cliquez sur Ajouter un élément et saisissez le stockage, l’emplacement et le type, comme indiqué dans ce tableau.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers où le nouveau fichier doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output Type)]</p>
      </td>
   <td>Sélectionnez le type de fichier dans lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">Remplacement de [!UICONTROL (sortie)]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà. Cela s’applique uniquement aux fichiers dans le stockage Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>



### Création d’un masque

Ce module d’action renvoie un fichier PNG avec un mât appliqué autour de l’objet.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers à partir duquel est stocké le fichier à partir duquel vous souhaitez créer un masque.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (entrée) Emplacement du fichier]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier à partir duquel vous souhaitez créer un masque. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier de masque doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du fichier de masque. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Remplacer]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà. Cela s’applique uniquement aux fichiers dans le stockage Adobe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Espace colorimétrique]</p>
      </td>
   <td>Indiquez si l’image de sortie utilise la couleur RGB ou RGBA. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Format de masque]</p>
      </td>
   <td>Indiquez si le masque doit être doux (plumes) ou binaire. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Optimize]</p>
      </td>
   <td>Sélectionnez Performance pour optimiser la vitesse ou Lot pour autoriser le temps d’attente. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Post-traitement]</p>
      </td>
   <td></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Version]</p>
      </td>
   <td>La valeur par défaut est 4.0</td> 
    </tr> 
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>

### Création d’un PSD

Ce module d’action crée un PSD avec des calques facultatifs et génère des rendus ou des enregistrements en tant que PSD.

Pour les champs liés à ce module, voir [Création d&#39;un PSD](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) dans la documentation Adobe Photoshop.

### Modifier des calques de texte

Ce module d’action modifie les calques de texte sur un fichier Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier d’entrée]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez modifier est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier d’entrée]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier à modifier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gérer les polices manquantes]</td>
      <td>
        <p>Sélectionnez l’action à effectuer en cas d’absence d’une ou de plusieurs polices dans le document. Si la police n’est pas fournie, le module utilise la police par défaut.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Police par défaut]  </td>
      <td>
        <p>Saisissez le nom complet du postscript de la police à utiliser comme valeur par défaut globale pour le document. Cette police sera utilisée pour tout calque de texte qui comporte une police manquante et aucune autre police n’a été spécifiquement fournie pour ce calque. Si cette police est manquante, l’option indiquée dans Gérer les polices manquantes prend effet.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Calques]</td>
   <td> <p>Pour plus d’informations sur les options de calque, voir <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">Modification de la couche de texte</a> dans la documentation Adobe Photoshop.</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier de sortie]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier modifié doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier de sortie]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Type de fichier de sortie]</p>
      </td>
   <td> Sélectionnez le type de fichier pour le fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Remplacer]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Sélectionnez le niveau de compression du fichier de sortie. </td> 
    </tr>
  </tbody>
</table>

### Exécuter le flou de profondeur

Ce module d’action exécute un flou de profondeur sur le fichier sélectionné.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier d’entrée]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez modifier est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier d’entrée]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier à modifier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier de sortie]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier modifié doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier de sortie]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Type de fichier de sortie]</p>
      </td>
   <td> Sélectionnez le type de fichier pour le fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Autres champs]</td>
      <td>
        <p>Pour plus d’informations sur les autres options de flou de profondeur, voir <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Execute Depth Blur </a> dans la documentation de l’API Adobe Photoshop.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Remplacer]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Sélectionnez le niveau de compression du fichier de sortie. </td> 
    </tr>
  </tbody>
</table>

### Exécuter les actions Photoshop

Ce module d’action exécute une action Photoshop sur l’image sélectionnée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier d’entrée]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez modifier est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier d’entrée]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier à modifier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier Actions]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier d’actions est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier d’actions]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier d’actions. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Nom de l’action]</p>
      </td>
   <td> Si vous souhaitez uniquement exécuter une action spécifique, vous pouvez spécifier l’action à lire à partir du jeu d’actions. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Police / Modèle / Stockage des formes]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez utiliser est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Police / Modèle / URL du fichier de forme]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier que vous souhaitez utiliser. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier de sortie]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier modifié doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier de sortie]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Type de fichier de sortie]</p>
      </td>
   <td> Sélectionnez le type de fichier pour le fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Remplacer]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Sélectionnez le niveau de compression du fichier de sortie. </td> 
    </tr>
  </tbody>
</table>

### Exécution d’actions Photoshop (JSON)

Ce module d’action exécute des actions Photoshop à l’aide de commandes JSON.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez modifier est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (entrée) Emplacement du fichier]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier à modifier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action JSON]</td>
      <td>
        <p>Saisissez la commande JSON de l’action que vous souhaitez effectuer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Polices / Modèles / Brosses / Images supplémentaires]</td>
      <td>
        <p>Pour chaque police, modèle, brosse ou image supplémentaire que vous souhaitez utiliser dans cette action, cliquez sur Ajouter un élément et saisissez l’emplacement de stockage et de fichier de l’élément.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Police / Modèle / URL du fichier de forme]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier que vous souhaitez utiliser. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sorties du stockage de fichiers]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier modifié doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier de sortie]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Type de fichier de sortie]</p>
      </td>
   <td> Sélectionnez le type de fichier pour le fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Remplacer]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Sélectionnez le niveau de compression du fichier de sortie. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Outputs]</td>
      <td>
        <p>Pour chaque fichier converti que vous souhaitez créer, cliquez sur Ajouter un élément et saisissez le stockage, l’emplacement et le type, comme indiqué dans ce tableau.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers où le nouveau fichier doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output Type)]</p>
      </td>
   <td>Sélectionnez le type de fichier dans lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">Remplacement de [!UICONTROL (sortie)]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà. Cela s’applique uniquement aux fichiers dans le stockage Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
      </tbody>
</table>

### Exécuter le recadrage de produit

Ce module d’action exécute Recadrage de produit sur l’image sélectionnée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier d’entrée]</td>
      <td>
        <p>Sélectionnez le service de fichiers où est stocké le fichier que vous souhaitez recadrer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier d’entrée]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier à recadrer. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Unit]</p>
      </td>
   <td> Indiquez si vous souhaitez décrire l’ajustement de hauteur et de largeur en pixels ou sous la forme d’un pourcentage. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Width]</p>
      </td>
   <td> Saisissez ou mappez la largeur de remplissage à ajouter. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Hauteur]</p>
      </td>
   <td> Saisissez ou mappez la hauteur de remplissage à ajouter. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier de sortie]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier modifié doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier de sortie]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Type de fichier de sortie]</p>
      </td>
   <td> Sélectionnez le type de fichier pour le fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Remplacer]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Sélectionnez le niveau de compression du fichier de sortie. </td> 
    </tr>
  </tbody>
</table>

### Obtention des informations sur le calque

Ce module d’action récupère les informations de calque du fichier de PSD spécifié.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier d’entrée]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier dont vous souhaitez récupérer les informations de couche est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier d’entrée]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier à partir duquel vous souhaitez récupérer les informations de calque. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Miniatures]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

### Effectuer un appel API personnalisé

Ce module d’action effectue un appel personnalisé à l’API Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Saisissez un chemin relatif à <code>https://image.adobe.io/pie/psdService</code>. Exemple : <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p>
        <p>Par exemple, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] ajoute automatiquement des en-têtes d’autorisation.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Saisissez la chaîne de requête.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Suppression de l’arrière-plan

Ce module d’action identifie le sujet principal de votre image et supprime l’arrière-plan.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier dont vous souhaitez supprimer l’arrière-plan est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (entrée) Emplacement du fichier]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier duquel vous souhaitez supprimer l’arrière-plan. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers où le nouveau fichier doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Remplacer]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà. Cela s’applique uniquement aux fichiers dans le stockage Adobe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Espace colorimétrique]</p>
      </td>
   <td>Indiquez si l’image de sortie utilise la couleur RGB ou RGBA. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Format de masque]</p>
      </td>
   <td>Indiquez si les bords de l’image doivent être doux (en plumes) ou binaires. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Optimize]</p>
      </td>
   <td>Sélectionnez Performance pour optimiser la vitesse ou Lot pour autoriser le temps d’attente. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Post-traitement]</p>
      </td>
   <td></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Version]</p>
      </td>
   <td>La valeur par défaut est 4.0</td> 
    </tr> 
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>



### Remplacement d’un objet dynamique

Ce module d’action remplace un objet dynamique dans un calque de PSD et génère de nouveaux rendus.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers où est stocké l’objet dynamique.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (entrée) Emplacement du fichier]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’objet dynamique. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Calques]</p>
      </td>
   <td>Pour chaque calque à ajouter à l’objet dynamique, cliquez sur Ajouter un élément et saisissez le nom ou l’identifiant de l’objet, le service de fichiers où l’objet dynamique est stocké et l’URL ou le chemin d’accès du calque.<p>Pour obtenir des descriptions des paramètres avancés de cette zone, voir <a href="https://developer.adobe.com/firefly-services/docs/photoshop/api/photoshop_replaceSmartObject/">Remplacer un objet dynamique</a> dans la documentation de l’API Photoshop. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Outputs]</td>
      <td>
        <p>Pour chaque nouveau rendu que vous souhaitez que le module génère, cliquez sur Ajouter un élément et renseignez les champs suivants. Vous pouvez avoir un maximum de 25 fichiers de sortie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers où le nouveau fichier doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Width]</p>
      </td>
   <td> Largeur, en pixels, du fichier de sortie. Le module conserve les proportions d’origine. </td> 
    </tr>
    <tr>
      <td role="rowheader">Remplacement de [!UICONTROL (sortie)]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà. Cela s’applique uniquement aux fichiers dans le stockage Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>



### Redimensionner une image

Cette action redimensionne une image en utilisant les mêmes proportions.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez redimensionner est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Emplacement du fichier]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier que vous souhaitez redimensionner. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Outputs]</td>
      <td>
        <p>Pour chaque fichier converti que vous souhaitez créer, cliquez sur Ajouter un élément et saisissez les options de stockage, d’emplacement et autres répertoriées dans ce tableau.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Type]</p>
      </td>
   <td>Sélectionnez le type de fichier dans lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Width]</p>
      </td>
   <td>Saisissez un nombre représentant la largeur, en pixels, de l’image redimensionnée. Les proportions seront conservées.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Largeur max.]</p>
      </td>
   <td>Lorsque la largeur est de 0, la valeur Max. avec peut être fournie pour obtenir la taille. La largeur maximale est prioritaire, car elle est inférieure à la largeur du document.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Remplacer]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà. Cela s’applique uniquement aux fichiers dans le stockage Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Rogner sur la zone de travail]</p>
      </td>
   <td>Sélectionnez Oui pour rogner les rendus à la taille de la zone de travail ou Non pour créer la taille de la couche des rendus.</td> 
    </tr>
    </tbody>
</table>

### Application d’un filigrane à une image

Ce module d’action ajoute un filigrane à l’image sélectionnée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour plus d’informations sur l’établissement d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer la connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Stockage de base/d’entrée)]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier auquel vous souhaitez ajouter un filigrane est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Emplacement du fichier [!UICONTROL (de base/d’entrée)]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin du fichier auquel vous souhaitez ajouter un filigrane. </td> 
    </tr>
    <tr>
      <td role="rowheader">Stockage [!UICONTROL (filigrane/entrée)]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le filigrane que vous souhaitez ajouter est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Stockage [!UICONTROL (filigrane/entrée)]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le filigrane que vous souhaitez ajouter est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Hauteur [!UICONTROL (Filigrane/limites)]</p>
      </td>
   <td>Saisissez ou mappez la hauteur souhaitée du filigrane en pixels.</td> 
    <tr>
      <td role="rowheader">
        <p>Largeur [!UICONTROL (Filigrane/limites)]</p>
      </td>
   <td> Saisissez ou mappez la largeur souhaitée du filigrane en pixels. </td> 
    </tr>  
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Filigrane/limites gauche)]</p>
      </td>
   <td> Saisissez ou mappez la distance en pixels du côté gauche de l’image que doit être le filigrane.</td> 
    </tr>  
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Filigrane/limites Haut)]</p>
      </td>
   <td> Saisissez ou mappez la distance en pixels du haut de l’image que doit être le filigrane.</td> 
    </tr>  
    </tr>  
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier filigrane doit être stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du fichier filigrane. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output Type)]</p>
      </td>
   <td>Sélectionnez le type de fichier dans lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Width]</p>
      </td>
   <td> Largeur, en pixels, du fichier de sortie. Le module conserve les proportions d’origine. </td> 
    </tr>
    <tr>
      <td role="rowheader">Remplacement de [!UICONTROL (sortie)]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera tout fichier de sortie qui existe déjà. Cela s’applique uniquement aux fichiers dans le stockage Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>















