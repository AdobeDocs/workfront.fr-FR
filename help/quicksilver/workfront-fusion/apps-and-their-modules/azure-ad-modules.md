---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Azure Principale Directory
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Azure] Principal Directory, et connectez-le à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: ac966231-251e-44de-be61-00afa5ece3fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 1%

---

# [!DNL Azure Active Directory] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Azure Active Directory], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
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

Pour utiliser [!DNL Azure Active Directory] modules, vous devez disposer d’un [!DNL Azure Active Directory] compte .

## [!DNL Azure Active Directory] modules et leurs champs

Lorsque vous configurez [!DNL Azure Active Directory] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Azure Active Directory] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Triggers

#### [!UICONTROL Surveiller les enregistrements] (planifié)

Ce module de déclenchement d’interrogation (planifié) exécute un scénario lorsqu’un enregistrement dans un objet sélectionné a été créé depuis la dernière exécution planifiée dans [!DNL Azure Active Directory]. Elle renvoie également tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Azure Active Directory] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Indiquez si vous souhaitez consulter les enregistrements d’utilisateur ou de groupe.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal d’enregistrements]</td> 
   <td>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Lecture d’enregistrement]](#read-record)
* [[!UICONTROL Créer un enregistrement]](#create-record)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)

#### [!UICONTROL Lecture d’enregistrement]

Ce module d’action lit les données d’un seul enregistrement dans [!DNL Azure Active Directory].

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous devez disposer des autorisations suffisantes pour accéder à l’enregistrement dans [!DNL Azure Active Directory] afin de récupérer ces informations.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Azure Active Directory] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Indiquez si vous souhaitez lire un enregistrement [!UICONTROL User] ou un enregistrement [!UICONTROL Group].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’unique [!DNL Azure Active Directory] Identifiant de l’enregistrement que vous souhaitez que le module lise.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un nouvel enregistrement d’utilisateur ou de groupe.

Vous indiquez le type d’enregistrement souhaité.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Azure Active Directory] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Indiquez si vous souhaitez lire un enregistrement [!UICONTROL User] ou un enregistrement [!UICONTROL Group].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Autres champs]</td> 
   <td>Renseignez ces champs pour définir les valeurs du nouvel enregistrement.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL Azure Active Directory] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL Azure Active Directory] modules.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Azure Active Directory] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Entrer ou mapper un chemin relatif à <code>https://graph.microsoft.com/{version}/{resource}?{query-parameters}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [Rechercher utilisateurs](#search-users)
* [Delta Utilisateurs/Groupes de recherche](#search-usersgroups-delta)

#### [!UICONTROL Rechercher utilisateurs]

Ce module de recherche recherche recherche des enregistrements dans un objet de la section [!DNL Azure Active Directory] qui correspondent à la requête de recherche que vous spécifiez. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Azure Active Directory] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Critères de recherche]</td> 
   <td> <p>Saisissez les critères à utiliser dans votre recherche.</p> <p>Pour plus d’informations sur les paramètres à utiliser, tels que "[!UICONTROL $filter]", voir <a href="https://docs.microsoft.com/en-us/graph/query-parameters">Utilisation des paramètres de requête pour personnaliser les réponses</a> dans le [!DNL Microsoft] Documentation de l’API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Sorties [!UICONTROL]</td> 
   <td>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Nombre maximal d’enregistrements]</td> 
   <td>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delta Utilisateurs/Groupes de recherche]

Ce module de recherche recherche recherche les enregistrements dans [!DNL Azure AD] qui ont été créés, mis à jour ou supprimés. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Azure Active Directory] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>
