---
title: Modules CloudConvert
description: Modules CloudConvert
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: e21ef8a0-bec0-43fc-a495-c00b4023a273
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3008'
ht-degree: 100%

---

# Modules [!DNL CloudConvert]

Dans un scénario Adobe Workfront Fusion, vous pouvez automatiser les workflows qui utilisent CloudConvert, et le connecter à plusieurs applications et services tiers. Les modules [!DNL CloudConvert] vous permettent de surveiller et de gérer des travaux et des tâches, ainsi que d’importer et d’exporter des fichiers dans votre compte [!DNL CloudConvert].

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
  <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre organisation doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

## Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion] {#connect-cloudconvert-to-workfront-fusion}

Pour connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], vous devez obtenir une clé API depuis votre compte [!DNL CloudConvert].

1. Connectez-vous à votre compte [!DNL CloudConvert] et ouvrez votre [!UICONTROL Tableau de bord].
1. Ouvrez la section **[!UICONTROL Autorisation] > [!UICONTROL Clés API]**.
1. Cliquez sur **[!UICONTROL Créer une clé API]**.
1. Saisissez le nom de la clé API, activez les étendues que vous souhaitez utiliser, puis cliquez sur **[!UICONTROL Créer]**.
1. Copiez le jeton fourni et stockez-le dans un endroit sûr.
1. Dans [!DNL Workfront Fusion], commencez à créer un scénario et ouvrez la boîte de dialogue **[!UICONTROL Créer une connexion]** du module [!DNL CloudConvert].

   Pour obtenir des instructions, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Saisissez le jeton que vous avez enregistré à l’étape 5, puis cliquez sur **[!UICONTROL Continuer]** pour établir la connexion.

## Modules [!DNL CloudConvert] et leurs champs {#cloudconvert-modules-and-their-fields}

Lorsque vous configurez les modules [!DNL CloudConvert], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL CloudConvert] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mappage des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Tâches courantes](#common-tasks)
* [Traitements](#jobs)
* [Tâches](#tasks)
* [Autre](#other)

### Tâches courantes

* [Capturer un site web](#capture-a-website)
* [[!UICONTROL Convertir un fichier]](#convert-a-file)
* [Créer une archive](#create-an-archive)
* [Fusionner des fichiers](#merge-files)
* [Optimiser un fichier](#optimize-a-file)

#### [!UICONTROL Capturer un site web]

Ce module d’action capture un site web spécifié et l’enregistre au format PDF, JPG ou PNG.

Vous spécifiez l’URL du site web et d’autres informations, telles que l’emplacement où vous souhaitez stocker les informations.

Le module renvoie l’ID du fichier et tous les champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez l’URL du site web que vous souhaitez capturer. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format] </td> 
   <td>Sélectionnez si vous souhaitez enregistrer le site web capturé au format PNG, JPG ou PDF. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File Name] </td> 
   <td>Saisissez un nom de fichier (extension incluse) pour le fichier de sortie cible.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>(Facultatif) Définissez des en-têtes de requête. </p> <p>Cela s’avère utile, par exemple, lorsque l’URL spécifiée requiert une autorisation. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conversion and engine specific options] </p> </td> 
   <td>Spécifiez les options de conversion et spécifiques au moteur. Pour afficher les options disponibles, voir la documentation sur l’API <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert]</a> pour <code>input_format</code> et <code>output_format</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Download a file] </td> 
   <td> <p>Activez cette option si vous souhaitez également inclure des données de fichier dans la sortie du module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convertir un fichier]

Convertit un fichier dans le format de sortie sélectionné.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], voir <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input file]</td> 
   <td>Indiquez si vous souhaitez charger un fichier à l’aide de [!DNL Workfront Fusion] ou indiquez l’URL à partir de laquelle le fichier sera chargé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload a file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Import a File from URL]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Saisissez l’URL du fichier que vous souhaitez convertir.</p> </li> 
     <li> <p><strong>[!UICONTROL Headers]</strong></p> <p>Définissez des en-têtes de demande (facultatif). Cela s’avère utile, par exemple, lorsque l’URL spécifiée requiert une autorisation.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Format]</td> 
   <td>Indiquez si vous souhaitez spécifier le format d’entrée du fichier à convertir. Si elle n’est pas spécifiée, l’extension du fichier d’entrée est utilisée comme format d’entrée.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Input Format]</td> 
   <td>Sélectionnez le format actuel du fichier.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td>Sélectionnez le format de fichier cible vers lequel vous souhaitez convertir le fichier.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL File Name]</td> 
   <td>Choisissez un nom de fichier (extension comprise) pour le fichier de sortie cible.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Conversion and engine specific options] </p> </td> 
   <td>Spécifiez les options de conversion et spécifiques au moteur. Pour afficher les options disponibles, voir la documentation sur l’API <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert]</a> pour <code>input_format</code> et <code>output_format</code>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Download a file] </td> 
   <td> <p>Activez cette option si vous souhaitez également inclure des données de fichier dans la sortie du module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer une archive]

Permet d’ajouter un ou plusieurs fichiers à l’archive ZIP, RAR, 7Z, TAR, TAR.GZ ou TAR.BZ2.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Input Files]</p> </td> 
   <td> <p>Spécifiez les fichiers que vous souhaitez ajouter à l’archive.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload a File]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Import a file from URL]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>Saisissez l’URL du fichier que vous souhaitez archiver.</p> <p><strong>[!UICONTROL Headers]</strong> </p> <p>Définissez des en-têtes de demande (facultatif). Cela s’avère utile, par exemple, lorsque l’URL spécifiée requiert une autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p> Sélectionnez le format cible du fichier archivé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td> <p> Saisissez le nom du fichier (extension incluse) pour le fichier de sortie cible.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conversion and engine specific options] </td> 
   <td> <p>Spécifiez les options de conversion et spécifiques au moteur. Pour afficher les options disponibles, consultez la documentation de l’API <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert]</a> pour <code>input_format</code> et <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Download a File]</td> 
   <td> <p>Activez cette option si vous souhaitez également inclure des données de fichier dans la sortie du module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fusionner des fichiers]

Fusionne au moins deux fichiers dans un PDF. Si les fichiers d’entrée ne sont pas des PDF, ils sont automatiquement convertis au format PDF.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Input Files]</p> </td> 
   <td> <p>Spécifiez les fichiers que vous souhaitez fusionner.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload a File]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Import a file from URL]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>Saisissez l’URL du fichier que vous souhaitez archiver.</p> <p><strong>[!UICONTROL Headers]</strong> </p> <p>Définissez des en-têtes de demande (facultatif). Cela s’avère utile, par exemple, lorsque l’URL spécifiée requiert une autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p> Sélectionnez le format cible du fichier fusionné.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td> <p> Saisissez le nom du fichier (extension incluse) pour le fichier de sortie cible.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conversion and engine specific options] </td> 
   <td> <p>Spécifiez les options de conversion et spécifiques au moteur. Pour afficher les options disponibles, consultez la documentation de l’API <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert]</a> pour <code>input_format</code> et <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Download a File]</td> 
   <td> <p>Activez cette option si vous souhaitez également inclure des données de fichier dans la sortie du module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Optimiser un fichier]

Ce module d’action optimise et compresse un fichier au format PDF, PNG ou JPG.

Vous spécifiez le fichier et les paramètres d’optimisation et de stockage.

Le module renvoie l’ID du fichier et tous les champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input File]</td> 
   <td>Indiquez si vous souhaitez charger un fichier à l’aide de Workfront Fusion ou fournissez l’URL à partir de laquelle le fichier sera chargé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Upload a File]</p> </td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Import a file from URL] </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong> : saisissez l’URL du fichier que vous souhaitez convertir.</li> 
     <li><strong>[!UICONTROL Headers]</strong> : (facultatif) définissez des en-têtes de demande. Cela s’avère utile, par exemple, lorsque l’URL spécifiée requiert une autorisation.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optimization for] </td> 
   <td> <p>Sélectionnez le profil d’optimisation en fonction des besoins spécifiques de la cible.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Web]</strong> : optimisation pour le web (par défaut).</p> 
      <ul> 
       <li>Supprimer les données redondantes et inutiles pour le web</li> 
       <li>Sous-échantillonner, écrêter et compresser intelligemment les images</li> 
       <li>Fusionner et créer des sous-ensembles de polices</li> 
       <li>Convertir les couleurs en RVB</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Print]</strong> : optimisation pour l’impression.</p> 
      <ul> 
       <li> <p>Supprimer les données redondantes et inutiles pour l’impression</p> </li> 
       <li> <p>Sous-échantillonner, écrêter et compresser intelligemment les images</p> </li> 
       <li> <p>Fusionner et créer des sous-ensembles de polices</p> </li> 
       <li> <p>Convertir les couleurs en CMJN</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Archive]</strong> : optimisation à des fins d’archivage.</p> 
      <ul> 
       <li> <p>Supprimer les données redondantes et inutiles pour l’archivage</p> </li> 
       <li> <p>Compresser intelligemment les images</p> </li> 
       <li> <p>Fusionner et créer des sous-ensembles de polices</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Scanned images]</strong> : optimisation pour les images numérisées.</p> 
      <ul> 
       <li> <p>Profil optimisé pour les PDF principalement composés d’images pixellisées</p> </li> 
       <li> <p>Compresser les images sans réduire significativement la qualité visuelle</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL maximal size reduction]</strong> : optimisation pour la réduction maximale de la taille.</p> 
      <ul> 
       <li> <p>Utiliser la compression maximale possible</p> </li> 
       <li> <p>Peut réduire la qualité visuelle</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input format] </td> 
   <td>Sélectionnez le format du fichier d’entrée que vous souhaitez optimiser. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td> <p>Saisissez un nom de fichier (extension incluse) pour le fichier de sortie cible.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conversion and engine specific options]</td> 
   <td> <p>Spécifiez les options de conversion et spécifiques au moteur. Pour afficher les options disponibles, voir la documentation sur l’API <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert]</a> pour <code>input_format</code> et <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Download a file]</td> 
   <td> <p>Activez cette option si vous souhaitez également inclure des données de fichier dans la sortie du module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Travaux

* [[!UICONTROL Créer un traitement (avancé)]](#create-a-job-advanced)
* [[!UICONTROL Nouvel événement de traitement]](#new-job-event)
* [[!UICONTROL Répertorier les traitements]](#list-jobs)
* [[!UICONTROL Obtenir un traitement]](#get-a-job)
* [[!UICONTROL Supprimer un traitement]](#delete-a-job)

#### [!UICONTROL Créer un traitement (avancé)]

Ce module crée un traitement. Un traitement peut correspondre à une ou plusieurs tâches identifiées dans le champ [!UICONTROL Nom] et liées entre elles à l’aide du champ [!UICONTROL Entrée].

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input Files]</td> 
   <td> <p>Indiquez si vous souhaitez charger un fichier à l’aide de [!DNL Workfront Fusion] ou fournissez l’URL à partir de laquelle le fichier sera chargé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload a File]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Import a File from URL]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong> : saisissez l’URL du fichier que vous souhaitez traiter.</li> 
     <li><strong>[!UICONTROL Headers]</strong> : (facultatif) définissez des en-têtes de demande. Cela s’avère utile, par exemple, lorsque l’URL spécifiée requiert une autorisation.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tasks]</p> </td> 
   <td> <p>Ajoutez les tâches qui seront exécutées dans le traitement.</p> <p>Retrouvez la description des champs des opérations dans la section correspondante.</p> 
    <ul> 
     <li><a href="#convert-a-file" class="MCXref xref">[!UICONTROL Convert a file]</a> </li> 
     <li><a href="#capture-a-website" class="MCXref xref">[!UICONTROL Capture a Website]</a> </li> 
     <li><a href="#optimize-a-file" class="MCXref xref">[!UICONTROL Optimize a File]</a> </li> 
     <li><a href="#create-an-archive" class="MCXref xref">[!UICONTROL Create an Archive]</a> </li> 
     <li><a href="#merge-files" class="MCXref xref">[!UICONTROL Merge Files]</a> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Execute a Command]</strong> </p> <p>Pour plus d’informations sur l’exécution d’une commande, voir la documentation de l’API <a href="https://cloudconvert.com/api/v2/command#command-tasks">[!DNL CloudConvert]</a>.</p> </li> 
     <li> <p><strong>[!UICONTROL Export a File to Temporary URL]</strong> </p> <p> Spécifiez le nom de la tâche et le nom de la tâche d’entrée (par exemple, Conversion).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag] </td> 
   <td> <p>Saisissez une balise. Les balises sont des chaînes arbitraires permettant d’identifier le traitement. Elles n’ont aucun effet et peuvent être utilisées pour associer le traitement à un ID.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un traitement]

Ce module supprime un traitement, y compris toutes les tâches et données.

>[!NOTE]
>
>Les traitements sont automatiquement supprimées 24 heures après leur fin.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Job ID]</td> 
   <td> <p>Saisissez ou mappez l’ID du traitement que vous souhaitez supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un traitement]

Ce module récupère les détails du traitement.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Job ID]</td> 
   <td> <p>Saisissez ou mappez l’ID du traitement dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Répertorier les traitements]

Ce module récupère tous les traitements qui ont été exécutés dans votre compte.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status] </td> 
   <td> <p>Sélectionnez le statut du traitement sur lequel filtrer les travaux renvoyés.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Définissez le nombre de traitements que Workfront Fusion 2.0 renverra au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nouvel événement de traitement]

Se déclenche lorsqu’un traitement ou une tâche est créé(e), terminé(e) ou échoue dans votre compte.

>[!NOTE]
>
>* Un traitement créé avec le module [!UICONTROL Créer un traitement (avancé)] est composé de *plusieurs* tâches.
>* Le déclencheur [!UICONTROL Nouvel événement de traitement] se déclenche également lorsqu’une tâche *individuelle* est créée, est terminée ou a échoué.
>

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td>Saisissez le nom du webhook. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format] </td> 
   <td>Sélectionnez si vous souhaitez enregistrer le site web capturé au format PNG, JPG ou PDF. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event]</td> 
   <td>Sélectionnez si le module se déclenche lorsque le traitement ou la tâche est créé(e), terminé(e) ou échoue.</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Si vous utilisez l’agrégateur de tableaux (par exemple, vous avez plusieurs fichiers dans différents formats à convertir), utilisez l’option **[!UICONTROL Je ne connais pas le format d’entrée]** dans la boîte de dialogue [!UICONTROL Ajouter une tâche]. Sinon, l’erreur est renvoyée.
>* Lier des tâches dans un traitement (nom > entrée, nom > entrée, etc.) :
>
>  ![](assets/linking-name-across-jobs-350x808.png)>

### Tâches

* [[!UICONTROL Obtenir une tâche]](#get-a-task)
* [[!UICONTROL Télécharger un fichier]](#download-a-file)
* [[!UICONTROL Lister des tâches]](#list-tasks)
* [[!UICONTROL Recommencer une tâche]](#retry-a-task)
* [[!UICONTROL Annuler une tâche]](#cancel-a-task)
* [[!UICONTROL Supprimer une tâche]](#delete-a-task)

#### [!UICONTROL Annuler une tâche]

Ce module annule une tâche dont le statut est en attente ou en cours de traitement.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Task ID]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de la tâche que vous souhaitez annuler.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer une tâche]

Supprime une tâche, y compris toutes les données.

>[!NOTE]
>
>Les tâches terminées sont automatiquement supprimées après 24 heures.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Task ID]</td> 
   <td> <p> Saisissez (mappez) l’identifiant de la tâche que vous souhaitez supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger un fichier]

Ce module récupère le nom de fichier et les données du fichier à partir de la tâche spécifiée.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Task ID]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de la tâche à partir de laquelle vous souhaitez télécharger le fichier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir une tâche]

Ce module récupère les détails d’une tâche.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Task ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la tâche dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lister des tâches]

Ce module récupère toutes les tâches de votre compte en fonction des paramètres de filtrage.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status] </td> 
   <td> <p>Sélectionnez le statut de la tâche pour filtrer les tâches renvoyées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Job ID] </td> 
   <td> <p>Saisissez ou mappez l’ID de traitement pour renvoyer uniquement les tâches du traitement spécifié.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Saisissez le type d’opération pour renvoyer uniquement les tâches avec l’opération spécifiée. </p> <p>Remarque : utilisez le module [!UICONTROL List Possible Operations] pour récupérer les opérations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Réessayer une tâche]

Ce module crée une nouvelle tâche, en fonction des paramètres (payload) d’une autre tâche.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Task ID]</td> 
   <td> <p> Saisissez ou mappez l’ID de la tâche à partir de laquelle vous souhaitez créer une tâche.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

* [[!UICONTROL Obtenir mes informations]](#get-my-info)
* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)

#### [!UICONTROL Obtenir mes informations]

Récupère les détails du compte authentifié de la personne actuelle.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], consultez la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effectuer un appel API]

Permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [Fusion App] à Workfront Fusion, voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe Workfront Fusion - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Saisissez un chemin d’accès relatif à <code>https://api.cloudconvert.com/</code>. Par exemple : <code>/v2/tasks</code></p> <p>Pour obtenir la liste des points d’entrée disponibles, voir la Documentation d’API v2 <a href="https://cloudconvert.com/api/v2">[!DNL CloudConvert]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0 ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard. Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre JSON, placez des guillemets à l’extérieur de l’instruction conditionnelle.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** répertorier les tâches

L’appel API suivant renvoie toutes les tâches de votre compte CloudFront :

URL : `/v2/tasks`

Méthode : `GET`

![](assets/cloudconvert-api-example-input.png)

Les résultats de la recherche peuvent être trouvés dans la sortie du module sous [!UICONTROL Lot] > [!UICONTROL Corps] > [!UICONTROL Données].

Dans notre exemple, 6 tâches ont été renvoyées :

![](assets/cloudconvert-api-example-output.png)

## Dépannage {#troubleshooting}

Voir le tableau suivant pour les erreurs possibles et leurs solutions :

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Erreur</p> </th> 
   <th>Étapes suivantes</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL The output file size exceeds the limit allowed for your scenario.]</span> </p> </td> 
   <td> <p>Référez-vous aux limites de taille des fichiers.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL You have exceeded the maximum conversion time.]</span> </p> </td> 
   <td> <p>Le plan gratuit [!DNL CloudConvert] offre 25 minutes de conversion par jour. Si votre utilisation dépasse la limite du plan gratuit, vous pouvez passer à un forfait (prépayé) ou à un abonnement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL Failed to read frame size: Could not seek to 1508. �/output/JLIADSA00137P0.mp3: Invalid argument.]</span> </p> </td> 
   <td> <p>Cette erreur se produit par exemple lors de la conversion de fichiers MP3 en fichiers WAV. Assurez-vous que vous avez sélectionné la bonne région, car des références à des fichiers seront trouvées, mais pas seulement le bon fichier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL RuntimeError:] </p> <p><span style="font-weight: normal;">[!UICONTROL Maximum number of repeats exceeded.]</span> </p> </td> 
   <td> <p>Localisez le traitement [!DNL CloudConvert] correspondant dans la liste des traitements de votre tableau de bord [!DNL CloudConvert] et vérifiez la durée du taitement :</p> <p> <img src="assets/cloudconvert-duration-350x177.png" style="width: 350;height: 177;"> </p> <p>Le délai d’expiration du module [!DNL CloudConvert] &gt; [!UICONTROL Convert a File] est fixé à 3 minutes. Si la durée du traitement dépasse 3 minutes (peut-être en raison d’une surcharge temporaire du service [!DNL CloudConvert]), le module génère l’erreur mentionnée ci-dessus.</p> <p>Dans ce cas, envisagez l’une des options suivantes :</p> 
    <ul> 
     <li>Activez l’option <strong>[!UICONTROL Allow storing of Incomplete Executions]</strong> dans les paramètres du scénario pour stocker les exécutions incomplètes en vue d’une résolution manuelle ultérieure. En option, vous pouvez joindre un itinéraire de gestion des erreurs au module [!DNL CloudConvert] avec la directive [!UICONTROL Break] pour résoudre automatiquement les exécutions incomplètes.</li> 
     <li>Désactivez l’option <strong>[!UICONTROL Download a file]</strong> dans le module [!DNL CloudConvert] &gt; [!UICONTROL Convert a file]. Dans ce cas, le module n’attend pas le résultat de la conversion. Pour obtenir le résultat de la conversion, créez un nouveau scénario et utilisez le déclencheur [!DNL CloudConvert] &gt; [!UICONTROL New Job Event].</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Exemple de workflow pour le connecteur [!DNL CloudConvert]

>[!INFO]
>
>**Exemple :** conversion d’une vidéo du format MOV au format MP4
>
>1. Consultez [https://cloudconvert.com/video-converter](https://>cloudconvert.com/video-converter).
>1. Cliquez sur **[!UICONTROL Sélectionner un fichier]** et choisissez votre exemple de fichier MOV.
>1. Cliquez sur le menu déroulant, à côté de **[!UICONTROL Convertir en]** et choisissez **[!UICONTROL MP4]**.
>
>1. Cliquez sur l’icône en forme de **[!UICONTROL clé à molette]**.
>1. Configurez les paramètres de compression MP4 selon vos besoins.
>1. Cliquez sur **[!UICONTROL Convertir]**.
>1. Une fois la conversion terminée, cliquez sur **[!UICONTROL Télécharger]**.
>1. Examinez la vidéo convertie.
>1. Répétez les étapes 1 à 8 jusqu’à ce que vous ayez trouvé les paramètres de conversion optimaux pour l’étape 5.
>1. Consultez [https://cloudconvert.com/api/v2/convert#convert-tasks](https://cloudconvert.com/api/v2/convert#convert-tasks).
>1. Choisissez **[!UICONTROL mov]** pour le champ **[!UICONTROL input_format]**.
>
>1. Choisissez **[!UICONTROL mp4]** pour le champ **[!UICONTROL output_format]**.
>
>1. Une liste de tous les paramètres possibles comme video_codec, crf, etc. apparaîtra.
>1. Dans Workfront Fusion 2.0, insérez le module **[!UICONTROL CloudConvert]** > **[!UICONTROL Convertir un fichier]** dans votre scénario.
>
>1. Ouvrez les paramètres du module.
>1. Configurez le module comme indiqué ci-dessous :
>
>   ![](assets/cloudconvert-mp4-example.png)
>
>1. Veillez à inclure tous les paramètres dans le champ Options spécifiques à la conversion et au moteur : pour chaque paramètre de l’étape 5, repérez le paramètre correspondant de l’étape 13 et sa valeur correspondante.
