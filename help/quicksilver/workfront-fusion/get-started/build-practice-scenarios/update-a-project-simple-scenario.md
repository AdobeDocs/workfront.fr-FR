---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Ajout d’un module de déclenchement à un scénario de base
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: f4588063-024f-4520-986e-45342a6b6777
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 3%

---

# Utilisation d’une fonction pour mettre à jour un projet dans un scénario simple dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Utiliser une fonction pour mettre à jour un projet dans un scénario de base](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/use-function-to-build-practice-scenario.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

La mise à jour d’un élément de travail Workfront est un cas d’utilisation courant pour Workfront Fusion. Dans cet exemple, vous allez utiliser une fonction pour modifier le nom d’un projet en majuscules.

Fusion comprend de nombreux types de fonctions qui vous permettent de transformer et d’exécuter une logique conditionnelle sur vos données. Pour plus d’informations sur l’utilisation des fonctions, voir [Mappage des informations d’un module à un autre dans Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

Cet exemple montre comment modifier le scénario créé dans [Créer un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Conditions préalables

Vous devez créer le scénario décrit dans [Créer un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) avant de suivre cette procédure.

## Utiliser une fonction pour mettre à jour un projet

### Ajoutez le module Mettre à jour l’enregistrement à votre scénario

1. Ouvrez le scénario dans l’éditeur de scénarios.
1. Pointez sur le cercle partiel à droite du du module, puis cliquez sur **[!UICONTROL Ajouter un autre module]**.
1. Sélectionnez [!DNL Adobe Workfront] dans la liste des applications, puis choisissez le module **[!UICONTROL Mettre à jour l&#39;enregistrement]**.
1. dans le champ ID , sélectionnez le bloc d’ID situé sous le module Convertir l’objet . Il s’agit de l’identifiant du projet qui a été généré par ce module.

   ![ID de l’objet Convert](assets/id-convert-object.png)

1. Dans le champ Type d’enregistrement , sélectionnez Projet, car l’objet à mettre à jour est un projet.
1. Dans la zone Sélectionner les champs à mapper, sélectionnez Nom.

   Un champ Nom s’ouvre.

### Mappez la fonction pour la mise à jour du nom.

Lorsque ce scénario convertit une demande en projet, le nom du projet est identique à celui de la demande. La fonction ici prend ce nom et met en majuscule toutes les lettres qu&#39;il contient.

1. Cliquez sur le champ **Nom**.

   Le panneau de mappage s’ouvre.
1. Dans le panneau de mappage, cliquez sur l’icône **Texte et fonctions binaires**. ![Icône Fonctions de texte](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Sélectionnez la fonction **upper**.

   La fonction apparaît dans le champ Nom, y compris la mise en forme de l’entrée attendue.

   L’entrée de cet exemple est le nom de l’événement à partir duquel le projet a été converti.

1. Déplacez le curseur entre les parenthèses, car c&#39;est là que va se trouver l&#39;entrée.
1. Dans le panneau de mappage, cliquez sur l’icône **sortie du module**. ![ Icône de sortie du module ](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Sélectionnez le bloc de nom qui a été généré par votre premier module.

   Le bloc de nom apparaît dans la fonction .

   ![Bloc de nom dans la fonction](assets/map-name.png)

1. Cliquez sur OK pour enregistrer les paramètres du module.

### Tester et activer

1. Testez le scénario en cliquant sur **Exécuter une fois** dans le coin inférieur gauche de l’écran.
1. Examinez la sortie pour vous assurer que le scénario s’est exécuté comme prévu.
1. Lorsque vous êtes convaincu que le scénario fonctionne comme prévu, cliquez sur le bouton (bascule) **Planification** dans le coin inférieur gauche de l’écran pour **Activé**.

   Le scénario est alors activé. Les scénarios actifs s’exécutent selon le planning défini dans le module de déclenchement.
1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** près du coin inférieur gauche pour enregistrer votre progression dans le scénario.

   >[!IMPORTANT]
   >
   >Sauvegardez souvent lorsque vous affinez et testez un scénario.

## Ressources :

* [Mapper des éléments à l’aide de fonctions dans  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
