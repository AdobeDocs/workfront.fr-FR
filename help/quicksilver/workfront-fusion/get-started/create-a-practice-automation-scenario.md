---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Créer un scénario d’automatisation pratique dans  [!DNL Adobe Workfront Fusion]
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 67%

---

# Créer un scénario d’automatisation pratique dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Workflow de création d’un scénario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Les scénarios d’automatisation permettent d’automatiser les processus Workfront, y compris la manipulation et la transformation des données. Cet article vous guide tout au long du processus de création d’un scénario qui recherche un projet, puis renvoie toutes les tâches associées à ce projet.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Formule Adobe Workfront</td>  
      <td>Tous</td>  
    </tr>  
    <tr>  
      <td>Licence Adobe Workfront</td>  
      <td>
        Nouveau : Standard<br>
        Ou <br>
        En cours : Travail ou version ultérieure
      </td>  
    </tr>  
    <tr>  
      <td>Licence Adobe Workfront Fusion</td>  
      <td> 
        Actuel : aucune exigence de licence Workfront Fusion.<br>
        Ou <br>
        Hérité : Tous
      </td>  
    </tr>  
    <tr>  
      <td>Produit</td>  
      <td> 
        Nouveau : sélectionnez ou Prime Workfront Plan : votre entreprise doit acheter Adobe Workfront Fusion.<br>
        Plan Ultimate Workfront : Workfront Fusion est inclus.<br>
        Ou <br>
        Actuel : votre entreprise doit acheter Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Créer un scénario de pratique d’automatisation

[!DNL Adobe Workfront Fusion] vous aide à vous concentrer sur les tâches importantes en automatisant les tâches répétitives. Il crée des scénarios qui gèrent automatiquement vos données sur différents services et applications.

Chaque scénario se compose de modules qui guident le traitement des données au sein d’une application ou leur transfert entre différents services et applications. Par exemple, vous pouvez créer un scénario dans Fusion pour rechercher automatiquement un projet [!DNL Workfront] et répertorier ses tâches. De cette façon, Fusion vous fait gagner du temps et vous évite des tâches de routine.

Ce scénario pratique vous guide tout au long du processus de création d’un scénario qui recherche un projet [!DNL Workfront] et renvoie les tâches du projet.

![](assets/create-practice-scenario-wf-only-350x157.png)

### Avant de commencer

Créez un projet avec des tâches dans Workfront que vous pouvez utiliser pour cet exercice. Vous n’avez pas besoin d’effectuer de configuration supplémentaire en dehors de l’ajout de tâches au projet.

Pour plus d&#39;informations sur la création d&#39;un projet dans Workfront, voir xxx.

### 1. Créer et nommer le scénario

1. Connectez-vous à votre compte [!DNL Workfront Fusion].
1. Cliquez sur **[!UICONTROL Scénarios]**![](assets/scenarios-icon.png) dans le panneau de gauche.

   >[!NOTE]
   >
   >Si le panneau de navigation de gauche ou ses icônes ne s’affichent pas, cliquez sur l’icône menu ![Menu](assets/main-menu-icon-left-nav.png).

1. Dans le panneau [!UICONTROL **Dossiers**], cliquez sur l’icône **[!UICONTROL Ajouter un dossier]**![](assets/add-folder-icon.png), puis saisissez un nom tel que « Scénarios pratique » pour votre premier dossier.

1. Ouvrez le dossier, puis cliquez sur **[!UICONTROL Créer un nouveau scénario]** dans le coin supérieur droit de la page.

1. Pour cet exercice, sélectionnez l’application **[!DNL Adobe Workfront]**, puis cliquez sur **Rechercher** en bas.


1. Sélectionnez le nom de l’espace réservé **[!UICONTROL Nouveau scénario]** dans le coin supérieur gauche, puis saisissez un nom tel que « Scénario pratique 1 ».

   ![](assets/name-the-scenario.png)

1. Continuez avec [Connecter le premier module](#2-connect-the-first-module) ci-dessous.

### 2. Connecter le premier module

Vous devez maintenant établir une connexion authentifiée à votre compte [!DNL Workfront]. Chaque module que vous ajoutez à un scénario doit avoir une connexion à son application.

1. Dans la zone **[!DNL Workfront]**, sous **[!UICONTROL Connexion]**, cliquez sur **[!UICONTROL Ajouter]**, tapez un nom pour la connexion, par exemple « Compte Workfront d’Olivia », puis cliquez sur **[!UICONTROL Continuer]**.
1. Authentifiez la connexion dans la fenêtre qui s’affiche.

   Le processus d’authentification d’une connexion peut varier légèrement d’une application à l’autre. Le processus suivant est spécifique à [!DNL Workfront], mais il est similaire à celui de nombreuses applications :

   1. Entrez votre domaine [!DNL Workfront], puis cliquez sur **[!UICONTROL Continuer]**.
   1. Connectez-vous à [!DNL Workfront].
   1. Examinez l’accès demandé par [!DNL Workfront Fusion], puis cliquez sur **[!UICONTROL Autoriser l’accès]**.

   Si vous avez besoin d’aide, voir [Vue d’ensemble des connexions](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

### 3. Configuration du premier module

Après la connexion de [!DNL Workfront Fusion] à votre compte [!DNL Workfront], vous pouvez spécifier un projet [!DNL Workfront] auquel vous avez accès et les données que vous souhaitez que le premier module traite.

1. Dans la zone [!UICONTROL Type d’enregistrement], sélectionnez **[!UICONTROL Projet]**. Cette option permet au module de ne rechercher que des projets.

   >[!TIP]
   >
   >Vous pouvez trouver **[!UICONTROL Projet]** dans la liste si vous commencez à taper le mot « [!UICONTROL projet] ».

1. Dans la zone **[!UICONTROL Jeu de résultats]**, sélectionnez **[!UICONTROL Premier enregistrement correspondant]**. Cela permet au module de ne renvoyer que le premier enregistrement qui répond aux critères. Pour cet exemple, nous n’avons besoin que d’un seul enregistrement renvoyé.
1. Dans la zone **[!UICONTROL Critères de recherche]**, nous allons configurer un filtre pour renvoyer le projet spécifique :

   | champ | Action |
   |--------|-------------|
   | Champs de critères de recherche | Sélectionnez le champ dont vous souhaitez rechercher les valeurs. Pour cet exemple, sélectionnez **[!UICONTROL Nom]**. |
   | Critères de recherche | Dans le premier menu déroulant, sélectionnez **[!UICONTROL Nom]**. |
   | Opérateurs de base | Dans la deuxième liste déroulante, sélectionnez [!UICONTROL Contient (non-respect de la casse)]. Cela permet au module de trouver des projets dont le nom contient les mots que vous avez choisis, même si vous ne saisissez pas le nom en entier ou si vous saisissez le nom avec une casse incorrecte (par exemple, tout en majuscules). |
   | Zone de texte | Entrez un mot ou une expression dont vous savez qu&#39;il se trouve dans le nom du projet que vous recherchez. |

+++ Développez pour afficher un exemple à l’écran.
   ![](assets/search-name.png)
+++

1. Dans la liste Sorties, sélectionnez les champs que le module doit générer. **** Pour cet exemple, sélectionnez les champs **[!UICONTROL ID]** et **[!UICONTROL Nom]**.

   >[!TIP]
   >
   >Vous pouvez utiliser **Cmd+F** (système d’exploitation [!DNL Mac]) ou **Ctrl+F** (système d’exploitation [!DNL Windows]) pour trouver rapidement un champ.

1. Cliquez sur **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Comme il ne s’agit pas d’un module de déclenchement, vous ne choisissez pas où le démarrer. Lors de l’utilisation d’un module de déclenchement, vous devez maintenant sélectionner l’endroit où il doit démarrer.
   >
   >
   >Pour plus d’informations, consultez [Choisir le point de départ d’un module de déclenchement dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Cliquez avec le bouton droit sur le module, cliquez sur **[!UICONTROL Renommer]**, tapez un nom qui décrit ce que vous voulez que le module fasse (par exemple, « Rechercher un projet »), puis cliquez sur **[!UICONTROL OK]**.

   Le nom apparaît juste en dessous du module. En dessous, [!DNL Workfront Fusion] inclut une brève description du type d’action effectuée par le module.

   ![](assets/module-renamed-wf.png)

1. Continuez avec [Ajouter et configurer le deuxième module](#add-and-configure-the-second-module).

### 4. Ajouter et configurer le deuxième module

1. Cliquez sur le cercle partiel à droite du module pour **[!UICONTROL Ajouter un autre module]**.
1. Sélectionnez [!DNL Workfront] dans la liste des applications, puis choisissez le module de recherche **[!UICONTROL Lire les enregistrements associés]**.
1. Dans la zone **[!UICONTROL Connexion]**, sélectionnez la connexion que vous avez créée pour le module précédent. Vous devez vous assurer que ce module utilise la même connexion que le module précédent.
1. Cliquez sur **[!UICONTROL Type d’enregistrement]**, puis sélectionnez **[!UICONTROL Projet]**, car nous voulons lire les enregistrements associés à un projet.

   >[!TIP]
   >
   >Vous trouverez **[!UICONTROL Projet]** dans la liste si vous commencez à taper le mot « projet ».

1. Cliquez sur le champ **[!UICONTROL Identifiant de l’enregistrement parent]**. Ce champ requiert l’identifiant Workfront du projet dont vous souhaitez renvoyer les tâches.

   En cliquant sur le champ, vous ouvrez la liste des variables que vous pouvez utiliser dans le champ **[!UICONTROL Identifiant de l’enregistrement parent]** pour identifier le projet dans Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Cliquez sur la variable **[!UICONTROL Identifiant]** pour l’ajouter au champ **[!UICONTROL Identifiant de l’enregistrement parent]**. Cela permet d’utiliser l’identifiant renvoyé par le premier module comme identifiant du projet avec lequel vous souhaitez travailler dans le second module, ce qui garantit que les tâches renvoyées appartiendront à ce projet.
1. Dans le champ **[!UICONTROL Collections]**, sélectionnez **[!UICONTROL Tâches]**. Cela indique que le module doit renvoyer les tâches associées au projet choisi.
1. Dans le champ **[!UICONTROL Sorties]**, sélectionnez **[!UICONTROL Id]** et **[!UICONTROL Name]**.
1. Cliquez sur **[!UICONTROL OK]**.

   Vous disposez à présent d’un scénario opérationnel.

1. Donnez au deuxième module un nom tel que « Renvoyer les tâches associées au projet », puis continuez avec [Tester le scénario](#test-the-scenario).

## Tester le scénario

Avant d’activer votre scénario, il est important de le tester en l’exécutant au moins une fois et en visualisant les résultats. Cela vous permet de comprendre comment les données circulent dans le scénario et de détecter les éventuelles erreurs.

Nous avons choisi de renvoyer un projet, ainsi que les tâches associées à ce projet. Si vous exécutez le scénario, c’est ce qui devrait se produire.

1. Cliquez sur **[!UICONTROL Exécuter une fois]** dans le coin inférieur gauche de l’éditeur de scénarios.
1. Une fois le scénario terminé, cliquez sur la bulle située au-dessus du premier module.

   ![](assets/click-bubble.png)

   Dans la boîte qui s’affiche, vous pouvez consulter des informations sur l’ensemble des données traitées par le module, y compris les données réelles extraites du projet et renvoyées par le module.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Cliquez sur la bulle de l’inspecteur d’exécution au-dessus du deuxième module pour voir l’entrée des informations et la sortie, qui est un ensemble de tâches contenues dans le projet.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Pour en savoir plus sur la lecture des informations relatives à l’exécution des scénarios, consultez les articles suivants :

   * Pour obtenir des informations générales, consultez la section [Flux d’exécution d’un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Pour plus d’informations sur les ensembles traités, voir [Exécuter des scénarios, cycles et phases dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** ![](assets/save-icon.png) dans le coin inférieur gauche pour enregistrer votre progression dans le scénario.

   >[!IMPORTANT]
   >
   >Sauvegardez souvent lorsque vous affinez et testez un scénario.

>[!TIP]
>
>Nous vous recommandons d’ajouter des notes sur chaque module, ce qui est facultatif mais utile.
>
>1. Cliquez avec le bouton droit de la souris sur un module [!DNL Workfront], puis cliquez sur **[!UICONTROL Ajouter une note]**.
>1. Dans la note qui s’affiche, saisissez un aperçu du module.
>
>    Vous pouvez ajouter plusieurs notes pour un module.
>
>1. Fermez la zone **[!UICONTROL Notes]**.
>
>     Après avoir ajouté une note à un scénario, un point orange s’affiche sur l’icône **[!UICONTROL Notes]**![](assets/notes-icon-w-dot.png) au bas de l’éditeur de scénario.
>
>1. Cliquez sur l’icône **[!UICONTROL Notes]** ![](assets/notes-icon-w-dot.png) pour afficher vos notes.
>

## Activer le scénario

Cet exemple de scénario ne comporte pas de module de déclenchement. S’il s’agissait d’un scénario que vous utiliseriez pour des données réelles, il commencerait par un module de déclenchement, et la dernière chose que vous feriez serait de l’activer. Une fois que vous avez activé un scénario, celui-ci s’exécute par défaut toutes les 15 minutes. Vous pouvez modifier cela en définissant quand et à quelle fréquence vous souhaitez qu’il s’exécute.

Pour plus d’informations sur l’activation des scénarios, voir [Activer ou désactiver un scénario dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Pour plus d’informations sur les plannings, voir [Planifier un scénario dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
