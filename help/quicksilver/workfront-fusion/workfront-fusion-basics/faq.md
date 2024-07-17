---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Questions fréquentes sur Adobe Workfront Fusion
description: Cet article traite des questions courantes relatives à [!DNL Adobe Workfront Fusion], y compris des informations sur l’objet couramment utilisé dans les workflows Fusion.
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 20%

---

# Questions fréquentes sur Adobe Workfront Fusion

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
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

## Qu&#39;est-ce qu&#39;un scénario ?

### Réponse

Un scénario définit une séquence d’étapes à exécuter par [!DNL Adobe Workfront Fusion]. Pour chaque scénario, vous spécifiez la source de données, le mode de traitement des données, les données à utiliser et les éléments à ignorer. [!DNL Workfront Fusion] vous permet de créer des scénarios aussi complexes que nécessaire ; même les scénarios les plus sophistiqués sont possibles.

Pour plus d’informations, voir [Création d’un scénario d’intégration d’une pratique dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Puis-je utiliser plusieurs modules dans un scénario ? Ou juste un déclencheur et une action ?

### Réponse

Vous pouvez utiliser autant de modules que vous le souhaitez dans un scénario. Vous pouvez créer des itinéraires indépendants et spécifier les données qui doivent les traverser. Vous pouvez également utiliser les résultats renvoyés par des actions individuelles, puis les transmettre à l’action suivante.

## [!DNL Workfront Fusion] peut-il fonctionner avec des fichiers ?

### Réponse

Oui. Grâce à [!DNL Workfront Fusion], les fichiers peuvent être reçus, enregistrés, transformés, convertis, chiffrés, etc. De plus, [!DNL Workfront Fusion] offre un large éventail de fonctionnalités intégrées conçues pour permettre aux utilisateurs de travailler efficacement et de manière créative avec les données contenues dans les fichiers.

Pour plus d’informations, voir [À propos des fichiers de mappage dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Que se passe-t-il si je laisse [!DNL Workfront Fusion] traiter un email contenant plusieurs pièces jointes ?

### Réponse

Si vous utilisez le module [!UICONTROL Email] [!UICONTROL  de récupération des pièces jointes], chaque pièce jointe est envoyée individuellement par le biais du reste des modules du scénario. Des modules similaires sont également disponibles dans d’autres applications qui reçoivent plusieurs fichiers à la fois.

Pour plus d’informations, voir [[!UICONTROL E-mail] modules](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Certains déclencheurs permettent aux scénarios de s’exécuter instantanément. Que signifie &quot;instantanément&quot; ?

### Réponse

Les scénarios courants sont exécutés à intervalles réguliers selon le planning que vous spécifiez (par exemple, toutes les heures, toutes les 5 minutes, une fois par mois, etc.). Il existe des déclencheurs spéciaux, appelés déclencheurs instantanés (webhooks), qui peuvent démarrer votre scénario immédiatement après avoir reçu des données d’un service donné. Les déclencheurs instantanés peuvent être extrêmement utiles. Nous vous recommandons de les utiliser dans la mesure du possible. Elles permettent de réduire le nombre d’opérations. Les données reçues sont traitées immédiatement sans attendre la prochaine exécution planifiée. Par exemple, le module [!DNL Google Sheets] [!UICONTROL Watch Changes] démarre un scénario immédiatement après la mise à jour d’une cellule.

## Que sont les agrégateurs ?

### Réponse

Un [!UICONTROL agrégateur] fusionne les données en une seule collection. Par exemple, les fichiers sont compressés dans une archive zip et envoyés en tant que pièce jointe à un email.

Pour plus d’informations, voir le module [[!UICONTROL Agrégateur] dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Qu&#39;est-ce qu&#39;une opération ?

### Réponse

Une opération est une tâche effectuée par un module. Une opération se produit, par exemple, chaque fois qu’un déclencheur s’exécute et qu’une action effectue une tâche.

## Qu’est-ce que le transfert de données ?

### Réponse

Le transfert de données fait référence à la quantité de données transférées par le biais de votre scénario. Supposons, par exemple, que vous ayez un scénario qui récupère une image de 100 Ko à partir du FTP et réduit sa taille à 50 Ko, puis enregistre les deux images à [!DNL Dropbox]. La quantité de données utilisée dans ce scénario est de 250 Ko.

## Qu&#39;est-ce qu&#39;une connexion ?

### Réponse

Une connexion est le lien entre votre compte [!DNL Workfront Fusion] et le service tiers que vous souhaitez utiliser. La connexion peut être facilement créée lors de la modification d’un scénario. Pour ajouter une connexion, cliquez sur le bouton **[!UICONTROL Ajouter]** dans le paramètre du module et suivez les instructions étape par étape.

Pour plus d’informations, voir [Présentation des connexions](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
