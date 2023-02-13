---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Dépannage - [!DNL Workfront Proof] visionneuse de vérification
description: Si le contenu de votre BAT ne se charge pas et que vous ne pouvez voir qu’une visionneuse de vérification dynamique des balises vide, c’est probablement parce qu’un blocage local de cette action se produit. Essayez les solutions possibles ci-dessous.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# Dépannage - [!DNL Workfront Proof] visionneuse de vérification

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Si le contenu de votre BAT ne se charge pas et que vous ne pouvez voir qu’une visionneuse de vérification dynamique des balises vide, c’est probablement parce qu’un blocage local de cette action se produit. Essayez les solutions possibles ci-dessous.

## Vérifiez votre navigateur et [!DNL Flash Player] Les versions sont à jour

Tous les développeurs travaillent constamment sur leurs applications et publient régulièrement de nouvelles fonctionnalités et correctifs pour leurs produits. Cela permet d’améliorer l’expérience utilisateur et de maintenir le niveau de sécurité afin qu’il soit recommandé d’utiliser uniquement les versions les plus récentes. Cela permet également d’éviter les conflits entre les applications.

### [!DNL Flash Player] Version du module externe

Pour vérifier votre [!DNL Flash Player] visite de la version [[!DNL Adobe] site web](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

Si votre numéro de version diffère de celui répertorié pour votre plateforme, accédez à la [[!DNL Flash Player] page de téléchargement](http://get.adobe.com/flashplayer/otherversions/) et obtenir la dernière version.

Remarque : il est recommandé d’utiliser l’original [!DNL Adobe] si votre navigateur utilise une solution intégrée, désactivez-la et installez la fonction [!DNL Adobe] solution.

### Version du navigateur

De nos jours, la plupart des navigateurs sont automatiquement mis à jour, mais si vous rencontrez des problèmes, il est utile de vérifier quelle version vous utilisez et d’effectuer la mise à jour, si nécessaire.

Dans votre navigateur, accédez à [!UICONTROL Menu] et recherchez la variable [!UICONTROL A propos] (dans certains cas, cela peut être visible sous [!UICONTROL Aide] ). Dans le [!UICONTROL A propos] s’affiche. Vous y trouverez des informations sur la version actuelle du navigateur, ainsi qu’une option permettant de mettre à jour/vérifier les mises à jour.

Voir dans Chrome :

![ProofView_3.png](assets/proofview-3-350x206.png)

Une fois que vous disposez de la dernière [!DNL Flash Player] module externe et version de navigateur installée essayez de rouvrir votre BAT et de voir si le problème est résolu.

## Assurez-vous que votre local [!DNL Flash] Le stockage est disponible

Notre [!DNL Workfront Proof] La visionneuse est basée sur le Flash et nous stockons des données sur les bons à tirer (c’est-à-dire, les commentaires, les mosaïques de BAT, etc.). [!DNL Workfront Proof] Paramètres de visionneuse) sur votre ordinateur à l’aide de [!DNL Flash Player]. Si la variable [!DNL Workfront Proof] La visionneuse s’ouvre, mais il n’y a pas de contenu à l’intérieur. Vérifiez que le stockage par Flash est disponible sur votre ordinateur et que [!DNL Workfront Proof] est autorisé à l’utiliser.

Si de l’espace de stockage est alloué, mais que vous travaillez avec les plus gros bons à tirer avec plusieurs pages et commentaires, essayez d’augmenter le [!DNL Flash] Stockez et rechargez votre BAT.

Consultez notre [Problèmes D&#39;Affichage Des Bons À Tirer - [!DNL Flash] Explication des objets partagés](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) pour obtenir des instructions détaillées.

## Identifier l’emplacement du problème

* Les bons à tirer s’ouvrent-ils dans un autre navigateur ?
* Si vous utilisez un navigateur tous les jours et que vous rencontrez des difficultés à afficher les bons à tirer, essayez d&#39;ouvrir le même bon à tirer dans un autre navigateur de votre ordinateur. Pour ce faire, il vous suffit de copier le lien du BAT depuis la barre d&#39;URL de votre navigateur principal et de le coller dans un autre navigateur. Si le BAT s’ouvre correctement, vérifiez la configuration, les modules externes et les extensions de votre navigateur principal, car ceux-ci peuvent interférer.
* Nous n’avons pas de navigateur préférable, mais si vous rencontrez des problèmes de performances dans votre navigateur actuel, nous vous conseillons de passer à un autre navigateur.
* Les bons à tirer s’ouvrent-ils sur une autre machine à votre emplacement ?
Si votre BAT ne s’ouvre dans aucun navigateur sur votre ordinateur, essayez de l’ouvrir sur un autre ordinateur à votre emplacement et/ou à l’extérieur de votre emplacement. Cela vous permet de déterminer si un problème concerne votre machine ou si c’est quelque chose dans votre réseau local.
Si votre niveau de sécurité est plus élevé, vos connexions à [!DNL Workfront Proof] peut être bloqué par :

   * Votre logiciel AV local
   * Votre solution de sécurité réseau
   * Configuration DNS, pare-feu ou proxy
   * Ce sont les paramètres qui échappent à notre contrôle. Plusieurs solutions de sécurité sont disponibles et nous ne sommes pas en mesure de déterminer lesquelles sont implémentées dans votre réseau et celles qui peuvent bloquer les connexions à [!DNL Workfront Proof]. Ce n&#39;est pas non plus à [!DNL Workfront Proof] pour décider de votre configuration de la sécurité interne. Si vous rencontrez des problèmes lors de l’ouverture des bons à tirer sur plusieurs machines de votre emplacement/réseau, nous vous recommandons de contacter votre équipe informatique afin qu’elle puisse vérifier les paramètres réseau et autoriser ou ajouter le [!DNL Workfront Proof] à la liste autorisée, le cas échéant.

* Les connexions à [!DNL Workfront Proof] autorisé dans votre réseau ?
Dans la visionneuse de BAT, nous chargeons les mosaïques - fragments des pages. Si ce contenu ne se charge pas correctement à votre fin, il se peut que certaines connexions à [!DNL Workfront Proof] sont bloqués sur votre réseau. Vous devrez vous assurer que toutes les connexions et tout le contenu de *.proofhq.com sont ajoutés à la liste autorisée. Votre équipe informatique devrait être en mesure de vous aider à vérifier cela.

## Vérifier les modules externes

Si votre navigateur et [!DNL Flash Player] Le module externe est à jour et votre réseau ne bloque pas les connexions à [!DNL Workfront Proof] il se peut qu’un élément du navigateur ait une incidence sur l’affichage des bons à tirer. De nos jours, plusieurs modules externes et extensions sont disponibles dans votre navigateur et certains d’entre eux interfèrent ou sont en conflit avec les autres.

La bonne pratique consiste à supprimer tous les modules complémentaires inconnus et à ne conserver que ceux que vous utilisez et auxquels vous faites confiance. Chaque navigateur doit vous donner des options pour vérifier/modifier/supprimer les modules externes et les extensions. Notre [!DNL Workfront Proof] La visionneuse est basée sur [!DNL Flash] et nous utilisons JavaScript pour charger la visionneuse afin que vous souhaitiez spécialement examiner les modules externes susceptibles d’affecter ces derniers.

Consultez les pages répertoriées ci-dessous pour obtenir des instructions plus détaillées des développeurs sur la désactivation des modules complémentaires de navigateur :

* Chrome : [plugins](https://support.google.com/chrome/answer/142064?hl=en-GB) / [extensions](https://support.google.com/chrome/answer/113907?hl=en-GB)
* Firefox : [add-ons](https://support.mozilla.org/en-US/kb/disable-or-remove-add-ons)
* Internet Explorer : [add-ons](http://windows.microsoft.com/en-GB/internet-explorer/manage-add-ons#ie=ie-11)
* Safari : [add-ons](http://support.apple.com/en-gb/HT203353)

Si un module complémentaire spécifique interfère avec le chargement des BAT, vous pouvez essayer de vérifier les détails dans la console du navigateur.

![ProofView_4.png](assets/proofview-4-350x57.png)

Dans la plupart des navigateurs plus récents, d’autres outils de développement sont disponibles et peuvent être utilisés pour un dépannage plus avancé.

Si vous rencontrez des problèmes lors de l’affichage des bons à tirer :

* Ouvrez la console de votre navigateur et rechargez le BAT.
* Vérifiez s’il existe des alertes ou des messages dans la console. Ces détails peuvent aider à identifier la cause profonde des problèmes.
* Demandez à votre équipe informatique d’analyser les résultats. Ils devraient être en mesure de conseiller et d&#39;aider à résoudre le problème local.
* Partagez les résultats avec notre [Équipe d’assistance](https://support.workfront.com/hc/en-us/requests/new). Nous serons heureux d&#39;aider.

Si vous ne savez pas comment ouvrir la console dans votre navigateur, veuillez consulter les étapes enregistrées :

* [Firefox](http://screencast.com/t/eP6FRtk4vxWS)
* [Internet Explorer](http://screencast.com/t/bYzq1iQv)
* [Google Chrome](http://screencast.com/t/2anpeAzOOyj)
* [Safari](http://screencast.com/t/rnOvgl3GidjL)

Vous pouvez également consulter la documentation du développeur de votre navigateur pour obtenir des instructions plus détaillées.

## Vérification des paramètres de contenu mixte

Toutes les connexions à [!DNL Workfront Proof] sont effectuées par HTTPS. Toutefois, dans la variable [!DNL Workfront Proof] La visionneuse charge les mosaïques via HTTP et les données sont sécurisées avec les jetons. Cela crée du contenu mixte que certains navigateurs ou solutions de sécurité peuvent bloquer (par défaut ou selon une configuration manuelle).

Si c’est la raison pour laquelle les bons à tirer ne s’ouvrent pas sur votre ordinateur (vous devriez pouvoir voir les alertes pertinentes dans la console du navigateur), autorisez de telles connexions pour [!DNL Workfront Proof] ou modifiez vos paramètres pour autoriser le contenu mixte passif sur votre machine. Le contenu mixte peut être bloqué par votre navigateur, votre logiciel AV, la configuration réseau, etc. Pour déterminer la cause exacte, contactez votre équipe informatique/vos administrateurs réseau. Ils doivent également pouvoir vous aider à activer le contenu mixte sur votre machine.

Contactez notre [Équipe d’assistance](https://support.workfront.com/hc/en-us/requests/new) si vous avez besoin d&#39;aide de notre part.
