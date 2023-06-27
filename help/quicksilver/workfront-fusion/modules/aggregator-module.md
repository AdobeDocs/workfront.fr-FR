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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# [!UICONTROL Agrégateur] module dans [!DNL Adobe Workfront Fusion]

Un module d’agrégation est un type de module conçu pour fusionner plusieurs lots de données en un seul lot.

Pour plus d’informations sur les types de module, voir [Types de modules](../../workfront-fusion/modules/module-types.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
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

## [!UICONTROL Agrégateur] module

Lorsqu’une [!UICONTROL Agrégateur] s’exécute, il effectue les opérations suivantes :

* Cumule tous les lots qu’il reçoit lors d’une seule opération du module source.
* Génère un seul lot avec un tableau contenant un élément pour chaque lot cumulé. Le contenu des éléments du tableau dépend de [!UICONTROL Agrégateur] et sa configuration.

L’illustration suivante présente une configuration standard de la variable [!UICONTROL Agrégateur] module :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Module source]</p> </td> 
   <td> <p>Module à partir duquel l’agrégation de lots démarrera. Le module source est généralement un itérateur ou un module de recherche qui génère une série de lots. Lorsque vous configurez le module source de l’agrégateur (et fermez la configuration de l’agrégateur), l’itinéraire entre le module source et le module de l’agrégateur est encadré dans une zone grise afin que vous puissiez voir clairement le début et la fin de l’agrégation. 
   </p> <p>Pour plus d’informations sur les itérateurs, voir <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Module [!UICONTROL Iterator] dans [!DNL Adobe Workfront Fusion]</a></p> <p>Pour plus d’informations sur les modules de recherche, voir Modules de recherche dans <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Types de modules</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type de structure de la cible]</p> </td> 
   <td> <p>(Applicable uniquement au module [!UICONTROL Array aggator] .) La structure cible dans laquelle les données doivent être agrégées. L’option par défaut, [!UICONTROL Personnalisé], vous permet de choisir les éléments qui doivent être agrégés dans le groupe de sortie de l’agrégateur de rayons A[!UICONTROL]. <code>Array </code>item:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Une fois que vous avez connecté plus de modules après le module [!UICONTROL Array aggator] et que vous êtes revenu à la configuration du module, la liste déroulante de type de structure [!UICONTROL Target] contient tous les modules suivants et leurs champs de type Array of Collections, comme illustré dans le champ [!UICONTROL Attachments] du champ [!DNL Slack] &gt; Module[!UICONTROL Créer un message] :</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Champs agrégés]</td> 
   <td>Sélectionnez les champs que vous souhaitez inclure dans la sortie du module d'agrégation.</td> 
  </tr> 
  <tr> 
   <td> <p>Groupe [!UICONTROL par]</p> </td> 
   <td> <p>La sortie de l'agrégateur peut être divisée en plusieurs groupes à l'aide du champ [!UICONTROL Group by] . Le champ [!UICONTROL Group by] peut contenir une formule évaluée pour chaque lot d’entrée d’agrégateur. L’agrégateur génère ensuite un lot par valeur de formule distincte. Chaque lot contient deux éléments :</p> 
    <ul> 
     <li><code>Key </code>contient la valeur distincte.</li> 
     <li><code>Array </code>contient les données agrégées des lots pour lesquels la formule a été évaluée sur la variable <code>Key </code>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Arrêter le traitement après une agrégation vide</p> </td> 
   <td> <p>Par défaut, le module [!UICONTROL Aggregator] génère le résultat de l’agrégation même si aucun lot n’a atteint le module [!UICONTROL Aggregator] (par exemple, parce qu’ils ont tous été filtrés sur leur chemin). Si l’option [!UICONTROL Arrêter le traitement après une agrégation vide] est activée, le module [!UICONTROL Agrégateur] ne produira aucun lot de sortie dans ce cas et le flux s’arrêtera.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Lots générés par les modules entre le module source et le [!UICONTROL Agrégateur] ne sont pas générés par le module [!UICONTROL Agrégateur] , de sorte qu’ils ne soient pas accessibles par les modules du flux après l’événement [!UICONTROL Agrégateur]. Si vous avez besoin de données provenant d’un lot généré par un module entre le module source et la variable [!UICONTROL Agrégateur] , veillez à inclure l’élément donné dans la variable [!UICONTROL Agrégateur] configuration du module (comme dans la variable [!UICONTROL Champs agrégés] dans la configuration de la propriété [!UICONTROL Agrégateur de tableau] ).


>[!INFO]
>
>**Exemple :** Cas pratique : Zipulation de toutes les pièces jointes d’email et chargement du fichier ZIP vers [!DNL Dropbox]
>
>Le scénario ci-dessous montre comment :
>
>* Surveillez une boîte aux lettres pour les emails entrants : [!UICONTROL Email] >[!UICONTROL Regarder les emails] Le déclencheur génère un lot avec l’élément `Attachments[]`, qui est un tableau contenant toutes les pièces jointes du courrier électronique.
>
>* Itérer les pièces jointes de l&#39;email : [!UICONTROL Email] >[!UICONTROL Itérer les pièces jointes] L’itérateur récupère les éléments de la variable `Attachments[]` tableau un par un et les envoie sous forme de lots distincts.
>
>* Agrégez les lots générés par le [!UICONTROL Email] >[!UICONTROL Itérer les pièces jointes] module : [!UICONTROL Archiver] >[!UICONTROL Création d’un agrégateur d’archives] accumule tous les lots qu’il reçoit et génère un seul lot contenant le fichier ZIP.
>
>* Chargez le fichier ZIP obtenu dans [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Chargement d’un fichier] récupère le fichier ZIP à partir de la fonction [!UICONTROL Archiver] > [!UICONTROL Création d’une archive] et le charge sur [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>Vous trouverez ci-dessous un exemple de configuration de la fonction [!UICONTROL Archiver] > [!UICONTROL Création d’une archive] agrégateur :
>
>![](assets/archive-create-an-archive-350x484.png)
