---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Adobe Firefly de modules
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Firefly], ainsi que de la connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: f20192ea-e363-4fba-8bd2-b1d50443918d
source-git-commit: 4f583c7826625e08af6b63b21cacf9c770b11567
workflow-type: tm+mt
source-wordcount: '1215'
ht-degree: 20%

---

# Modules [!DNL Adobe Firefly]

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Firefly], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Création d’un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>Nouveau : [!UICONTROL Standard]</p><p>Ou</p><p>Actuel : [!UICONTROL Travail] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Actuel : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Hérité : Tout </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Nouveau :</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] Plan : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan : [!DNL Workfront Fusion] est inclus.</li></ul>
   <p>Ou</p>
   <p>Actuel : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Avant d’utiliser la variable [!DNL Adobe Firefly] , vous devez vous assurer que les conditions préalables suivantes sont remplies :

* Vous devez disposer d’un [!DNL Adobe Firefly] compte .

## Créer une connexion à [!DNL Adobe Firefly]

Pour créer une connexion pour votre [!DNL Adobe Firefly] modules :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la zone Connexion .

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
          <p>Saisissez un nom pour cette connexion.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Indiquez si vous vous connectez à un environnement de production ou hors production.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Choisissez si vous vous connectez à un compte de service ou à un compte personnel.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Saisissez votre [!UICONTROL Adobe] [!UICONTROL ID client]. Vous pouvez le trouver dans la section de détails [!UICONTROL Credentials] de la variable [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre [!DNL Adobe] [!UICONTROL Client Secret]. Vous pouvez le trouver dans la section de détails [!UICONTROL Credentials] de la variable [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.

## Modules [!DNL Adobe Firefly] et leurs champs

Lorsque vous configurez des modules [!DNL Adobe Firefly], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Adobe Firefly] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Effectuer un appel API personnalisé

Ce module d’action effectue un appel personnalisé à l’API du Firefly.

Pour connaître les API disponibles spécifiques, voir [API ADOBE FIREFLY](https://developer.adobe.com/firefly-services/docs/firefly-api/) dans la documentation Adobe Developer.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Firefly], voir <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Créer une connexion à [!DNL Adobe Firefly]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Saisissez un chemin relatif à <code>https://firefly-api-enterprise-stage.adobe.io/</code>.</p>
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
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Développer une image

Ce module d’action développe une image, éventuellement avec le contenu d’une invite que vous fournissez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Créer une connexion à [!DNL Adobe Firefly]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invite]</td> 
   <td>Saisissez ou mappez une invite pour le contenu avec lequel vous souhaitez développer l’image. Si aucune invite n’est fournie, l’image est développée avec du contenu correspondant à l’image d’origine.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Format d’image étendu]</td> 
   <td>Sélectionnez le format de fichier sous lequel l’image étendue sera enregistrée.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>  <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom du fichier image et le fichier image (données) du fichier source.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Sélectionnez la taille de l’image étendue.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Saisissez ou mappez un entier. Vous pouvez utiliser cette même source dans un autre module Développer une image pour générer une image similaire avec différents styles. </td> 
  </tr> 
 </tbody> 
</table>

## Renseignement d’une image

Ce module d’action remplit la zone masquée d’une image, éventuellement avec le contenu d’une invite que vous fournissez.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Créer une connexion à [!DNL Adobe Firefly]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invite]</td> 
   <td>Saisissez ou mappez une invite pour le contenu avec lequel vous souhaitez remplir l’image. Si aucune invite n’est fournie, l’image est remplie avec du contenu correspondant à l’image d’origine.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Format d’image rempli]</td> 
   <td>Sélectionnez le format de fichier sous lequel l’image remplie sera enregistrée.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Image]</td> 
   <td>  <p> Cliquez sur <b>Ajout d’une image</b>. Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom du fichier image et les données image du fichier source.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Masque]</td> 
   <td>  <p> Cliquez sur <b>Ajouter un masque</b>. Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom du fichier de masque et les données de masque du fichier source. Le fichier Masque représente le masque personnalisé qui sera rempli avec le contenu généré.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Sélectionnez la taille de l’image à remplir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Saisissez ou mappez un entier. Vous pouvez utiliser cette même source dans un autre module Développer une image pour générer une image similaire avec différents styles. </td> 
  </tr> 
 </tbody> 
</table>

## Générer une image

Ce module d’action génère une image à partir d’une invite que vous fournissez. Vous pouvez également fournir une image de référence facultative et l’image générée correspond au style de l’image de référence.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Campaign], voir <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Créer une connexion à [!DNL Adobe Firefly]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invite]</td> 
   <td>Saisissez ou mappez une invite pour l’image que vous souhaitez créer. Plus de détails dans l’invite vous permettront de mieux contrôler ce qui apparaît dans l’image.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Format d’image généré]</td> 
   <td>Sélectionnez le format de fichier sous lequel l’image étendue sera enregistrée. Si vous sélectionnez la valeur par défaut, le format de fichier sera JPEG si aucune image de référence n’est fournie. Si une image de référence est fournie, le format de fichier de l’image générée est identique à celui de l’image de référence.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>  <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom du fichier image de référence et le fichier image de référence (données) du fichier source. L’image générée sera créée pour correspondre au style de l’image de référence.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Paramètres prédéfinis]</td> 
   <td>Si vous souhaitez utiliser un style prédéfini, cliquez sur Ajouter un élément et saisissez ou mappez le style que vous souhaitez utiliser.<p>Pour obtenir la liste des styles prédéfinis, voir <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/styles/" >Styles de modèle d’image</a> dans la documentation destinée aux développeurs d’Adobes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL invite négative]</td> 
   <td>Saisissez ou mappez les mots à éviter dans le contenu généré. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Classe de contenu]</td> 
   <td>Choisissez si vous souhaitez que l’image générée ressemble davantage à une photo ou à un art créé. <ul><li><b>Photo</b><p>Saisissez les valeurs des champs Ouverture, Vitesse d’obturation (en secondes) et Champ de vue (en millimètres).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Saisissez ou mappez un entier. Vous pouvez utiliser cette même source dans un autre module Développer une image pour générer une image similaire avec différents styles. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Size]</td> 
   <td>Sélectionnez la taille de l’image générée.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Force]</td> 
   <td>Saisissez ou mappez un entier représentant l’intensité avec laquelle l’image générée correspondra au style du style prédéfini ou de l’image de référence. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Intensité visuelle]</td> 
   <td>Saisissez ou mappez un entier représentant l’intensité globale des caractéristiques visuelles existantes de la photo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td>Si un paramètre régional est fourni, le module génère du contenu plus pertinent par rapport au paramètre régional spécifié. <p>Les paramètres régionaux doivent être fournis dans le code de langue ISO 639-1 et dans la région ISO 3166-1.</p><p> Exemple : <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>


