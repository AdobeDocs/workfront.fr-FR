---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Ajouter un module de déclenchement à un scénario de base
description: Découvrez comment ajouter un module de déclenchement pour permettre au scénario de rechercher périodiquement de nouvelles requêtes et de les convertir en projets.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Utilisez une fonction pour mettre à jour un projet dans un scénario simple de la fonction [!DNL Adobe Workfront Fusion]

La mise à jour d’un élément de travail Workfront est un cas d’utilisation courant de Workfront Fusion. Dans cet exemple, vous utiliserez une fonction pour modifier le nom d’un projet en majuscules.

Fusion comprend de nombreux types de fonctions qui vous permettent de transformer et d’exécuter une logique conditionnelle sur vos données. Pour plus d’informations sur l’utilisation des fonctions, voir [Mappage des informations d’un module à un autre dans Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

Cet exemple modifie le scénario créé dans [Création d’un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Conditions préalables

Vous devez créer le scénario décrit dans la section [Création d’un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) avant de suivre cette procédure.

## Utilisation d’une fonction pour mettre à jour un projet

### Ajout du module Mettre à jour l’enregistrement à votre scénario

1. Ouvrez le scénario dans l’éditeur de scénarios.
1. Pointez sur le cercle partiel à droite du module, puis cliquez sur **[!UICONTROL Ajouter un autre module]**.
1. Sélectionner [!DNL Adobe Workfront] dans la liste des applications, puis choisissez le module **[!UICONTROL Mettre à jour l’enregistrement]**.
1. dans le champ ID , sélectionnez le bloc ID situé sous le module d’objet Convert . Il s’agit de l’identifiant du projet qui a été généré par ce module.

   ![ID de l’objet Convert](assets/id-convert-object.png)

1. Dans le champ Type d’enregistrement , sélectionnez Projet , car l’objet à mettre à jour est un projet.
1. Dans la zone Sélectionner les champs à mapper, sélectionnez Nom.

   Un champ Nom s’ouvre.

### Faire correspondre la fonction de la mise à jour du nom

Lorsque ce scénario convertit une requête en projet, le nom du projet est identique à celui de la requête. La fonction ici prend ce nom et met en majuscules toutes les lettres qu&#39;il contient.

1. Cliquez sur le bouton **Nom** champ .

   Le panneau de mappage s’ouvre.
1. Dans le panneau de mappage, cliquez sur le **Fonctions de texte et binaires** Icône ![Icône Fonctions de texte](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Sélectionner la fonction **upper**.

   La fonction apparaît dans le champ Nom , y compris le formatage de l’entrée attendue.

   L’entrée pour cet exemple est le nom du problème à partir duquel le projet a été converti.

1. Placez le curseur entre les parenthèses, car c’est là que va aller l’entrée.
1. Dans le panneau de mappage, cliquez sur le **sortie de module** Icône ![Icône de sortie du module](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Sélectionnez le bloc de nom qui a été généré par votre premier module.

   Le bloc de nom apparaît dans la fonction .

   ![Bloc de nom dans la fonction](assets/map-name.png)

1. Cliquez sur OK pour enregistrer les paramètres du module.

### Tester et activer

1. Testez le scénario en cliquant sur **Exécuter une seule fois** dans le coin inférieur gauche de l’écran.
1. Examinez la sortie pour vous assurer que le scénario s’est exécuté comme prévu.
1. Lorsque vous êtes satisfait que le scénario fonctionne comme prévu, cliquez sur le bouton **Planification** basculez le curseur dans le coin inférieur gauche de l’écran sur **Activé**.

   Cela active le scénario. Les scénarios actifs s’exécutent selon le planning défini dans le module de déclenchement.
1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** près du coin inférieur gauche pour enregistrer la progression sur le scénario.

   >[!IMPORTANT]
   >
   >Enregistrez souvent lorsque vous affinez et testez un scénario.

## Ressources :

* [Mise en correspondance des éléments à l’aide de fonctions dans [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
