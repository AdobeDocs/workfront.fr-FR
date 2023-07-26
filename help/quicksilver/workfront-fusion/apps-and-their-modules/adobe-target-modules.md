---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules Adobe Target
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] Les modules vous permettent de créer, lire, mettre à jour ou supprimer des enregistrements, répertorier tous les enregistrements d’un type donné, rechercher des enregistrements en fonction de critères que vous spécifiez ou effectuer un appel API personnalisé à la fonction [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '2646'
ht-degree: 0%

---

# [!DNL Adobe Target] Modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Target], ainsi que de la connecter à plusieurs applications et services tiers. [!DNL Adobe Target] Les modules vous permettent de créer, lire, mettre à jour ou supprimer des enregistrements, répertorier tous les enregistrements d’un type donné, rechercher des enregistrements en fonction de critères que vous spécifiez ou effectuer un appel API personnalisé à la fonction [!DNL Adobe Target] API.


Si vous avez besoin d’instructions sur la création d’un scénario, voir [Création d’un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
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
   <p>Exigences de licence actuelles : non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Produit</td>
      <td>
   <p>Conditions requises du produit actuel : si vous disposez de l’[!UICONTROL Select] ou de l’[!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td>
    </tr>
    </tr>
  </tbody>
</table>


Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Avant d’utiliser la variable [!DNL Adobe Target] , vous devez vous assurer que les conditions préalables suivantes sont remplies :

* Vous devez avoir une principale [!DNL Adobe Target] compte .

## Créer une connexion à [!DNL Adobe Target]

Pour créer une connexion pour votre [!DNL Adobe Target] modules :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la zone Connexion .

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
        <td>Saisissez votre [!DNL Adobe] ID client. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre [!DNL Adobe] Secret du client. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID d’organisation]</td>
        <td>Saisissez votre [!DNL Adobe] ID d’organisation. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID du compte technique]</td>
        <td>Saisissez votre [!DNL Adobe] Identifiant du compte technique. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
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

## [!DNL Adobe Target] modules et leurs champs

Lorsque vous configurez [!DNL Adobe Target] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Adobe Target] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
    <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#Create" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Type d’enregistrement]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Sélectionnez le type d’enregistrement que vous souhaitez créer.</p>
      <ul>
        <li>
          <p>[!UICONTROL Activité AB]</p>
          <p>Passez à <a href="#AB%C2%A0Activ" class="MCXref xref" >Champs d’activité AB</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Activité XT]</p>
          <p>Passez à <a href="#XT" class="MCXref xref" >Champs d’activité XT</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Offre]</p>
          <p>Passez à <a href="#Offer" class="MCXref xref" >Champs de l'offre</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p>Passez à <a href="#Audience" class="MCXref xref" >Champs d’audience</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### Champs d’activité AB

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
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Audiences avec création de rapports]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
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
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Audiences avec création de rapports]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
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
  </tbody>
</table>

##### Champs d’audience

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Saisissez ou mappez un nom pour cette audience. Le nom ne peut pas dépasser 250 caractères.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Saisissez ou mappez une description de cette audience.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target Rule]</td>
      <td>
        <p>Activez le bouton d’activation/désactivation pour créer des règles ET, en d’autres termes, toutes les règles doivent être appliquées.</p>
        <p>Pour chaque règle à appliquer à l’audience, cliquez sur <b>[!UICONTROL Ajouter un élément]</b> et saisissez le code JSON de la règle à appliquer. </p>
        <div class="example"><span class="autonumber"><span><b>Exemple: </b></span></span>
          <p>Exemples:</p>
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
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Saisissez ou mappez l'identifiant de l'espace de travail associé à l'audience. Si rien n’est indiqué, l’offre est associée à l’espace de travail par défaut du compte. Cette fonctionnalité s’applique uniquement à [!DNL Target Premium] comptes.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Effectuer un appel API personnalisé]

Ce module effectue un appel API personnalisé à la fonction [!DNL Adobe Target] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#Create" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
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
        <p>Méthode [!UICONTROL]</p>
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
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
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
    <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#Create" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
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
    <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#Create" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
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

Ce module d’action met à jour une activité, une offre ou une audience.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#Create" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type d’enregistrement]</td>
      <td>
        <p>Sélectionnez le type d’enregistrement que vous souhaitez mettre à jour.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Activité AB]</b>
            </p>
            <p>Voir la description des champs dans <a href="#AB%C2%A0Activ" class="MCXref xref" >Champs d’activité AB</a> under <a href="#Create2" class="MCXref xref" >Création d’un enregistrement</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Activité XT]</b>
            </p>
            <p>Voir la description des champs dans <a href="#XT" class="MCXref xref" >Champs d’activité XT</a> under <a href="#Create2" class="MCXref xref" >Création d’un enregistrement</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Autre activité]</b>
            </p>
            <p>Sélectionnez le champ pour lequel vous souhaitez mettre à jour une valeur, puis saisissez la nouvelle valeur pour le champ.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offre]</b>
            </p>
            <p>Voir la description des champs dans <a href="#Offer" class="MCXref xref" >Champs de l'offre</a> under <a href="#Create2" class="MCXref xref" >Création d’un enregistrement</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>Voir la description des champs dans <a href="#Audience" class="MCXref xref" >Champs d’audience</a> under <a href="#Create2" class="MCXref xref" >Création d’un enregistrement</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
      <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez mettre à jour.</td>
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
      <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#Create" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
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
    <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Target], voir <a href="#Create" class="MCXref xref" >Créer une connexion à [!DNL Adobe Target]</a> dans cet article.</td>
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
    <td role="rowheader">[!UICONTROL Critères de recherche]</td>
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
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Nombre maximal de résultats renvoyés]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario. Utilisez ce champ conjointement avec le champ [!UICONTROL Décalage] pour paginer les réponses.</p>
      <p>Par exemple, pour voir la troisième page de réponses, lorsque chaque page comporte dix réponses, définissez [!UICONTROL Décalage] sur 20 et [!UICONTROL Nombre maximum de réponses renvoyées] sur 10.</p>
    </td>
  </tr>
</tbody>
</table>
