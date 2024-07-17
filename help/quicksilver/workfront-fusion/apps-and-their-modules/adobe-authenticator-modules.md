---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Module Adobe Authenticator
description: Avec le module Adobe Authenticator, vous pouvez vous connecter à n’importe quel produit Adobe à l’aide d’une API, à l’aide d’une connexion unique.
author: Becky
feature: Workfront Fusion
exl-id: 74c943fb-37ad-4d91-8af7-9808ba69992e
source-git-commit: 443bdb5caee4b8a7ba9df95b0befff27b7aaabc2
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 24%

---

# Modules Adobe Authenticator

Le module Adobe Authenticator vous permet de vous connecter à n’importe quelle API Adobe à l’aide d’une connexion unique. Cela vous permet de vous connecter plus facilement à des produits Adobe qui n’ont pas encore de connecteur Fusion dédié.

L’avantage des modules HTTP est que vous pouvez créer une connexion, comme dans une application dédiée.

Pour obtenir la liste des API d’Adobe disponibles, voir [API d’Adobe](https://developer.adobe.com/apis). Vous pouvez ne pouvoir utiliser que les API auxquelles vous êtes affecté.

## Conditions d’accès

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan</td>
      <td>
        <p>Nouveau : Tous</p><p>Ou</p><p>Actuel : [!UICONTROL Pro] ou version ultérieure</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licence</td>
      <td>
        <p>Nouvelle : standard</p><p>Ou</p><p>Actuel : [!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licence</td>
      <td>
   <p>Exigences de licence Fusion actuelles : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences de licence Fusion héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Produit</td>
      <td>
   <p>Nouveau forfait Workfront : si vous disposez du forfait [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Formule Workfront actuelle : votre organisation doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td>
    </tr>
  </tbody>
</table>

## Conditions préalables

* Vous devez avoir accès au produit Adobe auquel vous souhaitez que le module se connecte.
* Vous devez avoir accès à Adobe Developer Console.
* Sur Adobe Developer Console, vous devez disposer d’un projet incluant l’API à laquelle vous souhaitez que le module se connecte. Vous pouvez effectuer les opérations suivantes :

   * Créez un projet avec l’API .

     Ou
   * Ajouter l’API à un projet existant.

  Pour plus d’informations sur la création ou l’ajout d’une API à un projet sur Adobe Developer Console, voir [Création d’un projet](https://developer.adobe.com/dep/guides/dev-console/create-project/) dans la documentation Adobe.

## Création d’une connexion

Une connexion Adobe Authenticator se connecte à un seul projet sur Adobe Developer Console. Pour utiliser la même connexion pour plusieurs API d’Adobe, ajoutez les API au même projet, puis créez une connexion à ce projet.

Vous pouvez créer des connexions distinctes à des projets distincts, mais vous ne pouvez pas utiliser de connexion pour accéder à une API qui ne se trouve pas sur le projet spécifié dans cette connexion.

>[!IMPORTANT]
>
>Avec le connecteur Adobe Authenticator, vous avez le choix entre établir une connexion OAuth serveur à serveur ou une connexion à un compte de service (JWT). Adobe a abandonné les informations d’identification JWT, qui cesseront de fonctionner après le 1er janvier 2025. **Nous vous recommandons donc vivement de créer des connexions OAuth.**
>
>Pour plus d’informations sur ces types de connexions, voir [Authentification serveur à serveur](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) dans la documentation Adobe

Pour créer une connexion :

1. Dans un module Adobe Authenticator, cliquez sur **Ajouter** en regard du champ Connexion.
1. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>
          <p>Indiquez si vous souhaitez créer une connexion OAuth serveur à serveur ou une connexion au compte de service (JWT).</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Nommez cette connexion.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Saisissez votre ID client [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre secret client [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">Portées [!UICONTROL]</td>
        <td>Si vous avez sélectionné une connexion OAuth, saisissez les portées nécessaires pour cette connexion.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID du compte technique]</td>
        <td>Saisissez votre ID de compte technique [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID d’organisation]</td>
        <td>Si vous avez sélectionné une connexion JWT, saisissez votre ID d’organisation [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Portées des métadonnées]</td>
        <td>Si vous avez sélectionné une connexion JWT, saisissez les méta-portées nécessaires pour cette connexion. </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Clé privée]</td>
        <td>
          <p>Si vous avez sélectionné une connexion JWT, saisissez la clé privée générée lors de la création de vos informations d’identification dans le [!DNL Adobe Developer Console]. </p>
          <p>Pour extraire votre clé privée ou votre certificat :</p>
          <ol>
            <li value="1">
              <p>Cliquez sur <b>[!UICONTROL Extract]</b>.</p>
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
        <td role="rowheader">[!UICONTROL URL de base]</td>
        <td>Vous devez ajouter les URL de base que vous souhaitez que cet authentificateur autorise. Lors de l’utilisation ultérieure du scénario Créer un module d’appel API personnalisé , vous ajouterez un chemin relatif à l’URL choisie. En saisissant ici des URL, vous pouvez contrôler à quoi le module d’appel d’API personnalisé peut se connecter, ce qui renforce la sécurité.<p>Pour chaque URL de base à ajouter à l’authentificateur, cliquez sur <b>Ajouter un élément</b> et saisissez l’URL de base.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentication URL]</td>
        <td>Laissez ce champ vide pour utiliser l’URL d’authentification Adobe IMS standard de <code>https://ims-na1.adobelogin.com</code>. Si vous n’utilisez pas Adobe IMS pour l’authentification, saisissez l’URL à utiliser pour l’authentification.</td>
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
        <p>[!UICONTROL Method]</p>
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
        <p>Saisissez la chaîne de requête.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Saisissez le nombre maximal de résultats que le module doit renvoyer dans un cycle d’exécution.</p>
      </td>
    </tr>
  </tbody>
</table>
