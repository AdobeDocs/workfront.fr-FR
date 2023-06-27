---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Workday
description: Dans un scénario Adobe Workfront Fusion, vous pouvez automatiser les workflows qui utilisent [!DNL Workday], ainsi que de la connecter à plusieurs applications et services tiers.
author: Becky
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 2%

---

# [!DNL Workday] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Workday], ainsi que de la connecter à plusieurs applications et services tiers.

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
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser la variable [!DNL Workday] , vous devez :

* Prenez un [!DNL Workday] compte .

* Création d’une application OAuth dans [!DNL Workday]. Pour obtenir des instructions, voir [!DNL Workday] documentation.

## Connexion [!DNL Workday] to [!DNL Workfront Fusion]

1. Dans n’importe quel [!DNL Workfront Fusion] module, cliquez sur [!UICONTROL Ajouter] en regard de [!UICONTROL Connexion] field

2. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Nom de la connexion]</p>
                </td>
                <td>Saisissez un nom pour la connexion.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Hôte Workday]</td>
                <td>Saisissez l’adresse de votre [!DNL Workday] hôte sans <code>https://</code>. Par exemple: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL URL des services]</td>
                <td>Saisissez l’adresse de votre [!DNL Workday] services web sans <code>https://</code>. Par exemple: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Nom du tenant]</td>
                <td>Saisissez le client correspondant [!DNL Workday] compte . Votre client est l’identifiant de votre organisation. Vous pouvez le voir dans l’URL que vous utilisez pour vous connecter à Workday. Exemple : dans l’adresse <code>https://www.myworkday.com/mycompany</code>, le client est <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL ID client]</td>
                <td>Saisissez l’identifiant du client pour la variable [!DNL Workday] application utilisée par cette connexion. Vous obtenez ce résultat lorsque vous créez l’application dans [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Client Secret]</td>
                <td>Saisissez le secret client pour le [!DNL Workday] application utilisée par cette connexion. Vous obtenez ce résultat lorsque vous créez l’application dans [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Délai d’expiration de la session (min)]</td>
                <td >Saisissez le nombre de minutes après lesquelles votre jeton d’autorisation expire.</td>
            </tr>
        </tbody>
    </table>


3. Cliquez sur [!UICONTROL Continuer] pour enregistrer la connexion et revenir au module

## [!DNL Workday] modules et leurs champs

Lorsque vous configurez [!DNL Workday] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Workday] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Action](#action)

* [Recherche](#search)


### Action

* [[!UICONTROL Création d’un enregistrement]](#create-a-record)

* [[!UICONTROL Suppression d’un enregistrement]](#delete-a-record)

* [[!UICONTROL Effectuer un appel API personnalisé]](#make-a-custom-api-call)

* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)


#### [!UICONTROL Création d’un enregistrement]

Ce module d’action crée un enregistrement unique dans [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Pour obtenir des instructions sur la connexion à [!DNL Workday] compte Workfront Fusion, voir <a href="#Connect" class="MCXref xre[!DNL ]f" >Connexion [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record Type]</td>
            <td>Sélectionnez le type d’enregistrement que vous souhaitez créer.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez créer.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID de sous-ressource]</td>
            <td >Saisissez ou mappez l’identifiant de la sous-ressource que vous souhaitez créer.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Suppression d’un enregistrement]

Ce module d’action supprime un seul enregistrement dans [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Pour obtenir des instructions sur la connexion à [!DNL Workday] compte à [!DNL Workfront Fusion], voir <a href="#Connect" class="MCXref xre[!DNL ]f" >Connexion [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Type d’enregistrement]</td>
            <td>Sélectionnez le type d’enregistrement que vous souhaitez supprimer.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Type d’enregistrement spécifique]</td>
            <td>Sélectionnez le type d’enregistrement spécifique que vous souhaitez supprimer. Ils sont basés sur le type d’enregistrement que vous avez choisi.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL ID de sous-ressource]</td>
            <td>Saisissez ou mappez l’identifiant de la sous-ressource que vous souhaitez supprimer.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez supprimer.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL Effectuer un appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL Workday] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL Workday] modules.

Lors de la configuration de ce module, les champs suivants s’affichent.

Le module renvoie un code d’état, ainsi que les en-têtes et le corps de l’appel API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Pour obtenir des instructions sur la connexion à [!DNL Workday] compte à [!DNL Workfront Fusion], voir <a href="#Connect" class="MCXref xre[!DNL ]f" >Connexion [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] ajoute les en-têtes d’autorisation à votre place.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour un seul enregistrement dans [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Pour obtenir des instructions sur la connexion à [!DNL Workday] compte Workfront Fusion, voir <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] à Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">Type d’enregistrement</td>
            <td>Sélectionnez le type d’enregistrement à mettre à jour.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez mettre à jour.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID de sous-ressource]</td>
            <td >Saisissez ou mappez l'identifiant de la sous-ressource que vous souhaitez mettre à jour.</td>
        </tr>
    </tbody>
</table>

### Recherche

* [[!UICONTROL Lire un enregistrement]](#read-a-record)

* [[!UICONTROL Lister des enregistrements]](#list-records)


#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit un seul enregistrement.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Pour obtenir des instructions sur la connexion à [!DNL Workday] compte Workfront Fusion, voir <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] à Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Type d’enregistrement]</td>
            <td>Sélectionnez le type d’enregistrement que vous souhaitez supprimer.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Type d’enregistrement spécifique]</td>
            <td>Sélectionnez le type d’enregistrement spécifique que vous souhaitez lire. Ils sont basés sur le type d’enregistrement que vous avez choisi.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez supprimer.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Lister des enregistrements]

Ce module de recherche récupère une liste d’enregistrements du type spécifié.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Connection]</td>
              <td>Pour obtenir des instructions sur la connexion à [!DNL Workday] compte à [!DNL Workfront Fusion], voir <a href="#Connect" class="MCXref xref" >Connexion [!DNL Workday] to [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Record Type]</td>
              <td>Sélectionnez le type d’enregistrement que vous souhaitez récupérer.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limite]</td>
              <td >
                  <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit récupérer au cours de chaque cycle d'exécution de scénario.</p>
              </td>
          </tr>
      </tbody>
  </table>
