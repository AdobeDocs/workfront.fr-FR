---
product-area: documents
navigation-topic: proofing-overview
title: Vue d’ensemble du retraitement des documents pour la relecture
description: Lorsque vous envoyez un document (DOCX, PDF, XLSX, AI) à des fins de vérification, Adobe Workfront le retraite afin qu’il puisse s’afficher dans la visionneuse de vérification sans l’application logicielle que vous avez utilisée pour le créer.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 1%

---

# Vue d’ensemble du retraitement des documents pour la relecture

Lorsque vous envoyez un document (DOCX, PDF, XLSX, AI) à des fins de vérification, Adobe Workfront le retraite afin qu’il puisse s’afficher dans la visionneuse de vérification sans l’application logicielle que vous avez utilisée pour le créer. 

Chaque page de votre document apparaît dans la visionneuse de vérification sous la forme d’une miniature. Lorsque vous cliquez sur une miniature, vous pouvez zoomer sur une version bitmap de cette page à 100 %, 200 % et 400 %. Pour les bons à tirer d’une hauteur ou d’une largeur supérieure à 800 mm, le niveau de zoom maximal est de 200 %.

Les couleurs de votre document s’affichent en sRVB avec conversion de couleurs à partir de la dernière bibliothèque d’Adobes. La visionneuse de vérification prend en charge tous les profils ICC (International Color Consortium) incorporés dans le document.

Tout le texte de la police est extrait dans son calque tant que vous incluez l’extension de fichier correcte lors du téléchargement du document vers le système. Le texte inclus en tant qu’images ou courbes ne s’affiche pas.

>[!NOTE]
>
>Workfront prend actuellement en charge les documents contenant jusqu’à 2 000 pages. Cela inclut les bons à tirer combinés. Pour plus d’informations, voir [Création d’un BAT multi-page](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Conseils généraux

* Comme les fichiers de PDF sont les plus normalisés et les plus fiables, il est recommandé de convertir les documents dans ce format avant de les télécharger.
* Utilisez la dernière version possible de votre logiciel pour créer vos documents originaux.
* Si vous ne savez pas quels paramètres utiliser lors de l’enregistrement ou de l’export de vos documents dans l’application dans laquelle vous les avez créés, utilisez les paramètres par défaut. 
* Veillez à incorporer toutes les polices que vous utilisez dans un document à l’intérieur. Si vous utilisez des polices personnalisées, votre document affiche ces polices uniquement sur les machines où elles sont installées. Cependant, comme les polices personnalisées ne sont pas incluses dans le système de BAT, elles ne peuvent pas être utilisées lors de la génération du fichier, même lorsqu’elles sont incorporées.
* Si possible, placez tous les éléments de texte dans les calques supérieurs de votre conception. Cela permet de s’assurer que le texte est extrait et sélectionnable dans l’outil Annotation de texte .
* Placez toutes les images et tous les éléments de votre document à l’intérieur. Si vous les reliez à partir de sources externes, telles qu’un autre fichier sur votre ordinateur, elles ne s’afficheront pas dans le BAT que vous créez.
* Créez votre document selon les normes recommandées pour son type et optimisez-le avant de le télécharger. Cela permet de s’assurer que le document s’ouvre correctement dans la visionneuse de correctifs, ainsi que dans toutes les autres applications et plateformes.
* Dans votre logiciel de conception, essayez d’exécuter les options de contrôle en amont pour voir si votre document génère des avertissements. Ces options sont disponibles dans la plupart des applications sous forme d’aperçu de sortie, d’impression, etc. Pour plus d’informations, consultez la documentation de votre application .
* Assurez-vous que les paramètres de couleur sont cohérents dans tout le document.
* Si votre document est protégé contre des actions telles que la copie de fichiers, l’outil d’extraction de correctif peut ne pas être en mesure d’accéder à son contenu.

## Temps de traitement

Normalement, le traitement prend quelques secondes par page. Cependant, divers facteurs peuvent prolonger cette situation, tels que le trafic/la bande passante du réseau, la vitesse des connexions locales et la vitesse des connexions internationales (pour les utilisateurs situés en dehors des États-Unis). Les éléments suivants peuvent également affecter le temps de traitement :

* Pour les documents et images statiques : nombre de pages, dimensions de page, volume de texte, image et complexité des objets (éléments tels que plusieurs éléments vectoriels, calques, transparences).
* Pour les vidéos : longues durées, grandes dimensions et codecs utilisés.
* Pour les captures web : temps de chargement des pages web et dimensions de la page.

## Étapes du processus

Les fichiers envoyés suivent certaines ou toutes les étapes suivantes :

1. **Envoi**. Lorsque vous téléchargez un document sur le système, vous utilisez la page New BAT ou une interface de programmation d’application (API). 
1. **Queue**. Lors de périodes de trafic importantes, Workfront peut avoir besoin de mettre en file d’attente les envois pour éviter de surcharger le système. La plupart des bons à tirer ne passent que quelques secondes dans une file d&#39;attente. 
1. **Traitement.** Les fichiers atteignent les machines de traitement selon le type de contenu. Nous utilisons différents outils pour traiter les BAT vidéo, les captures web, les images statiques et les documents. Les envois de conteneurs ZIP (Rich Media Container) et de capture web interactive ne nécessitent pas de traitement.
