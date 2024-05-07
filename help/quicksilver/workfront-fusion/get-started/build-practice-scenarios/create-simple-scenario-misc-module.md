---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Créez un scénario simple dans [!DNL Adobe Workfront Fusion]
description: Découvrez comment créer un scénario d’automatisation simple avec Adobe Workfront Fusion. Les scénarios d’automatisation automatisent les processus Workfront, notamment la manipulation et la transformation des données. Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche un problème, puis le convertit en projet.
author: Becky
hide: true
hidefromtoc: true
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '1260'
ht-degree: 0%

---

# Créez un scénario de base dans [!DNL Adobe Workfront Fusion]

Le rôle de [!DNL Adobe Workfront Fusion] est d’automatiser vos processus afin que vous puissiez vous concentrer sur de nouvelles tâches plutôt que de répéter les mêmes tâches encore et encore. Il fonctionne en liant les actions dans et entre les applications et les services pour créer un scénario qui transfère et transforme vos données automatiquement. Le scénario que vous créez recherche les données dans une application ou un service et traite ces données pour obtenir le résultat souhaité.

Cet exemple vous guide tout au long du processus de création d’un scénario qui recherche un problème dans Workfront et le convertit en projet.

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

## Création d’un scénario d’entraînement

### Commencer à créer le scénario

1. Dans le **Scénarios** zone, cliquez sur **Création d’un scénario**.

   <!--To locate the Scenarios area, see navigation article-->

   L’éditeur de scénario s’affiche, contenant un module vide au centre.

   <!--picture?-->

1. Sélectionnez la variable **[!UICONTROL Nouveau scénario]** nom de l’espace réservé dans le coin supérieur gauche, puis saisissez un nom.
1. Passez à la [Ajouter et configurer le premier module](#add-and-configure-the-first-module) ci-dessous

### Ajouter et configurer le premier module

1. Cliquez sur le module vide pour choisir l’application à partir de laquelle vous allez sélectionner un module.

   Une liste d’applications s’affiche à droite du module.

1. Sélectionner **[!DNL Adobe Workfront]**. Si elle n’est pas visible, cliquez sur la barre de recherche située en bas de la liste, saisissez &quot;Workfront&quot;, puis sélectionnez-la lorsqu’elle apparaît dans la liste.

   La liste change pour afficher toutes les [!DNL Workfront] modules utilisables.

1. Cliquez sur le bouton **[!UICONTROL Rechercher]** module .

   La fenêtre de configuration du module s’ouvre.

1. Dans le [!UICONTROL Connexion] , sélectionnez votre connexion Workfront.

   Si vous ne disposez pas d’une connexion Workfront, voir [Créer une connexion à [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. Dans le [!UICONTROL Type d’enregistrement] , sélectionnez **[!UICONTROL Problème]**. Le module est ainsi configuré pour rechercher uniquement les problèmes.

   Vous pouvez trouver **[!UICONTROL Problème]** dans la liste si vous commencez à saisir le mot &quot;[!UICONTROL issue].&quot;

1. Dans le **[!UICONTROL Jeu de résultats]** , sélectionnez **[!UICONTROL Premier enregistrement correspondant]**.

   Cela définit le module pour renvoyer uniquement le premier enregistrement qui répond aux critères.
1. Dans le **[!UICONTROL Critères de recherche]** , configurez les critères pour renvoyer le problème spécifique.

   1. Dans la première zone sous [!UICONTROL Critères de recherche], sélectionnez le champ à inclure dans votre recherche. Pour cet exemple, sélectionnez **[!UICONTROL Nom]**.

      Vous pouvez trouver **[!UICONTROL Nom]** dans la liste si vous commencez à saisir le mot &quot;[!UICONTROL name].&quot;
   1. Pour l’opérateur, cliquez sur la flèche déroulante en regard de **Existe** et modifiez-le en [!UICONTROL **Contient (non-respect de la casse)**].

      Cela permet au module de rechercher des projets dont le nom contient les mots de votre choix, même si vous ne saisissez pas l’intégralité du nom, ou si vous saisissez le nom avec une casse incorrecte (toutes les majuscules, par exemple).
   1. Dans le dernier champ sous [!UICONTROL Critères de recherche], saisissez un mot ou une expression dont vous savez qu’il se trouve dans le nom du problème que vous recherchez.

1. Dans le **[!UICONTROL Sorties]** sélectionnez les champs que le module doit générer. Dans cet exemple, sélectionnez l’option **[!UICONTROL ID]** et **[!UICONTROL Nom]** des champs.

   >[!TIP]
   >
   >Vous pouvez utiliser **Cmd+F** ([!DNL Mac] OS) ou **Ctrl+F** ([!DNL Windows] Système d’exploitation) pour trouver rapidement un champ.

1. Cliquez sur **[!UICONTROL OK]** pour enregistrer la configuration du module.

1. Cliquez avec le bouton droit sur le module, puis cliquez sur **[!UICONTROL Renommer]**, puis saisissez un nom qui décrit ce que le module doit faire (par exemple &quot;Rechercher un problème&quot;), puis cliquez sur **[!UICONTROL OK]**.

   Le nom apparaît juste en dessous du module. En dessous : [!DNL Workfront Fusion] inclut une brève description du type d’action effectuée par le module.

   ![](assets/)

1. Passez à la [Ajouter et configurer le deuxième module](#add-and-configure-the-second-module).

## Ajouter et configurer le deuxième module

1. Pointez sur le cercle partiel à droite du module, puis cliquez sur **[!UICONTROL Ajouter un autre module]**.
1. Sélectionner [!DNL Adobe Workfront] dans la liste des applications, puis choisissez le module **[!UICONTROL Diverses actions]**.

   Le module Divers actes vous permet d’effectuer dans Workfront des actions qui ne comportent pas de module dédié. Dans cet exemple, ce module est utilisé pour convertir le problème en projet.
1. Dans le [!UICONTROL Connexion] , sélectionnez la même connexion Workfront que celle utilisée dans le module précédent .
1. Dans le **[!UICONTROL Type d’enregistrement]**, sélectionnez **[!UICONTROL Problème]**, car l’action à effectuer est liée à un problème.
1. Dans le **[!UICONTROL Action]** champ, sélectionnez **convertToProject**. Il s’agit de l’action qui convertira le problème sélectionné en projet.
1. Cliquez sur le bouton **[!UICONTROL ID]** champ .

   Un panneau s’ouvre. Il vous permet de sélectionner l’ID du problème que vous souhaitez convertir en projet. Le panneau comprend la sortie de tous les modules précédents. Comme vous avez sélectionné ID en tant que sortie du module précédent, il est désormais disponible dans le panneau .

   Ce panneau s’appelle le panneau de mappage. Pour plus d’informations sur le panneau de mappage, voir [Mise en correspondance des informations d’un module avec un autre](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Sélectionner **ID** dans le panneau de mappage.

   Un bloc ID apparaît dans le champ ID. Il indique le nombre du module à partir duquel il est mappé et le champ qui est mappé.

   ![ID de mappage](assets/map-id.png)

1. (Facultatif) Dans la section Projet, recherchez le champ ID de propriétaire et commencez à saisir votre nom dans le champ, puis sélectionnez-le lorsqu’il s’affiche. Vous serez ainsi le propriétaire du projet et vous pourrez trouver plus facilement dans Workfront.

   >[!TIP]
   >
   >Vous pouvez utiliser **Cmd+F** ([!DNL Mac] OS) ou **Ctrl+F** ([!DNL Windows] Système d’exploitation) pour trouver rapidement un champ.

1. Cliquez sur **[!UICONTROL OK]** pour enregistrer la configuration du module.

1. Cliquez avec le bouton droit sur le module, puis cliquez sur **[!UICONTROL Renommer]**, puis saisissez un nom qui décrit ce que le module doit faire (par exemple &quot;Convertir en projet&quot;), puis cliquez sur **[!UICONTROL OK]**.

1. Passez à [Test du scénario](#test-the-scenario).

## Test du scénario

Avant d’activer votre scénario, il est important de le tester en l’exécutant au moins une fois et en affichant les résultats. Vous pouvez ainsi comprendre le flux des données dans le scénario et rechercher les erreurs.

Pour ce scénario, un test réussi permet de localiser le problème et de le convertir en projet.

1. Cliquez sur **[!UICONTROL Exécuter une seule fois]** dans le coin inférieur gauche de l’éditeur de scénarios.
1. Une fois le scénario en cours d’exécution terminé, cliquez sur la bulle au-dessus du premier module pour afficher des informations sur le lot de données traité par le module, y compris les données extraites du problème renvoyé par le module.

1. Cliquez sur la bulle d’inspection d’exécution au-dessus du deuxième module pour voir l’entrée (le problème) et la sortie (le projet converti).

   Pour plus d’informations sur les données des bulles d’inspection, voir :

   * Pour obtenir des informations générales, voir [Flux d’exécution du scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Pour plus d’informations sur les lots traités, voir [Exécution, cycles et phases d’un scénario [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** près du coin inférieur gauche pour enregistrer la progression sur le scénario.

   >[!IMPORTANT]
   >
   >Enregistrez souvent lorsque vous affinez et testez un scénario.

>[!TIP]
>
>Nous recommandons la pratique facultative mais utile d’ajouter des notes sur chaque module.
>
>1. Cliquez avec le bouton droit sur un [!DNL Workfront] module, puis cliquez sur **[!UICONTROL Ajouter une note]**.
>1. Dans la note qui s’affiche, saisissez un aperçu du module.
>
>    Vous pouvez ajouter plusieurs notes pour un module.
>
>1. Fermez la **[!UICONTROL Remarques]** zone.
>
>     Après avoir ajouté une note à un scénario, un point orange s’affiche sur la page **[!UICONTROL Remarques]** icon ![](assets/notes-icon-w-dot.png) au bas de l’éditeur de scénario.
>
>1. Cliquez sur le bouton **[!UICONTROL Remarques]** icon ![](assets/notes-icon-w-dot.png) pour afficher vos notes.
>

## Activation du scénario

La dernière étape de la création d’un scénario consiste à l’activer.

Comme ce scénario recherche un problème spécifique, il n’est pas nécessaire de l’activer. L’activation d’un scénario entraîne son exécution selon un planning ou lorsqu’une action spécifique se produit dans une application. Une fois que vous avez activé un scénario, celui-ci s’exécute par défaut toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant quand et à quelle fréquence il doit s’exécuter.

Pour plus d’informations sur l’activation de scénarios, voir [Activez ou désactivez un scénario dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Pour plus d’informations sur les plannings, voir [Planification d’un scénario dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
