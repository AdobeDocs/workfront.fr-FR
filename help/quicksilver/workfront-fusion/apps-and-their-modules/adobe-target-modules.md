---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules Adobe Target
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] Les modules vous permettent de créer, lire, mettre à jour ou supprimer des enregistrements, répertorier tous les enregistrements d’un type donné, rechercher des enregistrements en fonction de critères que vous spécifiez ou effectuer un appel API personnalisé à la fonction [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: b20f08a3c039ac2f1ece9fc4cef7ad5f58421482
workflow-type: tm+mt
source-wordcount: '2119'
ht-degree: 16%

---

# [!DNL Adobe Target] Modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Target], ainsi que de la connecter à plusieurs applications et services tiers. [!DNL Adobe Target] Les modules vous permettent de créer, lire, mettre à jour ou supprimer des enregistrements, répertorier tous les enregistrements d’un type donné, rechercher des enregistrements en fonction de critères que vous spécifiez ou effectuer un appel API personnalisé à la fonction [!DNL Adobe Target] API.


Si vous avez besoin d’instructions sur la création d’un scénario, voir [Création d’un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
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
    </tr>
  </tbody>
</table>


Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Avant d’utiliser la variable [!DNL Adobe Target] , vous devez vous assurer que les conditions préalables suivantes sont remplies :

* Vous devez disposer d’un [!DNL Adobe Target] compte .

## Créer une connexion à [!DNL Adobe Target]

Pour créer une connexion pour votre [!DNL Adobe Target] modules :

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
        <td>Indiquez si vous vous connectez à un environnement de production ou hors production.
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Choisissez si vous vous connectez à un compte de service ou à un compte personnel.
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Saisissez votre ID client [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre [!DNL Adobe] Secret du client. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID du compte technique]</td>
        <td>Saisissez votre [!DNL Adobe] Identifiant du compte technique. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID d’organisation]</td>
        <td>Saisissez votre [!DNL Adobe] ID d’organisation. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tenant]</td>
        <td>
          <p> Pour localiser votre tenant, connectez-vous au [!DNL Adobe Experience Cloud], ouvrez [!DNL Target], puis cliquez sur le bouton [!DNL Target] carte. Utilisez la valeur de l’identifiant du client comme indiqué dans le sous-domaine de l’URL.</p>
          <p>Par exemple, si votre URL lors de la connexion à [!DNL Adobe Target] is <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> alors votre identifiant de tenant est "mycompany".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Portées des métadonnées]</td>
        <td>Entrée <code>ent_marketing_sdk</code>       </td>
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

## Modules [!DNL Adobe Target] et leurs champs

Lorsque vous configurez des modules [!DNL Adobe Target], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Adobe Target] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)

* [Recherches](#searches)


### Actions

* [[!UICONTROL Création d’un enregistrement]](#create-a-record)

* [[!UICONTROL Effectuer un appel API personnalisé]](#make-a-custom-api-call)

* [[!UICONTROL Suppression d’un enregistrement]](#delete-a-record)

* [[!UICONTROL Lire un enregistrement]](#read-a-record)

* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)


#### [!UICONTROL Création d’un enregistrement]

Ce module d’action crée une activité AB ou XT, une offre ou une audience.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Type d’enregistrement]</td>
    <td>
      <p>Sélectionnez le type d’enregistrement que vous souhaitez créer.</p>
      <ul>
        <li>
        <b>Propriété</b><p>Pour plus d’informations sur les champs, voir <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Properties/operation/createProperty">Création d’une propriété</a> dans la documentation de l’API Adobe Target.</p>
        </li>
        <li>
        <b>Recommandation d’offre</b><p>Pour plus d’informations sur les champs, voir <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Offers/operation/createOffer">Créer une offre de recette</a> dans la documentation de l’API Adobe Target.</p>
        </li>
        <li>
          <b>[!UICONTROL Offre JSON]</b>
          <p>Passez à <a href="#offer-fields" class="MCXref xref" >Champs de l'offre</a>.</p>
        </li>
        <li>
          <b>[!UICONTROL Contenu de l’offre]</b>
          <p>Passez à <a href="#offer-fields" class="MCXref xref" >Champs de l'offre</a>.</p>
        </li>
        <li>
        <b>Environnement</b><p>Pour plus d’informations sur les champs, voir <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Environments/operation/createEnvironment">Créer un environnement</a> dans la documentation de l’API Adobe Target.</p>
        </li>
        <li>
          <b>[!UICONTROL Audience]</b>
          <p>Pour plus d’informations sur les champs, voir <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Audiences/operation/createAudience_1_1">Créer une audience</a> dans la documentation de l’API Adobe Target.</p>
        </li>
        <li>
          <b>[!UICONTROL Activité AB]</b>
          <p>Pour plus d’informations sur les champs, voir <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_4_1">Créer une activité AB</a> dans la documentation de l’API Adobe Target.</p>
        </li>
        <li>
          <b>[!UICONTROL Activité XT]</b>
          <p>Passez à <a href="#xt-activity-fields" class="MCXref xref" >Champs d’activité XT</a>.</p>
        </li>
        <li>
          <b>[!UICONTROL Activité AP]</b>
          <p>Pour plus d’informations sur les champs, voir <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_2">Créer une activité AP</a> dans la documentation de l’API Adobe Target.</p>
        </li>
        <li>
          <b>[!UICONTROL Jeton de réponse]</b>
          <p>Pour plus d’informations sur les champs, voir <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Response-tokens/operation/createResponseToken">Création d’un jeton de réponse</a> dans la documentation de l’API Adobe Target.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

<!--

##### AB Activity fields

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this activity. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>For each option that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the option across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the option. The name must be no more than 250 characters.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Select or map the Offer associated with the option.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Mboxes]</td>
      <td>
        <p>For each Mbox that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>For each audience that you want to add to the Mbox, click <b>[!UICONTROL Add item]</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selectors]</td>
      <td>
        <p>For each selector that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>For each audience that you want to add to the Mbox, click <b>[!UICONTROL Add item]</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Selector]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiences]</td>
      <td>
        <p>A list of locations on the page where the content offer is served. A location contains the following:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Enter or map the ID of the experience</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map the name of the experience
</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>For each audience that you want to see the experience, click <b>[!UICONTROL Add item]</b> and enter the Audience ID.
</p>
          </li>
          <li>
            <p><b>[!UICONTROL Visitor Percentage]</b>
            </p>
            <p>Enter or map the percentage of visitors that is allocated to the experience</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td><p>For details on metrics, see <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_4_1">Create AB activity</a> in the Adobe Target API documentation.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>Enter or map an ID to identify this activity. You can choose this ID. This ID must not be the same as another activity, and can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts at]</td>
      <td>Enter or map the date and time to start the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends at]</td>
      <td>Enter or map the date and time to end the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Enter or map the state of the activity.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL Deactivated]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL Saved] </p>
          </li>
          <li>
            <p>[!UICONTROL Deleted]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Enter a number that defines the priority of the activity. Higher numbers have higher priority. This value must be between 0 and 999. The default value is 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auto-allocate traffic]</td>
      <td>
        <p>Enable this option to auto-allocate traffic. Auto-allocating sends more traffic to the more successful experience.</p>
        <p>Select or map the evaluation criteria by which to judge which experience is more successful.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Enter or map the workspace that the activity is associated with</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>For each property that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and select or map the property's ID.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td>
        <p>For each reporting audience that you want to add to the activity, click [!UICONTROL Add item] and enter the following information:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the Reporting Audience across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Enter or map the Segment to be used in reporting</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the metric across API requests.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

##### Champs d’activité XT

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Saisissez ou mappez un nom pour cette activité. Le nom ne peut pas dépasser 250 caractères.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>Pour chaque option à ajouter à l’activité, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et renseignez les champs suivants :</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Identifiant local de l’option]</b>
            </p>
            <p>Saisissez ou mappez une chaîne à utiliser pour effectuer le suivi de l’option dans les demandes d’API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Saisissez ou mappez un nom pour l’option. Le nom ne doit pas dépasser 250 caractères.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID d’offre]</b>
            </p>
          </li>
          <li>
            <p>Sélectionnez ou mappez l'offre associée à l'option.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Emplacements]</td>
      <td>
        <p>Pour chaque mbox à ajouter à l’activité, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et renseignez les champs suivants :</p>
        <ul>
          <li>
            <p>[!UICONTROL ID d’audience]</p>
            <p>Pour chaque audience à ajouter à la mbox, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et sélectionnez l’ID d’audience.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID local de l’emplacement]</b>
            </p>
            <p>Saisissez ou mappez une chaîne à utiliser pour effectuer le suivi de l’emplacement entre les demandes d’API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Saisissez ou mappez un nom pour l’emplacement. Le nom ne doit pas dépasser 250 caractères.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Expériences]</td>
      <td>
        <p>Liste des emplacements sur la page où l’offre de contenu est diffusée. Un emplacement contient les éléments suivants :
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience ID local]</b>
            </p>
            <p>Entrer ou mapper l’identifiant de l’expérience</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Saisissez ou mappez le nom de l’expérience.

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Pour chaque audience que vous souhaitez voir l’expérience, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et saisissez l’ID d’audience.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Pourcentage de visiteurs]</b>
            </p>
            <p>Entrer ou mapper le pourcentage de visiteurs qui est affecté à l’expérience</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Mesures]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID tiers]</td>
      <td>Saisissez ou mappez un identifiant pour identifier cette activité. Vous pouvez choisir cet identifiant. Cet identifiant ne doit pas être identique à une autre activité et ne peut pas dépasser 250 caractères.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Commence à]</td>
      <td>Saisissez ou mappez la date et l’heure de début de l’activité au format . <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Se termine à]</td>
      <td>Saisissez ou mappez la date et l’heure de fin de l’activité au format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Saisissez ou mappez l’état de l’activité.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approuvé]</p>
          </li>
          <li>
            <p>[!UICONTROL Désactivé]</p>
          </li>
          <li>
            <p>[!UICONTROL En pause]</p>
          </li>
          <li>
            <p>[!UICONTROL Enregistré] </p>
          </li>
          <li>
            <p>[!UICONTROL supprimé]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Saisissez un nombre qui définit la priorité de l’activité. Les nombres plus élevés ont une priorité plus élevée. Cette valeur doit être comprise entre 0 et 999. La valeur par défaut est 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Affectation automatique du trafic]</td>
      <td>
        <p>Activez cette option pour affecter automatiquement le trafic. L’affectation automatique envoie plus de trafic vers l’expérience la plus performante.</p>
        <p>Sélectionnez ou mappez les critères d’évaluation selon lesquels vous souhaitez juger quelle expérience est la plus réussie.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Entrer ou mapper l’espace de travail auquel l’activité est associée</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de propriété] </td>
      <td>Pour chaque propriété à ajouter à l’activité, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et sélectionnez ou mappez l’identifiant de la propriété.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Audiences avec création de rapports]</td>
      <td>
        <p>Pour chaque audience de rapport à ajouter à l’activité, cliquez sur [!UICONTROL Ajouter un élément] et saisissez les informations suivantes :</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience ID local]</b>
            </p>
            <p>Saisissez ou mappez une chaîne à utiliser pour effectuer le suivi de l’audience de création de rapports dans les demandes d’API.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID d’audience]</b>
            </p>
            <p>Entrer ou mapper le segment à utiliser dans les rapports</p>
          </li>
          <li>
            <p><b>[!UICONTROL ID local de la mesure]</b>
            </p>
            <p>Saisissez ou mappez une chaîne à utiliser pour effectuer le suivi de la mesure dans les demandes d’API.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Champs de l&#39;offre

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Saisissez ou mappez un nom pour cette activité. Le nom ne peut pas dépasser 250 caractères.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Saisissez ou mappez le contenu de l’offre qui sera présentée à l’utilisateur.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Saisissez ou mappez l'identifiant de l'espace de travail associé à l'offre. Si rien n’est indiqué, l’offre est associée à l’espace de travail par défaut du compte. Cette fonctionnalité s’applique uniquement à [!DNL Target] Comptes Premium.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Saisissez ou mappez la date et l’heure de modification de cette offre.</p>
      </td>
    </tr>
  </tbody>
</table>

<!--

##### Audience fields

>[!NOTE]
>
>Audiences created through Workfront Fusion can only be edit in Fusion or through the API. They cannot be edited from within Target.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this audience. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Description]</td>
      <td>
        <p>Enter or map a description of this audience.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Origin]</td>
      <td>
        <p>Select whether this audience's origin is from Target or from the cloud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target Rule]</td>
      <td>
        <p>Enable the toggle to make rules AND, that is, all rules must be applied.</p>
        <p>For each rule that you want to apply to the audience, click <b>[!UICONTROL Add item]</b> and enter the JSON of the rule you want to apply. </p>
        <div class="example"><span class="autonumber"><span><b>Example: </b></span></span>
          <p>Example 1:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p>Example 2</p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Enter or map the ID of the workspace associated with the audience. If left blank, the offer is associated with the default workspace of the account. This functionality applies only to [!DNL Target Premium] accounts.</p>
      </td>
    </tr>
  </tbody>
</table>

-->

#### [!UICONTROL Effectuer un appel API personnalisé]

Ce module effectue un appel API personnalisé à la fonction [!DNL Adobe Target] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] URL de base]</td>
      <td>Saisissez ou mappez vos [!DNL Target] URL de base.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Saisissez un chemin relatif à {baseURL}/</p>
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
        <p>[!DNL Workfront Fusion] ajoute automatiquement des en-têtes d’autorisation et des en-têtes x-api-key.</p>
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
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Suppression d’un enregistrement]

Ce module d’action supprime une seule activité AB, une seule activité XT, une seule offre ou une seule audience.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Type d’enregistrement]</td>
    <td>Sélectionnez le type d’enregistrement que vous souhaitez supprimer.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez supprimer.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action récupère les données d’une seule activité, offre, audience, propriété ou rapport.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Type d’enregistrement]</td>
    <td>Sélectionnez le type d’enregistrement à lire.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez lire.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour un enregistrement dans Target.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type d’enregistrement]</td>
      <td>
        <p>Sélectionnez le type d’enregistrement que vous souhaitez mettre à jour.</p>
       </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Noms des champs]</td>
      <td>Sélectionnez les champs que vous souhaitez mettre à jour. Les champs apparaissent ci-dessous.
          <p>Pour plus d’informations sur les champs, voir <a href="https://developer.adobe.com/target/administer/admin-api/">la documentation de l’API Adobe Target ;</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

### Recherches

* [[!UICONTROL Obtenir des enregistrements]](#get-records)

* [[!UICONTROL Rechercher]](#search)


#### [!UICONTROL Obtenir des enregistrements]

Ce module de recherche récupère une liste d&#39;enregistrements du type sélectionné.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type d’enregistrement]</td>
      <td>Sélectionnez le type d’enregistrement que vous souhaitez mettre à jour.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Trier par]</td>
      <td>Pour chaque champ de tri, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et sélectionnez le champ et indiquez si les résultats renvoyés doivent être ascendant ou descendant.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Commence À]</td>
      <td>
        <p>Saisissez la date la plus ancienne à laquelle vous souhaitez récupérer les enregistrements. </p>
        <p>Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Se Termine À]</td>
      <td>
        <p>Saisissez la date la plus récente pour laquelle vous souhaitez récupérer les enregistrements. </p>
        <p>Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Rechercher]

Ce module de recherche recherche recherche des activités, des offres ou des audiences en fonction des critères que vous avez spécifiés.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Type d’enregistrement]</td>
    <td>Sélectionnez le type d’enregistrement que vous souhaitez mettre à jour.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Trier par]</td>
    <td>Pour chaque champ de tri, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et sélectionnez le champ et indiquez si les résultats renvoyés doivent être ascendant ou descendant.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Search criteria]</td>
    <td>Pour chaque règle à configurer, sélectionnez le champ, l’opérateur et la valeur. Cliquez sur <b>[!UICONTROL Ajouter une règle AND]</b> pour créer des règles supplémentaires.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>Saisissez le numéro de la première réponse que le module doit renvoyer. La première réponse renvoyée comporte un décalage de <code>0</code>. Utilisez ce champ en combinaison avec le champ [!UICONTROL Nombre maximal de résultats renvoyés] pour paginer les réponses.</p>
      <p>Par exemple, pour voir la troisième page de réponses, lorsque chaque page comporte dix réponses, définissez [!UICONTROL Décalage] sur 20 et [!UICONTROL Nombre maximum de réponses renvoyées] sur 10.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]</td>
    <td>
      <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario. Utilisez ce champ conjointement avec le champ [!UICONTROL Décalage] pour paginer les réponses.</p>
      <p>Par exemple, pour voir la troisième page de réponses, lorsque chaque page comporte dix réponses, définissez [!UICONTROL Décalage] sur 20 et [!UICONTROL Nombre maximum de réponses renvoyées] sur 10.</p>
    </td>
  </tr>
</tbody>
</table>
