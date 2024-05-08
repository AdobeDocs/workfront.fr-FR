---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Ajouter un filtre à un scénario de base
description: Les filtres vous permettent de vous assurer que votre scénario avance uniquement si certaines conditions sont remplies.
author: Becky
feature: Workfront Fusion
source-git-commit: 5ba5b2e37e2ce58d96d11f24786feef57f8eb638
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Ajoutez un filtre à un scénario de base dans [!DNL Adobe Workfront Fusion]

Les filtres vous permettent de vous assurer que votre scénario avance uniquement si certaines conditions sont remplies.

Dans cet exemple, vous allez ajouter à votre scénario un filtre qui permet de créer un projet à partir d’une requête uniquement si la requête a été envoyée à une file d’attente de requêtes spécifique.

Cet exemple modifie le scénario créé dans [Création d’un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Les modules de déclencheur Workfront incluent des filtres qui permettent à un scénario de démarrer uniquement si certaines conditions sont remplies. Cependant, comme les filtres entre modules sont utilisés pour chaque cas d’utilisation non déclencheur et non Workfront, il est important d’apprendre à utiliser les filtres entre les modules. Cet exemple utilise un filtre entre modules pour les fonctionnalités qui peuvent être configurées avec un filtre interne au module.

## Conditions préalables

Vous devez créer le scénario décrit dans la section [Création d’un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) avant de suivre cette procédure.

## Ajouter un filtre

### Préparation à l’ajout du filtre

1. Ouvrez le premier scénario.
1. Dans le **Sorties** zone, sélectionnez `Project`.
Vous devriez maintenant avoir `ID`, `Name`, et `Project` sélectionné.
1. Cliquez sur OK pour enregistrer les paramètres du module.
1. Ouvrez Workfront.
1. Dans Workfront, localisez le projet qui représente la file d’attente des demandes avec laquelle le scénario Fusion fonctionnera.

   Ce projet doit se trouver dans le même compte Workfront pour lequel la connexion Fusion est configurée.

1. Notez l’ID de projet dans l’URL.

   Exemple : https://\&lt;mydomain>.my.workfront.com/project/\&lt;projectid>/tasks

### Ajouter et configurer le filtre

1. Ouvrez le scénario dans l’éditeur de scénarios.
1. Cliquez sur l’icône de clé à molette ![Icône Forme](assets/wrench-icon.png) entre le premier et le deuxième module, puis sélectionnez **Configurer un filtre**.
1. Dans le champ Libellé , saisissez un libellé pour ce filtre, par exemple &quot;Filtrer la file d’attente des demandes&quot;.
1. Dans le **Condition** , dans le champ supérieur, faites correspondre la variable `projectID` du premier module.

   ![Mappage de l’ID de projet](assets/map-proj-id.png)
1. Laissez le champ **Condition** comme égal à.
1. Dans le champ inférieur du **Condition** , collez dans l’ID de projet que vous avez pris note de l’URL du projet dans [Préparation à l’ajout du filtre](#prepare-to-add-the-filter).
1. Cliquez sur **OK** pour enregistrer les paramètres de filtre.

### Tester et activer

1. Accédez à l’environnement Workfront auquel Fusion se connecte et ajoutez un problème au projet que vous avez spécifié dans le filtre. Ajoutez un autre problème à un autre projet.
1. Cliquez sur **[!UICONTROL Exécuter une seule fois]** dans le coin inférieur gauche de l’éditeur de scénarios.
1. Examinez la sortie pour vous assurer que le scénario s’est exécuté comme prévu.

   Les deux problèmes doivent apparaître dans la sortie du premier scénario, mais seul le problème du projet spécifié doit apparaître comme entrée dans le second scénario,
1. Lorsque vous êtes satisfait que le scénario fonctionne comme prévu, cliquez sur le bouton **Planification** basculez le curseur dans le coin inférieur gauche de l’écran sur **Activé**.

   Cela active le scénario.
1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** près du coin inférieur gauche pour enregistrer la progression sur le scénario.

   >[!IMPORTANT]
   >
   >Enregistrez souvent lorsque vous affinez et testez un scénario.

## Ressources

* Pour plus d’informations sur les filtres, voir [Ajout d’un filtre à un scénario](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

