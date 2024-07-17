---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules de stockage de données
description: Un  [!DNL Adobe Workfront Fusion] entrepôt de données, similaire à une base de données ou à un tableau simple, peut stocker des données de scénarios, ce qui permet de transférer des données entre des scénarios individuels ou des exécutions de scénarios. Vous pouvez utiliser un magasin de données pour stocker de nouvelles données provenant de différents systèmes lors de la synchronisation.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 30%

---

# [!UICONTROL Modules Entrepôt de données]

Un entrepôt de données [!DNL Adobe Workfront Fusion], similaire à une base de données ou à un tableau simple, peut stocker des données de scénarios, ce qui permet de transférer des données entre des scénarios individuels ou des exécutions de scénarios. Vous pouvez utiliser un magasin de données pour stocker de nouvelles données provenant de différents systèmes lors de la synchronisation.

Les modules d’entrepôt de données vous permettent d’ajouter, de remplacer, de mettre à jour, de récupérer, de supprimer, de rechercher ou de compter des enregistrements dans votre entrepôt de données [!DNL Adobe Workfront Fusion].

Pour plus d’informations sur la création, la modification et la résolution des problèmes liés aux entrepôts de données, voir [Stockages de données dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

Pour obtenir une vidéo d’introduction aux magasins de données dans Workfront Fusion, voir :

* [Magasins de données](https://video.tv.adobe.com/v/3427029/){target=_blank}

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
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

Pour utiliser les modules [!UICONTROL Data Store], vous devez d’abord créer un entrepôt de données.

Pour plus d’informations sur la création d’entrepôts de données, voir [Entrepôts de données dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## Modules [!UICONTROL Entrepôt de données] et leurs champs

Lorsque vous configurez les modules de l’entrepôt de données, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En outre, d’autres champs de l’entrepôt de données peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Tous les modules [!UICONTROL Data Store] sont des modules de type Action.

* [Ajout/remplacement d’un enregistrement](#addreplace-a-record)
* [Mettre à jour un enregistrement](#update-a-record)
* [Obtention d’un enregistrement](#get-a-record)
* [Vérification de l’existence d’un enregistrement](#check-the-existence-of-a-record)
* [Suppression d’un enregistrement](#delete-a-record)
* [Supprimer tous les enregistrements](#delete-all-records)
* [Enregistrements de recherche](#search-records)
* [Nombre d’enregistrements](#count-records)

### [!UICONTROL Ajouter/Remplacer un enregistrement]

Ce module d’action ajoute ou remplace un enregistrement.

Vous spécifiez l’entrepôt de données et la clé de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

>[!NOTE]
>
>Le module renvoie une erreur lorsque vous essayez d’ajouter l’enregistrement qui se trouve déjà dans l’entrepôt de données sous le même nom et que l’option [!UICONTROL Remplacer un enregistrement existant] est désactivée.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Sélectionnez ou ajoutez l’entrepôt de données dans lequel vous souhaitez créer un enregistrement. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Saisissez la clé unique de l’enregistrement que vous souhaitez que le module ajoute ou remplace. La clé peut être utilisée ultérieurement pour récupérer l’enregistrement. Si vous laissez ce champ vide, une clé est générée automatiquement.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remplacer un enregistrement existant] </td> 
   <td> <p>Activez cette option pour remplacer l’enregistrement. L’enregistrement que vous souhaitez remplacer doit être spécifié dans le champ Clé ci-dessus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record] </td> 
   <td> <p>Saisissez les valeurs souhaitées dans les champs de l’enregistrement.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour un enregistrement.

Vous spécifiez l’entrepôt de données et la clé de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Sélectionnez ou ajoutez l’entrepôt de données dans lequel vous souhaitez créer un enregistrement. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Saisissez la clé unique de l’enregistrement que le module doit mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insérer l’enregistrement manquant] </td> 
   <td> <p>Activez cette option pour créer un nouvel enregistrement si l’enregistrement avec la clé spécifiée n’existe pas déjà.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p> Saisissez les valeurs souhaitées dans les champs de l’enregistrement que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtenir un enregistrement]

Ce module d’action récupère un enregistrement.

Vous spécifiez l’entrepôt de données et la clé de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Sélectionnez l’entrepôt de données duquel vous souhaitez récupérer un enregistrement.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Saisissez la clé unique de l’enregistrement que le module doit récupérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Vérifier l&#39;existence d&#39;un enregistrement]

Ce module d’action indique s’il existe un enregistrement particulier.

Vous spécifiez l’entrepôt de données et la clé de l’enregistrement.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Sélectionnez l’entrepôt de données à vérifier pour l’existence de l’enregistrement.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Saisissez la clé unique de l’enregistrement que vous souhaitez que le module vérifie l’existence.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Supprimer un enregistrement]

Ce module d’action supprime un enregistrement.

Vous spécifiez l’entrepôt de données et la clé de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Sélectionnez l’entrepôt de données à vérifier pour l’existence de l’enregistrement.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Saisissez la clé unique de l’enregistrement que le module doit supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Supprimer tous les enregistrements]

Ce module d’action supprime tous les enregistrements d’un entrepôt de données spécifique.

Vous spécifiez l’entrepôt de données.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Sélectionnez l’entrepôt de données dans lequel vous souhaitez supprimer tous les enregistrements.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Enregistrements de recherche]

Ce module de recherche recherche recherche les enregistrements d’un objet de l’entrepôt de données correspondant à la requête que vous spécifiez.

Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Sélectionnez l’entrepôt de données à rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Définissez le filtre pour la recherche.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Sort]</p> </td> 
   <td> <p style="font-weight: normal;">Pour chaque champ par lequel vous souhaitez trier, renseignez les champs suivants :</p> <p style="font-weight: bold;">[!UICONTROL Key]</p> <p>Sélectionnez le nom de la colonne selon laquelle vous souhaitez trier les résultats.</p> <p style="font-weight: bold;">[!UICONTROL Ordre]</p> <p>Indiquez si vous souhaitez trier les résultats dans l’ordre croissant ou décroissant.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Définissez le nombre maximal de résultats de recherche [!DNL Workfront Fusion] renvoyés au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Poursuivre l’exécution de l’itinéraire même si le module ne renvoie aucun résultat]</td> 
   <td> <p> S’il est activé, l’itinéraire dont fait partie ce module continue le traitement même si ce module ne renvoie aucun résultat.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Count Records]

Ce module d’action numérote les enregistrements dans un entrepôt de données.

Vous spécifiez l’entrepôt de données.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Sélectionnez l’entrepôt de données contenant les enregistrements à comptabiliser.</p> </td> 
  </tr> 
 </tbody> 
</table>
