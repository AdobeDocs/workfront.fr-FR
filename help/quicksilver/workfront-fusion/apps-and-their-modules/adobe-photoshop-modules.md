---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Adobe Photoshop
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: f20192ea-e363-4fba-8bd2-b1d50443918d
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '4360'
ht-degree: 21%

---

# Modules [!DNL Adobe Photoshop]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules Adobe Photoshop](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/adobe-photoshop-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Photoshop] et le connecter à plusieurs applications et services tiers.


Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

+++**Développez pour afficher les exigences d’accès pour la fonctionnalité de cet article.**

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
      <td>
        <p>[!UICONTROL Pro] ou version supérieure</p>
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
        <p>[!UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Produit</td>
      <td>Votre organisation doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice de [!DNL Workfront].

&#42;&#42;Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

+++

## Conditions préalables

Avant d’utiliser le connecteur [!DNL Adobe Photoshop], vous devez vous assurer que les conditions préalables suivantes sont remplies :

* Vous devez disposer d’un compte [!DNL Adobe Photoshop].

## Informations sur l’API Adobe Photoshop

Le connecteur Adobe Photoshop utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td>https://image.adobe.io/pie/psdService</td> 
  </tr>
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.12.31</td> 
  </tr>
 </tbody> 
 </table>

## Créer une connexion à [!DNL Adobe Photoshop]

Pour créer une connexion pour vos modules [!DNL Adobe Photoshop], procédez comme suit :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la case Connexion.

1. Remplissez les champs suivants :

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
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Saisissez votre [!UICONTROL Adobe] [!UICONTROL Client ID]. Vous pouvez le consulter dans la section des détails [!UICONTROL Credentials] de la [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre [!UICONTROL Client Secret] [!DNL Adobe]. Vous pouvez le consulter dans la section des détails [!UICONTROL Credentials] de la [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>Saisissez votre [!UICONTROL Technical account ID] [!DNL Adobe]. Vous pouvez le consulter dans la section des détails [!UICONTROL Credentials] de la [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Saisissez votre [!UICONTROL Organization ID] [!DNL Adobe]. Vous pouvez le consulter dans la section des détails [!UICONTROL Credentials] de la [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Private key]</td>
        <td>
          <p>Saisissez la clé privée générée lors de la création de vos informations d’identification dans l’[!DNL Adobe Developer Console]. </p>
          <p>Pour extraire votre clé privée ou votre certificat privé, procédez comme suit :</p>
          <ol>
            <li value="1">
              <p>Cliquez sur <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Sélectionnez le type de fichier que vous extrayez.</p>
            </li>
            <li value="3">
              <p>Sélectionnez le fichier contenant la clé privée ou le certificat privé.</p>
            </li>
            <li value="4">
              <p>Saisissez le mot de passe du fichier.</p>
            </li>
            <li value="5">
              <p>Cliquez sur <b>Enregistrer</b> pour extraire le fichier et revenir à la configuration de la connexion[!UICONTROL ]e.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.

## Modules [!DNL Adobe Photoshop] et leurs champs

Lorsque vous configurez les modules [!DNL Adobe Photoshop], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Adobe Photoshop] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Appliquer les modifications du PSD](#apply-psd-edits)
* [Correction automatique des couleurs d’une image](#auto-color-correct-an-image)
* [Convertir le format d’image](#convert-image-format)
* [Création d’un masque](#create-a-mask)
* [Création d’un PSD](#create-a-new-psd)
* [Modifier des calques de texte](#edit-text-layers)
* [Flou relatif à la profondeur d’exécution](#execute-depth-blur)
* [Exécution d’actions Photoshop](#execute-photoshop-actions)
* [Exécution d’actions Photoshop (JSON)](#execute-photoshop-actions-json)
* [Exécuter le recadrage de produit](#execute-product-crop)
* [Obtenir les informations sur le calque](#get-layer-info)
* [Effectuer un appel API personnalisé.](#make-a-custom-api-call)
* [Supprimer l’arrière-plan](#remove-background)
* [Remplacement d’un objet dynamique](#replace-a-smart-object)
* [Redimensionnement d’une image](#resize-an-image)
* [Filigrane d’une image](#watermark-an-image)

### Appliquer les modifications du PSD

Ce module d’action applique diverses modifications au niveau du document et des calques.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez modifier est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Input) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier que vous souhaitez modifier. </td> 
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
        <p>[!UICONTROL (Options &gt; Document &gt; Taille de la zone de travail) à gauche]</p>
      </td>
   <td> Saisissez ou mappez, en pixels, la coordonnée x du coin supérieur gauche du document. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options &gt; Document &gt; Taille de la zone de travail) Droite]</p>
      </td>
   <td> Saisissez ou mappez, en pixels, la coordonnée x du coin inférieur droit du document. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options &gt; Document) Trim]</p>
      </td>
   <td> Sélectionnez Pixels transparents pour baser le rognage sur les pixels transparents de l’image. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options) Default font]</p>
      </td>
   <td> Saisissez le nom postscript complet de la police à utiliser comme valeur par défaut globale pour le document. Cette police sera utilisée pour tout calque de texte qui comporte une police manquante et pour lequel aucune autre police n’a été spécifiquement fournie. Si cette police est manquante, l’option spécifiée dans Gérer les polices manquantes prend effet. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options) Fonts]</p>
      </td>
   <td> Pour chaque police dont le document a besoin, cliquez sur Ajouter un élément et saisissez l’emplacement de stockage et de fichier de la police. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options) Gérer les polices manquantes]</p>
      </td>
   <td> Sélectionnez l’action à effectuer s’il manque une ou plusieurs polices dans le document. <ul><li><code>fail</code>: la tâche ne réussira pas et le statut sera défini sur échec, avec les détails de l’erreur fournis dans la section détails du statut.</li><li><code>useDefault</code>: le traitement réussira, mais par défaut, toutes les polices manquantes seront remplacées par ArialMT.</li></ul></td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Options) Calques]</p>
      </td>
   <td> Pour chaque calque à ajouter, cliquez sur Ajouter un élément et renseignez les détails du calque. <p>Pour plus d’informations sur les options de calque, voir <a href="https://developer.adobe.com/firefly-services/docs/photoshop/api/photoshop_applyPsdEdits/">Appliquer les modifications de PSD </a> dans la documentation d’Adobe Photoshop.  </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Outputs]</td>
      <td>
        <p>Pour chaque fichier converti que vous souhaitez créer, cliquez sur Ajouter un élément et saisissez le stockage, l’emplacement et le type répertoriés dans ce tableau.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le nouveau fichier.</p><p>La sélection du stockage interne Fusion rend le fichier disponible pour les modules ultérieurs, mais ne rend pas le fichier disponible en dehors du scénario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier. Cela n’est nécessaire que si vous n’avez pas choisi le stockage interne Fusion pour le stockage de sortie.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Type]</p>
      </td>
   <td>Sélectionnez le type de fichier vers lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant. Cela s’applique uniquement aux fichiers dans un stockage d’Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>



### Correction automatique des couleurs d’une image

Ce module d’action corrige automatiquement la couleur de l’image spécifiée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier dont vous souhaitez corriger les couleurs est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Input) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier dont vous souhaitez corriger la couleur. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le nouveau fichier.</p><p>La sélection du stockage interne Fusion rend le fichier disponible pour les modules ultérieurs, mais ne rend pas le fichier disponible en dehors du scénario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier. Cela n’est nécessaire que si vous n’avez pas choisi le stockage interne Fusion pour le stockage de sortie.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Type]</p>
      </td>
   <td>Sélectionnez le type de fichier vers lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant. Cela s’applique uniquement aux fichiers dans un stockage d’Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>


### Convertir le format d’image

Ce module d’action convertit un fichier en JPEG, PNG, PSD ou TIFF.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel est stocké le fichier que vous souhaitez supprimer de l’arrière-plan.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Input) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès au fichier duquel vous souhaitez supprimer l’arrière-plan. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Outputs]</td>
      <td>
        <p>Pour chaque fichier converti que vous souhaitez créer, cliquez sur Ajouter un élément et saisissez le stockage, l’emplacement et le type répertoriés dans ce tableau.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le nouveau fichier.</p><p>La sélection du stockage interne Fusion rend le fichier disponible pour les modules ultérieurs, mais ne rend pas le fichier disponible en dehors du scénario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier. Cela n’est nécessaire que si vous n’avez pas choisi le stockage interne Fusion pour le stockage de sortie. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Type]</p>
      </td>
   <td>Sélectionnez le type de fichier vers lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant. Cela s’applique uniquement aux fichiers dans un stockage d’Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>



### Création d’un masque

Ce module d’action renvoie un fichier PNG avec un mât appliqué autour du sujet.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers à partir duquel est stocké le fichier à partir duquel vous souhaitez créer un masque.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Input) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès au fichier à partir duquel vous souhaitez créer un masque. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le fichier de masque.</p><p>La sélection du stockage interne Fusion rend le fichier disponible pour les modules ultérieurs, mais ne rend pas le fichier disponible en dehors du scénario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès où le fichier de masque sera stocké. Cela n’est nécessaire que si vous n’avez pas choisi le stockage interne Fusion pour le stockage de sortie.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant. Cela s’applique uniquement aux fichiers dans un stockage d’Adobe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Color space]</p>
      </td>
   <td>Choisissez si l’image de sortie utilise la couleur RGB ou RGBA. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Mask format]</p>
      </td>
   <td>Indiquez si le masque doit être souple (en drapeau) ou binaire. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Optimize]</p>
      </td>
   <td>Sélectionnez Performances pour optimiser la vitesse ou Lot pour permettre le temps d’attente. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Post process]</p>
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
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>

### Création d’un PSD

Ce module d’action permet de créer un PSD avec des calques facultatifs et de générer des rendus ou des enregistrements en tant que PSD.

Pour les champs liés à ce module, consultez la section [Création d’un PSD ](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) dans la documentation d’Adobe Photoshop.

### Modifier des calques de texte

Ce module d’action modifie les calques de texte d’un fichier Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez modifier est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier que vous souhaitez modifier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gérer les polices manquantes]</td>
      <td>
        <p>Sélectionnez l’action à effectuer s’il manque une ou plusieurs polices dans le document. Si la police n’est pas fournie, le module utilise la police par défaut.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default font]  </td>
      <td>
        <p>Saisissez le nom postscript complet de la police à utiliser comme valeur par défaut globale pour le document. Cette police sera utilisée pour tout calque de texte qui comporte une police manquante et pour lequel aucune autre police n’a été spécifiquement fournie. Si cette police est manquante, l’option spécifiée dans Gérer les polices manquantes prend effet.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Layers]</td>
   <td> <p>Pour plus d’informations sur les options de calque, voir <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">Modifier le calque de texte</a> dans la documentation d’Adobe Photoshop.</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier de sortie]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le fichier modifié.</p>
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
        <p>[!UICONTROL Type de fichier Output]</p>
      </td>
   <td> Sélectionnez le type de fichier pour le fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant.</p>
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
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez modifier est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Input) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier que vous souhaitez modifier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL, action JSON]</td>
      <td>
        <p>Saisissez la commande JSON correspondant à l’action à effectuer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Polices / Motifs / Brosses / Images supplémentaires]</td>
      <td>
        <p>Pour chaque police, modèle, pinceau ou image supplémentaire à utiliser dans cette action, cliquez sur Ajouter un élément et saisissez l’espace de stockage et l’emplacement du fichier de l’élément.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Font / Pattern / Brush file URL]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès au fichier que vous souhaitez utiliser. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stocke le fichier de sortie]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le fichier modifié.</p><p>La sélection du stockage interne Fusion rend le fichier disponible pour les modules ultérieurs, mais ne rend pas le fichier disponible en dehors du scénario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL du fichier de sortie]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du fichier modifié.  Cela n’est nécessaire que si vous n’avez pas choisi le stockage interne Fusion pour le stockage de sortie.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Type de fichier Output]</p>
      </td>
   <td> Sélectionnez le type de fichier pour le fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant.</p>
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
        <p>Pour chaque fichier converti que vous souhaitez créer, cliquez sur Ajouter un élément et saisissez le stockage, l’emplacement et le type répertoriés dans ce tableau.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le nouveau fichier.</p>
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
        <p>[!UICONTROL (Output) Type]</p>
      </td>
   <td>Sélectionnez le type de fichier vers lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant. Cela s’applique uniquement aux fichiers dans un stockage d’Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
      </tbody>
</table>

### Flou relatif à la profondeur d’exécution

Ce module d’action exécute l’action Flou de profondeur sur le fichier sélectionné.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez modifier est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier que vous souhaitez modifier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier de sortie]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le fichier modifié.</p>
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
        <p>[!UICONTROL Type de fichier Output]</p>
      </td>
   <td> Sélectionnez le type de fichier pour le fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Other fields]</td>
      <td>
        <p>Pour plus d’informations sur les autres options de flou de profondeur, voir <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Execute Depth Blur</a> dans la documentation de l’API Adobe Photoshop.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant.</p>
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

### Exécution d’actions Photoshop

Ce module d’action exécute une action Photoshop sur l’image sélectionnée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez modifier est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier que vous souhaitez modifier. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Actions file storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier d’actions est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Actions file URL]</p>
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
      <td role="rowheader">[!UICONTROL Font / Pattern / Brush storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier que vous souhaitez utiliser est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Font / Pattern / Brush file URL]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès au fichier que vous souhaitez utiliser. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier de sortie]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le fichier modifié.</p>
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
        <p>[!UICONTROL Type de fichier Output]</p>
      </td>
   <td> Sélectionnez le type de fichier pour le fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant.</p>
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

### Exécuter le recadrage de produit

Ce module d’action exécute le recadrage de produit sur l’image sélectionnée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier à recadrer est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier que vous souhaitez recadrer. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Unit]</p>
      </td>
   <td> Choisissez si vous souhaitez décrire l’ajustement de la hauteur et de la largeur en pixels ou en pourcentage. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Width]</p>
      </td>
   <td> Saisissez ou mappez la quantité de remplissage de largeur que vous souhaitez ajouter. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Height]</p>
      </td>
   <td> Saisissez ou mappez la quantité de remplissage en hauteur à ajouter. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Stockage du fichier de sortie]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le fichier modifié.</p>
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
        <p>[!UICONTROL Type de fichier Output]</p>
      </td>
   <td> Sélectionnez le type de fichier pour le fichier modifié. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant.</p>
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

### Obtenir les informations sur le calque

Ce module d&#39;action récupère les informations de calque du fichier de PSD spécifié.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel est stocké le fichier à partir duquel vous souhaitez récupérer les informations de calque.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès au fichier à partir duquel vous souhaitez récupérer les informations de calque. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Thumbnails]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

### Effectuer un appel API personnalisé.

Ce module d’action effectue un appel personnalisé à l’API Photoshop.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
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
        <p>[!DNL Workfront Fusion] Ajoute automatiquement des en-têtes d’autorisation.</p>
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
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets à l’extérieur de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Supprimer l’arrière-plan

Ce module d’action identifie l’objet principal de votre image et supprime l’arrière-plan.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel est stocké le fichier que vous souhaitez supprimer de l’arrière-plan.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Input) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès au fichier duquel vous souhaitez supprimer l’arrière-plan. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le nouveau fichier.</p><p>La sélection du stockage interne Fusion rend le fichier disponible pour les modules ultérieurs, mais ne rend pas le fichier disponible en dehors du scénario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier.  Cela n’est nécessaire que si vous n’avez pas choisi le stockage interne Fusion pour le stockage de sortie.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant. Cela s’applique uniquement aux fichiers dans un stockage d’Adobe.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Color space]</p>
      </td>
   <td>Choisissez si l’image de sortie utilise la couleur RGB ou RGBA. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Mask format]</p>
      </td>
   <td>Indiquez si les bords de l’image doivent être lisses (contours progressifs) ou binaires. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Optimize]</p>
      </td>
   <td>Sélectionnez Performances pour optimiser la vitesse ou Lot pour permettre le temps d’attente. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Post process]</p>
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
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
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
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Input) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel l’objet dynamique est stocké.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Input) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’objet dynamique. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Layers]</p>
      </td>
   <td>Pour chaque calque que vous souhaitez ajouter à l’objet dynamique, cliquez sur Ajouter un élément et saisissez le nom ou l’ID de l’objet, le service de fichiers dans lequel l’objet dynamique est stocké et l’URL ou le chemin d’accès du calque.<p>Pour obtenir une description des paramètres avancés dans cette zone, voir <a href="https://developer.adobe.com/firefly-services/docs/photoshop/api/photoshop_replaceSmartObject/">Remplacer un objet dynamique</a> dans la documentation de l’API Photoshop </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Outputs]</td>
      <td>
        <p>Pour chaque nouveau rendu que vous souhaitez que le module produise, cliquez sur Ajouter un élément et renseignez les champs suivants. Vous pouvez avoir un maximum de 25 fichiers de sortie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le nouveau fichier.</p><p>La sélection du stockage interne Fusion rend le fichier disponible pour les modules ultérieurs, mais ne rend pas le fichier disponible en dehors du scénario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du nouveau fichier.  Cela n’est nécessaire que si vous n’avez pas choisi le stockage interne Fusion pour le stockage de sortie.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Sortie) Largeur]</p>
      </td>
   <td> Largeur, en pixels, du fichier de sortie. Le module conserve les proportions d’origine. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant. Cela s’applique uniquement aux fichiers dans un stockage d’Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>



### Redimensionnement d’une image

Cette action redimensionne une image en utilisant les mêmes proportions.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel le fichier à redimensionner est stocké.</p><p>La sélection du stockage interne Fusion rend le fichier disponible pour les modules ultérieurs, mais ne rend pas le fichier disponible en dehors du scénario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Emplacement du fichier]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier à redimensionner.  Cela n’est nécessaire que si vous n’avez pas choisi le stockage interne Fusion pour le stockage de sortie.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Outputs]</td>
      <td>
        <p>Pour chaque fichier converti que vous souhaitez créer, cliquez sur Ajouter un élément et saisissez les options de stockage, d’emplacement et autres, comme indiqué dans ce tableau.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Type]</p>
      </td>
   <td>Sélectionnez le type de fichier vers lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Width]</p>
      </td>
   <td>Saisissez un nombre qui représente la largeur, en pixels, de l’image redimensionnée. Les proportions sont conservées.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Largeur max.]</p>
      </td>
   <td>Lorsque la largeur est égale à 0, la propriété Max avec peut être fournie pour obtenir la taille. La largeur maximale est prioritaire et est inférieure à la largeur du document.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant. Cela s’applique uniquement aux fichiers dans un stockage d’Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Rogner sur la zone de travail]</p>
      </td>
   <td>Sélectionnez Oui pour ajuster les rendus à la taille de la zone de travail ou Non pour définir la taille du calque des rendus.</td> 
    </tr>
    </tbody>
</table>

### Filigrane d’une image

Ce module d’action ajoute un filigrane à l’image sélectionnée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Photoshop], voir <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Créer une connexion à [!DNL Adobe Photoshop]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">Stockage [!UICONTROL (Base/Entrée)]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel est stocké le fichier auquel vous souhaitez ajouter un filigrane.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Base / Entrée) Emplacement du fichier]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès du fichier auquel vous souhaitez ajouter un filigrane. </td> 
    </tr>
    <tr>
      <td role="rowheader">Stockage [!UICONTROL (filigrane / entrée)]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel est stocké le filigrane que vous souhaitez ajouter.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Stockage [!UICONTROL (filigrane / entrée)]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel est stocké le filigrane que vous souhaitez ajouter.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Filigrane / Limites) Hauteur]</p>
      </td>
   <td>Saisissez ou mappez la hauteur souhaitée du filigrane en pixels.</td> 
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Filigrane / Limites) Largeur]</p>
      </td>
   <td> Saisissez ou mappez la largeur souhaitée du filigrane en pixels. </td> 
    </tr>  
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Filigrane / Limites) À Gauche]</p>
      </td>
   <td> Saisissez ou mappez la distance en pixels entre le côté gauche de l’image et le filigrane.</td> 
    </tr>  
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Filigrane / Limites) Haut]</p>
      </td>
   <td> Saisissez ou mappez la distance en pixels entre le haut de l’image et le filigrane.</td> 
    </tr>  
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Storage]</td>
      <td>
        <p>Sélectionnez le service de fichiers dans lequel vous souhaitez stocker le fichier en filigrane.</p><p>La sélection du stockage interne Fusion rend le fichier disponible pour les modules ultérieurs, mais ne rend pas le fichier disponible en dehors du scénario.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) File location]</p>
      </td>
   <td> Saisissez ou mappez l’URL ou le chemin d’accès de l’emplacement de stockage du fichier en filigrane. Cela n’est nécessaire que si vous n’avez pas choisi le stockage interne Fusion pour le stockage de sortie.</td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Output) Type]</p>
      </td>
   <td>Sélectionnez le type de fichier vers lequel vous souhaitez convertir le fichier. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL (Sortie) Largeur]</p>
      </td>
   <td> Largeur, en pixels, du fichier de sortie. Le module conserve les proportions d’origine. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL (Output) Overwrite]</td>
      <td>
        <p>Indiquez si le fichier nouvellement modifié remplacera un fichier de sortie existant. Cela s’applique uniquement aux fichiers dans un stockage d’Adobe.</p>
      </td>
    </tr>
        <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned results]</p>
      </td>
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
    </tr>
    </tbody>
</table>















