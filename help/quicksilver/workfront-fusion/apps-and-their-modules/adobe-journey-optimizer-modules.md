---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules Adobe Journey Optimizer
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL Adobe Journey Optimizer] et le connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3692'
ht-degree: 30%

---

# Modules [!DNL Adobe Journey Optimizer]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Adobe Journey Optimizer] et le connecter à plusieurs applications et services tiers. Les modules [!DNL Adobe Journey Optimizer] vous permettent de créer, lire, mettre à jour ou supprimer des enregistrements, ou d’effectuer un appel API personnalisé à l’API [!DNL Adobe Journey Optimizer].


Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table>
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
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td>
    </tr>
  </tbody>
</table>


Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Conditions préalables

Avant d’utiliser le connecteur [!DNL Adobe Journey Optimizer], vous devez vous assurer que les conditions préalables suivantes sont remplies :

* Vous devez disposer d’un compte [!DNL Adobe Journey Optimizer].

## Informations sur l’API Adobe Journey Optimizer

Le connecteur Adobe Journey Optimizer utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td>{{connection.url}</td> 
  </tr>
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.7.11</td> 
  </tr>
 </tbody> 
 </table>

## Création d’une connexion à Adobe Journey Optimizer

Vous pouvez créer une connexion dans n’importe quel module Adobe Journey Optimizer.

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la case Connexion.

1. Remplissez les champs suivants :

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
        <td>Indiquez si vous vous connectez à un environnement de production ou hors production.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Indiquez si vous vous connectez à un compte de service ou à un compte personnel.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Saisissez votre [!UICONTROL Adobe] [!UICONTROL ID client]. Vous pouvez le trouver dans la section de détails [!UICONTROL Credentials] de la variable [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre [!UICONTROL Client Secret] [!DNL Adobe]. Vous pouvez le trouver dans la section de détails [!UICONTROL Credentials] de la variable [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Saisissez votre [!UICONTROL Organization ID] [!DNL Adobe]. Vous pouvez le trouver dans la section de détails [!UICONTROL Credentials] de la variable [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Sandbox Name]</td>
        <td>Saisissez le nom de l’environnement de test que cette connexion utilisera.</td>
        </tr>
      </tbody>
    </table>


## Modules [!DNL Adobe Journey Optimizer] et leurs champs

Lorsque vous configurez les modules [!DNL Adobe Journey Optimizer], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Adobe Journey Optimizer] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Gestion des configurations](#configuration-management)
* [Gestion des packages](#package-management)
* [Gestion des enregistrements](#record-management)
* [Gestion des messages](#message-management)
* [Vérifications d’état](#status-checks)
* [Recherches](#searches)
* [Autre](#other)




### Gestion des configurations

* [Création d’une configuration](#create-a-configuration)
* [Déployer une configuration](#deploy-a-configuration)
* [Mise à jour d’une configuration](#update-a-configuration)
* [Annulation du déploiement d’une configuration](#undeploy-a-configuration)
* [Vérifiez si la configuration peut être déployée.](#check-if-configuration-can-be-deployed)
* [Suppression d’une configuration](#delete-a-configuration)
* [Obtention d’une configuration](#get-a-configuration)

#### Création d’une configuration

Ce module d’action crée une configuration de point de terminaison de limitation ou de ralentissement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de configuration]</td> 
   <td>Indiquez si vous créez une configuration de limitation ou une configuration de limitation.<ul><li><p><b>Limitation</b></p>Passez à <a href="#capping-fields" class="MCXref xref" >Champs de limitation</a>.</li><li><p><b>Ralentissement</b></p>Passez à <a href="#throttling-fields" class="MCXref xref" >Champs de limitation</a>.</li></ul></td> 
  </tr> 
   </tbody> 
</table>

##### Champs de limitation

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez ou mappez l’URL du point de terminaison que vous souhaitez configurer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identifiant de l’organisation IMS]</td> 
   <td>Saisissez ou mappez l’ID Adobe IMS de l’organisation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Méthodes]</td> 
   <td>Sélectionnez les méthodes à utiliser dans cette configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service]</td> 
   <td>Indiquez si vous utilisez une action ou une source de données pour cette configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de connexions HTTP]</td> 
   <td>Saisissez ou mappez le nombre maximal de connexions simultanées à ce point de terminaison.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal d’appels]</td> 
   <td>Saisissez ou mappez le nombre maximum d'appels à effectuer dans la période spécifiée dans le champ Période .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Période (millisecondes)]</td> 
   <td>Saisissez ou mappez le nombre de millisecondes correspondant au champ Nombre maximum d'appels .</td> 
  </tr> 
 </tbody> 
</table>

##### Champs de limitation

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Saisissez ou mappez un nom pour cette configuration.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Saisissez ou mappez une description pour cette configuration.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Modèle d’URL]</td> 
   <td>Saisissez ou mappez l’URL du point de terminaison que vous souhaitez limiter.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Méthodes]</td> 
   <td>Sélectionnez les méthodes à utiliser dans cette configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Débit max.]</td> 
   <td>Indiquez si vous utilisez une action ou une source de données pour cette configuration.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de connexions HTTP]</td> 
   <td>Saisissez ou mappez le nombre maximal de connexions simultanées à ce point de terminaison.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal d’appels]</td> 
   <td>Saisissez ou mappez le débit maximal souhaité pour ce point de terminaison. Cette valeur doit être comprise entre 200 et 5000.</td> 
  </tr> 
 </tbody> 
</table>

#### Déployer une configuration

Ce module d’action déploie la configuration de limitation ou de ralentissement spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de configuration]</td> 
   <td>Choisissez si vous déployez une configuration de limitation ou une configuration de limitation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de configuration]</td> 
   <td>Saisissez ou mappez l’identifiant de la configuration que vous souhaitez déployer.</td> 
  </tr> 
 </tbody> 
</table>

#### Mise à jour d’une configuration

Ce module d’action met à jour la configuration de limitation ou de ralentissement spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de configuration]</td> 
   <td>Indiquez si vous mettez à jour une configuration de limitation ou une configuration de limitation.<ul><li><p><b>Limitation</b></p>Pour les champs, voir <a href="#capping-fields" class="MCXref xref" >Champs de limitation</a> dans la section Créer une configuration de cet article.</li><li><p><b>Ralentissement</b></p>Pour les champs, voir <a href="#throttling-fields" class="MCXref xref" >Champs de limitation</a> dans la section Créer une configuration de cet article.</li></ul></td> 
  </tr> 
  </tbody> 
</table>

#### Annulation du déploiement d’une configuration

Ce module d’action annule le déploiement d’une configuration de limitation ou de ralentissement. L’état de configuration est rétabli sur l’état avant le déploiement (`created` ou `updated`).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de configuration]</td> 
   <td>Indiquez si vous annulez le déploiement d’une configuration de limitation ou d’une configuration de limitation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de configuration]</td> 
   <td>Saisissez ou mappez l’identifiant de la configuration que vous souhaitez annuler le déploiement.</td> 
  </tr> 
 </tbody> 
</table>

#### Vérifiez si la configuration peut être déployée.

Ce module d’action vérifie si une configuration de limitation ou de limitation peut être déployée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de configuration]</td> 
   <td>Indiquez si vous vérifiez une configuration de limitation ou une configuration de limitation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de configuration]</td> 
   <td>Saisissez ou mappez l’identifiant de la configuration à vérifier.</td> 
  </tr> 
 </tbody> 
</table>

#### Suppression d’une configuration

Ce module d’action supprime une configuration de point de terminaison de limitation ou de ralentissement.

Si la configuration a été déployée, elle doit être dédéployée avant de pouvoir être supprimée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de configuration]</td> 
   <td>Choisissez si vous supprimez une configuration de limitation ou une configuration de limitation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de configuration]</td> 
   <td>Saisissez ou mappez l’identifiant de la configuration que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

#### Obtention d’une configuration

Ce module d’action renvoie la configuration de limitation ou de ralentissement identifiée par l’identifiant spécifié. La dernière définition est renvoyée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de configuration]</td> 
   <td>Choisissez si vous récupérez une configuration de limitation ou une configuration de limitation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de configuration]</td> 
   <td>Saisissez ou mappez l’identifiant de la configuration que vous souhaitez récupérer.</td> 
  </tr> 
 </tbody> 
</table>




### Gestion des packages

* [Créer un package](#create-a-package)
* [Mettre à jour un package](#update-a-package)
* [Supprimer un package](#delete-a-package)
* [Recherche d’un module](#look-up-a-package)
* [Importer un package](#import-a-package)
* [Publish d’un package](#publish-a-package)
* [Envoyer un import](#submit-an-import)



#### Créer un package

Ce module d’action crée un module multi-artefact.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Saisissez ou mappez un nom pour le module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Saisissez ou mappez une description du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expiration date]</td> 
   <td>Saisissez ou mappez l’horodatage qui définit la date d’expiration du package. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de module]</td> 
   <td>Sélectionnez le type de package que vous souhaitez créer.<ul><li><p><b>Plein</b></p>Le module comprend tous les artefacts.</p></li><li><p><b>Partiel</b></p><p>Le module comprend uniquement les artefacts que vous ajoutez. </p></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>Si vous créez un module partiel, pour chaque artefact à ajouter, cliquez sur <b>Ajouter un artefact</b> et spécifiez l’identifiant, le type et le titre de l’artefact. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Sandbox]</td> 
   <td>Saisissez ou mappez le nom et l’identifiant de l’organisation IMS de l’environnement de test qui contient les éléments que le module doit contenir.</td> 
  </tr> 
 </tbody> 
</table>

#### Mettre à jour un package

Ce module d’action ajoute ou supprime des artefacts d’un module ou met à jour les métadonnées du module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner une action]</td> 
   <td>Sélectionnez l’action que vous souhaitez effectuer.<ul><li><p><b>Ajouter un artefact</b></p><p>Pour chaque artefact à ajouter, cliquez sur <b>Ajouter un artefact</b> et indiquez l’identifiant, le type et le titre de l’artefact, puis saisissez ou mappez la date d’expiration du module. </p></li><li><p><b>Supprimer l’artefact</b></p><p>Pour chaque artefact que vous souhaitez supprimer, cliquez sur <b>Ajouter un artefact</b> et indiquez l’identifiant, le type et le titre de l’artefact. </p></li><li><p><b>Mise à jour des métadonnées</b></p><p>Saisissez de nouvelles valeurs pour le nom, la description ou le nom de l’environnement de test source ou l’identifiant de l’organisation IMS.</p></li></ul></td> 
  </tr> 
 </tbody> 
</table>

#### Supprimer un package

Ce module d’action supprime un module multi-artefact.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de module]</td> 
   <td>Saisissez ou mappez l’identifiant du module à supprimer.</td> 
  </tr> 
 </tbody> 
</table>

#### Recherche d’un module

Ce module d’action récupère les détails du module spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de module]</td> 
   <td>Saisissez ou mappez l’identifiant du package pour lequel vous souhaitez renvoyer les détails.</td> 
  </tr> 
 </tbody> 
</table>

#### Importer un package

Ce module d’action récupère les objets en conflit dans l’environnement de test cible spécifié. Les objets en conflit représentent des objets similaires déjà présents dans l’environnement de test cible.

Vous devez publier un package avant de pouvoir l’importer.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de module]</td> 
   <td>Saisissez ou mappez l'identifiant du package que vous souhaitez importer.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Environnement de test Target]</td> 
   <td>Saisissez ou mappez le nom de l’environnement de test dans lequel vous souhaitez importer le package.</td> 
  </tr> 
 </tbody> 
</table>

#### Publish d’un package

Vous devez publier un package avant de pouvoir l’importer.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de module]</td> 
   <td>Saisissez ou mappez l’identifiant du module que vous souhaitez publier.</td> 
  </tr> 
 </tbody> 
</table>

#### Envoyer un import

Ce module d’action envoie un import pour un package après avoir passé en revue les conflits et fourni des substitutions. Le résultat est fourni sous la forme d’un payload, qui lance la tâche d’importation pour l’environnement de test de destination, comme indiqué dans le payload.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de module]</td> 
   <td>Saisissez ou mappez l’identifiant du module que vous souhaitez publier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Saisissez ou mappez un nom pour la tâche d’importation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Saisissez ou mappez une description de la tâche d’importation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nom [!UICONTROL (Destination sandbox)]</td> 
   <td>Saisissez ou mappez le nom de l’environnement de test dans lequel vous envoyez l’importation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (ID d’organisation IMS de destination sandbox)]</td> 
   <td>Saisissez ou mappez l’identifiant de l’organisation Adobe IMS pour l’environnement de test dans lequel vous envoyez l’importation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Source sandbox ID)]</td> 
   <td>Saisissez ou mappez l’identifiant de l’environnement de test qui contient le module que vous souhaitez publier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type [!UICONTROL (Source sandbox)]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Lien [!UICONTROL (sandbox Source)]</td> 
   <td>Saisissez ou mappez le lien pour le module que vous souhaitez publier.</td> 
  </tr> 
 </tbody> 
</table>


<!--

### Artifact management

* [Copy artifacts synchronously](#copy-artifacts-synchronously)
* [Export artifacts asynchronously](#export-artifacts-asynchronously)
* [Import artifacts asynchronously](#import-artifacts-asynchronously)

#### Copy artifacts synchronously

This action module copies artifacts from a source sandbox into a destination sandbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the new file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the new file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination sandbox]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>For each artifact you want to copy, click <b>Add artifact</b> and continue to <a href="#artifact-fields" class="MCXref xref" >Artifact fields</a>.</td> 
  </tr> 
 </tbody> 
</table>

##### Artifact fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the artifact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Enter or map the artifact type, such as <code>REGISTRY_SCHEMA<code> or <code>JOURNEY</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version]</td> 
   <td>Enter or map the visibility of the artifact. This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Enter or map the visibility (tenant or global). This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Found]</td> 
   <td>Select <b>Yes</b> if this item was found using a GET operation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tasks]</td> 
   <td>For each task you want to add, click <b>Add task</b> and fill in the following:
   <ul>
   <li><p><b>Method</b></p></li>
   <li><p><b>Action</b></p></li>
   <li><p><b>Using</b></p></li>
   <li><p><b>With</b></p></li>
   </ul>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>For each task you want to add, click <b>Add message</b> and fill in the following:
   <ul>
   <li><p><b>Status</b></p><p>Enter or map the status that this message represents, such as <code>ERROR</code>.</li>
   <li><p><b>Attempt</b></p><p>Enter or map the attempt number related to this message. This may be useful if different attempts produce different messages.</p></li>
   <li><p><b>Message</b></p><p>Enter or map the text of the message.</li>
   <li><p><b>Object</b></p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

#### Export Artifacts asynchronously

This action module exports artifacts from the specified sandbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the export file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the export file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>For each artifact you want to export, click <b>Add artifact</b> and continue to <a href="#artifact-fields" class="MCXref xref" >Artifact fields</a>.</td> 
  </tr> 
 </tbody> 
</table>

##### Artifact fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the artifact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Enter or map the artifact type, such as <code>REGISTRY_SCHEMA<code> or <code>JOURNEY</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version]</td> 
   <td>Enter or map the visibility of the artifact. This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Enter or map the visibility (tenant or global). This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Found]</td> 
   <td>Select <b>Yes</b> if this item was found using a GET operation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tasks]</td> 
   <td>For each task you want to add, click <b>Add task</b> and fill in the following:
   <ul>
   <li><p><b>Method</b></p></li>
   <li><p><b>Action</b></p></li>
   <li><p><b>Using</b></p></li>
   <li><p><b>With</b></p></li>
   </ul>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>For each task you want to add, click <b>Add message</b> and fill in the following:
   <ul>
   <li><p><b>Status</b></p><p>Enter or map the status that this message represents, such as <code>ERROR</code>.</li>
   <li><p><b>Attempt</b></p><p>Enter or map the attempt number related to this message. This may be useful if different attempts produce different messages.</p></li>
   <li><p><b>Message</b></p><p>Enter or map the text of the message.</li>
   <li><p><b>Object</b></p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



#### Import Artifacts asynchronously

This action module imports a snapshot containing artifacts.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Snapshot ID]</td> 
   <td>Enter or map the ID of the snapshot you want to import.</td> 
  </tr> 
 </tbody> 
</table>

-->

### Gestion des enregistrements

* [Créer un enregistrement](#create-a-record)
* [Mettre à jour un enregistrement](#update-a-record)
* [Supprimer un enregistrement](#delete-a-record)
* [Corriger un enregistrement](#patch-a-record)
* [Obtenir un enregistrement](#get-a-record)

#### Créer un enregistrement

Ce module d’action crée un modèle de contenu ou un fragment de contenu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de contenu]</td> 
   <td>Indiquez si vous créez un modèle de contenu ou un fragment de contenu.<ul><li><p><b>Modèle de contenu</b></p>Passez à <a href="#template-fields" class="MCXref xref" >Champs du modèle</a>.</li><li><p><b>Fragment de contenu</b></p>Passez à <a href="#fragment-fields" class="MCXref xref" >Champs de fragment</a>.</li></ul></td> 
  </tr> 
  </tbody> 
</table>

##### Champs de modèle

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Saisissez ou mappez un nom pour ce modèle de contenu.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Saisissez ou mappez une description pour ce modèle de contenu.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Sélectionnez le type de modèle que vous souhaitez créer.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Canaux]</td> 
   <td>Sélectionnez les canaux inclus dans ce modèle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Origine du modèle de contenu]</td> 
   <td>Sélectionnez la source de ce modèle.</td>  
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Pour inclure des propriétés personnalisées dans le nouveau modèle, sélectionnez "Ajouter des métadonnées" et saisissez ou mappez la clé et la valeur des métadonnées. Répétez l’opération pour chaque champ personnalisé à inclure.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL HTML de messagerie]</td> 
   <td>Saisissez ou mappez l'HTML de l'email inclus dans ce modèle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contexte de l’éditeur]</td> 
   <td>Pour inclure des propriétés personnalisées dans l'email, sélectionnez "Ajouter un contexte d'éditeur" et saisissez ou mappez la clé et la valeur du contexte. Répétez l’opération pour chaque champ personnalisé à inclure.</td> 
  </tr> 
 </tbody> 
</table>

##### Champs de fragment

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Saisissez ou mappez un nom pour ce fragment de contenu.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Saisissez ou mappez une description pour ce fragment de contenu.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Sélectionnez le type de modèle que vous souhaitez créer.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Canaux]</td> 
   <td>Sélectionnez les canaux inclus dans ce modèle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Origine du fragment de contenu]</td> 
   <td>Sélectionnez la source de ce fragment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Pour inclure des propriétés personnalisées dans le nouveau modèle, sélectionnez "Ajouter des métadonnées" et saisissez ou mappez la clé et la valeur des métadonnées. Répétez l’opération pour chaque champ personnalisé à inclure.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td>Saisissez ou mappez le contenu du fragment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contexte de l’éditeur]</td> 
   <td>Pour inclure des propriétés personnalisées dans l'email, sélectionnez "Ajouter un contexte d'éditeur" et saisissez ou mappez la clé et la valeur du contexte. Répétez l’opération pour chaque champ personnalisé à inclure.</td> 
  </tr> 
 </tbody> 
</table>

#### Mettre à jour un enregistrement

Ce module d’action met à jour un modèle de contenu ou un fragment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de contenu]</td> 
   <td>Indiquez si vous mettez à jour une configuration de limitation ou une configuration de limitation.<ul><li><p><b>Modèle</b></p>Pour les champs, voir <a href="#template-fields" class="MCXref xref" >Champs du modèle</a> dans la section Créer un enregistrement de cet article.</li><li><p><b>Fragment</b></p>Pour les champs, voir <a href="#fragment-fields" class="MCXref xref" >Champs de fragment</a> dans la section Créer un enregistrement de cet article.</li></ul></td> 
  </tr> 
  </tbody> 
  </table>

#### Supprimer un enregistrement

Ce module d’action supprime un modèle de contenu ou un fragment de contenu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de contenu]</td> 
   <td>Indiquez si vous supprimez un modèle de contenu ou un fragment de contenu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de modèle/fragment]</td> 
   <td>Saisissez ou mappez l’identifiant du modèle ou du fragment que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

#### Corriger un enregistrement

Ce module d’action met à jour un enregistrement à l’aide d’un PATCH au format de pointeur JSON.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de contenu]</td> 
   <td>Indiquez si vous corrigez un modèle de contenu ou un fragment de contenu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de modèle/fragment]</td> 
   <td>Saisissez ou mappez l’identifiant du modèle ou du fragment à corriger.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Données de charge utile]</td> 
   <td>Pour ajouter un enregistrement au payload de ce correctif : <ol><li>Cliquez sur <b>Ajouter un enregistrement</b>.</li><li>Sélectionnez l’opération : Ajouter, Supprimer ou Remplacer.</li><li>Dans le champ Chemin d’accès , choisissez si vous souhaitez corriger le nom ou la description.</li><li> Dans le champ De , saisissez ou mappez une chaîne contenant une valeur de pointeur JSON.</li><li>Dans le champ Valeur , saisissez la valeur à utiliser dans l'opération.</li></ol></td> 
  </tr> 
 </tbody> 
</table>

#### Obtenir un enregistrement

Ce module d’action renvoie le modèle de contenu ou le fragment de contenu identifié par l’identifiant spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de contenu]</td> 
   <td>Indiquez si vous récupérez un modèle de contenu ou un fragment de contenu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de modèle/fragment]</td> 
   <td>Saisissez ou mappez l’identifiant du modèle ou du fragment que vous souhaitez récupérer.</td> 
  </tr> 
 </tbody> 
</table>


### Gestion des messages

* [Déclencher l&#39;exécution d&#39;un message unitaire](#trigger-a-unitary-message-execution)
* [Déclenchement d’un message basé sur une audience](#trigger-an-audience-based-message)
* [Vérification du statut d’un message basé sur l’audience](#check-the-status-for-audience-based-message)



#### Déclencher l&#39;exécution d&#39;un message unitaire

Ce module d’action déclenche un message unitaire à l’intention des destinataires que vous spécifiez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de demande]</td> 
   <td>Saisissez ou mappez l'identifiant de la requête associée à ce message.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Saisissez ou mappez l'identifiant de la campagne associée à ce message.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recipients]</td> 
   <td>Pour chaque destinataire que vous souhaitez recevoir ce message, cliquez sur <b>Ajouter un destinataire</b> et saisissez ce qui suit :
   <ul>
   <li><p><b>Type</b></p>Sélectionnez <code>aep</code>.</li>
   <li><p><b>Identifiant utilisateur</b></p>Saisissez ou mappez l’identifiant de profil Adobe Experience Platform du destinataire.</li>
   <li><p><b>Espace de noms</b></p>Saisissez ou mappez l’espace de noms du profil Adobe Experience Platform du destinataire.</li>
   <li><p><b>Adresse e-mail</b></p></li>
   <li><p><b>Numéro de téléphone mobile</b></p></li>
   <li><p><b>Prénom</b></p></li>
   <li><p><b>Nom</b></p></li>
   <li><p><b>Produit</b></p>Saisissez ou mappez le produit associé à ce message. Il est utilisé pour la substitution des variables dynamiques dans le contenu du message.</li>
   </ul></td> 
  </tr> 
 </tbody> 
</table>

#### Déclenchement d’un message basé sur une audience

Ce module d’action déclenche l’exécution d’un message basé sur l’audience, en fonction de la requête et de la campagne que vous spécifiez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de demande]</td> 
   <td>Saisissez ou mappez l'identifiant de la requête associée à ce message.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Saisissez ou mappez l'identifiant de la campagne associée à ce message.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Product]</td> 
   <td>Saisissez ou mappez le produit associé à ce message. Il est utilisé pour la substitution des variables dynamiques dans le contenu du message.</td> 
  </tr> 
 </tbody> 
</table>

#### Vérification du statut du message basé sur l’audience

Ce module d’action vérifie l’état d’un message par lots basé sur l’audience.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’exécution du message]</td> 
   <td>Saisissez ou mappez l'identifiant de l'exécution du message que vous souhaitez vérifier.</td> 
  </tr> 
 </tbody> 
</table>

### Vérifications d’état

<!--* [Check service health](#check-service-health)-->
* [Vérifier les dépendances d&#39;import](#check-the-import-dependencies)
* [Vérification du statut d&#39;un traitement d&#39;import](#check-the-status-of-an-import-job)

<!--

#### Check service health

This action module checks that the service represented by the connection is running.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
 </tbody> 
</table>

-->

#### Vérifier les dépendances d&#39;import

Ce module d’action vérifie les dépendances des artefacts de package. Vous pouvez ainsi vérifier si vous disposez des autorisations nécessaires pour importer des artefacts de package.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de module]</td> 
   <td>Saisissez ou mappez l’identifiant du package pour lequel vous souhaitez vérifier les autorisations.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environnement de test Target]</td> 
   <td>Saisissez ou mappez le nom de l’environnement de test dans lequel vous souhaitez importer le package.</td> 
  </tr> 
 </tbody> 
</table>

#### Vérification du statut d&#39;un traitement d&#39;import

Ce module d’action vérifie si une tâche d’importation a été un succès ou un échec.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Job ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la tâche pour laquelle vous souhaitez récupérer des données.</td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [Liste de tous les objets dépendants](#list-all-dependent-objects)
* [Paramétrages de liste](#list-configurations)
* [Liste des traitements d&#39;export et d&#39;import](#list-export-and-import-jobs)
* [Lister des packages](#list-packages)
* [Lister des enregistrements](#list-records)

#### Liste de tous les objets dépendants

Ce module de recherche répertorie tous les objets dépendants pour les objets du package spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objet de module]</td> 
   <td>Pour chaque objet du package pour lequel vous souhaitez renvoyer un objet dépendant, cliquez sur <b>Ajouter un objet</b> et saisissez le nom et le type de l’objet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de module]</td> 
   <td>Saisissez ou mappez l’identifiant du package pour lequel vous souhaitez répertorier les objets dépendants.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Environnement de test Target]</td> 
   <td>Saisissez ou mappez le nom de l’environnement de test qui contient le module pour lequel vous souhaitez répertorier les objets dépendants.</td> 
  </tr> 
 </tbody> 
</table>

#### Paramétrages de liste

Ce module d’action répertorie toutes les configurations de limitation ou de ralentissement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de configuration]</td> 
   <td>Indiquez si vous souhaitez répertorier les configurations de limitation ou les configurations de limitation.</td> 
  </tr> 
 </tbody> 
</table>

#### Liste des traitements d&#39;export et d&#39;import

Ce module de recherche répertorie les tâches d’exportation et d’importation actuelles. Vous pouvez utiliser des paramètres de requête pour filtrer la liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned results]</td> 
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
      <td>Indiquez si vous souhaitez classer les résultats par date de création ou de modification.</td>
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Paramètre de requête]</td> 
   <td>Pour chaque paramètre de requête par lequel vous souhaitez filtrer, cliquez sur <b>Ajouter un paramètre de requête</b>, puis sélectionnez le champ et l’opérateur, et saisissez la valeur du champ pour le filtre.</td> 
  </tr> 
 </tbody> 
</table>



#### Lister des packages

Ce module de recherche répertorie tous les modules de votre organisation. Vous pouvez utiliser des paramètres de requête pour filtrer la liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned results]</td> 
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
      <td>Indiquez si vous souhaitez classer les résultats par date de création ou de modification.</td>
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Paramètre de requête]</td> 
   <td>Pour chaque paramètre de requête par lequel vous souhaitez filtrer, cliquez sur <b>Ajouter un paramètre de requête</b>, puis sélectionnez le champ et l’opérateur, et saisissez la valeur du champ pour le filtre.</td> 
  </tr> 
 </tbody> 
</table>

#### Lister des enregistrements

Ce module de recherche répertorie toutes les configurations de limitation ou de ralentissement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner le type de contenu]</td> 
   <td>Indiquez si vous récupérez un modèle de contenu ou un fragment de contenu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td>Saisissez ou mappez le nom du paramètre selon lequel vous souhaitez trier cette liste. Ajoutez <code>-</code> ou <code>+</code> pour trier par ordre croissant ou décroissant. Si aucun signe n’est spécifié, la liste est triée de manière descendante.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>Ce champ est utilisé pour la pagination. Saisissez ou mappez les critères de la page suivante par rapport à la propriété spécifiée dans le champ Classer par .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td>Saisissez ou mappez le nom du paramètre selon lequel vous souhaitez trier cette liste. Ajoutez <code>-</code> ou <code>+</code> pour trier par ordre croissant ou décroissant. Si aucun signe n’est spécifié, la liste est triée de manière descendante.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtrage par propriété]</td> 
   <td>Pour chaque filtre de propriété à ajouter, cliquez sur <b>Ajouter un élément</b> et saisissez la clé et la valeur de la propriété. Les enregistrements qui incluent la valeur spécifiée pour la propriété sont inclus dans la liste.</td> 
  </tr> 
 </tbody> 
</table>


### Autre


#### Effectuer un appel API personnalisé.

Ce module d’action effectue un appel API personnalisé à l’API Adobe Journey Optimizer.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Pour obtenir des instructions sur la création d’une connexion à [!DNL Adobe Journey Optimizer], voir <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Créer une connexion à [!DNL Adobe Journey Optimizer]</a> dans cet article.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Saisissez un chemin relatif à l’URL de base.</p>
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
        <p>[!DNL Workfront Fusion] ajoute automatiquement les en-têtes d’autorisation, <code>x-api-key</code> et <code>x-gw-ims-org-id</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Saisissez la chaîne de requête.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>







<!--

* [Check if configuration can be deployed](#check-if-configuration-can-be-deployed)
* [Check service health](#check-service-health)
* [Check the import dependencies](#check-the-import-dependencies)
* [Check the status for audience-based message](#status-for-audience-based-message)
* [Copy artifacts synchronously](#copy-artifacts-synchronously)
* [Create a configuration](#create-a-configuration)
* [Create a package](#create-a-package)
* [Create a record](#create-a-record)
* [Delete a configuration](#delete-a-configuration)
* [Delete a package](#delete-a-package)
* [Delete a record](#delete-a-record)
* [Deploy a configuration](#deploy-a-configuration)
* [Export artifacts asynchronously](#export-artifacts-asynchronously)
* [Get a configuration](#get-a-configuration)
* [Get a record](#get-a-record)
* [Import a package](#import-a-package)
* [Import artifacts asynchronously](#import-artifacts-asynchronously)
* [List all dependent objects](#list-all-dependent-objects)
* [List export and import jobs](#list-import-and-export-jobs)
* [Look up a package](#look-up-a-package)
* [Make a custom API call](#make-a-custom-api-call)
* [Patch a record](#patch-a-record)
* [Publish a package](#publish-a-package)
* [Submit an import](#submit-an-import)
* [Trigger a unitary message execution](#trigger-a-unitary-message-execution)
* [Trigger an audience-based message](#trigger-an-audience-based-message)
* [Undeploy a configuration](#undeploy-a-configuration)
* [Update a configuration](#update-a-configuration)
* [Update a package](#update-a-package)
* [Update a record](#update-a-record)
* [List configurations](#list-configurations)
* [List packages](#list-packages)
* [List records](#list-records)

-->
