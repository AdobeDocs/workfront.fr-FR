---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Module Adobe Authenticator
description: Avec le module Adobe Authenticator, vous pouvez vous connecter à n’importe quel produit Adobe à l’aide d’une API, à l’aide d’une connexion unique.
author: Becky
feature: Workfront Fusion
source-git-commit: 61a579c19228381d0aa06de3db5217614999731b
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 1%

---

# Modules Adobe Authenticator

Le module Adobe Authenticator vous permet de vous connecter à n’importe quelle API Adobe à l’aide d’une connexion unique. Cela vous permet de vous connecter plus facilement à des produits Adobe qui n’ont pas encore de connecteur Fusion dédié.

L’avantage des modules HTTP est que vous pouvez créer une connexion, comme dans une application dédiée.

Pour obtenir la liste des API d’Adobe disponibles, voir [API d’Adobe](https://developer.adobe.com/apis). Vous pouvez ne pouvoir utiliser que les API auxquelles vous êtes affecté.

## Exigences d’accès

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan</td>
      <td>
        <p>Nouveau : Quelconque</p><p>Ou</p><p>Actuel : [!UICONTROL Pro] ou version ultérieure</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license</td>
      <td>
        <p>Nouveau : Standard</p><p>Ou</p><p>Actuel : [!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] license</td>
      <td>
   <p>Exigences de licence Fusion actuelle : non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence Fusion héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Produit</td>
      <td>
   <p>Nouveau plan Workfront : si vous disposez de l’option [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Formule Workfront actuelle : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td>
    </tr>
  </tbody>
</table>

## Conditions préalables

* Vous devez avoir accès au produit Adobe auquel vous souhaitez que le module se connecte.
* Vous devez avoir accès à la console Adobe Developer.
* Vous devez disposer d’un projet sur la console Adobe Developer qui inclut l’API à laquelle le module doit se connecter. Vous pouvez :

   * Créez un projet avec l’API .

     Ou
   * Ajouter l’API à un projet existant.

  Pour plus d’informations sur la création ou l’ajout d’une API à un projet dans la console Adobe Developer, voir [Création d’un projet](https://developer.adobe.com/dep/guides/dev-console/create-project/) dans la documentation de l’Adobe.

## Création d’une connexion

Une connexion Adobe Authenticator se connecte à un seul projet dans la console Adobe Developer. Pour utiliser la même connexion pour plusieurs API d’Adobe, ajoutez les API au même projet, puis créez une connexion à ce projet.

Vous pouvez créer des connexions distinctes à des projets distincts, mais vous ne pouvez pas utiliser de connexion pour accéder à une API qui ne se trouve pas sur le projet spécifié dans cette connexion.

>[!IMPORTANT]
>
>Avec le connecteur Adobe Authenticator, vous avez le choix entre établir une connexion OAuth serveur à serveur ou une connexion à un compte de service (JWT). Adobe a abandonné les informations d’identification JWT, qui cesseront de fonctionner après le 1er janvier 2025. **Nous vous recommandons donc vivement de créer des connexions OAuth.**
>
>Pour plus d’informations sur ces types de connexions, voir [Authentification serveur à serveur](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) dans la documentation de l’Adobe

Pour créer une connexion :

1. Dans un module Adobe Authenticator, cliquez sur **Ajouter** en regard du champ Connexion .
1. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Type de connexion]</td>
        <td>
          <p>Indiquez si vous souhaitez créer une connexion OAuth serveur à serveur ou une connexion au compte de service (JWT).</p>
        </td>
      </tr>
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
        <td role="rowheader">Portées [!UICONTROL]</td>
        <td>Si vous avez sélectionné une connexion OAuth, saisissez les portées nécessaires pour cette connexion.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID du compte technique]</td>
        <td>Saisissez votre [!DNL Adobe] Identifiant du compte technique. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID d’organisation]</td>
        <td>Si vous avez sélectionné une connexion JWT, saisissez votre [!DNL Adobe] ID d’organisation. Vous pouvez le trouver dans la section [!UICONTROL Informations d’identification] du [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Portées des métadonnées]</td>
        <td>Si vous avez sélectionné une connexion JWT, saisissez les méta-portées nécessaires pour cette connexion. </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Clé privée]</td>
        <td>
          <p>Si vous avez sélectionné une connexion JWT, saisissez la clé privée générée lors de la création de vos informations d’identification dans la variable [!DNL Adobe Developer Console]. </p>
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
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Indiquez si vous vous connectez à un environnement de production ou hors production.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Choisissez si vous vous connectez à un compte de service ou à un compte personnel.</td>
      </tr>
    </tbody>
    </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.

## Module

### Effectuer un appel API personnalisé

Ce module d’action vous permet d’effectuer un appel à n’importe quelle API Adobe.

>[!TIP]
>
>Vous devez saisir l’URL complète de l’API à laquelle vous souhaitez vous connecter. Ce module n’accepte pas les URL relatives.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Pour obtenir des instructions sur la création d’une connexion au module Adobe Authenticator, voir <a href="#create-a-connection" class="MCXref xref" >Création d’une connexion</a> dans cet article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Saisissez l’URL complète du point API auquel vous souhaitez vous connecter.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Méthode [!UICONTROL]</p>
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p>
        <p>Par exemple, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion ajoute automatiquement des en-têtes d’autorisation.</p>
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
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
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

