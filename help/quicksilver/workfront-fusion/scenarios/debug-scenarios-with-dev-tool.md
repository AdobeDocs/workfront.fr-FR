---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Déboguer des scénarios avec le DevTool d’Adobe Workfront Fusion
description: Le Devtool d’Adobe Workfront Fusion vous permet de comprendre des scénarios et de résoudre les problèmes qui y sont liés. Le Devtool ajoute un panneau supplémentaire aux outils de développement Chrome. Grâce à ce panneau du débogueur, vous pouvez vérifier toutes les exécutions manuelles de votre scénario, réviser toutes les opérations effectuées et afficher les détails de chaque appel API effectué. Vous pouvez voir quel module, quelle opération ou quelle réponse unique a provoqué l’erreur et utiliser ces connaissances pour affiner votre scénario.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 6edcb5b826bdcf37b62396a926c923875a3a1436
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 100%

---

# Déboguer les scénarios avec le Devtool d’[!DNL Adobe Workfront Fusion]

Le Devtool d’[!DNL Adobe Workfront Fusion] vous permet de comprendre des scénarios et de résoudre les problèmes qui y sont liés. Le Devtool ajoute un panneau supplémentaire aux [!DNL Chrome Developer Tools]. Grâce à ce panneau du débogueur, vous pouvez vérifier toutes les exécutions manuelles de votre scénario, réviser toutes les opérations effectuées et afficher les détails de chaque appel API effectué. Vous pouvez voir quel module, quelle opération ou quelle réponse unique a provoqué l’erreur et utiliser ces connaissances pour affiner votre scénario.

>[!NOTE]
>
>La connexion au panneau du débogueur sera limitée ou indisponible pour les scénarios confidentiels, les exécutions automatiques et les opérations réussies.

Pour une vidéo d’introduction et une présentation de l’outil Fusion Devtool, voir

* [Outil de développement Fusion](https://video.tv.adobe.com/v/3427031/){target=_blank}.
* [Présentation du Devtool](https://experienceleague.adobe.com/fr/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough)

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir [[!DNL Adobe Workfront Fusion] Licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Accéder au Devtool de Workfront Fusion

L’accès au Devtool varie selon que vous utilisez ou non Fusion dans [!DNL Adobe Unified Experience].

* [Accéder au Devtool dans  [!DNL Adobe Unified Experience]](#access-the-devtool-in-the-adobe-unified-experience)
* [Accéder au Devtool dans l’expérience [!DNL Fusion] classique](#access-the-devtool-in-the-classic-fusion-experience)

### Accéder au Devtool dans [!DNL Adobe Unified Experience] ou dans la nouvelle expérience Fusion 

Si vous utilisez Fusion dans Adobe Unified Shell ou si vous avez effectué la mise à jour vers la nouvelle expérience Fusion, vous pouvez accéder au Devtool à partir de l’éditeur de scénario.

1. Cliquez sur l’icône **Outils d’assistance** ![Outils d’assistance](assets/debugger-icon.png) située en bas de l’écran.

Ou :

1. Accédez à l’éditeur de scénarios pour le scénario que vous souhaitez déboguer.

   Pour localiser l’éditeur de scénario, consultez [Éditeur de scénario](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md).

1. Cliquez avec le bouton droit dans une zone vide de la page (et non sur un module).
1. Sélectionnez **Ouvrir le Devtool**.

### Accéder au Devtool dans l’expérience [!DNL Fusion] classique

Pour utiliser le Devtool dans l’expérience [!DNL Fusion] classique, vous devez installer une extension [!DNL Chrome]. Vous pouvez ensuite utiliser cette extension à partir des outils de développement [!DNL Chrome].

* [Installer l’extension Devtool  [!DNL Chrome] ](#install-the-chrome-devtool-extension)
* [Rechercher le Devtool  [!DNL Workfront Fusion] ](#locate-the-workfront-fusion-devtool)

#### Installer l’extension Devtool [!DNL Chrome]

Vous pouvez ajouter le Devtool de [!DNL Workfront Fusion] à [!DNL Chrome] par le biais du [!UICONTROL [!DNL Chrome] Web Store].

1. Cliquez sur [ce lien](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn) pour accéder au Devtool de [!DNL Workfront Fusion] sur le [!UICONTROL [!DNL Chrome] Web Store].
1. Cliquez sur **[!UICONTROL Ajouter à[!DNL Chrome]]**.
1. Dans la fenêtre qui s’ouvre, examinez les autorisations. Si vous acceptez les autorisations, cliquez sur **[!UICONTROL Ajouter une extension]**.

L’extension Devtool [!DNL Workfront Fusion] est ajoutée à vos extensions [!DNL Chrome].


#### Localiser l’exension Devtool [!DNL Workfront Fusion]

Pour utiliser l’extension Devtool [!DNL Workfront Fusion], vous devez ajouter l’extension Devtool [!DNL Workfront Fusion] à votre navigateur [!DNL Chrome], comme décrit dans [Installer l’extension Chrome Devtool](#install-the-chrome-Devtool-extension).

1. Ouvrez votre scénario [!DNL Workfront Fusion].
1. Ouvrez [!DNL Chrome Developer Tools] :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Commande+Option+I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Ctrl+Maj+I</p> <p> Ou </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Il est recommandé d’ancrer la [!DNL Chrome Developer Console] en bas pour une meilleure vue de vos modules.

1. Cliquez sur l’onglet **[!DNL Workfront Fusion]** dans [!DNL Chrome Dev Tools].

## Utiliser l’extension Devtool [!DNL Workfront Fusion]

Le Devtool de Workfront Fusion est divisé en trois sections principales. Vous pouvez les trouver dans le panneau de gauche de votre fenêtre Devtool.

* [Live Stream](#live-stream)
* [Débogueur de scénario](#scenario-debugger)
* [Outils](#tools)

### Live Stream

Le Live Stream affiche ce qui se passe en arrière-plan lorsque vous cliquez sur Exécuter une fois dans votre scénario.

1. Cliquez sur l’icône **[!UICONTROL Live Stream]** ![](assets/live-stream-icon.png) pour ouvrir la section Live Stream.
1. Effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Action</th> 
      <th>Instructions</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">Afficher les informations sur la requête</td> 
      <td> <p>Vous pouvez afficher les informations suivantes pour chaque module dans votre scénario.</p> 
       <ul> 
        <li> <p>En-têtes de la requête (URL du point d’entrée de l’API, méthode HTTP, heure et date d’appel de la requête, en-têtes de la requête et chaîne de requête)</p> </li> 
        <li> <p>Corps de la requête</p> </li> 
        <li> <p>En-têtes de la réponse</p> </li> 
        <li> <p>Corps de la réponse</p> </li> 
       </ul> <p>Pour afficher ces informations, cliquez sur l’onglet approprié dans le panneau de droite du Devtool de [!DNL Workfront Fusion].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Rechercher des requêtes et des réponses</p> </td> 
      <td> <p>Saisissez le terme de recherche dans le champ de recherche du panneau de gauche du Devtool de [!DNL Workfront Fusion] pour afficher uniquement les requêtes qui contiennent le terme de recherche.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Supprimer la liste des requêtes </p> </td> 
      <td> <p>Cliquez sur l’icône de la corbeille dans le coin supérieur droit du panneau de gauche du Devtool pour effacer la liste des requêtes enregistrées par le Devtool de [!DNL Workfront Fusion]. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Activer la connexion à la console</p> </td> 
      <td> <p>Cliquez sur l’icône d’ordinateur <img src="assets/console-computer-icon.png"> dans le coin supérieur droit du panneau de gauche du Devtool.</p> <p>La connexion à la console est activée lorsque l’icône d’ordinateur est verte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Récupérer la requête au format JSON brut ou cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>JSON brut</strong> </p> <p>Cliquez sur <strong>[!UICONTROL Copy RAW]</strong> dans le coin supérieur droit du volet de droite du Devtool.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Cliquez sur <strong>[!UICONTROL Copy cURL]</strong> dans le coin supérieur droit du volet de droite du Devtool.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Débogueur de scénario

Le débogueur de scénario est utile pour les scénarios plus complexes. Il affiche l’historique du scénario qui s’exécute et vous permet de rechercher les modules par leur nom ou ID.

1. Cliquez sur l’icône **[!UICONTROL Débogueur de scénario]** ![](assets/scenario-debugger-icon.png) pour ouvrir le débogueur de scénario.
1. (Facultatif) Saisissez le terme de recherche (nom ou ID de module) dans le champ de recherche du volet de gauche du Devtool de [!DNL Workfront Fusion] dans la section [!UICONTROL Débogueur de scénario].
1. Double-cliquez sur le nom du module pour en ouvrir les paramètres dans l’éditeur de scénarios.
1. Affichez les détails de la requête en cliquant sur l’opération souhaitée.

### Outils

Le Devtool [!DNL Workfront Fusion] contient des outils qui facilitent la configuration de scénario.

1. Cliquez sur l’icône **[!UICONTROL Outils]** ![](assets/console-tools-icon.png) pour ouvrir les outils.
1. Sélectionnez l’outil que vous souhaitez utiliser.
1. Configurez les champs comme indiqué ci-dessous.
1. Cliquez sur **[!UICONTROL Exécuter]**.

Outils et leurs champs :

* [Cibler un module](#focus-a-module)
* [Rechercher des modules par mappage](#find-modules-by-mapping)
* [Obtenir les métadonnées de l’application](#get-app-metadata)
* [Copier le mappage](#copy-mapping)
* [Copier le filtre](#copy-filter)
* [Permuter la connexion](#swap-connection)
* [Permuter la variable](#swap-variable)
* [Permuter l’application](#swap-app)
* [Base 64](#base-64)
* [Copier le nom du module](#copy-module-name)
* [Remapper la source](#remap-source)
* [Mettre en surbrillance l’application](#highlight-app)
* [Migrer GS](#migrate-gs)

#### [!UICONTROL Cibler un module]

Ouvre les paramètres du module spécifié par ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module ID]</td>
        <td>Saisissez l’ID du module dont vous souhaitez ouvrir les paramètres.</td>
    </tr>
</table>

#### [!UICONTROL Rechercher des modules par mappage]

Permet de rechercher les valeurs des modules pour un terme spécifique. La sortie inclut les ID des modules qui contiennent le terme recherché.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Keyword]</td> 
   <td> <p> Saisissez le terme à rechercher. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Use Only Values]</p> </td> 
   <td> <p>Activez cette option pour rechercher uniquement dans les valeurs des champs du module.</p> <p>Désactivez cette option pour rechercher également dans les noms des champs du module.</p> <p>La recherche est effectuée par le biais des paramètres de nom et de libellé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir les métadonnées de l’application]

Récupère les métadonnées de l’application par le nom ou l’ID du module de l’application. Cette fonction est utile, par exemple, lorsque vous devez connaître la version de l’application utilisée dans votre scénario.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Sélectionnez le module dont vous souhaitez récupérer les métadonnées.</td>
    </tr>
</table>

#### [!UICONTROL Copier le mappage]

Copie les valeurs du module source vers le module cible.

>[!CAUTION]
>
>Veillez à définir les modules source et cible appropriés. Si vous sélectionnez un autre type de module, les valeurs du module cible seront supprimées.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Sélectionnez le module ou saisissez l’ID du module dont vous souhaitez copier les valeurs de champ.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Sélectionnez le module ou saisissez l’ID du module dans lequel vous souhaitez insérer les valeurs du module source.</p> <p>Important : les valeurs du module cible seront remplacées.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier le filtre]

Copie les paramètres de filtre du module source vers le module cible.

>[!NOTE]
>
>L’action de copie est effectuée sur le filtre placé sur le côté gauche du module sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Sélectionnez le module ou saisissez l’identifiant du module à partir duquel vous souhaitez copier les valeurs de filtre.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Sélectionnez le module ou saisissez l’identifiant du module dans lequel vous souhaitez insérer les valeurs de filtre du module source.</p> <p>Important : les valeurs du module cible seront remplacées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Preserve Fallback Route setting]</p> </td> 
   <td> <p>Le filtre source est défini comme l’itinéraire de secours. Activez cette option pour définir également le filtre cible comme itinéraire de secours.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Permuter la connexion]

Duplique une connexion du module source à tous les modules de la même application dans le scénario.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Sélectionnez le module ou saisissez l’identifiant du module à partir duquel vous souhaitez dupliquer la connexion.</td>
    </tr>
</table>

#### [!UICONTROL Permuter la variable]

Recherche les variables spécifiées dans le scénario et les remplace par une nouvelle variable.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable to Find]</td> 
   <td> <p> Localisez la variable que vous souhaitez remplacer à partir du module dans votre scénario et copiez-la dans ce champ ([!UICONTROL Variable to Find]). Dans le champ, elle apparaît avec des accolades doubles. Exemple : <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace With]</p> </td> 
   <td> <p>Localisez la variable que vous souhaitez remplacer à partir du module dans votre scénario et copiez-la dans ce champ ([!UICONTROL Variable to Find]). Dans le champ, elle apparaît avec des accolades doubles. Exemple : <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>Sélectionnez le module dans lequel vous souhaitez remplacer la variable. Si aucun module n’est sélectionné, la variable sera remplacée dans l’ensemble du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Permuter l’application]

Remplace la version sélectionnée de l’application dans votre scénario par une autre version de l’application.

Cela peut être utilisé, par exemple, pour mettre à jour les modules de Gmail et des applications de messagerie vers la dernière version.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Replaced]</td> 
   <td> <p> Sélectionnez l’application que vous souhaitez remplacer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace with]</p> </td> 
   <td> <p>Sélectionnez l’application par laquelle vous souhaitez la remplacer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Permet de coder les données saisies en Base64 ou de décoder du Base64. Certaines requêtes sont codées en Base64. Cet outil est utile lorsque vous souhaitez rechercher des données spécifiques dans la requête codée.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Indiquez si vous souhaitez coder les données du champ [!UICONTROL Raw Data] en Base64 ou décoder Base64 en données brutes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Raw Data]</p> </td> 
   <td> <p> Saisissez les données que vous souhaitez encoder en Base64, ou les données Base64 que vous souhaitez décoder en données brutes, en fonction de l’option sélectionnée dans le champ [!UICONTROL Operation] ci-dessus.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier le nom du module]

Copie le nom du module sélectionné dans le presse-papiers.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module] </td> 
   <td> <p>Sélectionnez le module dont vous souhaitez copier le nom.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remapper la source]

Vous permet de modifier la source de mappage d’un module à un autre.

Vous devez d’abord ajouter le module que vous voulez utiliser comme module source à l’itinéraire de votre scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> Sélectionnez le module que vous souhaitez remplacer en tant que source de mappage pour les autres modules de votre scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Sélectionnez le module à utiliser comme nouvelle source de mappage.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module to Edit]</p> </td> 
   <td> <p>Sélectionnez le module pour lequel vous souhaitez modifier le mappage si vous ne souhaitez pas modifier le mappage dans l’ensemble du scénario. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre l’application en surbrillance]

Met en surbrillance les modules de l’application spécifiée dans votre scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Highlighted] </td> 
   <td> <p> Sélectionnez l’application que vous souhaitez mettre en surbrillance dans votre scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Version] </p> </td> 
   <td> <p>Sélectionnez la version de l’application que vous souhaitez mettre en surbrillance.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Highlight Color]</p> </td> 
   <td> <p> Saisissez la couleur hexadécimale à utiliser pour la mise en surbrillance des modules.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migrer GS]

Cet outil est conçu spécifiquement pour mettre à niveau les modules [!DNL Google Sheets] (ancienne version) vers la dernière version de [!DNL Google Sheets]. Cela ajoute une nouvelle version du module juste après l&#39;ancienne version du module dans l’itinéraire du scénario.

Ce module ne nécessite pas la configuration d’un paramètre en particulier.
