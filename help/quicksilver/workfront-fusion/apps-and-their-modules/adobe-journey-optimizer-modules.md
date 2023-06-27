---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules Adobe Journey Optimizer
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Journey Optimizer], ainsi que de la connecter à plusieurs applications et services tiers.
author: Becky
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] Modules

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Journey Optimizer], ainsi que de la connecter à plusieurs applications et services tiers. [!DNL Adobe Journey Optimizer] Les modules vous permettent de créer, lire, mettre à jour ou supprimer des enregistrements, ou d’effectuer un appel API personnalisé à la fonction [!DNL Adobe Journey Optimizer] API.


Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] ou version ultérieure</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
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

Avant d’utiliser la variable [!DNL Adobe Journey Optimizer] , vous devez vous assurer que les conditions préalables suivantes sont remplies :

* Vous devez avoir une principale [!DNL Adobe Journey Optimizer] compte .

## Créer une connexion à [!DNL Adobe Journey Optimizer]

Pour créer une connexion pour votre [!DNL Adobe Journey Optimizer] modules :

1. Dans n’importe quel [!DNL Adobe Journey Optimizer] module, cliquez sur **[!UICONTROL Ajouter]** en regard de la zone Connexion .

1. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Nom de la connexion]</td>
          <td>
            <p>Saisissez un nom pour cette connexion.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID client]</td>
          <td>Saisissez votre [!DNL Adobe] [!UICONTROL ID client]. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Saisissez votre [!DNL Adobe] [!UICONTROL Client Secret]. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID du compte technique]</td>
          <td>Saisissez votre [!DNL Adobe] [!UICONTROL ID du compte technique]. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID d’organisation]</td>
          <td>Saisissez votre [!DNL Adobe] [!UICONTROL ID d’organisation]. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta-scopes]</td>
          <td>
            Saisissez les portées de métadonnées nécessaires à la connexion.
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Clé privée]</td>
          <td>
            <p>Saisissez la clé privée générée lors de la création de vos informations d’identification dans la variable [!DNL Adobe Developer Console]. </p>
            <p>Pour extraire votre clé privée ou votre certificat :</p>
            <ol>
              <li value="1">
                <p>Cliquez sur <b>[!UICONTROL Extraction]</b>.</p>
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
                <p>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour extraire le fichier et revenir à la configuration de la connexion.</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.

## [!DNL Adobe Journey Optimizer] modules et leurs champs

Lorsque vous configurez [!DNL Adobe Journey Optimizer] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Adobe Journey Optimizer] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Recherches](#searches)

### Actions

* [[!UICONTROL Création d’un enregistrement]](#create-a-record)
* [[!UICONTROL Effectuer un appel API personnalisé]](#make-a-custom-api-call)
* [[!UICONTROL Suppression d’un enregistrement]](#delete-a-record)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)

#### [!UICONTROL Création d’un enregistrement]

Ce module d’action crée un emplacement, une règle de décision, une balise, une offre personnalisée, une collection ou une offre de secours.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Type d’enregistrement]
      </td>
      <td>
        Sélectionnez le type d’enregistrement que vous souhaitez créer.
        <ul>
        <li><b>[!UICONTROL Placement]</b>: Passez à la <a href="#placement-fields" >Champs [!UICONTROL Placement]</a>.</li>
        <li><b>[!UICONTROL Règle de décision]</b>: Passez à la <a href="#decision-rule-fields" >Champs de règle de décision [!UICONTROL]</a>.</li>
        <li><b>[!UICONTROL Decision]</b>: Passez à la <a href="#decision-fields" >Champs [!UICONTROL Decision]</a>.</li>
        <li><b>[!UICONTROL Tag]</b>: Passez à la <a href="#tag-fields" >Champs [!UICONTROL Tag]</a>.</li>
        <li><b>[!UICONTROL Collection]</b>: Passez à la <a href="#collection-fields" >Champs [!UICONTROL Collection]</a>.</li>
        <li><b>[!UICONTROL Offre de secours]</b>: Passez à la <a href="#fallback-offer-fields" >Champs d’[!UICONTROL Offre de secours]</a>.</li>
        <li><b>[!UICONTROL Offre personnalisée]</b>: Passez à la <a href="#personalized-offer-fields" >Champs d’[!UICONTROL Offre personnalisée]</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Emplacement] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Saisissez ou mappez un nom pour l’emplacement.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>Saisissez ou mappez une description de l’emplacement.
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Règle de décision] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Saisissez ou mappez un nom pour la règle de description.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>Saisissez ou mappez une description pour la règle de décision.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Condition]
      </td>
      <td>Saisissez ou mappez la condition dans la règle de décision.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Décision] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Saisissez ou mappez un nom pour la règle de description.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Sélectionnez l’état de la décision.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Date de début]</td>
      <td><p>Saisissez ou mappez la date de début de la décision.</p><p>Pour obtenir la liste des formats de date pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Date de fin]</td>
      <td><p>Saisissez ou mappez la date de fin de la décision.</p><p>Pour obtenir la liste des formats de date pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Emplacements]</td>
      <td>Sélectionner les emplacements à ajouter à cette décision
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Collection]</td>
      <td>Sélectionnez la collection d’offres qui contient les offres que cette décision prendra en compte.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Offre de secours]</td>
      <td>Sélectionnez l’offre de secours qui sera présentée aux clients qui ne correspondent pas aux règles de cette décision.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Balise] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Saisissez ou mappez un nom pour la balise.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Collection] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Saisissez ou mappez un nom pour la collection.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Type de filtre]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elements]
      </td>
      <td>Sélectionnez les balises à inclure dans la collection.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Offre de secours] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Saisissez ou mappez un nom pour l’offre de secours.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Status]
      </td>
      <td> Sélectionnez l’état de l’offre de secours.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Placement]
      </td>
      <td>Saisissez ou mappez l’emplacement de l’offre de secours.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Offre personnalisée] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Saisissez ou mappez un nom pour la règle de description.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Sélectionnez l’état de la décision.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Emplacement</td>
      <td>Sélectionnez l'emplacement de l'offre personnalisée.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Date de début]</td>
      <td><p>Saisissez ou mappez la date de début de l'offre personnalisée.</p><p>Pour obtenir la liste des formats de date pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Date de fin]</td>
      <td><p>Saisissez ou mappez la date de fin de l'offre personnalisée.</p><p>Pour obtenir la liste des formats de date pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Règles de décision]</td>
      <td>Sélectionnez les règles de décision à ajouter à cette offre personnalisée.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Sélectionnez la priorité de cette offre. La priorité affecte la présentation de cette offre plutôt que d’une autre.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Contrainte de limitation]</td>
      <td>Saisissez ou mappez le nombre de fois où cette offre sera présentée.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Suppression d’un enregistrement]

Ce module d’action supprime un seul enregistrement dans [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Type d’enregistrement]
      </td>
      <td>
        Sélectionnez le type d’enregistrement à supprimer.
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Règle de décision]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Offre de secours]</li>
        <li>[!UICONTROL Offre personnalisée]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Règle de décision]/[!UICONTROL Décision]/[!UICONTROL Balise]/[!UICONTROL Collection]/[!UICONTROL Offre de secours]/[!UICONTROL Offre personnalisée]
      </td>
      <td>
        Sélectionnez l’enregistrement à supprimer.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Effectuer un appel API personnalisé]

Ce module effectue un appel API personnalisé à la fonction [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Saisissez un chemin relatif à {baseURL} en commençant par<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Méthode [!UICONTROL]</p>
      </td>
      <td>
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p>
        <p>Par exemple, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion ajoute automatiquement des en-têtes d’autorisation et des en-têtes x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Saisissez la chaîne de requête de requête de requête.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Saisissez le nombre maximal de résultats que le module doit renvoyer dans un cycle d’exécution.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Suppression d’un enregistrement]

Ce module d’action supprime un seul enregistrement dans [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record Type]
      </td>
      <td>
        Sélectionnez le type d’enregistrement à supprimer.
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Règle de décision]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Offre de secours]</li>
        <li>[!UICONTROL Offre personnalisée]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Règle de décision]/[!UICONTROL Décision]/[!UICONTROL Balise]/[!UICONTROL Collection]/[!UICONTROL Offre de secours]/[!UICONTROL Offre personnalisée]
      </td>
      <td>
        Sélectionnez l’enregistrement à supprimer.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action crée un emplacement, une décision, une règle de décision, une balise, une offre personnalisée, une collection ou une offre de secours.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Type d’enregistrement]
      </td>
      <td>
        Sélectionnez le type d'enregistrement que vous souhaitez mettre à jour.
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Règle de décision]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Offre de secours]</li>
        <li>[!UICONTROL Offre personnalisée]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Règle de décision]/[!UICONTROL Décision]/[!UICONTROL Balise]/[!UICONTROL Collection]/[!UICONTROL Offre de secours]/[!UICONTROL Offre personnalisée]
      </td>
      <td>
        Sélectionnez l'enregistrement que vous souhaitez mettre à jour.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Fields]
      </td>
      <td>Pour chaque champ à mettre à jour :
      <ol>
      <li>Cliquez sur <b>[!UICONTROL Ajouter]</b>.</li>
      <li>Indiquez si vous souhaitez ajouter, remplacer ou supprimer des valeurs.</li>
      <li>Saisissez le champ que vous souhaitez mettre à jour.</li>
      <li>Saisissez la nouvelle valeur pour le champ.</li>
      </td>
    </tr>

</tbody>
</table>


### Recherches

#### [!UICONTROL Lister des enregistrements]

Ce module de recherche répertorie les enregistrements du type sélectionné, renvoyant des résultats selon les critères que vous avez spécifiés.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Type d’enregistrement]</p>
      </td>
      <td>
        <p>Sélectionnez le type d’enregistrement que vous souhaitez répertorier.</p>
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Règle de décision]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Offre de secours]</li>
        <li>[!UICONTROL Offre personnalisée]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Opérateur de requête]</p>
      </td>
      <td>
        <p>Sélectionner un opérateur à appliquer aux paramètres de la requête</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fields]</td>
      <td><p>Si vous souhaitez limiter la recherche à des champs spécifiques, renseignez les champs. Pour chaque champ auquel vous souhaitez limiter la recherche, cliquez sur [!UICONTROL Ajouter un élément] et saisissez le nom du champ.</p><p>Les expressions de chemin se présentent sous la forme de chemins séparés par des points, tels que <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ordre par] </td>
      <td>Saisissez ou mappez la propriété par laquelle vous souhaitez classer les résultats.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Direction de la commande]</td>
   <td>Indiquez si vous souhaitez classer les résultats par ordre croissant ou décroissant.
    </td>
     </tr>
  </tbody>
</table>
