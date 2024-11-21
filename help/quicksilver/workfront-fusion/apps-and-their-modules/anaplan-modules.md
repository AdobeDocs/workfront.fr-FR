---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Anaplan
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Anaplan, ainsi que le connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1863'
ht-degree: 97%

---

# Modules [!DNL Anaplan]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Anaplan]et le connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, consultez [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

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
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Avant d’utiliser le connecteur [!DNL Anaplan], assurez-vous que les conditions préalables suivantes sont remplies :

* Vous devez avoir un compte [!UICONTROL Anaplan] actif.
* Vous devez configurer des espaces de travail, des modèles et d’autres objets [!DNL Anaplan] dans votre compte [!UICONTROL Anaplan] avant que [!DNL Workfront Fusion] puisse interagir avec eux.

## Informations sur l’API Anplan

Le connecteur Anaplan utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td>https://api.anaplan.com/2/0/
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Version de l’API</td> 
   <td> v2 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.11.5/td&gt; 
 </tbody> 
</table>

## Connecter [!DNL Anaplan] à [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

Pour créer une connexion pour vos modules [!DNL Anaplan], procédez comme suit :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la zone [!UICONTROL Connexion].
1. Sélectionnez le type de connexion.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL Basic]</td> 
      <td> <p>La création d’une connexion [!UICONTROL Basic] [!DNL Anaplan] nécessite uniquement une adresse électronique et un mot de passe. </p> <p>Saisissez un nom pour la connexion, puis votre adresse e-mail et le mot de passe de votre compte [!DNL Anaplan].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL CA Certificate]</td> 
      <td> <p>Une connexion [!UICONTROL CA Certificate] [!DNL Anaplan] requiert ces éléments : [!UICONTROL Certificate Key], [!UICONTROL Encoded Data] et [!UICONTROL Encoded Signed Data]. Vous pouvez les générer dans votre compte [!DNL Anaplan]. Pour obtenir des instructions, consultez la documentation [!DNL Anaplan].</p> <p>Saisissez un nom pour la connexion, puis saisissez les informations [!UICONTROL Certificate Key], [!UICONTROL Encoded Data] et [!UICONTROL Encoded Signed Data] que vous avez générées dans votre compte [!DNL Anaplan].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.

## Modules [!DNL Anaplan] et leurs champs

Lorsque vous configurez les modules [!DNL Anaplan], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Anaplan] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

#### [!DNL Watch records]

Ce module de déclenchement lance un scénario lorsqu’un enregistrement du type choisi est créé ou mis à jour.

>[!NOTE]
>
>Ce module renvoie les données des nouveaux enregistrements. Il ne renvoie pas les données des enregistrements existants modifiés.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Anaplan], voir <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Anaplan] à [!DNL Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type d’objet à surveiller</td> 
   <td>Sélectionnez le type d’élément à surveiller. Le scénario commence lorsque ce type d’enregistrement est créé ou mis à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID d’&lt;Object&gt;</td> 
   <td>Saisissez l’identifiant de l’objet dans Anplan, tel qu’un modèle ou un module, associé aux objets que vous souhaitez surveiller.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit [action] au cours de chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Créer un élément de liste]](#create-a-list-item)
* [[!UICONTROL Lancer un appel API personnalisé]](#make-a-custom-api-call)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Exécuter une action]](#run-an-action)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)
* [[!UICONTROL Charger un fichier]](#upload-a-file)

#### [!UICONTROL Créer un élément de liste]

Ce module d’action ajoute un nouvel élément à une liste dans Anaplan.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Connection]</td>
        <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Anaplan], voir <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Anaplan] à [!DNL Workfront Fusion]</a> dans cet article.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Workspace ID]</td>
        <td>Sélectionnez ou mappez l’identifiant de l’espace de travail Anaplan qui contient la liste dans laquelle vous souhaitez ajouter un élément.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Model ID]</td>
        <td>Sélectionnez ou mappez l’identifiant du modèle qui contient la liste dans laquelle vous souhaitez ajouter un élément.</td>
    </tr>
    <tr>
        <td>[!UICONTROL List ID]</td>
        <td>Sélectionnez ou mappez l’identifiant de la liste dans laquelle vous souhaitez créer un élément.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Name]</td>
        <td>Saisissez un nom pour le nouvel élément.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Code]</td>
        <td>Saisissez le code du nouvel élément. Les codes sont des codes générés par la personne qui vous permettent de distinguer les éléments de ligne portant le même nom.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Parent]</td>
        <td>Saisissez le nom de l’élément parent sous lequel vous souhaitez créer l’élément.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Properties]</td>
        <td>Si la liste dans laquelle vous souhaitez ajouter un élément comporte des propriétés personnalisées, sélectionnez les propriétés pour lesquelles vous souhaitez ajouter des valeurs, puis ajoutez les valeurs.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Subsets]</td>
        <td>Si la liste dans laquelle vous souhaitez ajouter des éléments comporte des sous-ensembles personnalisés, sélectionnez les sous-ensembles auxquels vous souhaitez ajouter l’élément, puis sélectionnez <b>[!UICONTROL Yes]</b> pour ajouter le nouvel élément à ce sous-ensemble.</td>
    </tr>
</table>

#### [!UICONTROL Lancer un appel API personnalisé]

Ce module vous permet d’effectuer un appel API personnalisé à l’API [!DNL Anaplan].

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Anaplan], voir <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Anaplan] à [!DNL Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisir un chemin relatif à <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] Ajoute automatiquement des en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Saisissez la chaîne de requête.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un enregistrement]

Ce module d’action supprime un enregistrement existant.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Anaplan], voir <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Anaplan] à [!DNL Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Sélectionnez ou mappez l’identifiant de l’espace de travail Anaplan qui contient l’objet que vous souhaitez supprimer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model ID]</td> 
   <td>Saisissez ou mappez l’identifiant du modèle qui contient l’objet que vous souhaitez supprimer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Supprimer</td> 
   <td> <p>Sélectionnez le type d’objet à supprimer.</p> 
    <ul> 
     <li> <p><b>Actions</b> </p> <p>Sélectionnez ou mappez l’action à supprimer.</p> </li> 
     <li> <p><b>Élément de liste</b> </p> <p>Sélectionnez la liste dans laquelle vous souhaitez supprimer un élément, puis saisissez ou mappez l’identifiant ou le code de l’élément à supprimer.</p>  </li> 
     <li> <p><b>[!UICONTROL File]</b> </p> <p>Sélectionnez ou mappez le fichier à supprimer.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit un seul enregistrement.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Anaplan], voir <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Anaplan] à [!DNL Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement à lire.</p> 
    <ul> 
     <li> <p><b>Modèle</b> </p> <p>Sélectionnez ou mappez l’identifiant du modèle à lire.</p> </li> 
     <li> <p><b>Liste de modèles</b> </p> <p>Sélectionnez ou mappez les identifiants de l’espace de travail et du modèle qui contiennent la liste que vous souhaitez lire, puis sélectionnez la liste. Dans le champ [!UICONTROL Data type], indiquez si vous souhaitez lire des données ou des métadonnées.</p> </li> 
     <li> <p><b>Version du modèle</b> </p> <p>Sélectionnez ou mappez l’identifiant du modèle que vous souhaitez lire.</p> </li> 
     <li> <p><b>Utilisateur ou utilisatrice</b> </p> <p>Indiquez si vous souhaitez renvoyer des données sur le ou la propriétaire du compte utilisé ou sur une autre personne. Si vous sélectionnez une autre personne, sélectionnez son nom.</p> </li> 
     <li> <p><b>Espace de travail</b> </p> <p>Sélectionnez ou mappez l’identifiant de l’espace de travail que vous souhaitez lire.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Exécuter une action]

Ce module d’action importe, exporte, supprime ou traite une action.

<table style="table-layout:auto"> 
     <col/>
     <col/>
     <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Anaplan], voir <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect Anaplan to Workfront Fusion]</a> dans cet article.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Workspace ID]</td>
        <td>Sélectionnez ou mappez l’identifiant de l’espace de travail[!DNL Anaplan] dans lequel vous souhaitez effectuer l’action.</td>
      </tr>
      <tr >
        <td role="rowheader">[!UICONTROL Model ID]</td>
        <td>Sélectionnez ou mappez l’identifiant du modèle dans lequel vous souhaitez effectuer l’action.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Action type]</td>
        <td>
          <p>Sélectionnez l’action que vous souhaitez effectuer.</p>
            <ul>
              <li>
                <p><b>[!UICONTROL Delete]</b>
                </p>
                <p>Saisissez ou mappez l’identifiant de l’action que vous souhaitez supprimer.</p>
              </li>
              <li>
                <p><b>[!UICONTROL Export]</b>
                </p>
                <p>Saisissez ou mappez l’identifiant de la définition d’exportation que vous souhaitez utiliser. Vous pouvez exporter vers les formats de fichier suivants :</p>
                  <ul>
                    <li>
                      <p>XLS</p>
                    </li>
                    <li>
                      <p>XLSX</p>
                    </li>
                    <li>
                      <p>CSV</p>
                    </li>
                  </ul>
                </li>
                <li>
                  <p><b>[!UICONTROL Import] </b>
                  </p>
                  <p style="font-weight: normal;">Saisissez ou mappez l’identifiant de la définition d’importation que vous souhaitez utiliser.</p>
                </li>
                <li>
                 <p><b>[!UICONTROL Process]</b>
                 </p>
                  <p>Saisissez ou mappez l’identifiant du processus que vous souhaitez utiliser. </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour un seul enregistrement dans [!UICONTROL Anaplan].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Anaplan], voir <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Anaplan] à [!DNL Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez mettre à jour.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL List item]</b> </p> <p>Pour les champs, voir <a href="#create-a-list-item" class="MCXref xref">Créer un élément de liste</a> dans cet article.</p> </li> 
     <li> <p><b>[!UICONTROL Module cell data]</b> </p> <p>Lorsque vous mettez à jour les données de cellule, tous les calculs en aval qui utilisent ces données sont également mis à jour.</p> <p>Remplissez les champs suivants :</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Model ID]</b> </p> <p>Sélectionnez ou mappez le modèle qui contient la cellule que vous souhaitez mettre à jour.</p> </li> 
       <li> <p><b>[!UICONTROL Module ID]</b> </p> <p>Sélectionnez ou mappez le module contenant la cellule que vous souhaitez mettre à jour.</p> </li> 
       <li> <p><b>[!UICONTROL Line item name]</b> </p> <p>Sélectionnez ou mappez l’élément de ligne de la cellule à mettre à jour.</p> </li> 
       <li> <p style="font-weight: bold;">[!UICONTROL Dimension ID]</p> <p>Sélectionnez ou mappez la dimension qui se trouve sur l’élément de ligne.</p> 
       <p><b>Note :</b> 
       <ul>
       <li> La clé de Dimension (valeur) doit être : <code>dimensionName</code> (suivant) ou <code>dimensionId</code> (ID).</li>
       <li>La clé d’élément (valeur) doit être <code>itemName</code> (texte), <code>itemCode</code> (texte) ou <code>itemId</code> (ID).</li>
       <li>Les clés de Dimension et d’élément doivent être du même type (texte ou identifiant).
       </ul>
        </p> 
        <p>Pour plus d’informations sur les dimensions, recherchez Dimensions dans le [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[!UICONTROL Value]</b> </p> <p>Saisissez ou mappez la nouvelle valeur pour la cellule.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Model current fiscal year]</b> </p> <p>Saisissez l’identifiant de l’espace de travail et l’identifiant du modèle pour lequel vous souhaitez mettre à jour l’année fiscale, puis saisissez ou mappez la nouvelle année pour le modèle.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Charger un fichier]

Ce module d’action charge un fichier vers Anaplan. Le fichier doit avoir déjà été chargé vers Anaplan. Vous pouvez utiliser ce module pour le charger vers d’autres emplacements dans Anaplan.
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Connection]</td>
<td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Anaplan], voir <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Anaplan] à [!DNL Workfront Fusion]</a> dans cet article.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Workspace ID]</td>
<td>Sélectionnez ou mappez l’identifiant de l’espace de travail [!DNL Anaplan] dans lequel vous souhaitez charger un fichier.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Model ID]</td>
<td>Sélectionnez ou mappez l’identifiant du modèle dans lequel vous souhaitez charger un fichier.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL File ID]</td>
<td>Sélectionnez ou mappez l’identifiant du fichier que vous souhaitez charger.</td>
</tr>
</tbody>
</table>
</div>

### Recherches

#### [!UICONTROL Obtenir un enregistrement]

Ce module de recherche renvoie tous les enregistrements accessibles du type sélectionné.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Anaplan], voir <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connecter [!DNL Anaplan] à [!DNL Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record types]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez récupérer.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Workspaces]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Models]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Line items]</b> </p> <p>Sélectionnez ou mappez l’identifiant du modèle qui contient les éléments [!DNL line] que vous souhaitez récupérer.</p> </li> 
       <li> <p><b>[!UICONTROL Model lists]</b> </p> <p>Sélectionnez ou mappez l’identifiant de l’espace de travail et l’identifiant du modèle qui contiennent les listes de modèles que vous souhaitez récupérer.</p> </li> 
       <li> <p><b>[!UICONTROL Model calendar]</b> </p> <p>Sélectionnez ou mappez l’identifiant de l’espace de travail qui contient le calendrier du modèle que vous souhaitez récupérer.</p> </li> 
       <li> <p><b>Versions de modèles</b> </p> </li> 
       <li> <p>Sélectionnez ou mappez [!UICONTROL ]l’identifiant du modèle contenant les versions de modèle que vous souhaitez récupérer.</p> </li> 
       <li> <p><b>[!UICONTROL Users]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Views]</b> </p> <p>Choisissez si vous souhaitez choisir la vue par module ou par modèle, puis sélectionnez ou mappez l’identifiant du module ou du modèle qui contient la vue que vous souhaitez récupérer.</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Return workspace size]</td> 
   <td>Activez cette option pour renvoyer une estimation de la taille actuelle de l’espace de travail. Cette estimation est basée sur la taille de tous les modules de l’espace de travail.</td> 
  </tr> 
 </tbody> 
</table>
