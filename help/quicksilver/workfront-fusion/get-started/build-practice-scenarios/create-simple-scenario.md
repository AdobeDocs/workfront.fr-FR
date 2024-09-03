---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Créer un scénario de base dans  [!DNL Adobe Workfront Fusion]
description: Découvrez comment créer un scénario d’automatisation simple avec Adobe Workfront Fusion. Les scénarios d’automatisation permettent d’automatiser les processus Workfront, y compris la manipulation et la transformation des données. Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche une tâche  [!DNL Workfront] dans Workfront et la convertit en projet.
author: Becky
feature: Workfront Fusion
exl-id: 06fa7e15-b8dc-4fe1-9703-c160d580ef79
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 34%

---

# Création d’un scénario de base dans [!DNL Adobe Workfront Fusion]

Le rôle d’[!DNL Adobe Workfront Fusion] consiste à automatiser vos processus afin que vous puissiez vous concentrer sur de nouvelles tâches, plutôt que de répéter les mêmes tâches encore et encore. La plateforme fonctionne en liant les actions dans et entre les applications et les services pour créer un scénario qui transfère et transforme vos données automatiquement. Le scénario que vous créez recherche les données dans une application ou un service et traite ces données pour obtenir le résultat souhaité.

Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche une tâche [!DNL Workfront] dans Workfront et la convertit en projet.

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Créer un scénario pratique

### Commencer à créer le scénario

1. Dans la zone **Scénarios**, cliquez sur **Créer un nouveau scénario**.

   <!--To locate the Scenarios area, see navigation article-->

   L’éditeur de scénario s’affiche, contenant un module vide au centre.

   <!--picture?-->

1. Sélectionnez le nom d’espace réservé **[!UICONTROL Nouveau scénario]** dans le coin supérieur gauche, puis saisissez un nom.
1. Passez à la section [Ajouter et configurer le premier module](#add-and-configure-the-first-module) ci-dessous.

### Ajouter et configurer le premier module

1. Cliquez sur le module vide pour choisir l’application à partir de laquelle vous allez sélectionner un module.

   Une liste d’applications s’affiche à droite du module.

1. Sélectionnez **[!DNL Adobe Workfront]**. Si elle n’est pas visible, cliquez sur la barre de recherche située en bas de la liste, saisissez &quot;Workfront&quot;, puis sélectionnez-la lorsqu’elle apparaît dans la liste.

   La liste change pour afficher tous les modules [!DNL Workfront] que vous pouvez utiliser.

1. Cliquez sur le module **[!UICONTROL Recherche]** .

   La fenêtre de configuration du module s’ouvre.

1. Dans la zone [!UICONTROL Connexion], sélectionnez votre connexion Workfront.

   Si vous ne disposez pas d’une connexion Workfront, voir [Création d’une connexion à [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. Dans la zone [!UICONTROL Record Type], sélectionnez **[!UICONTROL Task]**. Le module est ainsi configuré pour effectuer uniquement des recherches dans les tâches.

   Vous pouvez trouver **[!UICONTROL Tâche]** dans la liste si vous commencez à saisir le mot &quot;[!UICONTROL tâche]&quot;.

1. Dans la zone **[!UICONTROL Result Set]**, sélectionnez **[!UICONTROL First Matching Record]**.

   Cela définit le module pour renvoyer uniquement le premier enregistrement qui répond aux critères.
1. Dans la zone **[!UICONTROL Critères de recherche]**, configurez les critères pour renvoyer la tâche spécifique.

   1. Dans la première zone sous [!UICONTROL Critères de recherche], sélectionnez le champ que vous souhaitez inclure dans votre recherche. Pour cet exemple, sélectionnez **[!UICONTROL Nom]**.

      **[!UICONTROL Name]** est disponible dans la liste si vous commencez à saisir le mot &quot;[!UICONTROL name]&quot;.
   1. Pour l’opérateur, cliquez sur la flèche de liste déroulante en regard de **Exist** et remplacez-la par [!UICONTROL **Contains (insensible à la casse)**].

      Cela permet au module de trouver des projets dont le nom contient les mots que vous avez choisis, même si vous ne saisissez pas le nom en entier ou si vous saisissez le nom avec une casse incorrecte (par exemple, tout en majuscules).
   1. Dans le dernier champ sous [!UICONTROL Critères de recherche], saisissez un mot ou une expression qui figure dans le nom de la tâche que vous recherchez.

1. Dans la liste Sorties, sélectionnez les champs que le module doit générer. **** Pour cet exemple, sélectionnez les champs **[!UICONTROL ID]** et **[!UICONTROL Nom]**.

   >[!TIP]
   >
   >Vous pouvez utiliser **Cmd+F** (système d’exploitation [!DNL Mac]) ou **Ctrl+F** (système d’exploitation [!DNL Windows]) pour trouver rapidement un champ.

1. Cliquez sur **[!UICONTROL OK]** pour enregistrer la configuration du module.

1. Cliquez avec le bouton droit sur le module, cliquez sur **[!UICONTROL Renommer]**, puis saisissez un nom qui décrit ce que vous souhaitez que le module fasse (par exemple &quot;Rechercher une tâche&quot;), puis cliquez sur **[!UICONTROL OK]**.

   Le nom apparaît juste en dessous du module. En dessous, [!DNL Workfront Fusion] inclut une brève description du type d’action effectuée par le module.

   ![](assets/module-renamed-wf.png)

1. Continuez avec [Ajouter et configurer le deuxième module](#add-and-configure-the-second-module).

## Ajouter et configurer le deuxième module

1. Passez la souris sur le cercle partiel situé à droite du du module, puis cliquez sur **[!UICONTROL Ajouter un autre module]**.
1. Sélectionnez [!DNL Adobe Workfront] dans la liste des applications, puis choisissez le module **[!UICONTROL Convert object]**.
1. Dans le champ [!UICONTROL Connexion] , sélectionnez la même connexion Workfront que celle utilisée dans le module précédent .
1. Dans le champ **[!UICONTROL Type d&#39;enregistrement]**, sélectionnez **[!UICONTROL Tâche]**, car le module convertit une tâche.
1. Dans le champ **[!UICONTROL Convertir en]**, sélectionnez **Projet**.
1. En regard du champ ID de la tâche, cliquez sur le bouton bascule de la carte pour l’activer.

   Le bouton bascule devient bleu lorsqu’il est activé. Cela vous permet de mapper l’identifiant de tâche du module précédent.

   ![Bascule de carte](assets/map-toggle.png)
1. Cliquez sur le champ **[!UICONTROL Task ID]** .

   Un panneau s’ouvre. Il vous permet de sélectionner l’identifiant de la tâche à convertir en projet. Comme vous avez activé le mappage, le panneau inclut la sortie de tous les modules précédents. Vous avez sélectionné ID en tant que sortie du module précédent. Il est donc désormais disponible dans le panneau.

   Ce panneau s’appelle le panneau de mappage. Pour plus d’informations sur le panneau de mappage, voir [Mappage des informations d’un module vers un autre](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Sélectionnez **ID** dans le panneau de mappage.

   Un bloc ID apparaît dans le champ ID. Il indique le nombre du module à partir duquel il est mappé et le champ qui est mappé.

   ![ID de carte](assets/map-id.png)

1. Cliquez sur le champ **ID de modèle**, commencez à saisir le nom du modèle Workfront que vous souhaitez utiliser pour ce projet, puis sélectionnez-le lorsqu’il apparaît dans la liste.
1. Cliquez sur **[!UICONTROL OK]** pour enregistrer la configuration du module.

1. Cliquez avec le bouton droit sur le module, cliquez sur **[!UICONTROL Renommer]**, puis saisissez un nom qui décrit ce que vous souhaitez que le module fasse (par exemple &quot;Convertir en projet&quot;), puis cliquez sur **[!UICONTROL OK]**.

1. Passez à [Test du scénario](#test-the-scenario).

## Tester le scénario

Avant d’activer votre scénario, il est important de le tester en l’exécutant au moins une fois et en visualisant les résultats. Cela vous permet de comprendre comment les données circulent dans le scénario et de détecter les éventuelles erreurs.

Pour ce scénario, un test réussi permet de localiser la nouvelle tâche et de la convertir en projet.

1. Cliquez sur **[!UICONTROL Exécuter une fois]** dans le coin inférieur gauche de l’éditeur de scénario.
1. Une fois le scénario en cours d’exécution terminé, cliquez sur la bulle au-dessus du premier module pour afficher des informations sur le lot de données traité par le module, y compris les données extraites de la tâche renvoyée par le module.

1. Cliquez sur la bulle d’inspection d’exécution au-dessus du deuxième module pour voir l’entrée (la tâche) et la sortie (le projet converti).

   Pour plus d’informations sur les données des bulles d’inspection, voir :

   * Pour obtenir des informations générales, consultez la section [Flux d’exécution d’un scénario dans  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * Pour plus d’informations sur les lots traités, consultez la section [Exécution, cycles et phases d’un scénario [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** près du coin inférieur gauche pour enregistrer la progression sur le scénario.

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

La dernière étape de la création d’un scénario consiste à l’activer.

Comme ce scénario recherche une tâche spécifique, il n’est pas nécessaire de l’activer. L’activation d’un scénario entraîne son exécution selon un planning ou lorsqu’une action spécifique se produit dans une application. Une fois que vous avez activé un scénario, celui-ci s’exécute par défaut toutes les 15 minutes. Vous pouvez modifier cela en définissant quand et à quelle fréquence vous souhaitez qu’il s’exécute.

Pour plus d’informations sur l’activation des scénarios, voir [Activer ou désactiver un scénario dans [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Pour plus d’informations sur les plannings, voir [Planifier un scénario dans [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## Étapes suivantes

* [Ajoutez un module de déclenchement](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) pour permettre au scénario de rechercher régulièrement de nouvelles requêtes et de les convertir en projets.
* Ajoutez un webhook pour permettre au scénario de s’exécuter chaque fois qu’une requête est saisie.
* Ajoutez un filtre pour vous assurer que seules certaines requêtes sont converties en projets.
* Ajoutez une fonction qui personnalise le nom du nouveau projet.
* Ajoutez une gestion des erreurs pour vous assurer que le scénario est résilient face aux erreurs.
