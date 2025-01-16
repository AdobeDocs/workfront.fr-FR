---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Workday
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 89%

---

# Modules [!DNL Workday]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules Workday](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/workday-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Workday] et le connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, consultez [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
  <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
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

Pour utiliser les modules [!DNL Workday], vous devez :

* Disposer d’un compte [!DNL Workday].

* Créer une application OAuth dans [!DNL Workday]. Pour obtenir des instructions, voir la documentation [!DNL Workday].

## Informations sur l’API Workday

Le connecteur Workday utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td>https://{{connection.servicesUrl}}/api</td> 
  </tr>
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.6.4</td> 
  </tr>
 </tbody> 
 </table>

## Connecter [!DNL Workday] à [!DNL Workfront Fusion]

1. Dans n’importe quel module [!DNL Workfront Fusion], cliquez sur [!UICONTROL Ajouter] à côté du champ [!UICONTROL Connexion] 

2. Remplissez les champs suivants :

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Connection name]</p>
                </td>
                <td>Saisir le nom de la connexion</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday host]</td>
                <td>Saisissez l’adresse de votre hôte [!DNL Workday] sans <code>https://</code>. Par exemple, <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Services URL]</td>
                <td>Saisissez l’adresse de vos services web [!DNL Workday] sans <code>https://</code>. Par exemple, <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Tenant name]</td>
                <td>Saisissez le nom du locataire de ce compte [!DNL Workday]. Pour votre locataire, indiquez l’identifiant de votre organisation. Il est visible dans l’URL que vous utilisez pour vous connecter à Workday. Exemple : dans l’adresse <code>https://www.myworkday.com/mycompany</code>, le locataire est <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Client ID]</td>
                <td>Saisissez l’identifiant du client pour l’application [!DNL Workday] que cette connexion utilise. Vous l’obtenez lorsque vous créez l’application dans [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Client Secret]</td>
                <td>Saisissez le secret du client pour l’application [!DNL Workday] que cette connexion utilise. Vous l’obtenez lorsque vous créez l’application dans [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Session timeout (min)]</td>
                <td >Saisissez le nombre de minutes après lequel votre jeton d’autorisation expire.</td>
            </tr>
        </tbody>
    </table>


3. Cliquez sur [!UICONTROL Continuer] pour enregistrer la connexion et revenir au module.

## Les modules [!DNL Workday] et leurs champs

Lorsque vous configurez les modules [!DNL Workday], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Workday] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
            <td>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL Workday] à Workfront Fusion, consultez <a href="#Connect" class="MCXref xre[!DNL ]f" >Connecter [!DNL Workday] à [!DNL Workfront Fusion]</a>.</td>
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
            <td role="rowheader">[!UICONTROL Subresource ID]</td>
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
            <td>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL Workday] à [!DNL Workfront Fusion], consultez <a href="#Connect" class="MCXref xre[!DNL ]f" >Connecter [!DNL Workday] à [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record type]</td>
            <td>Sélectionnez le type d’enregistrement que vous souhaitez supprimer.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Specific record type]</td>
            <td>Sélectionnez le type d’enregistrement que vous souhaitez supprimer. Cette sélection se base sur le type d’enregistrement que vous avez choisi.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Subresource ID]</td>
            <td>Saisissez ou mappez l’identifiant de la sous-ressource que vous souhaitez supprimer.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez supprimer.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL Effectuer un appel d’API personnalisé]

Ce module d’action vous permet d’effectuer un appel personnalisé et authentifié vers l’API [!DNL Workday]. Cela vous permet de créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Workday].

Lorsque vous configurez ce module, les champs suivants s’affichent.

Le module renvoie le code d’état, ainsi que les en-têtes et le corps de l’appel API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL Workday] à [!DNL Workfront Fusion], consultez <a href="#Connect" class="MCXref xre[!DNL ]f" >Connecter [!DNL Workday] à [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin d’accès relatif à <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre code JSON, saisissez les guillemets à l’extérieur de l’instruction conditionnelle.</p> 
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
            <td>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL Workday] à Workfront Fusion, consultez <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] to Workfront Fusion].</a></td>
        </tr>
        <tr>
            <td  role="rowheader">Type d’enregistrement</td>
            <td>Sélectionnez le type d’enregistrement [!UICONTROL ]que vous souhaitez mettre à jour.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez mettre à jour.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Subresource ID]</td>
            <td >Saisissez ou mappez l’identifiant de la sous-ressource que vous souhaitez mettre à jour.</td>
        </tr>
    </tbody>
</table>

### Recherche

* [[!UICONTROL Lire un enregistrement]](#read-a-record)

* [[!UICONTROL Répertorier des enregistrements]](#list-records)


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
            <td>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL Workday] à Workfront Fusion, consultez <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] to Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record type]</td>
            <td>Sélectionnez le type d’enregistrement que vous souhaitez supprimer.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Specific record type]</td>
            <td>Sélectionnez le type d’enregistrement que vous souhaitez lire. Cette sélection se base sur le type d’enregistrement que vous avez choisi.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez supprimer.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Répertorier des enregistrements]

Ce module de recherche permet d’obtenir une liste des enregistrements du type spécifié.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Connection]</td>
              <td>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL Workday] à [!DNL Workfront Fusion], consultez la section <a href="#Connect" class="MCXref xref" >Connecter [!DNL Workday] à [!DNL Workfront Fusion]</a>.</td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Record Type]</td>
              <td>Sélectionnez le type d’enregistrement que vous souhaitez récupérer.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limit]</td>
              <td >
                  <p>Saisissez ou mappez le nombre maximum d’enregistrements que vous souhaitez que le module récupère au cours de chaque cycle d’exécution du scénario.</p>
              </td>
          </tr>
      </tbody>
  </table>
