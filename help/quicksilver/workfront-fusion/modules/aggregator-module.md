---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Module d’agrégation dans Adobe Workfront Fusion
description: Un module d’agrégation est un type de module conçu pour fusionner plusieurs lots de données en un seul lot.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 948fe5fc249e0dcb04655f015c8e46493159c3ed
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 68%

---

# Module d’[!UICONTROL Agrégation] dans [!DNL Adobe Workfront Fusion]

Un module d’agrégation est un type de module conçu pour fusionner plusieurs lots de données en un seul lot.

Pour plus d’informations sur les types de module, voir [Types de modules](../../workfront-fusion/modules/module-types.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Présentation du module [!UICONTROL Agrégateur]

Lorsqu’un module d’[!UICONTROL Agrégation] s’exécute, il effectue les opérations suivantes :

* Cumule tous les lots qu’il reçoit lors d’une seule opération du module source.
* Génère un seul lot avec un tableau contenant un élément pour chaque lot cumulé. Le contenu des éléments du tableau dépend du module d’[!UICONTROL Agrégation] et de sa configuration.

L’illustration suivante présente une configuration standard du module d’[!UICONTROL Agrégation] :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source Module]</p> </td> 
   <td> <p>Module de démarrage de l’agrégation du lot. Le module source est généralement un itérateur ou un module de recherche qui génère une série de lots.</p><p>Lorsque vous configurez le module source de l’agrégateur (et fermez la configuration de l’agrégateur), l’itinéraire entre le module source et le module de l’agrégateur est encadré dans une zone grise afin que vous puissiez voir clairement le début et la fin de l’agrégation. 
   </p> <p>Pour plus d’informations sur les itérateurs, voir <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Module [!UICONTROL Iterator] dans [!DNL Adobe Workfront Fusion]</a>.</p> <p>Pour plus d’informations sur les modules de recherche, voir Modules de recherche dans <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Types de modules</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target structure type]</p> </td> 
   <td> <p>(Applicable uniquement au module [!UICONTROL Array aggregator]). Structure cible dans laquelle les données sont agrégées. L’option par défaut, [!UICONTROL Personnalisé], vous permet de choisir les éléments qui doivent être agrégés dans l’élément <code>Array </code>de l’agrégateur de tableau [!UICONTROL] :</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Une fois que vous avez connecté plus de modules après le module [!UICONTROL Array aggator] et que vous êtes revenu à la configuration du module, le menu déroulant de type de structure [!UICONTROL Target] contient tous les modules suivants et leurs champs qui sont de type "Tableau de collections", comme illustré dans le champ [!UICONTROL Pièces jointes] du module [!DNL Slack] &gt;[!UICONTROL Créer un message] :</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td>Les champs que vous souhaitez inclure dans la sortie du module d’agrégation.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>La sortie de l’agrégateur peut être divisée en plusieurs groupes à l’aide du champ [!UICONTROL Group by]. Le champ [!UICONTROL Group by] peut contenir une formule évaluée pour chaque lot d’entrée d’agrégateur. L’agrégateur génère ensuite un lot par valeur de formule distincte. Chaque lot contient deux éléments :</p> 
    <ul> 
     <li><code>Key </code>contient la valeur distincte.</li> 
     <li><code>Array </code>contient les données agrégées des lots pour lesquels la formule a été évaluée sur la valeur <code>Key </code>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Arrêter le traitement après une agrégation vide</p> </td> 
   <td> <p>Par défaut, le module [!UICONTROL Aggregator] génère le résultat de l’agrégation même si aucun lot n’a atteint le module [!UICONTROL Aggregator] (par exemple, parce qu’ils ont tous été filtrés en chemin). Si l’option [!UICONTROL Stop processing after an empty aggregation] est activée, le module [!UICONTROL Aggregator] ne produira aucun lot de sortie dans ce cas et le flux s’arrêtera.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Les lots générés par les modules entre le module source et l’[!UICONTROL agrégateur] ne sont pas générés par le module [!UICONTROL Agrégateur] , de sorte qu’ils ne soient pas accessibles par les modules du flux après l’[!UICONTROL agrégateur]. Si vous avez besoin de données provenant d’un lot généré par un module entre le module source et le module [!UICONTROL Agrégateur], veillez à inclure l’élément donné dans la configuration du module [!UICONTROL Agrégateur] (comme dans le champ [!UICONTROL Champs agrégés] dans la configuration du module [!UICONTROL Agrégateur de tableau]).


## Exemple de scénario de fonctionnement des agrégateurs

Cet exemple de scénario montre comment compresser toutes les pièces jointes d’email et télécharger le fichier ZIP vers [!DNL Dropbox].

![](assets/dropbox-archive-350x87.png)

Le scénario ci-dessous montre comment :

* Le premier module surveille une boîte aux lettres pour les emails entrants : le déclencheur [!UICONTROL Email] >[!UICONTROL Watch emails] génère un lot avec l’élément `Attachments[]`, qui est un tableau contenant toutes les pièces jointes de l’email.

* Le deuxième modèle itère les pièces jointes de l&#39;email : [!UICONTROL Email] >[!UICONTROL Itérer les pièces jointes] récupère les éléments du tableau `Attachments[]` un par un et les envoie en tant que lots distincts.

* Le troisième module agrège les lots générés par le module [!UICONTROL Email] >[!UICONTROL Itérer les pièces jointes] : [!UICONTROL Archive] >[!UICONTROL Créer un agrégateur d’archive] accumule tous les lots qu’il reçoit et génère un seul lot contenant le fichier ZIP.

* Le dernier module charge le fichier ZIP obtenu sur [!DNL Dropbox] : [!DNL Dropbox] > [!UICONTROL Télécharger un fichier] obtient le fichier ZIP à partir du module [!UICONTROL Archive] > [!UICONTROL Créer une archive] et le charge vers [!DNL Dropbox].



Vous trouverez ci-dessous un exemple de configuration de l’agrégateur [!UICONTROL Archiver] > [!UICONTROL Créer une archive] :

![](assets/archive-create-an-archive-350x484.png)
