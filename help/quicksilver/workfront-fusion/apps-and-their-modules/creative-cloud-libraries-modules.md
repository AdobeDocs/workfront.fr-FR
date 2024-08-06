---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules des bibliothèques d’Adobe Creative Cloud
description: Avec les modules  [!DNL Adobe Workfront Fusion Adobe Creative Cloud] Libraries , vous pouvez lancer un scénario lorsqu’un élément ou une bibliothèque est créé ou mis à jour. Vous pouvez également charger, récupérer, archiver ou répertorier des éléments, ou effectuer un appel vers l’API  [!DNL Adobe Creative Cloud Libraries] .
author: Becky
feature: Workfront Fusion
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 103a4a7b58048678739d6125c042503458ae3722
workflow-type: tm+mt
source-wordcount: '1338'
ht-degree: 34%

---

# Modules de bibliothèques Adobe Creative Cloud

Avec les modules [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] , vous pouvez démarrer un scénario lorsqu’un élément ou une bibliothèque est créé ou mis à jour. Vous pouvez également charger, récupérer, archiver ou répertorier des éléments, ou effectuer un appel vers l’API [!DNL Adobe Creative Cloud Libraries].

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Création d’un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!IMPORTANT]
>
>La création de la connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.

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

Pour utiliser les modules [!DNL Adobe Creative Cloud Libraries], vous devez disposer d&#39;un compte [!UICONTROL Adobe Creative Cloud].

## Modules [!UICONTROL Bibliothèques Adobe Creative Cloud] et leurs champs

Lorsque vous configurez les modules [!UICONTROL Bibliothèques Adobe Creative Cloud], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Adobe Creative Cloud Libraries] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Éléments](#elements)

* [Bibliothèques](#libraries)

* [Autre](#other)


### Éléments

* [[!UICONTROL Archiver un élément]](#archive-an-element)

* [[!UICONTROL Obtenir un élément]](#get-an-element)

* [[!UICONTROL Eléments de liste]](#list-elements)

* [[!UICONTROL Télécharger un élément]](#upload-an-element)

* [!UICONTROL [Regarder un nouvel élément dans la bibliothèque]](#watch-new-element-in-library)

* [[!UICONTROL Regarder les éléments mis à jour]](#watch-updated-elements)


#### [!UICONTROL Archiver un élément]

Ce module d’action archive un élément d’une bibliothèque.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de la connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de bibliothèque]</td>
      <td >Sélectionnez la bibliothèque contenant l’élément que vous souhaitez archiver.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL ID d’élément]</td>
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
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de la connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de bibliothèque]</td>
      <td >Sélectionnez la bibliothèque contenant l’élément que vous souhaitez récupérer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’élément]</td>
      <td>Saisissez ou mappez l’identifiant de l’élément que vous souhaitez récupérer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sélecteur]</td>
      <td>
        <p>Sélectionnez le type d’informations que le module renvoie. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Par Défaut]</b>
            </p>
            <p>Données de base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Toutes les données disponibles</p>
          </li>
          <li>
            <p><b>[!UICONTROL Représentations]</b>
            </p>
            <p>Liste aplatie des ressources associées à l’élément de bibliothèque</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Eléments de liste]

Ce module d’action récupère une liste d’éléments dans une bibliothèque.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de la connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de bibliothèque]</td>
      <td >Sélectionnez la bibliothèque à partir de laquelle vous souhaitez répertorier les éléments.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordre par]</td>
      <td>Indiquez si vous souhaitez classer les résultats par nom ou par date de dernière modification de l’élément.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type]</td>
      <td >Entrez un type MIME pour limiter les résultats aux éléments identifiés avec le type MIME spécifié. Exemple : <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sélecteur]</td>
      <td>
        <p>Sélectionnez le type d’informations que le module renvoie. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Par Défaut]</b>
            </p>
            <p>Données de base</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Toutes les données disponibles</p>
          </li>
          <li>
            <p><b>[!UICONTROL Représentations]</b>
            </p>
            <p>Liste aplatie des ressources associées à l’élément de bibliothèque</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Télécharger un élément]

Ce module d’action charge une petite ressource de fichier dans une bibliothèque existante. La taille de fichier maximale est de 1 Go.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de la connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de bibliothèque]</td>
      <td >Sélectionnez la bibliothèque à partir de laquelle vous souhaitez répertorier les éléments.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Mode d’appel]</td>
      <td>
        <p>Sélectionnez le mode de traitement avec lequel appeler ce processus de requête.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sync]</b>
            </p>
            <p>L’appel API est traité de manière synchrone. La réponse est diffusée lorsque le traitement est terminé (sauf si l’appel expire).</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>La réponse du moniteur asynchrone est immédiatement renvoyée et le traitement des requêtes se produit de manière asynchrone. L’appel est chargé d’interroger le point de terminaison jusqu’à la fin.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (par défaut)</p>
            <p>Le traitement synchrone de la requête est tenté. Lorsque le traitement s’étend au-delà de 5 000 ms, la réponse du moniteur asynchrone est renvoyée. L’URL du moniteur doit être interrogée jusqu’à ce que la requête soit terminée.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type File]</td>
      <td >Saisissez ou mappez le type MIME du fichier téléchargé.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Source File]</td>
      <td>
        <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Regarder le nouvel élément dans la bibliothèque]

Ce module de déclenchement lance un scénario lorsqu’un élément est ajouté à une bibliothèque.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de la connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de bibliothèque]</td>
      <td >Sélectionnez la bibliothèque à surveiller pour les éléments mis à jour.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Regarder les éléments mis à jour]

Ce module de déclenchement lance un scénario lorsqu’un élément d’une bibliothèque est mis à jour.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de la connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de bibliothèque]</td>
      <td >Sélectionnez la bibliothèque à surveiller pour les nouveaux éléments.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

### Bibliothèques

* [[!UICONTROL Regarder les nouvelles bibliothèques]](#watch-new-libraries)

* [[!UICONTROL Regarder les bibliothèques mises à jour]](#watch-updated-libraries)


#### [!UICONTROL Regarder les nouvelles bibliothèques]

Ce module de déclenchement lance un scénario lorsqu’une nouvelle bibliothèque est créée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de la connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Regarder les bibliothèques mises à jour]

Ce module de déclenchement lance un scénario lorsqu’une bibliothèque existante est mise à jour.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Sélectionnez une connexion Creative Cloud Libraries existante. La création de la connexion n’est actuellement pas disponible dans le connecteur Creative Cloud Libraries. Les connexions existantes fonctionnent comme prévu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
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
      <td> <p>Pour plus d’informations sur la connexion de votre compte Adobe Creative Cloud à Workfront Fusion, voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à Adobe Workfront Fusion - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Saisissez un chemin relatif à <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>Par exemple, <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version de l’API]</td>
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
        <p>Workfront Fusion ajoute les en-têtes d’autorisation à votre place.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p>
        <p>Par exemple : <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Télécharger un document transitoire]</td>
      <td>
      <p>Si vous souhaitez télécharger un document transitoire, saisissez le fichier source du document à télécharger.</p>
      <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p>
    </td>
    </tr>

</tbody>
</table>
