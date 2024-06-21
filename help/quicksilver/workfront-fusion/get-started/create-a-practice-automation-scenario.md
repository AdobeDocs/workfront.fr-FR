---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Créer un scénario d’automatisation de test dans [!DNL Adobe Workfront Fusion]
description: Cet article décrit comment créer un scénario d’automatisation avec Adobe Workfront Fusion. Les scénarios d’automatisation automatisent les processus Workfront, notamment la manipulation et la transformation des données. Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche un projet, puis renvoie toutes les tâches associées à ce projet.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 97231a6021aa4e897059063293e649f45dc9908d
workflow-type: tm+mt
source-wordcount: '1842'
ht-degree: 99%

---

# Créer un scénario d’automatisation de test dans [!DNL Adobe Workfront Fusion]

Cet article décrit comment créer un scénario d’automatisation avec Adobe Workfront Fusion. Les scénarios d’automatisation automatisent les processus Workfront, notamment la manipulation et la transformation des données. Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche un projet, puis renvoie toutes les tâches associées à ce projet.

Pour plus d’informations sur la création d’un scénario d’intégration qui connecte des applications distinctes, consultez la section [Créer un scénario d’intégration de test dans Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

Pour plus d’informations sur les fonctionnalités disponibles pour chaque licence Workfront Fusion, consultez la section [Licences Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Créer un scénario de test

[!DNL Adobe Workfront Fusion] vise à automatiser vos processus afin que vous puissiez vous concentrer sur de nouvelles tâches, plutôt que de répéter les mêmes tâches encore et encore. L’application fonctionne en reliant les actions au sein et entre les applications et les services, pour créer un scénario qui transfère et transforme vos données automatiquement. Le scénario que vous créez recherche les données dans une application ou un service et traite ces données pour obtenir le résultat souhaité.

Un scénario se compose d’une série de modules qui indiquent comment les données doivent être transformées dans une application ou transférées entre les applications et les services web.
Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche un projet [!DNL Workfront] et renvoie les tâches du projet.

![](assets/create-practice-scenario-wf-only-350x157.png)

La création d’un scénario se compose de plusieurs tâches principales :

## Choisir les applications et nommer le scénario

1. Connectez-vous à votre compte [!DNL Workfront Fusion].
1. Cliquez sur **[!UICONTROL Scénarios]** ![](assets/scenarios-icon.png) dans le panneau de gauche.

   >[!NOTE]
   >
   >Si le panneau de navigation de gauche ou ses icônes ne s’affichent pas, cliquez sur l’icône de menu ![Menu](assets/main-menu-icon-left-nav.png).

   Dans le panneau gris [!UICONTROL Dossiers] qui s’affiche, vous pouvez organiser vos scénarios en dossiers.

   En haut de la zone principale à droite, vous pouvez afficher **[!UICONTROL Tous]** les scénarios que vous avez créés, les **[!UICONTROL Scénarios actifs]**, les **[!UICONTROL Scénarios inactifs]** et les **[!UICONTROL Concepts]**. Les concepts sont des scénarios qui nécessitent un peu plus de travail avant que [!DNL Workfront Fusion] puisse les classer comme actifs ou inactifs.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. Dans le panneau [!UICONTROL Dossiers], cliquez sur l’icône **[!UICONTROL Ajouter un dossier]** ![](assets/add-folder-icon.png), puis saisissez un nom tel que « Scénarios de test » pour votre premier dossier.

1. Ouvrez le dossier, puis cliquez sur **[!UICONTROL Créer un scénario]** dans le coin supérieur droit de la page.

   La page de destination qui s’affiche vous permet de précharger toutes les applications que vous souhaitez utiliser dans le scénario que vous allez créer.

1. Pour cet exercice, recherchez et sélectionnez l’application **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Continuer]** dans le coin supérieur droit.

   L’éditeur de scénario s’affiche avec un module vide au centre, l’application [!DNL Workfront] que vous avez préchargée et certaines options dans la barre d’outils en bas.

<!--
   ![](assets/scenario-editor-350x235.png)
-->

Lorsque vous créez un scénario, il est préférable de commencer par lui donner un nom.

1. Sélectionnez le nom de l’espace réservé **[!UICONTROL Nouveau scénario]** dans le coin supérieur gauche, puis saisissez un nom tel que « Scénario de test 1 ».
1. Passez à l’étape [Ajouter et configurer le premier module](#add-and-configure-the-first-module) ci-dessous.

## Ajouter et configurer le premier module

Le module vide avec un point d’interrogation représente le module de déclenchement que vous devez ajouter. Ce module démarre le scénario à chaque exécution. L’icône d’horloge sur le module vide indique qu’il s’agit d’un module planifié.

![](assets/empty-module.png)

Ce module contient les données que le scénario doit surveiller.

Pour cet exemple, nous n’utilisons pas de module de déclenchement. Ce scénario commence par une recherche.

1. Cliquez sur le module vide pour choisir l’application à partir de laquelle vous allez sélectionner un module.

   L’application que vous avez préchargée précédemment s’affiche en regard du module vide. Vous pouvez ajouter toute autre application qui comporte des modules dans la zone [!UICONTROL Rechercher].

   ![](assets/pre-loaded-app-wf-350x172.png)

1. Cliquez sur **[!DNL Workfront]**.

   La liste affiche alors tous les modules [!DNL Workfront] que vous pouvez utiliser comme module déclencheur.

1. Cliquez sur le module de recherche **[!UICONTROL Rechercher]**.

   Vous devez maintenant établir une connexion authentifiée à votre compte [!DNL Workfront]. Chaque module que vous ajoutez à un scénario doit avoir une connexion avec son application.

1. Dans la zone **[!DNL Workfront]** sous **[!UICONTROL Connexion]**, cliquez sur **[!UICONTROL Ajouter]**, puis donnez un nom à la connexion, par exemple « Compte Workfront d’Olivia », puis cliquez sur **[!UICONTROL Continuer]**.
1. Authentifiez la connexion dans la fenêtre qui s’affiche.

   Le processus d’authentification d’une connexion peut varier légèrement d’une application à l’autre. Le processus suivant est spécifique à [!DNL Workfront], mais le processus est similaire à de nombreuses applications.

   1. Saisissez votre domaine [!DNL Workfront], puis cliquez sur **[!UICONTROL Continuer]**.
   1. Connectez-vous à [!DNL Workfront].
   1. Examiner la demande d’accès de [!DNL Workfront Fusion], puis cliquez sur **[!UICONTROL Autoriser l’accès]**.

   Si vous avez besoin d’aide, voir [Présentation des connexions](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configurer le premier module

Après la connexion de [!DNL Workfront Fusion] à votre compte [!DNL Workfront], vous pouvez définir une file d’attente des demandes [!DNL Workfront] à laquelle vous avez accès et les données que vous souhaitez que le premier module traite.

1. Dans la zone [!UICONTROL Type d’enregistrement], sélectionnez **[!UICONTROL Projet]**. Le module est ainsi configuré pour rechercher uniquement les projets.

   >[!TIP]
   >
   >Vous trouverez **[!UICONTROL Projet]** dans la liste si vous commencez à saisir le mot « [!UICONTROL projet] ».

1. Dans la zone **[!UICONTROL Jeu de résultats]**, sélectionnez **[!UICONTROL Premier enregistrement correspondant]**. Cette option permet au module de ne renvoyer que le premier enregistrement qui répond aux critères. Dans cet exemple, un seul enregistrement est renvoyé.
1. Dans la zone **[!UICONTROL Critères de recherche]**, configurez un filtre pour renvoyer le projet spécifique.

   1. Dans la première zone sous [!UICONTROL Critères de recherche], sélectionnez le champ dont vous souhaitez rechercher les valeurs. Pour cet exemple, sélectionnez **[!UICONTROL Nom]**.
   1. Pour l’opérateur, sélectionnez [!UICONTROL Contient (non-respect de la casse)]. Cela permet au module de rechercher des projets dont le nom contient les mots de votre choix, même si vous ne saisissez pas l’intégralité du nom, ou si vous saisissez le nom avec une casse incorrecte (toutes les majuscules, par exemple).
   1. Dans le dernier champ sous [!UICONTROL Critères de recherche], saisissez un mot ou une expression qui se trouve dans le nom du projet que vous recherchez.

1. Dans la liste **[!UICONTROL Sorties]**, sélectionnez les champs que le module doit générer. Pour cet exemple, sélectionnez les champs **[!UICONTROL ID]** et **[!UICONTROL Nom]**.

   >[!TIP]
   >
   >Utilisez les raccourcis clavier **Cmd+F** ([!DNL Mac]OS) ou **Ctrl+F** (système d’exploitation [!DNL Windows]) pour trouver rapidement un champ.

1. Cliquez sur **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >(À titre d’informations uniquement) Puisqu’il ne s’agit pas d’un module de déclenchement, vous ne choisissez pas le point de départ. Lors de l’utilisation d’un module de déclenchement, vous devez maintenant sélectionner le point de départ.
   >
   >
   >Pour plus d’informations, consultez la section [Choisir le point de départ d’un module de déclenchement dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Cliquez avec le bouton droit sur le module, sélectionnez **[!UICONTROL Renommer]**, puis saisissez un nom décrivant l’objectif du module (par exemple « Rechercher un projet ») et cliquez sur **[!UICONTROL OK]**.

   Le nom apparaît juste en dessous du module. En dessous du nom, [!DNL Workfront Fusion] présente une brève description du type d’action effectuée par le module.

   ![](assets/module-renamed-wf.png)

1. Passez à l’étape [Ajouter et configurer le deuxième module](#add-and-configure-the-second-module).

## Ajouter et configurer le deuxième module

1. Cliquez sur le cercle partiel à droite du du module pour **[!UICONTROL Ajouter un autre module]**.
1. Sélectionnez [!DNL Workfront] dans la liste des applications, puis choisissez le module de recherche **[!UICONTROL Lire les enregistrements associés]**.
1. Vous avez déjà créé une connexion à [!DNL Workfront] pour le module précédent. Vous n’avez pas besoin de le recréer ici, mais vous devez vous assurer que ce module utilise la même connexion que le module précédent.\
   Dans la zone **[!UICONTROL Connexion]**, sélectionnez la connexion que vous avez créée pour le module précédent.
1. Cliquez sur **[!UICONTROL Type d’enregistrement]**, puis sélectionnez **[!UICONTROL Projet]** pour lire les enregistrements liés à un projet.

   >[!TIP]
   >
   >Commencez à saisir le mot « projet » pour trouver **[!UICONTROL Projet]** dans la liste.

1. Cliquez sur le champ **[!UICONTROL ID d’enregistrement parent]**. Ce champ nécessite l’ID Workfront du projet pour lequel vous souhaitez obtenir les tâches.

   Cliquez sur le champ pour ouvrir la liste des variables que vous pouvez utiliser dans le champ **[!UICONTROL ID d’enregistrement parent]** pour identifier le projet dans Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Clic sur la variable **[!UICONTROL ID]** pour l’ajouter au champ **[!UICONTROL ID d’enregistrement parent]**. Cela permet d’utiliser l’ID renvoyé par le premier module comme identifiant du projet avec lequel vous souhaitez travailler dans le deuxième module, ce qui garantit que les tâches renvoyées appartiendront à ce projet.
1. Dans le champ **[!UICONTROL Collections]**, sélectionnez **[!UICONTROL Tâche]**. Cela indique que le module doit renvoyer les tâches associées au projet sélectionné.
1. Cliquez sur **[!UICONTROL OK]**.

   Vous disposez maintenant d’un scénario de travail.

1. Donnez un nom au deuxième module, par exemple « Obtention des tâches associées au projet », puis passez à l’étape [Tester le scénario](#test-the-scenario).

## Tester le scénario

Avant d’activer votre scénario, il est important de le tester en l’exécutant au moins une fois et en consultant les résultats. Vous pouvez ainsi comprendre le flux des données dans le scénario et rechercher les erreurs.

Nous avons choisi de renvoyer un projet et ses tâches associées. Exécutons le scénario et jugeons de son efficacité.

1. Cliquez sur **[!UICONTROL Exécuter une seule fois]** dans le coin inférieur gauche de l’éditeur de scénario.
1. Une fois le scénario en cours d’exécution, cliquez sur la bulle au-dessus du premier module.

   ![](assets/click-bubble.png)

   Dans la zone qui s’affiche, vous pouvez afficher des informations sur le lot de données traité par le module, y compris les données réelles qui ont été extraites du projet que le module a renvoyé.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Cliquez sur la bulle Inspecteur d’exécution au-dessus du deuxième module pour voir l’entrée des informations et la sortie, qui est un ensemble de tâches contenues dans le projet.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Pour en savoir plus sur la lecture des informations d’exécution de scénario, consultez les articles suivants :

   * Pour obtenir des informations générales, voir [Flux d’exécution du scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Pour plus d’informations sur les lots traités, voir [Exécution, cycles et phases d’un scénario [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** ![](assets/save-icon.png) près du coin inférieur gauche pour enregistrer votre progression dans le scénario.

   >[!IMPORTANT]
   >
   >Enregistrez à intervalles réguliers lorsque vous affinez et testez un scénario.

>[!TIP]
>
>Nous recommandons d’ajouter des notes sur chaque module pour indiquer ses objectifs.
>
>1. Cliquez avec le bouton droit sur un module [!DNL Workfront], puis cliquez sur **[!UICONTROL Ajouter une note]**.
>1. Dans la note qui s’affiche, saisissez une description générale du module.
>
>    Vous pouvez ajouter plusieurs notes pour un module.
>
>1. Fermez la zone **[!UICONTROL Remarques]**.
>
>     Après avoir ajouté une note à un scénario, un point orange s’affiche sur l’icône **[!UICONTROL Remarques]** ![](assets/notes-icon-w-dot.png) au bas de l’éditeur de scénario.
>
>1. Cliquez sur l’icône **[!UICONTROL Remarques]** ![](assets/notes-icon-w-dot.png) pour afficher vos notes.
>



## Activer le scénario

Cet exemple de scénario ne comporte pas de module de déclenchement. Si s’agissait d’un scénario que vous utiliseriez pour des données réelles, il commencerait avec un module de déclenchement, et la dernière chose que vous feriez est de l’activer. Une fois que vous avez activé un scénario, celui-ci s’exécute par défaut toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant le moment et la fréquence d’exécution.

Pour plus d’informations sur l’activation de scénarios, voir [Activer ou désactiver un scénario dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Pour plus d’informations sur les plannings, voir [Planifier un scénario dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
