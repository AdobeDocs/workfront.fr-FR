---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 'Résolution des problèmes : police d’interface corrompue dans la visionneuse de relecture sur Mac'
description: Résoudre le problème de la police d’interface corrompue dans la visionneuse de relecture sur Mac
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 100%

---

# Résolution des problèmes : police d’interface corrompue dans la visionneuse de relecture sur Mac

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture à l’intérieur d’[!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Si vous constatez que la visionneuse de relecture n’affiche pas correctement la police d’interface, cela peut être dû à des problèmes liés aux polices sur votre ordinateur Mac. Pour résoudre le problème, essayez les solutions suivantes :

## Supprimer les doublons de polices

Vérifiez si le système contient des polices en double.

1. Fermez le navigateur que vous utilisez.
1. Ouvrez l’application Font Book dans votre dossier Applications.
1. Cliquez sur **[!UICONTROL Toutes les polices]** (1).
1. Cliquez sur **[!UICONTROL Modifier]** > **[!UICONTROL Rechercher les doublons activés]**.

1. Cliquez sur **[!UICONTROL Oui]** pour résoudre les doublons.
1. Si vous voyez un avertissement concernant les polices corrompues, cliquez sur **[!UICONTROL Oui]**.
1. Redémarrez votre ordinateur.
1. Réessayez l’épreuve.

## Effacer le cache des polices

Parfois, les caches des polices dans Mac OS X sont corrompus. Par exemple, lorsqu’une police ou une famille de polices est réinstallée un certain nombre de fois ou si une application a été mise à jour ou réinstallée. Outre les fichiers de cache des polices du système d’exploitation, certaines applications peuvent avoir leur propre cache des polices. La suppression de ces fichiers de cache de polices peut résoudre le problème lié au texte brouillé.

Tout d’abord, vous devrez lancer Font Book, sélectionner la police ou la famille avec laquelle vous rencontrez des problèmes et appuyer sur le bouton Supprimer de votre clavier. Vous pouvez également cliquer avec le bouton droit et sélectionner [!UICONTROL Supprimer la famille]. Si vous ne savez pas quelle police ou famille est à l’origine des problèmes, vous pouvez essayer de supprimer d’abord les doublons, comme décrit ci-dessus.

La deuxième étape consiste à effacer le cache des polices et il existe plusieurs façons de procéder.

La première consiste simplement à redémarrer en mode sans échec en maintenant la touche Maj enfoncée immédiatement lorsque vous entendez le carillon de démarrage. Lorsque ce mode se charge, une barre de progression s’affiche, pendant laquelle le système exécute diverses vérifications et routines de maintenance, dont l’une consiste à effacer le cache des polices.

La deuxième méthode consiste à utiliser le terminal, ce qui peut être effectué en exécutant la commande suivante à partir d’un compte d’administration : *sudo atsutil database -remove*.

>[!NOTE]
>
>Cette commande vous obligera à saisir votre mot de passe, qui ne s’affichera pas une fois saisi. Nous vous recommandons de consulter votre service informatique, car cette action peut nécessiter des autorisations d’administrateur ou administratrice sur votre ordinateur.

Une autre approche consiste à utiliser un utilitaire de mise en cache des polices, tel que FontNuke, et à effacer le cache avec son aide.

De nombreux studios de prépresse, d’illustration et de conception utilisent également le logiciel Universal Type Server pour gérer les licences et la distribution des polices. Parfois, un problème peut se produire avec le cache de polices du serveur de type universel, ce qui peut entraîner la disparition des annotations [!DNL Workfront Proof].

Pour corriger, effacez le cache de polices du serveur de type universel et redémarrez le serveur de type universel.

## Corriger le conflit de polices [!DNL Flash]

Il se peut que vous n’ayez pas accès à cette fonctionnalité, car elle est prise en charge par [!DNL Flash], qui a été abandonné dans la plupart des environnements.

La visionneuse de relecture héritée est basée sur [!DNL Flash Player] et parfois, lorsque le texte est manquant dans la visionneuse de relecture, il est possible qu’il y ait un conflit de police entre OS X et [!DNL Flash Player]. Essayez ce qui suit :

1. Ouvrez le Finder et ouvrez l’onglet **[!UICONTROL Aller]**.
1. Appuyez sur la touche Option ( ⌥ Alt) pour ouvrir le dossier [!UICONTROL Bibliothèque] dans la liste déroulante.
1. Tout en maintenant la touche Option enfoncée, cliquez sur le dossier [!UICONTROL Bibliothèque].
1. Une fois que le dossier [!UICONTROL Bibliothèque] s’ouvre, accédez au dossier [!UICONTROL Polices] situé à l’intérieur de ce dernier.
1. Déplacez toutes les polices situées dans le dossier [!UICONTROL Polices] dans un autre dossier, peut-être sur votre bureau (ne créez pas un autre dossier dans le dossier Polices).
1. Cette action masque toutes vos polices personnalisées. Les polices système standard doivent toujours être enregistrées dans leur emplacement distinct.
1. Quittez et redémarrez [!DNL Safari].
1. Rouvrez l’épreuve.

Vous devriez voir vos polices maintenant. Si vous n’avez pas besoin des polices que vous avez supprimées de votre répertoire personnel, vous pouvez les supprimer en toute sécurité. Sinon, examinez-les par lots, copiez-les à nouveau dans votre dossier Bibliothèque/Polices et voyez laquelle est à l’origine du problème.
