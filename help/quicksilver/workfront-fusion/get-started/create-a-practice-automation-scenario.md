---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Créer un scénario d’automatisation de test dans [!DNL Adobe Workfront Fusion]
description: Cet article décrit comment créer un scénario d’automatisation avec Adobe Workfront Fusion. Les scénarios d’automatisation automatisent les processus Workfront, notamment la manipulation et la transformation des données. Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche un projet, puis renvoie toutes les tâches associées à ce projet.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 8769ed5844e340e007f844370791e93393696819
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 71%

---

# Créer un scénario d’automatisation de test dans [!DNL Adobe Workfront Fusion]

Les scénarios d’automatisation automatisent les processus Workfront, notamment la manipulation et la transformation des données. Cet article vous guide tout au long du processus de création d’un scénario qui recherche un projet, puis renvoie toutes les tâches associées au projet.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Forfait Adobe Workfront</td>  
      <td>N’importe quelle</td>  
    </tr>  
    <tr>  
      <td>Licence Adobe Workfront</td>  
      <td>
        Nouveau : Standard<br>
        Ou<br>
        Actuel : travail ou plus élevé
      </td>  
    </tr>  
    <tr>  
      <td>Licence Adobe Workfront Fusion</td>  
      <td> 
        Actuel : aucune exigence de licence Workfront Fusion.<br>
        Ou<br>
        Hérité : Tout
      </td>  
    </tr>  
    <tr>  
      <td>Produit</td>  
      <td> 
        Nouveau : sélectionnez ou forfait Workfront Prime : votre entreprise doit acheter Adobe Workfront Fusion.<br>
        Formule Workfront ultime : Workfront Fusion est incluse.<br>
        Ou<br>
        Actuel : votre entreprise doit acheter Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Création d’un scénario de pratique d’automatisation

[!DNL Adobe Workfront Fusion] vous aide à vous concentrer sur des tâches importantes en automatisant les tâches répétitives. Il crée des scénarios qui gèrent automatiquement vos données dans différents services et applications.

Chaque scénario se compose de modules, qui déterminent la manière dont les données sont traitées dans une application ou transférées entre différentes applications et services. Par exemple, vous pouvez créer un scénario dans Fusion pour trouver automatiquement un projet [!DNL Workfront] et répertorier ses tâches. De cette façon, Fusion vous permet de gagner du temps et de l&#39;effort en gérant les tâches de routine.

Ce scénario de pratique vous guide tout au long du processus de création d’un scénario qui recherche un projet [!DNL Workfront] et renvoie les tâches du projet.

![](assets/create-practice-scenario-wf-only-350x157.png)

### Avant de commencer

Créez un projet avec des tâches dans le front de travail que vous pouvez utiliser pour cet exercice. Vous n’avez pas besoin d’effectuer de configuration supplémentaire en dehors de l’ajout de tâches au projet.

Pour plus d’informations sur la création d’un projet dans Workbench, voir xxx.

### 1. Créez et nommez le scénario

1. Connectez-vous à votre compte [!DNL Workfront Fusion].
1. Cliquez sur **[!UICONTROL Scénarios]** ![](assets/scenarios-icon.png) dans le panneau de gauche.

   >[!NOTE]
   >
   >Si le panneau de navigation de gauche ou ses icônes ne s’affichent pas, cliquez sur l’icône de menu ![Menu](assets/main-menu-icon-left-nav.png).

1. Dans le panneau [!UICONTROL **Dossiers**], cliquez sur l’icône **[!UICONTROL Ajouter un dossier]** ![](assets/add-folder-icon.png), puis saisissez un nom tel que « Scénarios de test » pour votre premier dossier.

1. Ouvrez le dossier, puis cliquez sur **[!UICONTROL Créer un scénario]** dans le coin supérieur droit de la page.

1. Pour cet exercice, sélectionnez l’application **[!DNL Adobe Workfront]**, puis cliquez sur **Rechercher** près du bas.


1. Sélectionnez le nom de l’espace réservé **[!UICONTROL Nouveau scénario]** dans le coin supérieur gauche, puis saisissez un nom tel que « Scénario de test 1 ».

   ![](assets/name-the-scenario.png)

1. Poursuivez avec [Connectez le premier module](#2-connect-the-first-module) ci-dessous.

### 2. Connexion au premier module

Maintenant, vous devez établir une connexion authentifiée à votre compte [!DNL Workfront]. Chaque module que vous ajoutez à un scénario doit avoir une connexion avec son application.

1. Dans la zone **[!DNL Workfront]** sous **[!UICONTROL Connexion]**, cliquez sur **[!UICONTROL Ajouter]**, puis donnez un nom à la connexion, par exemple « Compte Workfront d’Olivia », puis cliquez sur **[!UICONTROL Continuer]**.
1. Authentifiez la connexion dans la fenêtre qui s’affiche.

   Le processus d’authentification d’une connexion peut varier légèrement d’une application à l’autre. Le processus suivant est spécifique à [!DNL Workfront], mais il est similaire à de nombreuses applications :

   1. Saisissez votre domaine [!DNL Workfront], puis cliquez sur **[!UICONTROL Continuer]**.
   1. Connectez-vous à [!DNL Workfront].
   1. Examiner la demande d’accès de [!DNL Workfront Fusion], puis cliquez sur **[!UICONTROL Autoriser l’accès]**.

   Si vous avez besoin d’aide, voir [Vue d’ensemble des connexions](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

### 3. Configurer le premier module

Après avoir connecté [!DNL Workfront Fusion] à votre compte [!DNL Workfront], vous pouvez spécifier un projet [!DNL Workfront] auquel vous avez accès et les données que vous souhaitez que le premier module soit traité.

1. Dans la zone Type d’enregistrement, sélectionnez Projet. **** Le module est ainsi configuré pour rechercher uniquement les projets.

   >[!TIP]
   >
   >Vous trouverez **[!UICONTROL Projet]** dans la liste si vous commencez à saisir le mot « [!UICONTROL projet] ».

1. Dans la zone **[!UICONTROL Jeu de résultats]**, sélectionnez **[!UICONTROL Premier enregistrement correspondant]**. Cette option permet au module de ne renvoyer que le premier enregistrement qui répond aux critères. Dans cet exemple, un seul enregistrement est renvoyé.
1. Dans la zone **[!UICONTROL Critères de recherche]**, nous allons configurer un filtre pour renvoyer le projet spécifique :

   | champ | Action |
   |--------|-------------|
   | Champs de critères de recherche | Sélectionnez le champ dont vous souhaitez rechercher les valeurs. Pour cet exemple, sélectionnez **[!UICONTROL Nom]**. |
   | Critères de recherche | Dans le premier menu déroulant, sélectionnez **[!UICONTROL Nom]**. |
   | Opérateurs de base | Dans la seconde liste déroulante, sélectionnez [!UICONTROL Contient (non-respect de la casse)]. Cela permet au module de rechercher des projets dont le nom contient les mots de votre choix, même si vous ne saisissez pas l’intégralité du nom, ou si vous saisissez le nom avec une casse incorrecte (toutes les majuscules, par exemple). |
   | Zone de texte | Saisissez un mot ou une expression que vous savez trouver dans le nom du projet que vous recherchez. |

+++ Développez pour afficher un exemple à l’écran.
   ![](assets/search-name.png)
+++

1. Dans la liste Sorties, sélectionnez les champs que le module doit générer. **** Pour cet exemple, sélectionnez les champs **[!UICONTROL ID]** et **[!UICONTROL Nom]**.

   >[!TIP]
   >
   >Utilisez les raccourcis clavier **Cmd+F** ([!DNL Mac]OS) ou **Ctrl+F** (système d’exploitation [!DNL Windows]) pour trouver rapidement un champ.

1. Cliquez sur **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Puisqu’il ne s’agit pas d’un module déclencheur, vous ne choisissez pas où le démarrer. Lors de l’utilisation d’un module de déclenchement, vous devez maintenant sélectionner le point de départ.
   >
   >
   >Pour plus d’informations, consultez la section [Choisir le point de départ d’un module de déclenchement dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Cliquez avec le bouton droit sur le module, sélectionnez **[!UICONTROL Renommer]**, puis saisissez un nom décrivant l’objectif du module (par exemple « Rechercher un projet ») et cliquez sur **[!UICONTROL OK]**.

   Le nom apparaît juste en dessous du module. En dessous du nom, [!DNL Workfront Fusion] présente une brève description du type d’action effectuée par le module.

   ![](assets/module-renamed-wf.png)

1. Passez à l’étape [Ajouter et configurer le deuxième module](#add-and-configure-the-second-module).

### 4. Ajouter et configurer le deuxième module

1. Cliquez sur le cercle partiel à droite du du module pour **[!UICONTROL Ajouter un autre module]**.
1. Sélectionnez [!DNL Workfront] dans la liste des applications, puis choisissez le module de recherche **[!UICONTROL Lire les enregistrements associés]**.
1. Dans la zone **[!UICONTROL Connexion]**, sélectionnez la connexion que vous avez créée pour le module précédent. Vous devez vous assurer que ce module utilise la même connexion que le module précédent.
1. Cliquez sur **[!UICONTROL Type d’enregistrement]**, puis sélectionnez **[!UICONTROL Projet]** pour lire les enregistrements liés à un projet.

   >[!TIP]
   >
   >Commencez à saisir le mot « projet » pour trouver **[!UICONTROL Projet]** dans la liste.

1. Cliquez sur le champ ID d’enregistrement parent. **** Ce champ nécessite l’ID Workfront du projet pour lequel vous souhaitez obtenir les tâches.

   Cliquez sur le champ pour ouvrir la liste des variables que vous pouvez utiliser dans le champ **[!UICONTROL ID d’enregistrement parent]** pour identifier le projet dans Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Clic sur la variable **[!UICONTROL ID]** pour l’ajouter au champ **[!UICONTROL ID d’enregistrement parent]**. Cela permet d’utiliser l’ID renvoyé par le premier module comme identifiant du projet avec lequel vous souhaitez travailler dans le deuxième module, ce qui garantit que les tâches renvoyées appartiendront à ce projet.
1. Dans le champ Collections, sélectionnez Tâche. ******** Cela indique que le module doit renvoyer les tâches associées au projet sélectionné.
1. Dans le champ **[!UICONTROL Outputs]** , sélectionnez **[!UICONTROL Id]** et **[!UICONTROL Name]**.
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
