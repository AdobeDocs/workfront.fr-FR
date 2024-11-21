---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules de magasin de données
description: Un magasin de données  [!DNL Adobe Workfront Fusion] , similaire à une base de données ou à un tableau simple, peut stocker des données de scénarios, ce qui permet de transférer des données entre des scénarios individuels ou des exécutions de scénarios. Vous pouvez utiliser un magasin de données pour stocker de nouvelles données provenant de différents systèmes lors de la synchronisation.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 97%

---

# Modules de [!UICONTROL magasin de données]

Un magasin de données [!DNL Adobe Workfront Fusion], similaire à une base de données ou à un tableau simple, peut stocker des données de scénarios, ce qui permet de transférer des données entre des scénarios individuels ou des exécutions de scénarios. Vous pouvez utiliser un magasin de données pour stocker de nouvelles données provenant de différents systèmes lors de la synchronisation.

Les modules de magasin de données vous permettent d’ajouter, de remplacer, de mettre à jour, de récupérer, de supprimer, de rechercher ou de comptabiliser des enregistrements dans votre magasin de données [!DNL Adobe Workfront Fusion].

Pour plus d’informations sur la création, la modification et la résolution des problèmes des magasins de données, voir [Magasins de données dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).

Pour une vidéo de présentation des entrepôts de données dans Workfront Fusion, voir :

* [Entrepôts de données](https://video.tv.adobe.com/v/3427029/){target=_blank}

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
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Conditions préalables

Pour utiliser des modules de [!UICONTROL Magasin de données], vous devez d’abord créer un magasin de données.

Pour plus d’informations sur la création de magasins de données, voir [Magasins de données dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).

## Modules de [!UICONTROL Magasin de données] et leurs champs

Lorsque vous configurez des modules de magasin de données, [!DNL Workfront Fusion] affiche les champs listés ci-dessous. En plus de ces derniers, d’autres champs du magasin de données peuvent s’afficher, en fonction de facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Tous les modules de [!UICONTROL Magasin de données] sont des modules de type Action.

* [Ajouter/remplacer un enregistrement](#addreplace-a-record)
* [Mettre à jour un enregistrement](#update-a-record)
* [Obtenir un enregistrement](#get-a-record)
* [Vérifier l’existence d’un enregistrement](#check-the-existence-of-a-record)
* [Supprimer un enregistrement](#delete-a-record)
* [Supprimer tous les enregistrements](#delete-all-records)
* [Rechercher des enregistrements](#search-records)
* [Comptabiliser des enregistrements](#count-records)

### [!UICONTROL Ajouter/remplacer un enregistrement]

Ce module d’action ajoute ou remplace un enregistrement.

Vous spécifiez le magasin de données et la clé de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

>[!NOTE]
>
>Le module renvoie une erreur lorsque vous essayez d’ajouter l’enregistrement qui se trouve déjà dans le magasin de données sous le même nom et l’option [!UICONTROL Écraser un enregistrement existant] est désactivée.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Sélectionnez ou ajoutez le magasin de données dans lequel vous souhaitez créer un enregistrement. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Saisissez la clé unique de l’enregistrement que le module doit ajouter ou remplacer. La clé peut être utilisée ultérieurement pour récupérer l’enregistrement. Si vous laissez ce champ vide, une clé est générée automatiquement.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Overwrite an existing record] </td> 
   <td> <p>Activez cette option pour écraser l’enregistrement. L’enregistrement que vous souhaitez écraser doit être spécifié dans le champ Clé ci-dessus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record] </td> 
   <td> <p>Saisissez les valeurs souhaitées dans les champs de l’enregistrement.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour un enregistrement.

Vous spécifiez le magasin de données et la clé de l’enregistrement.

Le module renvoie l’ID de l’enregistrement et tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Sélectionnez ou ajoutez le magasin de données dans lequel vous souhaitez créer un enregistrement. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Saisissez la clé unique de l’enregistrement que le module doit mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insert missing record] </td> 
   <td> <p>Activez cette option pour créer un enregistrement si l’enregistrement avec la clé spécifiée n’existe pas déjà.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p> Saisissez les valeurs souhaitées dans les champs de l’enregistrement que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtenir un enregistrement]

Ce module d’action récupère un enregistrement.

Vous spécifiez le magasin de données et la clé de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Sélectionnez le magasin de données à partir duquel vous souhaitez récupérer un enregistrement.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Saisissez la clé unique de l’enregistrement que le module doit récupérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Vérifier l’existence d’un enregistrement]

Ce module d’action indique si un enregistrement spécifique existe.

Vous spécifiez le magasin de données et la clé de l’enregistrement.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Sélectionnez le magasin de données dans lequel l’existence de l’enregistrement doit être vérifiée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Saisissez la clé unique de l’enregistrement dont le module doit vérifier l’existence.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Supprimer un enregistrement]

Ce module d’action supprime un enregistrement.

Vous spécifiez le magasin de données et la clé de l’enregistrement.

Le module renvoie l’ID de l’enregistrement et tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Sélectionnez le magasin de données dans lequel l’existence de l’enregistrement doit être vérifiée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Saisissez la clé unique de l’enregistrement que le module doit supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Supprimer tous les enregistrements]

Ce module d’action supprime tous les enregistrements d’un magasin de données spécifique.

Vous spécifiez le magasin de données.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Sélectionnez le magasin de données dans lequel vous souhaitez supprimer tous les enregistrements.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Rechercher des enregistrements]

Ce module de recherche recherche des enregistrements d’un objet dans un magasin de données qui correspondent à la requête de recherche que vous avez spécifiée.

Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Sélectionnez le magasin de données dans lequel vous souhaitez effectuer une recherche.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Définissez le filtre pour la recherche.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Sort]</p> </td> 
   <td> <p style="font-weight: normal;">Pour chaque champ en fonction duquel vous souhaitez effectuer un tri, renseignez les champs suivants :</p> <p style="font-weight: bold;">[!UICONTROL Key]</p> <p>Sélectionnez le nom de la colonne en fonction de laquelle vous souhaitez trier les résultats.</p> <p style="font-weight: bold;">[!UICONTROL Order]</p> <p>Indiquez si vous souhaitez trier les résultats par ordre croissant ou décroissant.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Définissez le nombre maximal de résultats de recherche que [!DNL Workfront Fusion] renvoie pour un seul cycle d’exécution.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p> Si cette option est activée, l’itinéraire dont fait partie ce module continue le traitement même si ce module ne renvoie aucun résultat.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Comptabiliser des enregistrements]

Ce module d’action compte les enregistrements dans un magasin de données.

Vous spécifiez le magasin de données.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Sélectionnez le magasin de données qui contient les enregistrements à comptabiliser.</p> </td> 
  </tr> 
 </tbody> 
</table>
