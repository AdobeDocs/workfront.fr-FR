---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Dropbox
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Dropbox et les connecter à plusieurs applications et services tiers. Cela vous permet d’automatiser des activités telles que la surveillance, la recherche, la récupération, la mise en liste, la création et la modification de fichiers et de dossiers dans votre Dropbox.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 86be8b6e1c21f3fd5f5b66afa3bf930d6bafbd63
workflow-type: tm+mt
source-wordcount: '3208'
ht-degree: 100%

---

# Modules [!DNL Dropbox]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!UICONTROL Dropbox] ou [!DNL Dropbox Business], ainsi que les connecter à plusieurs applications et services tiers. Cela vous permet d’automatiser des activités telles que la surveillance, la recherche, la récupération, la mise en liste, la création et la modification de fichiers et de dossiers dans vos [!UICONTROL Dropbox].

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

* Pour utiliser des modules [!DNL Dropbox], vous devez disposer d’un compte [!DNL Dropbox].

>[!IMPORTANT]
>
>Dropbox doit approuver les demandes comptant plus de 50 utilisateurs et utilisatrices.
>
>Pour plus d’informations, recherchez « Production approval » dans le guide de développement de Dropbox.


## Créer une connexion à [!DNL Dropbox]

Pour créer une connexion pour vos modules [!DNL Dropbox] :

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
        <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Indiquez si cette connexion est destinée à un environnement de production ou hors production.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Choisissez si vous vous connectez à un compte de service ou à un compte personnel.</td>
        </tr>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Saisissez votre [!UICONTROL Dropbox] [!UICONTROL Client ID]. </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre [!DNL Dropbox] [!UICONTROL Client Secret]. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Account Type]</td>
        <td>Choisissez si vous vous connectez à un compte personnel Dropbox ou à un compte professionnel (Dropbox Business).</td>
        </tr>
      </tbody>
    </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.## Modules [!DNL Dropbox] et leurs champs

## Modules [!DNL Dropbox] et leurs champs

Lorsque vous configurez des modules [!DNL Dropbox], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Dropbox] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Modules déclencheurs](#trigger-modules)
* [Modules pour obtenir les fichiers et dossiers  [!DNL Dropbox] ](#modules-for-getting-dropbox-files-and-folders)
* [Modules pour la création et la modification des fichiers et dossiers  [!DNL Dropbox] ](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [Autres modules](#other-modules)

### Modules déclencheurs

#### [!UICONTROL Fichiers de contrôle]

Ce module de type Déclencheur renvoie les détails du fichier lorsque le fichier d’un dossier spécifié est modifié.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier dont vous souhaitez surveiller les modifications.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch also subfolders]</td> 
   <td> <p> Activez cette option pour surveiller également les sous-dossiers du dossier sélectionné pour les fichiers modifiés.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit] </td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modules pour obtenir des fichiers et dossiers [!DNL Dropbox]

* [[!UICONTROL Rechercher des fichiers/dossiers]](#search-filesfolders)
* [[!UICONTROL Télécharger un fichier]](#download-a-file)
* [[!UICONTROL Obtenir des métadonnées de dossier]](#get-a-folder-metadata)
* [[!UICONTROL Répertorier tous les fichiers/sous-dossiers dans un dossier]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL Répertorier des révisions de fichiers]](#list-file-revisions)

#### [!UICONTROL Rechercher des fichiers/dossiers]

Ce module de recherche recherche des enregistrements d’un objet dans [!DNL Dropbox] qui correspondent à la requête de recherche que vous avez spécifiée.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Saisissez le terme de recherche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier à rechercher. Ce module recherche [!DNL Dropbox] dans son intégralité si vous ne sélectionnez pas de dossier.</p> </td> 
  </tr> 
  <tr> 
   <td>Statut du fichier</td> 
   <td> <p> Sélectionnez le statut du fichier pour restreindre la recherche au statut du fichier sélectionné.</p> </td> 
  </tr> 
  <tr> 
   <td>Catégories de fichiers</td> 
   <td> <p> Sélectionnez les catégories de fichiers pour restreindre la recherche aux catégories sélectionnées.</p> </td> 
  </tr> 
  <tr> 
   <td>Extensions de fichiers</td> 
   <td> <p> Sélectionnez les extensions de fichier à rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>Limite </td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger un fichier]

Ce module d’action télécharge un fichier à partir d’un dossier.

Vous indiquez le fichier et son emplacement.

Le module renvoie l’ID du fichier et tous les champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

>[!NOTE]
>
>Ce module est utile pour fournir des fichiers aux modules suivants.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Sélection des fichiers</td> 
   <td> <p> Choisissez si vous souhaitez mapper le chemin du fichier, ou sélectionnez le fichier manuellement.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Chemin du fichier/Fichier</p> </td> 
   <td> <p style="font-weight: bold;">Chemin du fichier</p> <p>Saisissez ou mappez le chemin cible sur le fichier.</p> <p style="font-weight: bold;">Fichier</p> <p>Sélectionnez le fichier dans le menu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir des métadonnées de dossier]

Ce module d’action récupère les détails du dossier partagé.

Vous spécifiez l’identifiant du dossier.

Le module renvoie l’ID du dossier et des champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Identifiant de dossier partagé</td> 
   <td> <p> Saisissez ou mappez l’identifiant du dossier dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Répertorier tous les fichiers/sous-dossiers dans un dossier]

Ce module d’action répertorie les fichiers ou les dossiers d’un dossier spécifique.

Vous spécifiez l’identifiant du dossier.

Le module renvoie les ID des fichiers ou dossiers et des champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Liste </td> 
   <td> <p>Indiquez si vous souhaitez récupérer des fichiers ou des dossiers.</p> </td> 
  </tr> 
  <tr> 
   <td>Afficher uniquement les fichiers téléchargeables</td> 
   <td> <p> Activez cette option pour ne renvoyer que les fichiers téléchargeables. Certains types de fichiers, tels que les documents Google Docs, ne sont pas téléchargeables.</p> </td> 
  </tr> 
  <tr> 
   <td>Dossier </td> 
   <td> <p>Saisissez ou mappez le dossier à partir duquel vous souhaitez récupérer des fichiers ou des dossiers.</p> </td> 
  </tr> 
  <tr> 
   <td>Limite </td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit répertorier pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Répertorier des révisions de fichiers]

Ce module d’action récupère toutes les révisions de fichier (un historique de version) d’un fichier particulier.\
Vous spécifiez l’ID du fichier.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Sélection des fichiers</td> 
   <td> <p> Choisissez si vous souhaitez mapper le chemin du fichier, ou sélectionnez le fichier manuellement.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Chemin du fichier/Fichier</p> </td> 
   <td> <p style="font-weight: bold;">Chemin du fichier</p> <p>Saisissez ou mappez le chemin cible sur le fichier.</p> <p style="font-weight: bold;">Fichier</p> <p>Sélectionnez le fichier dans le menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Limite</p> </td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit répertorier pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modules pour la création et la modification de fichiers et dossiers [!DNL Dropbox]

* [[!UICONTROL Charger] un fichier](#upload-a-file)
* [[!UICONTROL Créer un dossier]](#create-a-folder)
* [[!UICONTROL Créer/remplacer un fichier texte]](#createoverwrite-a-text-file)
* [[!UICONTROL Créer/mettre à jour d’un lien de partage]](#createupdate-a-share-link)
* [[!UICONTROL Restaurer un fichier]](#restore-a-file)
* [[!UICONTROL Déplacer un fichier/dossier]](#move-a-filefolder)
* [[!UICONTROL Renommer un fichier/dossier]](#rename-a-filefolder)
* [[!UICONTROL Supprimer un fichier/dossier]](#delete-a-filefolder)

#### [!UICONTROL Charger un fichier]

Ce module d’action charge un fichier dans un dossier.

Renseignez des informations telles que l’emplacement du fichier, le fichier à charger et éventuellement un nouveau nom pour le fichier.

Le module renvoie l’ID du fichier et tous les champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre application [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td> <p> Sélectionnez le dossier de votre [!DNL Dropbox] dans lequel vous souhaitez charger le fichier.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Saisissez ou mappez le fichier à ajouter au dossier [!DNL Dropbox] sélectionné ci-dessus.</p> <p style="font-weight: bold;">[!UICONTROL File name]</p> <p>Saisissez ou mappez le nom du fichier, y compris son extension.</p> <p style="font-weight: bold;">[!UICONTROL File data]</p> <p>Saisissez ou mappez les données du fichier (du module précédent, tel que [!UICONTROL Google Drive] &gt; [!UICONTROL Get a File)].</p> <p>Note : la taille maximale du fichier chargé est de 150 Mo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Overwrite an existing file]</td> 
   <td> <p> Activez cette option pour remplacer le fichier existant par le nouveau fichier. Si cette option est désactivée, le fichier chargé est renommé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un dossier]

Ce module d’action crée un dossier.

Spécifiez le chemin et un nom pour le dossier.

Le module renvoie l’identifiant du dossier et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder Name] </td> 
   <td> <p>Saisissez un nom pour le nouveau dossier.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Folder]</p> </td> 
   <td> <p>Saisissez ou mappez le chemin d’accès où vous souhaitez créer un dossier.</p> <p>Remarque :   <p>Si vous utilisez un compte [!DNL Dropbox Business] (avec espaces d’équipe), vous devez supprimer la barre oblique <code>/</code>, ou ne cliquez pas sur <strong>[!UICONTROL Click here] pour sélectionner un dossier</strong> afin de créer un dossier d’équipe dans la racine.</p> <p>Si la barre oblique n’est pas supprimée, une erreur <code>[409] path/malformed_path/..</code> est renvoyée.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Auto rename]</td> 
   <td> <p> Activez cette option pour renommer le nouveau dossier si un dossier portant le même nom existe déjà à l’emplacement cible.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer/remplacer un fichier texte]

Ce module d’action crée un fichier DOC ou remplace le contenu d’un fichier existant.

Vous spécifiez le fichier source et le dossier.

Le module renvoie l’identifiant du dossier et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select to]</td> 
   <td> <p> Indiquez si vous souhaitez créer ou remplacer un fichier DOC.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez l’emplacement cible où vous souhaitez créer un fichier.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Saisissez ou mappez le fichier à ajouter au dossier [!DNL Dropbox].</p> <p style="font-weight: bold;">Nom du fichier</p> <p>Saisissez le nom de fichier du nouveau fichier DOC (sans extension).</p> <p style="font-weight: bold;">Contenu du fichier</p> <p>Saisissez le contenu texte du fichier DOC.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer/mettre à jour un lien de partage]

Ce module d’action crée un lien public vers un fichier 

Vous spécifiez le fichier et les informations sur le lien.

Le module renvoie l’ID du lien et des champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files]</td> 
   <td> <p> Choisissez si vous souhaitez mapper ou saisir le chemin d’accès au fichier, ou sélectionnez le fichier manuellement.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path / File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File Path]</p> <p>Saisissez ou mappez le chemin cible sur le fichier.</p> <p style="font-weight: bold;">[!UICONTROL File]</p> <p>Sélectionnez le fichier dans le menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Requested Visibility]</p> </td> 
   <td> <p>Indiquez si le lien est public, pour l’équipe ou limité par un mot de passe.</p> <p>Remarque : les options [!UICONTROL Team only] et [!UICONTROL Access with password] ne sont disponibles que pour les utilisateurs et utilisatrices qui disposent de [!DNL Dropbox Pro] ou d’une version ultérieure.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Link's Expiration Date]</td> 
   <td> <p> Saisissez la date et l’heure d’expiration du lien (il ne sera alors plus accessible). Si ce champ n’est pas renseigné, le lien n’expire pas. Pour consulter la liste des formats de date et d’heure pris en charge, voir la section <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> <p>Remarque : les options [!UICONTROL Team only] et [!UICONTROL Access with password] ne sont disponibles que pour les utilisateurs et utilisatrices disposant de [!UICONTROL Dropbox Pro] ou de versions ultérieures.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Link's Access Level]</p> </td> 
   <td> <p>Définissez l’autorisation pour la personne destinataire du lien.</p> <p>Les utilisateurs et utilisatrices <strong>[!UICONTROL Viewer]</strong> qui utilisent le lien peuvent afficher et commenter le contenu.</p> <p>Les utilisateurs et utilisatrices <strong>[!UICONTROL Editor]</strong> qui utilisent le lien peuvent modifier, afficher et commenter le contenu.</p> <p>Les utilisateurs et utilisatrices <strong>[!UICONTROL Max]</strong> qui utilisent le lien reçoivent le niveau d’accès maximal que vous pouvez définir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Restaurer un fichier]

Ce module d’action restaure une version précédente d’un fichier.

Spécifiez le fichier et le numéro de la révision que vous souhaitez.

Le module renvoie l’identifiant de la version et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files]</td> 
   <td> <p> Choisissez si vous souhaitez mapper ou saisir le chemin d’accès au fichier, ou sélectionnez le fichier manuellement.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path]/[!UICONTROL File]</p> </td> 
   <td> <p><strong>[!UICONTROL File Path]</strong> </p> <p>Saisissez ou mappez le chemin cible sur le fichier.</p> <p><strong>[!UICONTROL File]</strong> </p> <p>Sélectionnez le fichier dans le menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Revision]</p> </td> 
   <td> <p>Saisissez ou mappez le numéro de la révision à restaurer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un fichier/dossier]

Ce module d’action déplace un fichier ou un dossier vers un autre emplacement.

Spécifiez le fichier ou le dossier, ainsi que l’emplacement et la manière dont vous souhaitez le déplacer.

Le module renvoie l’identifiant du fichier ou du dossier et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files] </td> 
   <td> <p>Choisissez si vous souhaitez mapper ou saisir le chemin d’accès au fichier, ou sélectionnez le fichier manuellement.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File/Folder Path]/[!UICONTROL File/Folder]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File/Folder Path]</p> <p>Saisissez ou mappez le chemin cible sur le fichier ou le dossier.</p> <p style="font-weight: bold;">[!UICONTROL File/Folder]</p> <p>Sélectionnez le fichier ou le dossier dans le menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL To Folder]</p> </td> 
   <td> <p>Saisissez ou mappez l’emplacement cible du fichier ou du dossier.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL New Name]</p> </td> 
   <td> <p>Saisissez le nouveau nom du fichier ou du dossier au nouvel emplacement.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Auto Rename]</p> </td> 
   <td> <p>Activez cette option pour vous assurer que s’il existe un fichier ou un dossier portant le même nom, le module renomme le nouveau fichier ou dossier en ajoutant ([!UICONTROL NUMBER]) après le nom du fichier ou du dossier. Sinon, le fichier ou le dossier de l’emplacement cible est remplacé.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Allow ownership transfer]</p> </td> 
   <td> <p>Activez cette option pour permettre les déplacements par la personne propriétaire, même si cela entraînerait un transfert de propriété pour le contenu déplacé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Renommer un fichier/dossier]

Ce module d’action renomme un fichier ou un dossier.

Spécifiez le fichier ou le dossier, et le nouveau nom.

Le module renvoie l’identifiant du fichier ou du dossier et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>Sélection des fichiers</td> 
   <td> <p> Choisissez si vous souhaitez mapper ou saisir le chemin d’accès au fichier, ou sélectionnez le fichier manuellement.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Chemin du dossier/fichier / Fichier/Dossier</p> </td> 
   <td> <p style="font-weight: bold;">Chemin du fichier/dossier</p> <p>Saisissez ou mappez le chemin cible sur le fichier ou le dossier.</p> <p style="font-weight: bold;">Fichier/Dossier</p> <p>Sélectionnez le fichier ou le dossier dans le menu.</p> </td> 
  </tr> 
  <tr> 
   <td>Renommer </td> 
   <td> <p>Saisissez le [!UICONTROL target name] du fichier, y compris son extension.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un fichier/dossier]

Ce module d’action supprime un fichier ou un dossier.

Spécifiez le fichier ou le dossier.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files]</td> 
   <td> <p> Choisissez si vous souhaitez mapper ou saisir le chemin d’accès au fichier, ou sélectionnez le fichier manuellement.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path]/[!UICONTROL File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File Path]</p> <p>Saisissez ou mappez le chemin cible sur le fichier.</p> <p style="font-weight: bold;">[!UICONTROL File]</p> <p>Sélectionnez le fichier dans le menu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autres modules

#### [!UICONTROL Effectuer un appel API]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Dropbox]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Dropbox].

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Dropbox] à [!DNL Workfront Fusion], voir <a href="#create-a-connection-to-dropbox" class="MCXref xref">Créer une connexion à [!DNL Dropbox]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif <code>https://api.dropboxapi.com</code>. Par exemple, <code>/2/files/list_folder</code></p> <p>Remarque : pour obtenir la liste des points d’entrée disponibles, voir <a href="https://www.dropbox.com/developers/documentation/http/documentation">Documentation de l’API Dropbox v2</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers] </td> 
   <td> <p>Saisissez les en-têtes de requête de votre choix. [!DNL Workfront Fusion] ajoute automatiquement des en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p> Saisissez la chaîne de requête.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body] </td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :   <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** l’appel API suivant renvoie les 10 premiers fichiers du dossier [!DNL /Text files] dans votre compte [!DNL Dropbox] :
>
>URL : `/2/files/list_folder`
>
>Corps :
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>Les correspondances de la recherche se trouvent dans la sortie du module sous [!UICONTROL Lot] > [!UICONTROL Corps] > Entrées.
>
>Dans notre exemple, 10 tickets ont été renvoyés :

## Problèmes courants

* [Impossible de charger ou de mettre à jour un fichier](#unable-to-upload-or-update-a-file)
* [L’image référencée via un lien partagé n’est pas rendue.](#image-referenced-via-a-shared-link-does-not-render)

### Impossible de charger ou de mettre à jour un fichier

Il existe plusieurs situations entraînant l’échec du chargement ou de la mise à jour d’un fichier :

* Le fichier chargé est trop volumineux et dépasse la taille de fichier maximale autorisée pour votre plan [!DNL Dropbox] ou vous avez utilisé l’ensemble du quota de stockage de votre compte [!DNL Dropbox]. Vous devez supprimer les fichiers existants de votre compte [!DNL Dropbox] ou mettre à niveau votre plan.
* Le dossier précédemment sélectionné dans lequel le fichier est chargé n’existe plus. Le scénario s’arrête et vous devez sélectionner à nouveau le dossier cible.

### L’image référencée via un lien partagé n’est pas rendue.

L’URL retournée par [!UICONTROL Dropbox] >[!UICONTROL Créer un lien partagé] ne renvoie pas directement à une image, mais à une page [!DNL Dropbox]. Pour forcer le téléchargement de l’image, remplacez `?dl=0` par `?dl=1`. Pour forcer le rendu de l’image (par exemple, dans un navigateur web ou dans Facebook Messenger), ajoutez `&raw=1` à l’URL.

Si vous devez obtenir le lien direct ou brut de votre image pour votre site web ou pour d’autres modules [!DNL Workfront Fusion], vous devez modifier l’URL partagée initiale de la manière suivante :

URL d’origine :

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. Remplacez `www` par `dl`.
1. Supprimez `?dl=0`

URL finale :

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

Pour modifier automatiquement l’URL, vous pouvez utiliser la fonction `replace()` deux fois :

* Remplacez www par dl.

  ![](assets/www-to-dl-350x32.png)

* Et supprimez ?dl=0.

  ![](assets/remove-dl0-350x33.png)

Pour le faire en une seule étape, combinez les fonctions suivantes :

![](assets/replace-both-350x47.png)

Vous pouvez également le copier et le coller dans le champ. Remplacez `1.url` par l’URL.

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
