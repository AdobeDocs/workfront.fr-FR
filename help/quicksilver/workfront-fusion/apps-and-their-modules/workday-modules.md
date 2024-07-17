---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Workday
description: Dans un scénario Adobe Workfront Fusion, vous pouvez automatiser les workflows qui utilisent  [!DNL Workday] et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 44%

---

# Modules [!DNL Workday]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Workday] et les connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
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

Pour utiliser les modules [!DNL Workday], vous devez :

* Disposez d’un compte [!DNL Workday].

* Créez une application OAuth dans [!DNL Workday]. Pour obtenir des instructions, consultez la documentation [!DNL Workday].

## Connecter [!DNL Workday] à [!DNL Workfront Fusion]

1. Dans un module [!DNL Workfront Fusion], cliquez sur [!UICONTROL Ajouter] en regard du champ [!UICONTROL Connexion]

2. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Connection name]</p>
                </td>
                <td>Saisissez un nom pour la connexion.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Hôte Workday]</td>
                <td>Saisissez l’adresse de votre hôte [!DNL Workday] sans <code>https://</code>. Par exemple : <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL URL des services]</td>
                <td>Saisissez l’adresse de vos services web [!DNL Workday] sans <code>https://</code>. Par exemple : <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Nom du tenant]</td>
                <td>Saisissez le client pour ce compte [!DNL Workday]. Votre client est l’identifiant de votre organisation. Vous pouvez le voir dans l’URL que vous utilisez pour vous connecter à Workday. Exemple : dans l'adresse <code>https://www.myworkday.com/mycompany</code>, le client est <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Client ID]</td>
                <td>Saisissez l’identifiant du client pour l’application [!DNL Workday] utilisée par cette connexion. Vous obtenez cela lorsque vous créez l’application dans [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Client Secret]</td>
                <td>Saisissez le secret client pour l’application [!DNL Workday] utilisée par cette connexion. Vous obtenez cela lorsque vous créez l’application dans [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Délai d’expiration de la session (min)]</td>
                <td >Saisissez le nombre de minutes après lesquelles votre jeton d’autorisation expire.</td>
            </tr>
        </tbody>
    </table>


3. Cliquez sur [!UICONTROL Continuer] pour enregistrer la connexion et revenir au module

## Modules [!DNL Workday] et leurs champs

Lorsque vous configurez des modules [!DNL Workday], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Workday] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Action](#action)

* [Recherche](#search)


### Action

* [[!UICONTROL Créer un enregistrement]](#create-a-record)

* [[!UICONTROL Supprimer un enregistrement]](#delete-a-record)

* [[!UICONTROL Effectuer un appel d’API personnalisé]](#make-a-custom-api-call)

* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)


#### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un seul enregistrement dans [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Pour plus d'informations sur la connexion de votre compte [!DNL Workday] à Workfront Fusion, voir <a href="#Connect" class="MCXref xre[!DNL ]f" >Connexion [!DNL Workday] à [!DNL Workfront Fusion]</a>.</td>
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

#### [!UICONTROL Supprimer un enregistrement]

Ce module d’action supprime un seul enregistrement dans [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>Pour plus d'informations sur la connexion de votre compte [!DNL Workday] à [!DNL Workfront Fusion], voir <a href="#Connect" class="MCXref xre[!DNL ]f" >Connexion [!DNL Workday] à [!DNL Workfront Fusion]</a>.</td>
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


### [!UICONTROL Effectuer un appel d’API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Workday]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Workday].

Lors de la configuration de ce module, les champs suivants s’affichent.

Le module renvoie un code d’état, ainsi que les en-têtes et le corps de l’appel API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Pour plus d'informations sur la connexion de votre compte [!DNL Workday] à [!DNL Workfront Fusion], voir <a href="#Connect" class="MCXref xre[!DNL ]f" >Connexion [!DNL Workday] à [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] ajoute les en-têtes d’autorisation à votre place.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
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
            <td>Pour plus d’informations sur la connexion de votre compte [!DNL Workday] à Workfront Fusion, voir <a href="#Connect" class="MCXref xref" >[!UICONTROL Connecter [!DNL Workday] à Workfront Fusion]</a></td>
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

* [[!UICONTROL Répertorier les enregistrements]](#list-records)


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
            <td>Pour plus d’informations sur la connexion de votre compte [!DNL Workday] à Workfront Fusion, voir <a href="#Connect" class="MCXref xref" >[!UICONTROL Connecter [!DNL Workday] à Workfront Fusion]</a></td>
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

#### [!UICONTROL Répertorier les enregistrements]

Ce module de recherche récupère une liste d’enregistrements du type spécifié.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Connection]</td>
              <td>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workday] à [!DNL Workfront Fusion], voir <a href="#Connect" class="MCXref xref" >Se connecter [!DNL Workday] à [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Record Type]</td>
              <td>Sélectionnez le type d’enregistrement que vous souhaitez récupérer.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limit]</td>
              <td >
                  <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit récupérer au cours de chaque cycle d'exécution de scénario.</p>
              </td>
          </tr>
      </tbody>
  </table>
