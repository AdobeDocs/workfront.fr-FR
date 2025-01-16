---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Créez un scénario simple dans  [!DNL Adobe Workfront Fusion]
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
hide: true
hidefromtoc: true
feature: Workfront Fusion
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 34%

---

# Création d’un scénario de base dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Créer un scénario de base](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/create-basic-scenario.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Le rôle d’[!DNL Adobe Workfront Fusion] consiste à automatiser vos processus afin que vous puissiez vous concentrer sur de nouvelles tâches, plutôt que de répéter les mêmes tâches encore et encore. La plateforme fonctionne en liant les actions dans et entre les applications et les services pour créer un scénario qui transfère et transforme vos données automatiquement. Le scénario que vous créez recherche les données dans une application ou un service et traite ces données pour obtenir le résultat souhaité.

Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche un événement dans Workfront et le convertit en projet.

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

1. Dans la zone **Scénarios**, cliquez sur **Créer un scénario**.

   <!--To locate the Scenarios area, see navigation article-->

   L’éditeur de scénarios s’affiche, contenant un module vide au centre.

   <!--picture?-->

1. Sélectionnez le nom de l’espace réservé **[!UICONTROL Nouveau scénario]** dans le coin supérieur gauche, puis saisissez un nom.
1. Passez à la section [Ajouter et configurer le premier module](#add-and-configure-the-first-module) ci-dessous.

### Ajouter et configurer le premier module

1. Cliquez sur le module vide pour choisir l’application à partir de laquelle vous allez sélectionner un module.

   Une liste d&#39;applications s&#39;affiche à droite du module.

1. Sélectionnez **[!DNL Adobe Workfront]**. S’il n’est pas visible, cliquez sur la barre de recherche au bas de la liste, saisissez « Workfront », puis sélectionnez-le lorsqu’il apparaît dans la liste.

   La liste est modifiée afin d’afficher tous [!DNL Workfront] modules que vous pouvez utiliser.

1. Cliquez sur le module **[!UICONTROL Search]**.

   La fenêtre de configuration du module s’ouvre.

1. Dans la zone [!UICONTROL Connexion], sélectionnez votre connexion Workfront.

   Si vous ne disposez pas d’une connexion Workfront, voir [Créer une connexion à [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. Dans la zone [!UICONTROL Type d’enregistrement], sélectionnez **[!UICONTROL Événement]**. Cette option permet de définir le module pour rechercher uniquement les événements.

   Vous pouvez trouver **[!UICONTROL Problème]** dans la liste si vous commencez à saisir le mot « [!UICONTROL problème]. »

1. Dans la zone **[!UICONTROL Jeu de résultats]**, sélectionnez **[!UICONTROL Premier enregistrement correspondant]**.

   Cela définit le module pour renvoyer uniquement le premier enregistrement qu’il trouve et qui répond aux critères.
1. Dans la zone **[!UICONTROL Critères de recherche]**, configurez les critères pour renvoyer le problème spécifique.

   1. Dans la première zone sous [!UICONTROL Critères de recherche], sélectionnez le champ à inclure dans la recherche. Pour cet exemple, sélectionnez **[!UICONTROL Nom]**.

      Vous pouvez trouver **[!UICONTROL Nom]** dans la liste si vous commencez à saisir le mot « [!UICONTROL nom] ».
   1. Pour l’opérateur/opératrice, cliquez sur la flèche de liste déroulante en regard de **Exist** et remplacez-la par [!UICONTROL **Contient (non-respect de la casse)**].

      Cela permet au module de trouver des projets dont le nom contient les mots que vous avez choisis, même si vous ne saisissez pas le nom en entier ou si vous saisissez le nom avec une casse incorrecte (par exemple, tout en majuscules).
   1. Dans le dernier champ sous [!UICONTROL Critères de recherche], saisissez un mot ou une expression dont vous savez qu&#39;il est au nom de l&#39;événement recherché.

1. Dans la liste Sorties, sélectionnez les champs que le module doit générer. **** Pour cet exemple, sélectionnez les champs **[!UICONTROL ID]** et **[!UICONTROL Nom]**.

   >[!TIP]
   >
   >Vous pouvez utiliser **Cmd+F** (système d’exploitation [!DNL Mac]) ou **Ctrl+F** (système d’exploitation [!DNL Windows]) pour trouver rapidement un champ.

1. Cliquez sur **[!UICONTROL OK]** pour enregistrer la configuration du module.

1. Cliquez avec le bouton droit sur le module, cliquez sur **[!UICONTROL Renommer]**, puis entrez un nom décrivant ce que vous souhaitez que le module fasse (par exemple, « Rechercher un problème »), puis cliquez sur **[!UICONTROL OK]**.

   Le nom apparaît juste en dessous du module. En dessous, [!DNL Workfront Fusion] inclut une brève description du type d’action effectuée par le module.

   ![](assets/)

1. Continuez avec [Ajouter et configurer le deuxième module](#add-and-configure-the-second-module).

## Ajouter et configurer le deuxième module

1. Pointez sur le cercle partiel à droite du du module, puis cliquez sur **[!UICONTROL Ajouter un autre module]**.
1. Sélectionnez [!DNL Adobe Workfront] dans la liste des applications, puis choisissez le module **[!UICONTROL Action Divers]**.

   Le module Misc Action vous permet d’effectuer des actions dans Workfront qui ne disposent pas d’un module dédié. Dans cet exemple, ce module est utilisé pour convertir l’événement en projet.
1. Dans le champ [!UICONTROL Connexion], sélectionnez la même connexion Workfront que celle que vous avez utilisée dans le module précédent .
1. Dans le champ **[!UICONTROL Type d’enregistrement]**, sélectionnez **[!UICONTROL Événement]**, car l’action à effectuer est liée à un événement.
1. Dans le champ **[!UICONTROL Action]**, sélectionnez **convertToProject**. Il s&#39;agit de l&#39;action qui convertira l&#39;événement sélectionné en projet.
1. Cliquez sur le champ **[!UICONTROL ID]**.

   Un panneau s’ouvre, vous permettant de sélectionner les éléments à utiliser comme identifiant du problème que vous souhaitez convertir en projet. Le panneau comprend la sortie de tous les modules précédents. Étant donné que vous avez sélectionné l’ID comme sortie du module précédent, il est désormais disponible dans le panneau.

   Ce panneau est appelé panneau de mappage. Pour plus d’informations sur le panneau de mappage, voir [Mappage des informations d’un module à un autre](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Sélectionnez **ID** dans le panneau de mappage.

   Un bloc d’identifiant s’affiche dans le champ d’identifiant. Il indique le numéro du module à partir duquel il est mappé, ainsi que le champ qui est mappé.

   ![Identifiant de carte](assets/map-id.png)

1. (Facultatif) Dans la section Projet , recherchez le champ Identifiant du propriétaire et commencez à saisir votre nom dans le champ, puis sélectionnez-le lorsqu’il apparaît. Vous serez ainsi désigné(e) comme propriétaire du projet, et il sera plus facile de le retrouver dans Workfront.

   >[!TIP]
   >
   >Vous pouvez utiliser **Cmd+F** (système d’exploitation [!DNL Mac]) ou **Ctrl+F** (système d’exploitation [!DNL Windows]) pour trouver rapidement un champ.

1. Cliquez sur **[!UICONTROL OK]** pour enregistrer la configuration du module.

1. Cliquez avec le bouton droit sur le module, cliquez sur **[!UICONTROL Renommer]**, puis entrez un nom décrivant ce que vous souhaitez que le module fasse (par exemple, « Convertir en projet »), puis cliquez sur **[!UICONTROL OK]**.

1. Continuez pour [Tester le scénario](#test-the-scenario).

## Tester le scénario

Avant d’activer votre scénario, il est important de le tester en l’exécutant au moins une fois et en visualisant les résultats. Cela vous permet de comprendre comment les données circulent dans le scénario et de détecter les éventuelles erreurs.

Dans ce scénario, un test réussi permet de localiser le problème et de le convertir en projet.

1. Cliquez sur **[!UICONTROL Exécuter une fois]** dans le coin inférieur gauche de l’éditeur de scénario.
1. Une fois l’exécution du scénario terminée, cliquez sur la bulle située au-dessus du premier module pour afficher des informations sur le lot de données traité par le module, y compris les données extraites du problème renvoyé par le module.

1. Cliquez sur la bulle de l’inspecteur d’exécution au-dessus du deuxième module pour afficher l’entrée (le problème) et la sortie (le projet converti).

   Pour plus d&#39;informations sur les données des bulles d&#39;inspection, voir :

   * Pour obtenir des informations générales, consultez la section [Flux d’exécution d’un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Pour plus d’informations sur les lots traités, consultez la section [Exécution, cycles et phases d’un scénario [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** près du coin inférieur gauche pour enregistrer votre progression dans le scénario.

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

Ce scénario recherchant un problème spécifique, il n’est pas nécessaire de l’activer. L’activation d’un scénario entraîne son exécution selon un planning ou lorsqu’une action spécifique se produit dans une application. Une fois que vous avez activé un scénario, celui-ci s’exécute par défaut toutes les 15 minutes. Vous pouvez modifier cela en définissant quand et à quelle fréquence vous souhaitez qu’il s’exécute.

Pour plus d’informations sur l’activation des scénarios, voir [Activer ou désactiver un scénario dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Pour plus d’informations sur les plannings, voir [Planifier un scénario dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
