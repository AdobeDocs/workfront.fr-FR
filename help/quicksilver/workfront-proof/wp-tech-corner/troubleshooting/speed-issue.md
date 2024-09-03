---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problèmes de vitesse dans  [!DNL Workfront Proof]
description: Cette page d’aide peut vous aider à déterminer si les problèmes de vitesse que vous rencontrez lorsque vous utilisez  [!DNL Workfront Proof]  sont liés à votre fournisseur d’accès Internet ou au réseau de diffusion de contenu de  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 100%

---

# Problèmes de vitesse dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Cette page d’aide peut vous aider à déterminer si les problèmes de vitesse que vous rencontrez lorsque vous utilisez [!DNL Workfront Proof] sont liés à votre fournisseur d’accès Internet ou au réseau de diffusion de contenu de [!DNL Workfront Proof].

Les problèmes de vitesse sont généralement dus à la connexion locale du fournisseur d’accès à Internet ou à la configuration locale de l’accès à Internet (par exemple, en cas d’utilisation d’un serveur proxy) et échappent donc malheureusement au contrôle de [!DNL Workfront Proof].

Cela dit, vous pouvez prendre quelques mesures pour vérifier la vitesse de votre connexion, ce qui permettra de déterminer la cause première des problèmes que vous rencontrez. Toutes ces étapes sont également importantes pour le processus de dépannage et nous vous encourageons à prendre le temps de rassembler des informations sur toutes les étapes énumérées afin de garantir le diagnostic le plus précis possible du problème.

Une fois que vous aurez rassemblé tous les détails, nous vous recommandons de consulter votre service informatique local afin d’identifier les éventuels problèmes locaux.

## Déterminer la partie du système qui est lente

Lorsque vous utilisez [!DNL Workfront Proof], vous pouvez travailler avec le tableau de bord, par exemple pour gérer le contenu des dossiers et les personnes, ou avec la visionneuse [!DNL Workfront Proof] : effectuer une révision d’épreuve, vérifier les commentaires déjà formulés, etc.

La première étape de la résolution des problèmes de vitesse consiste à déterminer la partie exacte du système qui est lente. Lorsque vous signalez que le site [!DNL Workfront Proof] est lent, veillez à décrire les éléments suivants :

* D’autres pages web sont-elles également lentes ?
* Le problème se produit-il dans le tableau de bord ou dans la visionneuse [!DNL Workfront Proof] ?
* Quelle est précisément la partie du système qui est lente ? (Par exemple, traitement d’une nouvelle épreuve ou ouverture d’un commentaire dans la visionneuse [!DNL Workfront Proof].)

## Exécuter les tests traceroute et ping

Lorsque vous rencontrez des problèmes de performance, il est important d’exécuter la commande traceroute pour vérifier la connexion. Pour ce faire, ouvrez l’invite de commande de votre système (Terminal sous Mac/Linux) et effectuez les étapes suivantes :

1. Saisissez l’une des commandes suivantes, puis attendez que traceroute soit terminée :

   * Windows : **tracert app.proofhq.com**
   * Mac/Linux : **traceroute app.proofhq.com**

1. (Windows uniquement) Saisissez **ping app.proofhq.com**.
1. Lorsque l’exécution ping est terminée, cliquez avec le bouton droit de la souris sur l’invite de commande et sélectionnez Tout.
1. Copiez et collez les résultats dans la réponse à votre e-mail.
Veillez à laisser traceroute et ping se terminer avant d’envoyer les résultats à l’équipe de support.

## Tester la vitesse de connexion avec Speedtest.net

1. Ouvrez un navigateur et allez sur Speedtest.net.
1. Suivez les instructions de la base de connaissances Speedtest pour tester la vitesse de votre connexion Internet.
1. Copiez et collez les résultats dans un e-mail adressé à notre équipe de support.

## Vérifier l’onglet réseau dans la console du navigateur

La console web disponible dans les navigateurs modernes recueille des informations utiles sur les éventuelles latences du réseau, ce qui nous aidera à déterminer la cause première des problèmes de vitesse que vous rencontrez.

Pour vérifier les temps de chargement d’une page web :

1. Ouvrez la console de votre navigateur et l’onglet Réseau.
1. Rechargez la page.
1. Faites des captures d’écran ou enregistrez les résultats.
1. Partagez les résultats avec l’équipe de support.

Assurez-vous que la capture d’écran montre toutes les données. Vous pouvez agrandir la fenêtre de la console lorsque vous faites une capture d’écran ou faire défiler l’écran vers le bas dans un enregistrement.

Vous pouvez également consulter la documentation de votre navigateur pour obtenir des instructions plus détaillées.

## Vérifier votre connexion sur un autre réseau et une autre machine

Vérifier si vous rencontrez le même problème de vitesse de connexion en utilisant un autre appareil ou un autre réseau est une étape cruciale du processus de dépannage. Essayez de changer de machine ou d’appareil mobile, et essayez d’utiliser un autre réseau (par exemple, des données mobiles).

Comparez la connexion dans différentes combinaisons : en utilisant une machine différente sur le même réseau, en utilisant la même machine sur un réseau différent et en utilisant à la fois la machine et le réseau alternatifs, puis partagez les résultats avec l’équipe de support.
