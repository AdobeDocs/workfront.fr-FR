---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Questions fréquentes sur Adobe Workfront Fusion
description: Cet article répond aux questions les plus courantes concernant  [!DNL Adobe Workfront Fusion], y compris des informations sur les objets couramment utilisés dans les workflows de Fusion.
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 100%

---

# Questions fréquentes sur Adobe Workfront Fusion

## Conditions d’accès

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
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Qu’est-ce qu’un scénario ?

### Réponse

Un scénario définit une séquence d’étapes qu’[!DNL Adobe Workfront Fusion] doit exécuter. Pour chaque scénario, vous spécifiez la source de données, la manière dont les données doivent être traitées, les données à utiliser et celles à ignorer. [!DNL Workfront Fusion] vous permet de créer des scénarios aussi complexes que vous le souhaitez ; même les scénarios les plus sophistiqués sont possibles.

Pour plus d’informations, voir [Créer un scénario d’intégration pratique dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Puis-je utiliser plus d’un module dans un scénario ? Ou simplement un déclencheur et une action ?

### Réponse

Vous pouvez utiliser autant de modules que vous le souhaitez dans un scénario. Vous pouvez créer des itinéraires indépendants et spécifier les données qui doivent y transiter. Vous pouvez également utiliser les résultats renvoyés par des actions individuelles et les transmettre à l’action suivante.

## [!DNL Workfront Fusion] peut-il travailler avec des fichiers ?

### Réponse

Oui. Lorsque vous utilisez [!DNL Workfront Fusion], les fichiers peuvent être reçus, enregistrés, transformés, convertis, chiffrés, etc. En outre, [!DNL Workfront Fusion] offre une large gamme de fonctionnalités intégrées conçues pour permettre aux personnes de travailler de manière efficace et créative avec les données contenues dans les fichiers.

Pour plus d’informations, voir [À propos du mappage de fichiers dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Que se passe-t-il si je laisse [!DNL Workfront Fusion] traiter un e-mail contenant plus d’une pièce jointe ?

### Réponse

Si vous utilisez le module d’[!UICONTROL e-mail] [!UICONTROL Récupérer les pièces jointes], chaque pièce jointe est envoyée individuellement via les autres modules du scénario. Des modules similaires sont également disponibles dans d’autres applications qui reçoivent plusieurs fichiers à la fois.

Pour plus d’informations, voir modules d’[[!UICONTROL e-mail]](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Certains déclencheurs permettent aux scénarios de s’exécuter instantanément. Que signifie « instantanément » ?

### Réponse

Les scénarios courants sont exécutés à intervalles réguliers selon le calendrier que vous avez spécifié (par exemple, toutes les heures, toutes les 5 minutes, une fois par mois, etc.). Il existe des déclencheurs spéciaux, appelés déclencheurs instantanés (webhooks), qui peuvent démarrer votre scénario immédiatement après avoir reçu des données d’un service donné. Les déclencheurs instantanés peuvent être extrêmement utiles. Nous vous recommandons de les utiliser dans la mesure du possible. Cela permet de réduire le nombre d’opérations. Les données reçues sont traitées immédiatement, sans attendre la prochaine exécution prévue. Par exemple, le module [!DNL Google Sheets] [!UICONTROL Surveiller les changements] lance un scénario immédiatement après la mise à jour d’une cellule.

## Qu’est-ce qu’un agrégateur ?

### Réponse

Un [!UICONTROL agrégateur] fusionne les données en une seule collection. Il s’agit par exemple de fichiers compressés dans une archive zip et envoyés en pièce jointe à un e-mail.

Pour plus d’informations, consultez [[!UICONTROL Module Agrégateur] dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Qu’est-ce qu’une opération ?

### Réponse

Une opération est une tâche effectuée par un module. Une opération se produit, par exemple, chaque fois qu’un déclencheur s’exécute et chaque fois qu’une action exécute une tâche.

## Qu’est-ce que le transfert de données ?

### Réponse

Le transfert de données correspond à la quantité de données transférées par le biais de votre scénario. Vous pouvez par exemple imaginer un scénario qui récupère une image de 100 Ko sur un serveur FTP, réduit sa taille à 50 Ko et enregistre les deux images dans le dossier [!DNL Dropbox]. La quantité de données utilisée dans ce scénario est de 250 Ko.

## Qu’est-ce qu’une connexion ?

### Réponse

Une connexion est le lien entre votre compte [!DNL Workfront Fusion] et le service tiers que vous souhaitez utiliser. La connexion peut être facilement créée lorsque vous modifiez un scénario. Pour ajouter une connexion, cliquez sur le bouton **[!UICONTROL Ajouter]** dans la configuration du module et suivez les instructions détaillées.

Pour plus d’informations, voir [Vue d’ensemble des connexions](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
