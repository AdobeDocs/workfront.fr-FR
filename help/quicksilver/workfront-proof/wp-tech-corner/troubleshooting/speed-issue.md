---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problèmes de vitesse dans [!DNL Workfront Proof]
description: Cette page d’aide peut vous aider à déterminer si les problèmes de vitesse que vous pouvez rencontrer lors de l’utilisation de  [!DNL Workfront Proof] sont liés à votre FAI ou au réseau de diffusion de contenu de [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Problèmes de vitesse dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Cette page d’aide peut vous aider à déterminer si les problèmes de vitesse que vous pourriez rencontrer lors de l’utilisation de [!DNL Workfront Proof] sont liés à votre FAI ou au réseau de diffusion de contenu de [!DNL Workfront Proof].

Les problèmes de vitesse sont généralement dus à la connexion du FAI local ou à la configuration de l’accès Internet local (par exemple, où un serveur proxy est utilisé) et sont donc malheureusement hors de contrôle de [!DNL Workfront Proof].

Cela dit, il existe quelques étapes que vous pouvez suivre pour vérifier la vitesse de votre connexion, ce qui permettra de déterminer la cause principale des problèmes que vous rencontrez. Toutes ces étapes sont également importantes pour le processus de dépannage. Nous vous encourageons à prendre le temps de collecter des informations sur toutes les étapes répertoriées afin d’assurer un diagnostic le plus précis du problème.

Une fois que vous avez rassemblé tous les détails, nous vous recommandons de consulter votre service informatique local pour identifier les problèmes locaux.

## Déterminer quelle partie du système est lente

Lorsque vous utilisez [!DNL Workfront Proof], vous pouvez travailler avec le tableau de bord, par exemple, la gestion du contenu du dossier et des utilisateurs ou avec la visionneuse [!DNL Workfront Proof] : effectuer une révision du BAT, vérifier les commentaires déjà effectués, etc.

Déterminer quelle partie exacte du système est lente est la première étape de la résolution des problèmes de vitesse. Lorsque vous signalez que [!DNL Workfront Proof] est lent, veillez à décrire les éléments suivants :

* Vous rencontrez de la lenteur dans d’autres pages web ?
* Le problème se produit-il dans le tableau de bord ou la visionneuse [!DNL Workfront Proof] ?
* Quelle partie exacte du système est lente ? (par exemple, le traitement d’un nouveau BAT ou l’ouverture d’un commentaire dans la visionneuse [!DNL Workfront Proof])

## Exécution de tests traceroute et ping

Lorsque vous rencontrez des problèmes de performances, il est important d’exécuter la commande traceroute pour vérifier la connexion. Pour ce faire, ouvrez l’invite de commande dans votre système (Terminal dans Mac/Linux) et procédez comme suit :

1. Saisissez l’une des valeurs suivantes, puis attendez que le suivi soit terminé :

   * Windows : **tracert app.proofhq.com**
   * Mac/Linux : **traceroute app.proofhq.com**

1. (Windows uniquement) Saisissez **ping app.proofhq.com**.
1. Une fois le ping terminé, cliquez avec le bouton droit de la souris dans l’invite de commande et sélectionnez Tout.
1. Copiez et collez les résultats dans la réponse à votre email.
Veillez à laisser traceroute et ping se terminer avant d’envoyer les résultats à l’équipe d’assistance.

## Tester la vitesse de connexion à l’aide de Speedtest.net

1. Ouvrez un navigateur et accédez à Speedtest.net.
1. Suivez les instructions de la base de connaissances Speedtest pour tester la vitesse de votre connexion Internet.
1. Copiez et collez les résultats dans un email envoyé à l’équipe d’assistance.

## Onglet Réseau dans la console du navigateur

La console web disponible dans les navigateurs modernes rassemble des informations utiles sur les latences réseau, ce qui nous permettra de déterminer la cause principale des problèmes de vitesse que vous rencontrez.

Pour vérifier les temps de chargement d&#39;une page web :

1. Ouvrez la console de votre navigateur et l’onglet Réseau .
1. Rechargez la page.
1. Effectuez des captures d’écran ou enregistrez une capture d’écran des résultats.
1. Partagez les résultats avec l’équipe d’assistance.

Assurez-vous que la capture d’écran affiche toutes les données. Vous pouvez développer la fenêtre de la console lors d’une capture d’écran ou faire défiler la page vers le bas dans une capture d’écran.

Vous pouvez également consulter la documentation de votre navigateur pour obtenir des instructions plus détaillées.

## Vérifiez votre connexion sur un autre réseau et ordinateur.

Il est essentiel de vérifier si vous rencontrez le même problème avec la vitesse de connexion à l’aide d’un appareil ou d’un réseau différent dans le processus de dépannage. Essayez de passer à un autre ordinateur ou appareil mobile, et essayez d’utiliser un autre réseau (par exemple, les données mobiles).

Comparez la connexion selon différentes combinaisons : en utilisant une machine différente sur le même réseau, en utilisant la même machine sur un autre réseau et en utilisant la même machine et le même réseau, puis partagez les résultats avec l’équipe d’assistance.
