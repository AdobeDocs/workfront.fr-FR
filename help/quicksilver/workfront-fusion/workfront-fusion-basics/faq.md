---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: FAQ sur Adobe Workfront Fusion
description: Cet article traite des questions courantes relatives aux [!DNL Adobe Workfront Fusion], y compris des informations sur l’objet couramment utilisé dans les workflows Fusion
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# FAQ sur Adobe Workfront Fusion

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Qu&#39;est-ce qu&#39;un scénario ?

### Réponse

Un scénario définit une séquence d’étapes à exécuter par [!DNL Adobe Workfront Fusion]. Pour chaque scénario, vous spécifiez la source de données, le mode de traitement des données, les données à utiliser et les éléments à ignorer. [!DNL Workfront Fusion] vous permet de créer des scénarios aussi complexes que nécessaire ; même les scénarios les plus sophistiqués sont possibles.

Pour plus d’informations, voir [Créez un scénario d’intégration d’une pratique dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Puis-je utiliser plusieurs modules dans un scénario ? Ou juste un déclencheur et une action ?

### Réponse

Vous pouvez utiliser autant de modules que vous le souhaitez dans un scénario. Vous pouvez créer des itinéraires indépendants et spécifier les données qui doivent les traverser. Vous pouvez également utiliser les résultats renvoyés par des actions individuelles, puis les transmettre à l’action suivante.

## Peut [!DNL Workfront Fusion] travailler avec des fichiers ?

### Réponse

Oui. Utilisation [!DNL Workfront Fusion], les fichiers peuvent être reçus, enregistrés, transformés, convertis, chiffrés, etc. De plus, [!DNL Workfront Fusion] offre un large éventail de fonctionnalités intégrées conçues pour permettre aux utilisateurs de travailler de manière efficace et créative avec les données contenues dans les fichiers.

Pour plus d’informations, voir [À propos du mappage des fichiers dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Que se passe-t-il si je laisse [!DNL Workfront Fusion] traiter un email contenant plusieurs pièces jointes ?

### Réponse

Si vous utilisez la variable [!UICONTROL Email] module [!UICONTROL Récupération des pièces jointes], chaque pièce jointe est envoyée individuellement par le biais du reste des modules dans le scénario. Des modules similaires sont également disponibles dans d’autres applications qui reçoivent plusieurs fichiers à la fois.

Pour plus d’informations, voir [[!UICONTROL Email] modules](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Certains déclencheurs permettent aux scénarios de s’exécuter instantanément. Que signifie &quot;instantanément&quot; ?

### Réponse

Les scénarios courants sont exécutés à intervalles réguliers selon le planning que vous spécifiez (par exemple, toutes les heures, toutes les 5 minutes, une fois par mois, etc.). Il existe des déclencheurs spéciaux, appelés déclencheurs instantanés (webhooks), qui peuvent démarrer votre scénario immédiatement après avoir reçu des données d’un service donné. Les déclencheurs instantanés peuvent être extrêmement utiles. Nous vous recommandons de les utiliser dans la mesure du possible. Elles permettent de réduire le nombre d’opérations. Les données reçues sont traitées immédiatement sans attendre la prochaine exécution planifiée. Par exemple, la variable [!DNL Google Sheets] module [!UICONTROL Watch Changes] démarre un scénario immédiatement après la mise à jour d’une cellule .

## Que sont les agrégateurs ?

### Réponse

Un [!UICONTROL Agrégateur] fusionne les données en une seule collection. Par exemple, les fichiers sont compressés dans une archive zip et envoyés en tant que pièce jointe à un email.

Pour plus d’informations, voir [[!UICONTROL Agrégateur] module dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Qu&#39;est-ce qu&#39;une opération ?

### Réponse

Une opération est une tâche effectuée par un module. Une opération se produit, par exemple, à chaque exécution d’un déclencheur et à chaque exécution d’une action.

## Qu’est-ce que le transfert de données ?

### Réponse

Le transfert de données fait référence à la quantité de données transférées par le biais de votre scénario. Supposons, par exemple, que vous ayez un scénario qui récupère une image de 100 Ko à partir du FTP et réduit sa taille à 50 Ko, puis enregistre les deux images dans [!DNL Dropbox]. La quantité de données utilisée dans ce scénario est de 150 Ko.

## Qu&#39;est-ce qu&#39;une connexion ?

### Réponse

Une connexion est le lien entre votre [!DNL Workfront Fusion] et le service tiers que vous souhaitez utiliser. La connexion peut être facilement créée lors de la modification d’un scénario. Pour ajouter une connexion, cliquez sur le bouton **[!UICONTROL Ajouter]** dans le paramètre du module et suivez les instructions étape par étape.

Pour plus d’informations, voir [A propos de la connexion [!DNL Adobe Workfront Fusion] vers une application ou un service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
