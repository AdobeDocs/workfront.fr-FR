---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules des bibliothèques d’Adobe Creative Cloud
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 76%

---

# Modules des bibliothèques d’Adobe Creative Cloud


>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules de bibliothèques Adobe Creative Cloud](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/creative-cloud-libraries-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Avec les modules [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries], vous pouvez lancer un scénario lors de la création ou de la mise à jour d’un élément ou d’une bibliothèque. Vous pouvez également charger, récupérer, archiver ou répertorier des éléments, ou faire un appel à l’API [!DNL Adobe Creative Cloud Libraries].

Si vous avez besoin d’instructions sur la création d’un scénario, consultez la section [Créer un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!IMPORTANT]
>
>La création de connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.

## Conditions d’accès

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
      <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Produit</td>
      <td>
   <p>Exigences actuelles du produit : si vous disposez du plan de [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter du [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td>
    </tr>
  </tbody>
</table>


Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL Adobe Creative Cloud Libraries], vous devez disposer d’un compte [!UICONTROL Adobe Creative Cloud].

## Informations sur l’API des bibliothèques Adobe Creative Cloud

Le connecteur Bibliothèques Adobe Creative Cloud utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td>https://cc-libraries.adobe.io/api/v1</td> 
  </tr>
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.1.7</td> 
  </tr>
 </tbody> 
 </table>

## Modules [!UICONTROL Adobe Creative Cloud Libraries] et leurs champs

Lorsque vous configurez les modules [!UICONTROL Adobe Creative Cloud Libraries], [!DNL Workfront Fusion] affiche les champs indiqués ci-dessous. D’autres champs [!DNL Adobe Creative Cloud Libraries] peuvent s’afficher, en fonction de facteurs tels que votre niveau d’accès à l’application ou au service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Éléments](#elements)

* [Bibliothèques](#libraries)

* [Autre](#other)


### Éléments

* [[!UICONTROL Archiver un élément]](#archive-an-element)

* [[!UICONTROL Obtenir un élément]](#get-an-element)

* [[!UICONTROL Répertorier des éléments]](#list-elements)

* [[!UICONTROL Charger un élément]](#upload-an-element)

* [!UICONTROL [Watch New Element in Library]](#watch-new-element-in-library)

* [[!UICONTROL Surveiller les éléments mis à jour]](#watch-updated-elements)


#### [!UICONTROL Archiver un élément]

Ce module d’action archive un élément d’une bibliothèque.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Sélectionnez la bibliothèque qui contient l’élément à archiver.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Element ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Sélectionnez l’élément que vous souhaitez archiver.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtenir un élément]

Ce module d’action renvoie un seul élément d’une bibliothèque.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Sélectionnez la bibliothèque qui contient l’élément à récupérer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Element ID]</td>
      <td>Saisissez ou mappez l’ID de l’élément que vous souhaitez récupérer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Sélectionnez le type d’information que le module renvoie. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Default]</b>
            </p>
            <p>Données de base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Toutes les données disponibles</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representations]</b>
            </p>
            <p>Liste aplatie des ressources associées à l’élément de la bibliothèque</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Répertorier des éléments]

Ce module d’action permet de récupérer une liste d’éléments dans une bibliothèque.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Sélectionnez la bibliothèque dont vous voulez répertorier les éléments.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by]</td>
      <td>Sélectionnez si vous souhaitez classer les résultats par nom ou par date de dernière modification de l’élément.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type]</td>
      <td >Saisissez un type MIME pour limiter les résultats aux éléments identifiés par le type MIME spécifié. Exemple : <code>string</code></td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Sélectionnez le type d’information que le module renvoie. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Default]</b>
            </p>
            <p>Données de base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Toutes les données disponibles</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representations]</b>
            </p>
            <p>Liste aplatie des ressources associées à l’élément de la bibliothèque</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Charger un élément]

Ce module d’action charge un petit fichier de ressources dans une bibliothèque existante. Taille de fichier maximum : 1 Go.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Sélectionnez la bibliothèque dont vous voulez répertorier les éléments.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Invocation Mode]</td>
      <td>
        <p>Sélectionnez le mode de traitement avec lequel ce processus de demande doit être invoqué.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sync]</b>
            </p>
            <p>L’appel API est traité de manière synchrone. La réponse est remise lorsque le traitement est terminé (sauf si l’appel est interrompu).</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>La réponse du moniteur asynchrone est immédiatement renvoyée et le traitement de la demande se fait de manière asynchrone. L’appelant est responsable de l’interrogation du point d’entrée jusqu’à son achèvement.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (par défaut)</p>
            <p>Le traitement synchrone de la demande est tenté. Lorsque le traitement dépasse 5 000 ms, la réponse du moniteur asynchrone est renvoyée. L’URL du moniteur doit être interrogée jusqu’à ce que la demande soit terminée.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type File]</td>
      <td >Saisissez ou mappez le type MIME du fichier chargé.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Source File]</td>
      <td>
        <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Surveiller un nouvel élément dans la bibliothèque]

Ce module de déclenchement lance un scénario lorsqu’un élément est ajouté à une bibliothèque.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Sélectionnez la bibliothèque dont vous souhaitez surveiller les éléments mis à jour.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Surveiller les éléments mis à jour]

Ce module de déclenchement lance un scénario lorsqu’un élément d’une bibliothèque est mis à jour.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >Sélectionnez la bibliothèque dans laquelle vous souhaitez surveiller la présence de nouveaux éléments.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

### Bibliothèques

* [[!UICONTROL Surveiller les nouvelles bibliothèques]](#watch-new-libraries)

* [[!UICONTROL Surveiller les bibliothèques mises à jour]](#watch-updated-libraries)


#### [!UICONTROL Surveiller les nouvelles bibliothèques]

Ce module de déclenchement lance un scénario lorsqu’une nouvelle bibliothèque est créée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Surveiller les bibliothèques mises à jour]

Ce module de déclenchement lance un scénario lorsqu’une bibliothèque existante est mise à jour.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

### Autre

#### [!UICONTROL Effectuer un appel API]

Ce module effectue un appel API personnalisé à l’API [!DNL Adobe Creative Cloud Libraries].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour obtenir des instructions sur la connexion de votre compte Adobe Creative Cloud à Workfront Fusion, voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe Workfront Fusion - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Saisissez un chemin relatif à <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>Par exemple <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API version]</td>
      <td>
        <p>Sélectionnez la version de l’API [!DNL Adobe Analytics] à laquelle vous souhaitez vous connecter.</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL Method]</td>
      <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p>
        <p>Par exemple, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion ajoute les en-têtes d’autorisation pour vous.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p>
        <p>Par exemple : <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lorsque vous utilisez des instructions conditionnelles comme <code>if</code> dans votre JSON, mettez les guillemets à l’extérieur de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Upload a transient document]</td>
      <td>
      <p>Si vous souhaitez charger un document transitoire, saisissez le fichier source du document que vous souhaitez charger.</p>
      <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p>
    </td>
    </tr>

</tbody>
</table>
