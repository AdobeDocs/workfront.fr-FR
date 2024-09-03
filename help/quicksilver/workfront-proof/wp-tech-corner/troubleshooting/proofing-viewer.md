---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Dépannage - Visionneuse de relecture  [!DNL Workfront Proof]
description: Si le contenu de votre épreuve ne se charge pas et que vous ne pouvez voir qu’une visionneuse de relecture vide, c’est probablement parce qu’un blocage local de cette action se produit.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 39fdf5c2c2114a82c48f515c4a9f088596394045
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 100%

---

# Dépannage - Visionneuse de relecture [!DNL Workfront Proof]

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Si le contenu de votre épreuve ne se charge pas et que vous ne pouvez voir qu’une visionneuse de relecture vide, c’est probablement parce qu’un blocage local de cette action se produit. Essayez les solutions possibles ci-dessous.

## Vérifiez que la version de votre navigateur <!--and [!DNL Flash Player]--> est à jour.

Toutes les personnes chargées du développement travaillent constamment sur leurs applications et publient régulièrement de nouvelles fonctionnalités et correctifs pour leurs produits. Cela permet d’améliorer l’expérience client et de maintenir le niveau de sécurité ; il est donc recommandé d’utiliser uniquement les versions les plus récentes. Cela permet également d’éviter les conflits entre les applications.

<!--
### [!DNL Flash Player] Plugin Version

To check your current [!DNL Flash Player] version visit the [[!DNL Adobe] website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [[!DNL Flash Player] download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original [!DNL Adobe] plugin, so if your browser uses a built-in solution deactivate it and install the [!DNL Adobe] solution.
-->

### Version du navigateur

En règle générale, la plupart des navigateurs se mettent automatiquement à jour, mais si vous rencontrez des problèmes, vérifiez la version que vous utilisez et effectuez une mise à jour, le cas échéant.

Dans votre navigateur, accédez à [!UICONTROL Menu] et localisez l’option [!UICONTROL À propos] (dans certains cas, cette option peut être visible sous un menu d’[!UICONTROL Aide]). Dans la fenêtre pop-up [!UICONTROL À propos], vous trouverez des informations sur la version actuelle du navigateur, ainsi qu’une option permettant de mettre à jour/vérifier les mises à jour.

Par exemple, dans Chrome :

![Version du navigateur Chrome](assets/proofview-3.png)

Une fois que la dernière version du navigateur est installée, essayez de rouvrir votre épreuve et vérifiez si le problème est résolu.

<!--

## Ensure Your Local [!DNL Flash] Storage is Available

Our [!DNL Workfront Proof] Viewer is based on Flash, and we store some data about the proofs (i.e., comments, proof tiles, [!DNL Workfront Proof] Viewer settings) on your computer using [!DNL Flash Player]. If the [!DNL Workfront Proof] Viewer opens, but there is no content inside you will want to make sure that the Flash Storage is available on your machine and that [!DNL Workfront Proof] is allowed to use it.

If there is some storage allocated, but you're working with the bigger proofs with multiple pages and comments try to increase the [!DNL Flash] Storage and re-load your proof.

-->

## Identifier l’emplacement du problème

* Les épreuves s’ouvrent-elles dans un autre navigateur ?
* Si vous utilisez un navigateur tous les jours et que vous rencontrez des difficultés à afficher les épreuves, essayez d’ouvrir la même épreuve dans un autre navigateur sur votre ordinateur. Pour ce faire, il vous suffit de copier le lien de l’épreuve depuis la barre d’URL de votre navigateur principal et de le coller dans un autre navigateur. Si l’épreuve s’ouvre là-bas, vérifiez la configuration, les plug-ins et les extensions de votre navigateur principal, car ceux-ci peuvent interférer.
* Nous n’avons pas de navigateur préféré, mais si vous rencontrez des problèmes de performances avec votre navigateur actuel, nous vous conseillons de passer à un autre navigateur.
* Les épreuves s’ouvrent-elles sur un autre appareil dans votre emplacement ?
Si votre épreuve ne s’ouvre dans aucun navigateur sur votre ordinateur, essayez de l’ouvrir sur un autre ordinateur dans votre emplacement ou à l’extérieur de votre emplacement. Cela vous permet de déterminer si un problème se produit sur votre ordinateur ou si le problème se trouve sur votre réseau local.
Si votre niveau de sécurité est plus élevé, vos connexions à [!DNL Workfront Proof] peuvent être bloquées par les éléments suivants :

   * Votre logiciel AV local
   * Votre solution de sécurité réseau
   * Configuration DNS, pare-feu ou proxy
   * Ce sont des paramètres qui échappent à notre contrôle. Plusieurs solutions de sécurité sont disponibles et nous ne sommes pas en mesure de déterminer lesquelles sont implémentées dans votre réseau et celles qui peuvent bloquer les connexions à [!DNL Workfront Proof]. Ce n’est pas non plus à [!DNL Workfront Proof] de décider de votre configuration de sécurité interne. Si vous rencontrez des problèmes lors de l’ouverture des épreuves sur plusieurs appareils de votre emplacement/réseau, nous vous recommandons de contacter votre équipe informatique afin qu’elle puisse vérifier les paramètres réseau et autoriser ou ajouter [!DNL Workfront Proof] à la liste autorisée, le cas échéant.

* Les connexions à [!DNL Workfront Proof] sont-elles autorisées dans votre réseau ?
Dans la visionneuse de relecture, nous chargeons les miniatures et fragments des pages. Si ce contenu ne se charge pas correctement de votre côté, il se peut que certaines connexions à [!DNL Workfront Proof] soient bloquées sur votre réseau. Vous devrez vous assurer que toutes les connexions et tout le contenu de *.proofhq.com sont ajoutés à la liste autorisée. Votre équipe informatique devrait être en mesure de vous aider à vérifier cela.

## Vérifier les plug-ins

Si votre navigateur est à jour et que votre réseau ne bloque pas les connexions à [!DNL Workfront Proof], il se peut que quelque chose affecte l’affichage des épreuves dans votre navigateur. Plusieurs plug-ins et extensions sont souvent disponibles dans votre navigateur, et certains d’entre eux peuvent interférer ou être en conflit avec les autres.

La bonne pratique consiste à supprimer tous les modules complémentaires inconnus et à ne conserver que ceux que vous utilisez et auxquels vous faites confiance. Chaque navigateur doit vous donner des options pour vérifier/modifier/supprimer les plug-ins et les extensions. Nous utilisons JavaScript pour charger la visionneuse [!DNL Workfront Proof] : examinez donc particulièrement les plug-ins susceptibles d’affecter cela.

Si un module complémentaire spécifique interfère avec le chargement des épreuves, vous pouvez essayer de vérifier les détails dans la console du navigateur.

![Console du navigateur](assets/proofview-4.png)

Dans la plupart des navigateurs plus récents, d’autres outils de développement sont disponibles. Ils peuvent être utilisés pour un dépannage plus avancé.

Si vous rencontrez des problèmes lors de l’affichage des épreuves, procédez comme suit :

* Ouvrez la console de votre navigateur et rechargez l’épreuve.
* Vérifiez s’il existe des alertes ou des messages dans la console. Ces détails peuvent aider à identifier la cause profonde des problèmes.
* Demandez à votre équipe informatique d’analyser les résultats. Elle sera en mesure de vous conseiller et vous aidera à résoudre le problème local.
* Partagez les résultats avec notre équipe de support. Nous aurons plaisir à vous aider.

## Vérifier les paramètres de contenu mixte

Toutes les connexions à [!DNL Workfront Proof] sont effectuées par HTTPS. Toutefois, la visionneuse [!DNL Workfront Proof] charge les mosaïques via HTTP et les données sont sécurisées avec les jetons. Cela crée du contenu mixte que certains navigateurs ou solutions de sécurité peuvent bloquer (par défaut ou par configuration manuelle).

Si c’est la raison pour laquelle les épreuves ne s’ouvrent pas sur votre ordinateur (vous devriez pouvoir voir les alertes pertinentes dans la console du navigateur), autorisez ces connexions pour [!DNL Workfront Proof] ou modifiez vos paramètres pour autoriser le contenu mixte passif sur votre machine. Le contenu mixte peut être bloqué par votre navigateur, logiciel antivirus ou configuration réseau, afin de déterminer la cause exacte. Contactez votre équipe informatique ou votre administration réseau. Elles doivent également pouvoir vous aider à activer le contenu mixte sur votre machine.


