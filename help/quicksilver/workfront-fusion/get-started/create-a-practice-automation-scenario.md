---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Créez un scénario d’automatisation des pratiques dans [!DNL Adobe Workfront Fusion]
description: Cet article décrit comment créer un scénario d’automatisation avec Adobe Workfront Fusion. Les scénarios d’automatisation automatisent les processus Workfront, notamment la manipulation et la transformation des données. Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche un projet, puis renvoie toutes les tâches associées à ce projet.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1782'
ht-degree: 0%

---

# Créez un scénario d’automatisation des pratiques dans [!DNL Adobe Workfront Fusion]

Cet article décrit comment créer un scénario d’automatisation avec Adobe Workfront Fusion. Les scénarios d’automatisation automatisent les processus Workfront, notamment la manipulation et la transformation des données. Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche un projet, puis renvoie toutes les tâches associées à ce projet.

Pour plus d’informations sur la création d’un scénario d’intégration qui connecte des applications distinctes, voir [Création d’un scénario d’intégration d’une pratique dans Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

Pour plus d’informations sur les fonctionnalités disponibles avec chaque licence Workfront Fusion, voir [Licences Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p><p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>
Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Création d’un scénario d’entraînement

Le rôle de [!DNL Adobe Workfront Fusion] est d’automatiser vos processus afin que vous puissiez vous concentrer sur de nouvelles tâches plutôt que de répéter les mêmes tâches encore et encore. Il fonctionne en liant les actions dans et entre les applications et les services pour créer un scénario qui transfère et transforme vos données automatiquement. Le scénario que vous créez recherche les données dans une application ou un service et traite ces données pour obtenir le résultat souhaité.

Un scénario comprend une série de modules qui indiquent comment les données doivent être transformées dans une application ou transférées entre les applications et les services web.
Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche une [!DNL Workfront] et renvoie les tâches du projet.

![](assets/create-practice-scenario-wf-only-350x157.png)

La création d&#39;un scénario se compose de plusieurs tâches principales :

## Sélectionnez les applications et attribuez un nom au scénario.

1. Connectez-vous à [!DNL Workfront Fusion] compte .
1. Cliquez sur **[!UICONTROL Scénarios]** ![](assets/scenarios-icon.png) dans le panneau de gauche.

   Dans le panneau de gauche qui s’affiche, vous pouvez organiser vos scénarios en dossiers.

   En haut de la zone principale à droite, vous pouvez afficher **[!UICONTROL Tous]** les scénarios que vous avez créés, vos **[!UICONTROL Scénarios principaux]**, **[!UICONTROL Scénarios inactifs]**, et **[!UICONTROL Concepts]**. Les concepts sont des scénarios qui nécessitent un peu plus de travail avant [!DNL Workfront Fusion] peuvent les classer comme principal ou inactif.

   ![](assets/scenarios-left-panel-350x215.png)

1. Dans le panneau de gauche, cliquez sur le **[!UICONTROL Ajouter un dossier]** icon ![](assets/add-folder-icon.png), puis saisissez un nom tel que &quot;Scénarios d’entraînement&quot; pour votre premier dossier.

1. Ouvrez le dossier, puis cliquez sur **[!UICONTROL Création d’un scénario]** dans le coin supérieur droit de la page.

   La landing page qui s’affiche vous permet de précharger toutes les applications que vous souhaitez utiliser dans le scénario que vous allez créer.

1. Pour cet exercice, recherchez et sélectionnez le **[!DNL Workfront]** application.
1. Cliquez sur **[!UICONTROL Continuer]** dans le coin supérieur droit.

   L’éditeur de scénario s’affiche, contenant un module vide au centre, le [!DNL Workfront] vous avez pré-chargé l’application et certaines options de la barre d’outils située en bas.

   ![](assets/scenario-editor-350x235.png)

   Lorsque vous commencez à créer un scénario, il est préférable de commencer par en créer un nom.

1. Sélectionnez la **[!UICONTROL Nouveau scénario]** nom de l’espace réservé dans le coin supérieur gauche, puis saisissez un nom tel que &quot;Scénario pratique 1&quot;.
1. Passez à la [Ajouter et configurer le premier module](#add-and-configure-the-first-module) ci-dessous.

## Ajouter et configurer le premier module

Le module vide avec un point d’interrogation représente le module de déclenchement que vous devez ajouter. Ce module démarre le scénario chaque fois qu’il s’exécute. L’icône de l’horloge sur le module vide indique qu’il s’agit d’un module planifié.

![](assets/empty-module.png)

Ce module contient les données que vous souhaitez que le scénario recherche.

Pour cet exemple, nous n’utilisons pas de module de déclenchement. Ce scénario commence par une recherche.

1. Cliquez sur le module vide pour choisir l’application à partir de laquelle vous allez sélectionner un module.

   L’application que vous avez préchargée précédemment s’affiche en regard du module vide. Vous pouvez ajouter toute autre application qui comporte des modules à l’aide de la variable [!UICONTROL Rechercher] de la boîte.

   ![](assets/pre-loaded-app-wf-350x172.png)

1. Cliquez sur **[!DNL Workfront]**.

   La liste change pour afficher toutes les [!DNL Workfront] modules que vous pouvez utiliser comme module déclencheur.

1. Cliquez sur le module Rechercher . **[!UICONTROL Rechercher]**.

   Vous devez maintenant établir une connexion authentifiée à votre [!DNL Workfront] compte . Chaque module que vous ajoutez à un scénario doit avoir une connexion à son application.

1. Dans le **[!DNL Workfront]** sous **[!UICONTROL Connexion]**, cliquez sur **[!UICONTROL Ajouter]**, puis saisissez un nom pour la connexion, par exemple &quot;Compte Workfront d’Olivia&quot;, puis cliquez sur **[!UICONTROL Continuer]**.
1. Authentifiez la connexion dans la fenêtre qui s’affiche.

   Le processus d’authentification d’une connexion peut varier légèrement d’une application à l’autre. Le processus suivant est spécifique à [!DNL Workfront], mais le processus est similaire à de nombreuses applications.

   1. Saisissez votre [!DNL Workfront] domain, puis cliquez sur **[!UICONTROL Continuer]**.
   1. Se connecter [!DNL Workfront].
   1. Examiner l’accès qui [!DNL Workfront Fusion] demande, puis cliquez sur **[!UICONTROL Autoriser l’accès]**.

   Si vous avez besoin d’aide, voir [A propos de la connexion [!DNL Adobe Workfront Fusion] vers une application ou un service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configuration du premier module

Après la connexion [!DNL Workfront Fusion] à [!DNL Workfront] vous pouvez définir un [!DNL Workfront] la file d’attente des demandes à laquelle vous avez accès et les données que vous souhaitez que le premier module soit traité.

1. Dans le [!UICONTROL Type d’enregistrement] , sélectionnez **[!UICONTROL Projet]**. Le module est ainsi configuré pour rechercher uniquement les projets.

   >[!TIP]
   >
   >Vous pouvez trouver **[!UICONTROL Projet]** dans la liste si vous commencez à saisir le mot &quot;[!UICONTROL project].&quot;

1. Dans le **[!UICONTROL Jeu de résultats]** , sélectionnez **[!UICONTROL Premier enregistrement correspondant]**. Cela définit le module pour renvoyer uniquement le premier enregistrement qui répond aux critères. Pour cet exemple, un seul enregistrement est renvoyé.
1. Dans le **[!UICONTROL Critères de recherche]** , nous allons configurer un filtre pour renvoyer le projet spécifique.

   1. Dans la première zone sous [!UICONTROL Critères de recherche], sélectionnez le champ dont vous souhaitez rechercher les valeurs. Pour cet exemple, sélectionnez **[!UICONTROL Nom]**.
   1. Pour l’opérateur, sélectionnez [!UICONTROL Contient (non-respect de la casse)]. Cela permet au module de rechercher des projets dont le nom contient les mots de votre choix, même si vous ne saisissez pas l’intégralité du nom, ou si vous saisissez le nom avec une casse incorrecte (toutes les majuscules, par exemple).
   1. Dans le dernier champ sous [!UICONTROL Critères de recherche], saisissez un mot ou une expression que vous savez trouver dans le nom du projet que vous recherchez.

1. Dans le **[!UICONTROL Sorties]** sélectionnez les champs que vous souhaitez que le problème génère. Dans cet exemple, sélectionnez l’option **[!UICONTROL ID]** et **[!UICONTROL Nom]** champs.

   >[!TIP]
   >
   >Vous pouvez utiliser **Cmd+F** ([!DNL Mac] OS) ou **Ctrl+F** ([!DNL Windows] Système d’exploitation) pour trouver rapidement un champ.

1. Cliquez sur **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >(Informations uniquement) Puisqu’il ne s’agit pas d’un module de déclenchement, vous ne choisissez pas où le démarrer. Lors de l’utilisation d’un module de déclenchement, vous devez maintenant sélectionner l’emplacement où le démarrer.
   >
   >
   >Pour plus d’informations, voir [Sélectionnez l’endroit où commence un module de déclenchement dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Cliquez avec le bouton droit sur le module, puis cliquez sur **[!UICONTROL Renommer]**, puis saisissez un nom qui décrit ce que le module doit faire (par exemple &quot;Rechercher un projet&quot;), puis cliquez sur **[!UICONTROL OK]**.

   Le nom apparaît juste en dessous du module. En dessous : [!DNL Workfront Fusion] inclut une brève description du type d’action effectuée par le module.

   ![](assets/module-renamed-wf.png)

1. Passez à la [Ajouter et configurer le deuxième module](#add-and-configure-the-second-module).

## Ajouter et configurer le deuxième module

1. Cliquez sur le cercle partiel à droite du du module pour **[!UICONTROL Ajouter un autre module]**.
1. Sélectionner [!DNL Workfront] dans la liste des applications, puis choisissez le module de recherche **[!UICONTROL Lire les enregistrements associés]**.
1. Vous avez déjà créé une connexion à [!DNL Workfront] pour le module précédent. Vous n’avez pas besoin de le recréer ici, mais vous devez vous assurer que ce module utilise la même connexion que le module précédent.\
   Dans le **[!UICONTROL Connexion]** , sélectionnez la connexion que vous avez créée pour le module précédent.
1. Cliquez sur **[!UICONTROL Type d’enregistrement]**, puis sélectionnez **[!UICONTROL Projet]**, car nous voulons lire les enregistrements liés à un projet.

   >[!TIP]
   >
   >Vous pouvez trouver **[!UICONTROL Projet]** dans la liste si vous commencez à saisir le mot &quot;projet&quot;.

1. Cliquez sur le bouton **[!UICONTROL ID d’enregistrement parent]** champ . Ce champ nécessite l’identifiant Workfront du projet à partir duquel vous souhaitez renvoyer des tâches.

   Cliquez sur le champ pour ouvrir la liste des variables que vous pouvez utiliser dans la variable **[!UICONTROL ID d’enregistrement parent]** pour identifier le projet dans Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Clic sur la variable **[!UICONTROL ID]** pour l’ajouter au **[!UICONTROL ID d’enregistrement parent]** champ . Cela permet d’utiliser l’identifiant renvoyé par le premier module comme identifiant du projet avec lequel vous souhaitez travailler dans le deuxième module, ce qui garantit que les tâches renvoyées appartiendront à ce projet.
1. Dans le **[!UICONTROL Collections]** champ, sélectionnez **[!UICONTROL Tâches]**. Cela indique que le module doit renvoyer les tâches associées au projet sélectionné.
1. Cliquez sur **[!UICONTROL OK]**

   Maintenant, vous avez un scénario de travail.

1. Donnez un nom au deuxième module, par exemple &quot;Tâches de retour associées au projet&quot;, puis continuez avec [Test du scénario](#test-the-scenario).

## Test du scénario

Avant d’activer votre scénario, il est important de le tester en l’exécutant au moins une fois et en affichant les résultats. Vous pouvez ainsi comprendre le flux des données dans le scénario et rechercher les erreurs.

Nous avons choisi de renvoyer 1 projet, ainsi que les tâches associées à ce projet. Si vous exécutez le scénario, c’est ce qui devrait se produire.

1. Cliquez sur **[!UICONTROL Exécuter une seule fois]** dans le coin inférieur gauche de l’éditeur de scénarios.
1. Une fois le scénario en cours d’exécution, cliquez sur la bulle au-dessus du premier module.

   ![](assets/click-bubble.png)

   Dans la zone qui s’affiche, vous pouvez afficher des informations sur le lot de données traité par le module, y compris les données réelles qui ont été extraites du projet que le module a renvoyé.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Cliquez sur la bulle Inspecteur d’exécution au-dessus du deuxième module pour voir la saisie des informations et la sortie, qui est un ensemble de tâches contenues dans le projet.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Vous pouvez en savoir plus sur la lecture des informations d’exécution de scénario dans les articles suivants :

   * Pour obtenir des informations générales, voir [Flux d’exécution du scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Pour plus d’informations sur les lots traités, voir [Exécution de scénarios, cycles et phases dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** ![](assets/save-icon.png) près du coin inférieur gauche pour enregistrer la progression sur le scénario.

   >[!IMPORTANT]
   >
   >Enregistrez souvent lorsque vous affinez et testez un scénario.

>[!TIP]
>
>Nous recommandons la pratique facultative mais utile d’ajouter des notes sur chaque module.
>
>1. Cliquez avec le bouton droit de la souris sur un [!DNL Workfront] module, puis cliquez sur **[!UICONTROL Ajouter une note]**.
>1. Dans la note qui s’affiche, saisissez un aperçu du module.

>
>   Vous pouvez ajouter plusieurs notes pour un module.
>
>1. Fermez la **[!UICONTROL Remarques]** zone.
>
>   Une fois que vous avez ajouté une note à un scénario, un point orange s’affiche sur la page **[!UICONTROL Remarques]** icon ![](assets/notes-icon-w-dot.png) au bas de l’éditeur de scénario.
>
>1. Cliquez sur le bouton **[!UICONTROL Remarques]** icon ![](assets/notes-icon-w-dot.png) pour afficher vos notes.

>




## Activation du scénario

Cet exemple de scénario ne comporte pas de module de déclenchement. Si c’était un scénario que vous utiliseriez pour des données réelles, il commencerait avec un module de déclenchement, et la dernière chose que vous feriez est de l’activer. Une fois que vous avez activé un scénario, celui-ci s’exécute par défaut toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant quand et à quelle fréquence il doit s’exécuter.

Pour plus d’informations sur l’activation de scénarios, voir [Activez ou désactivez un scénario dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Pour plus d’informations sur les plannings, voir [Planification d’un scénario dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
