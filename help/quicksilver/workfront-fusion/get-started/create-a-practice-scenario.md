---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Créer un scénario d’intégration pratique dans Adobe Workfront Fusion
description: Cet article décrit comment créer un scénario d’intégration avec Adobe Workfront Fusion. Les scénarios d’intégration connectent des applications distinctes, ce qui permet à vos données d’évoluer dans différentes applications.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '2139'
ht-degree: 39%

---

# Créer un scénario d’intégration pratique dans Adobe Workfront Fusion

Cet article décrit comment créer un scénario d’intégration avec Adobe Workfront Fusion. Les scénarios d’intégration connectent des applications distinctes, ce qui permet à vos données d’évoluer dans différentes applications.

Pour créer un scénario d’intégration, votre organisation doit disposer d’une licence [!DNL Workfront Fusion for Work Automation and Integration].

Pour plus d’informations sur la création d’un scénario d’automatisation pour Workfront uniquement, voir [Création d’un scénario d’automatisation de l’exercice dans Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Pour plus d’informations sur les licences Workfront Fusion, voir [Licences Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>Votre entreprise peut ne pas autoriser l’accès aux feuilles de calcul Google. Si tel est le cas, vous ne pourrez pas configurer cette intégration, mais les informations présentées ici peuvent être utilisées comme exemple général du fonctionnement des scénarios d’intégration.

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

Pour expliquer comment créer un scénario et renforcer les bonnes pratiques à mesure que vous apprenez à utiliser [!DNL Workfront Fusion], cet article vous guide tout au long du processus, étape par étape. Nous allons créer un scénario qui crée un nouvel enregistrement dans [!DNL Workfront] pour chaque ligne d’une feuille de calcul [!DNL Google Sheets].

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Un tel scénario serait utile si vous disposiez d’une feuille de calcul répertoriant les projets qui doivent être traités à l’aide de projets dans [!DNL Workfront]. Le scénario peut &quot;regarder&quot; la feuille de calcul pour les nouvelles lignes et ajouter un nouveau projet dans [!DNL Workfront] pour chacune d’elles.

La création d’un scénario se compose de plusieurs tâches principales :

## Choisir les applications et nommer le scénario

1. Téléchargez cette [feuille de calcul](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx), puis chargez-la dans votre [!DNL Google Drive] pour l’utiliser tout au long de cet exercice.

   Ou

   Créez ou recherchez votre propre feuille de calcul [!DNL Google Sheets] simple similaire à celle-ci :

   ![](assets/spreadsheet-headers-350x55.png)

1. Connectez-vous à votre compte [!DNL Workfront Fusion].
1. Cliquez sur **[!UICONTROL Scénarios]** ![](assets/scenarios-icon.png) dans le panneau de gauche.

   >[!NOTE]
   >
   >Si le panneau de navigation de gauche ou ses icônes ne s’affichent pas, cliquez sur l’icône de menu ![Menu](assets/main-menu-icon-left-nav.png).

   Dans le panneau gris [!UICONTROL Dossiers] qui s’affiche, vous pouvez organiser vos scénarios en dossiers.

   Dans la partie supérieure de la zone principale à droite, vous pouvez afficher **[!UICONTROL Tous]** scénarios que vous avez créés, vos **[!UICONTROL scénarios actifs]** et **[!UICONTROL scénarios inactifs]** et **[!UICONTROL concepts]**, qui sont des scénarios qui nécessitent un travail supplémentaire avant que [!DNL Workfront Fusion] puisse les classer comme actifs ou inactifs.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. Dans le panneau [!UICONTROL Dossiers], cliquez sur l’icône **[!UICONTROL Ajouter un dossier]** ![](assets/add-folder-icon.png), puis saisissez un nom tel que « Scénarios de test » pour votre premier dossier.

1. Ouvrez le dossier, puis cliquez sur **[!UICONTROL Créer un scénario]** dans le coin supérieur droit de la page.

   La page de destination qui s’affiche vous permet de précharger toutes les applications que vous souhaitez utiliser dans le scénario que vous allez créer.

1. Pour cet exercice, recherchez et sélectionnez l’application **[!UICONTROL Google Sheets]**.
1. Cliquez sur **[!UICONTROL Continuer]** dans le coin supérieur droit.

   L’éditeur de scénario s’affiche avec un module vide au centre, l’application [!DNL Google Sheets] que vous avez préchargée et certaines options dans la barre d’outils en bas.

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

1. Cliquez sur le module vide pour choisir l’application à partir de laquelle vous allez sélectionner un module.

   L’application que vous avez préchargée précédemment s’affiche en regard du module vide. Vous pouvez ajouter toute autre application qui comporte des modules dans la zone [!UICONTROL Rechercher].

   ![](assets/pre-loaded-apps-350x139.png)

1. Cliquez sur **[!DNL Google Sheets]**.

   La liste affiche alors tous les modules [!DNL Google Sheets] que vous pouvez utiliser comme module déclencheur.

1. Cliquez sur le module déclencheur **[!UICONTROL Watch for Records]**.

   Vous devez maintenant établir une connexion authentifiée à votre compte Google. Chaque module que vous ajoutez à un scénario doit avoir une connexion avec son application.

1. Dans la zone **[!DNL Google Sheets]**, sous **[!UICONTROL Connexion]**, cliquez sur **[!UICONTROL Ajouter]**, puis saisissez un nom pour la connexion, par exemple &quot;Compte Google d&#39;Olivia&quot;, puis cliquez sur **[!UICONTROL Continuer]**.
1. Authentifiez la connexion dans la fenêtre qui s’affiche.

   Le processus d’authentification d’une connexion peut varier légèrement d’une application à l’autre. Vous devrez peut-être vous connecter à l’application. Vous devez généralement cliquer sur un bouton **[!UICONTROL Autoriser]** . Si vous avez besoin d’aide, reportez-vous à la section [Présentation des connexions](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configurer le premier module

Une fois que vous avez connecté [!DNL Workfront Fusion] à votre compte [!DNL Google Sheets], vous pouvez spécifier une feuille de calcul [!DNL Google Sheets] à laquelle vous avez accès et les données que vous souhaitez que le premier module soit traité.

1. Cliquez sur la zone **[!UICONTROL Feuille de calcul]** , puis sélectionnez la feuille de calcul **[!UICONTROL Scénario de pratique de fusion Workfront] #1** dans la liste qui s’affiche.

   Cette feuille de calcul contient 2 feuilles (onglets). Nous devons donc spécifier la feuille contenant les données souhaitées :

1. Dans la liste déroulante **[!UICONTROL Sheet]**, sélectionnez **[!UICONTROL Projects]**.

   Notre feuille de calcul contient des en-têtes que le module doit utiliser pour identifier les données à traiter :

   ![](assets/spreadsheet-headers-350x55.png)

1. Laissez **[!UICONTROL Oui]** sélectionné pour **[!UICONTROL La table contient des en-têtes]**.

1. Dans la zone **[!UICONTROL Rangée avec en-têtes]**, vous pouvez spécifier une plage de lignes à inclure, mais laissez la valeur par défaut A1:Z1 pour cet exercice.
1. Dans la zone **[!UICONTROL Limit]**, saisissez 1.

   Ainsi, chaque fois que vous exécutez le scénario, le module ne traite qu’une ligne dans la feuille de calcul. Cela s’avère utile pour simplifier les exécutions de test pendant que vous créez le scénario.

1. Cliquez sur **[!UICONTROL OK]**.

   La zone **[!UICONTROL Choisir où démarrer]** vous invite à indiquer où, dans la feuille de calcul, vous souhaitez que le module commence le traitement.

1. Cliquez sur **[!UICONTROL Choisir manuellement]**, sélectionnez l’option supérieure dans la liste qui s’affiche, puis cliquez sur **[!UICONTROL OK]**.
1. Cliquez avec le bouton droit de la souris sur le module, cliquez sur **[!UICONTROL Renommer]**, puis saisissez un nom qui décrit ce que vous souhaitez que le module fasse (par exemple &quot;Regarder la liste des projets&quot;), puis cliquez sur **[!UICONTROL OK]**.

   Le nom apparaît juste en dessous du module. En dessous du nom, [!DNL Workfront Fusion] présente une brève description du type d’action effectuée par le module.

   ![](assets/module-renamed-350x388.png)

1. Passez à l’étape [Ajouter et configurer le deuxième module](#add-and-configure-the-second-module).

## Ajouter et configurer le deuxième module

1. Cliquez sur le cercle partiel à droite du du module pour **[!UICONTROL Ajouter un autre module]**.

   Ce deuxième module doit être un module [!DNL Workfront], mais nous n’avons pas pré-chargé l’application [!DNL Workfront].

1. Pour rechercher l’application [!DNL Workfront], commencez à saisir &quot;[!DNL Workfront]&quot; et cliquez sur l’application lorsqu’elle apparaît.
1. Dans la liste des [!DNL Workfront] modules qui s’affichent, cliquez sur **[!UICONTROL Créer un enregistrement]**.

1. Comme vous l’avez fait auparavant avec l’application Google Sheets, cliquez sur **[!UICONTROL Ajouter]** dans la zone [!DNL Workfront] pour ajouter une connexion entre Workfront Fusion et Workfront.

   Maintenant, nous allons commencer à spécifier ce que nous voulons faire avec les données de la feuille de calcul.

1. Cliquez sur **[!UICONTROL Type d&#39;enregistrement]**, puis sélectionnez **[!UICONTROL Projet]** car nous voulons créer un projet dans [!DNL Workfront] à l&#39;aide d&#39;une ligne de la feuille de calcul.

   >[!TIP]
   >
   >Vous trouverez **[!UICONTROL Projet]** dans la liste si vous commencez à saisir le mot « [!UICONTROL projet] ».

   La boîte se développe pour afficher tous les champs de projet [!DNL Workfront] disponibles où vous pouvez placer les informations trouvées par le premier module.

   Nous allons utiliser le champ **[!UICONTROL Nom]** : nous voulons que ce module nomme chaque projet dans [!DNL Workfront] en utilisant le texte de la ligne [!UICONTROL Google Sheets] correspondante.

1. Recherchez et cliquez sur le champ **[!UICONTROL Nom]** .

   >[!TIP]
   >
   >Vous pouvez utiliser **Cmd+F** ([!DNL Mac] OS) ou **Ctrl+F**([!DNL Windows] OS) pour trouver rapidement un champ.

   Cela ouvre la liste des variables que vous pouvez utiliser dans le champ **[!UICONTROL Nom]** pour définir le nom de chaque projet créé dans Workfront.

   ![](assets/list-of-available-variables-350x261.png)

   Notez que les variables proches du haut de la liste correspondent aux en-têtes de colonne de la feuille de calcul.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Cliquez sur la variable **[!UICONTROL My Project Name (A)]** pour l’ajouter au champ **[!UICONTROL Name]**.

   Vous venez de mettre en correspondance votre première donnée pour ce scénario.

   Mappez une donnée supplémentaire de la feuille de calcul à [!DNL Workfront] : la date de début de chaque projet.

1. Recherchez et cliquez sur le champ **[!UICONTROL Date de début planifiée]** , puis cliquez sur la variable **[!UICONTROL Date de début planifiée (E)]** pour extraire des données de cette colonne dans la feuille de calcul.

1. Cliquez sur **[!UICONTROL OK]**.

   Vous disposez maintenant d’un scénario de travail.

1. Attribuez au deuxième module un nom tel que &quot;Créer un projet Workfront&quot;, puis continuez avec [Tester le scénario](#test-the-scenario).

## Tester le scénario

Avant d’activer votre scénario, il est important de le tester en l’exécutant au moins une fois et en consultant les résultats. Vous pouvez ainsi comprendre le flux des données dans le scénario et rechercher les erreurs.

Nous avons choisi de traiter 1 ligne de la feuille de calcul pour créer un projet dans Workfront. Exécutons le scénario et jugeons de son efficacité.

1. Cliquez sur **[!UICONTROL Exécuter une seule fois]** dans le coin inférieur gauche de l’éditeur de scénario.
1. Une fois le scénario en cours d’exécution, cliquez sur la bulle au-dessus du module [!DNL Google Sheets].

   ![](assets/click-bubble.png)

   Dans la zone qui s’affiche, vous pouvez afficher des informations sur le lot de données traité par le module, y compris les données réelles extraites de la feuille de calcul pour la ligne avec laquelle vous avez commencé.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Cliquez sur la bulle d’inspection d’exécution au-dessus du module [!DNL Workfront] pour voir la saisie des informations et la sortie, qui est l’identifiant du projet créé dans [!DNL Workfront].

   ![](assets/execution-inspector-wf-350x384.png)

   Pour en savoir plus sur la lecture des informations d’exécution de scénario, consultez les articles suivants :

   * Pour obtenir des informations générales, voir [Flux d’exécution du scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Pour plus d’informations sur les lots traités, voir [Exécution, cycles et phases d’un scénario [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Accédez à [!DNL Workfront] et recherchez &quot;soho town loft&quot; pour voir le projet créé par le scénario. Il s’agissait de la dernière ligne de la feuille de calcul.
1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** ![](assets/save-icon.png) près du coin inférieur gauche pour enregistrer votre progression dans le scénario.

   >[!IMPORTANT]
   >
   >Enregistrez à intervalles réguliers lorsque vous affinez et testez un scénario.

## Finalisez le scénario et testez-le à nouveau.

Nous devons toujours configurer le scénario pour créer des projets pour toutes les autres lignes de la feuille de calcul.

1. Cliquez sur le module **[!UICONTROL Lignes de contrôle]** que vous avez créé pour les feuilles de calcul Google.
1. Remplacez la **[!UICONTROL Limit]** par 100.

   La spécification d’un nombre supérieur au nombre de lignes que vous connaissez figure dans la feuille de calcul pour garantir que le scénario les capturera toutes.

1. Cliquez avec le bouton droit de la souris sur le module **[!UICONTROL Watch Rows]**, cliquez sur **[!UICONTROL Choose where to start]**, cliquez sur **[!UICONTROL All]**, puis sur **[!UICONTROL OK]**.

1. Cliquez sur **[!UICONTROL Exécuter une fois]** et observez ce qui se passe dans les bulles d’inspection d’exécution.

   Le module [!DNL Google] Sheets **[!UICONTROL Watch Rows]** s’exécute une fois pour lire toutes les lignes. Ensuite, le module Workfront **[!UICONTROL Créer un enregistrement]** s’exécute 20 fois pour créer un projet pour chacune des 20 lignes restantes de la feuille de calcul.

1. Cliquez sur la bulle d’inspection d’exécution du module [!DNL Workfront] pour afficher les 20 opérations, puis cliquez sur l’une des opérations pour afficher les informations sur le projet créé.
1. Cliquez sur **[!UICONTROL Enregistrer]** ![](assets/save-icon.png) près du coin inférieur gauche.
1. Accédez à [!DNL Workfront] pour voir les projets créés par le scénario.

>[!TIP]
>
>Nous recommandons d’ajouter des notes sur chaque module pour indiquer ses objectifs.
>
>1. Cliquez avec le bouton droit sur le module [!DNL Workfront], puis cliquez sur **[!UICONTROL Ajouter une note]**.
>1. Dans la note qui s’affiche, saisissez une description générale du module.
>
>    Cela s’avère utile, car vous n’aurez pas à ouvrir continuellement le module pour voir ce qu’il fait. Vous pouvez saisir &quot;Crée un projet avec le nom, la date de début planifiée et la priorité mappés à partir d’une feuille de calcul&quot;.
>
>    Pour le module [!UICONTROL Google Sheets] , vous pouvez saisir quelque chose comme &quot;Regarder la liste des projets pour les nouvelles lignes/projets ajoutés&quot;.
>
>    Vous pouvez ajouter plusieurs notes pour un module.
>
>1. Fermez la zone **[!UICONTROL Remarques]**.
>
>    Après avoir ajouté une note à un scénario, un point orange s’affiche sur l’icône **[!UICONTROL Remarques]** ![](assets/notes-icon-w-dot.png) au bas de l’éditeur de scénario.
>
>1. Cliquez sur l’icône **[!UICONTROL Remarques]** ![](assets/notes-icon-w-dot.png) pour afficher vos notes.
>



## Activer le scénario

Si c’était un scénario que vous utiliseriez pour des données réelles, la dernière chose que vous feriez est de l’activer. Une fois que vous avez activé un scénario, celui-ci s’exécute par défaut toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant le moment et la fréquence d’exécution.

Pour plus d’informations sur l’activation de scénarios, voir [Activation ou désactivation d’un scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Pour plus d’informations sur les plannings, voir [Planification d’un scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
