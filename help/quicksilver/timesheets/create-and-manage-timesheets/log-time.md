---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Enregistrer des heures
description: Vous pouvez consigner les heures consacrées aux éléments de travail Adobe Workfront à des fins de suivi. Vous pouvez également consigner les heures extra-professionnelles, comme les vacances, les congés maladie ou le temps passé en réunion. Les heures consignées s’affichent dans votre feuille de temps.
author: Alina
feature: Timesheets
role: User
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '3856'
ht-degree: 89%

---

# Enregistrer des heures

<!--Audited: 12/2023-->

<!--remove all preview and production references from this article with 23.3 release-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). 

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 
-->

Vous pouvez consigner les heures consacrées aux éléments de travail Adobe Workfront à des fins de suivi. Vous pouvez également consigner les heures extra-professionnelles, comme les vacances, les congés maladie ou le temps passé en réunion. Les heures consignées s’affichent dans votre feuille de temps.

Pour plus d’informations sur le type d’heures que vous pouvez consigner dans Workfront, consultez [Gérer les types d’heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Pour effectuer les étapes décrites dans cet article et consigner les heures spécifiques au projet, vous devez disposer de l’accès suivant :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : </p>
   <p>Clair ou plus pour consigner les heures sur un projet, une tâche, un problème ou les Heures générales sur une feuille de temps</p>
   <p>Actuel : 
   <ul><li>Révision ou supérieur pour consigner les heures générales dans une feuille de temps</li>
   <li>Travail ou supérieur pour consigner les heures liées à un projet, à une tâche ou à un problème</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès à la modification pour le type d’élément de travail pour lequel vous consignez les heures. </p> <p>À titre d’exemple, vous avez besoin de l’accès à la modification pour les problèmes si vous souhaitez consigner les heures liées à des problèmes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Contribuer ou des autorisations supérieures pour l’élément de travail pour lequel vous consignez des heures, y compris les autorisations de consignation des heures.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant la consignation des heures dans Workfront

* Vous pouvez consigner des heures pour des projets, des tâches ou des problèmes, ou vous pouvez consigner les heures directement dans votre feuille de temps.

  Pour plus d’informations sur la création de feuilles de temps, consultez la section [Créer une feuille de temps à usage unique](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* Les heures consignées par le biais d’outils autres que la feuille de temps apparaissent dans la feuille de temps à la période correspondante.
* Les tâches et les problèmes d’un projet qui n’est pas en cours ne sont pas prérenseignés dans une feuille de temps.
* Les heures consignées dans la feuille de temps sont immédiatement appliquées à la tâche, au problème ou au projet.
* Les feuilles de temps renseignent la durée totale pour toutes les dates consignées. Les week-ends sont toujours inclus, même si des calculs de la chronologie ont été configurés pour les exclure (comme décrit dans [Configurer les préférences de projet à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* Le nombre maximal d’éléments affichés dans une feuille de temps est de 45. S’il existe plus de 45 éléments dont les dates correspondent à la période de la feuille de temps, seuls les éléments les plus récemment mis à jour s’affichent.
* Les entrées correspondant aux enregistrements de facturation sont grisées et ne peuvent pas être modifiées dans la feuille de temps. Pour plus d’informations, consultez [Créer des enregistrements de facturation](../../manage-work/projects/project-finances/create-billing-records.md).
* Les tâches personnelles ne s’affichent pas par défaut sur la feuille de temps. Les tâches personnelles ne s’affichent dans la feuille de temps que lorsqu’elles ont été consignées. Après avoir consigné les heures dédiées à une tâche personnelle, vous pouvez épingler la tâche à la feuille de temps et elle restera sur la feuille de temps si elle reste épinglée. Pour plus d’informations, consultez [Créer des éléments de travail dans la zone Accueil](../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Enregistrer des heures {#log-time-section}

Vous pouvez consigner les heures dans les zones suivantes de Workfront :

* [Feuille de temps](#timesheet)
* [Accueil](#home)
* [Projet, tâche ou problème](#project-task-or-issue)
* [Panneau Résumé](#summary-panel)
* [Panneaux](#boards)
* [Application mobile](#mobile-app)

### Feuille de temps {#timesheet}

#### Consigner des heures sur une feuille de temps {#log-time-on-a-timesheet}

Vous pouvez consigner les heures pour les éléments suivants dans la feuille de temps :

* Tâches, problèmes et projets prérenseignés qui s’affichent automatiquement, en fonction de la manière dont votre administrateur ou administratrice Workfront définit les préférences de la feuille de temps. Pour plus d’informations sur la façon dont les feuilles de temps sont préremplies, consultez [Configurer les préférences des feuilles de temps et des heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  Uniquement les tâches et les problèmes qui vous sont affectés sont préremplis dans votre feuille de temps. Les tâches et les problèmes affectés à vos équipes ou à vos fonctions ne sont pas automatiquement repris dans votre feuille de temps.

  Sur un élément affecté à vos équipes, cliquez sur Travailler dessus pour vous l’attribuer et l’afficher dans votre feuille de temps.

* Tâches, problèmes ou projets que vous ajoutez manuellement.
* Tâches, problèmes ou projets pour lesquels vous avez déjà consigné des heures ailleurs dans Workfront.
* Durée générale (vacances, formation, durée supplémentaire).

>[!NOTE]
>
>Les réviseurs et réviseuses affectés à un profil de feuille de temps peuvent afficher la zone Feuilles de temps et consigner les heures générales. Cependant, ils ne peuvent pas consigner d’heures sur les tâches ou problèmes qui leur sont affectés et qui apparaissent sur la feuille de temps.

Pour consigner des heures sur une feuille de temps :

{{step1-click-main-menu}}

1. Cliquez sur Feuilles de temps. [!UICONTROL ****] Votre feuille de temps actuelle s’affiche par défaut.
   ![Feuille de temps](assets/timesheet-redesigned-nwe.png)


1. (Facultatif) Sélectionnez l’icône **Plein écran** ![](assets/full-screen.png) pour afficher la feuille de temps en mode plein écran et l’icône **Quitter le mode plein écran** ![](assets/exit-full-screen.png) pour revenir à la feuille de temps.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (Facultatif) Pour ajouter un projet, une tâche ou un problème à la feuille de temps, sélectionnez le menu déroulant **Ajouter un élément** dans le coin supérieur gauche de la feuille de temps, puis **Ajouter des projets**, **Ajouter des tâches** ou **Ajouter des problèmes**.

   Une liste de projets, de tâches ou de problèmes s’affiche.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (Facultatif) Cliquez sur l’icône de recherche ![Rechercher un élément](assets/search-icon.png) pour rechercher un élément spécifique à l’aide d’un mot-clé et l’ajouter à la feuille de temps.

1. (Facultatif) Développez les menus déroulants de filtrage, d’affichage ou de regroupement pour affiner votre sélection et afficher les informations sur l’élément de votre choix.

1. Sélectionnez un ou plusieurs éléments de la liste, puis cliquez sur **Ajouter**.

   Si vous avez ajouté moins de 50 éléments à la fois, ils sont ajoutés à la feuille de temps. Les tâches et les problèmes sont répertoriés sous le nom du projet.

   >[!NOTE]
   >
   >Lorsque vous ajoutez des tâches ou des problèmes à la feuille de temps, le projet est également ajouté.


1. (Le cas échéant) Si vous ajoutez 50 éléments ou plus à la fois, un message de confirmation affichant le nombre d’éléments ajoutés à votre feuille de temps s’affiche.

   Sélectionnez **Tout ajouter** pour ajouter tous les éléments,
ou
**Annuler** pour arrêter l’ajout des éléments sélectionnés, puis cliquez sur **Annuler** pour fermer la liste des éléments.

   Les tâches et les problèmes sont répertoriés sous le nom du projet.

   >[!NOTE]
   >
   >Les éléments que vous ajoutez manuellement à la feuille de temps sont épinglés sur les feuilles de temps actuelles et futures jusqu’à ce que vous les détachiez manuellement pour les supprimer. Pour plus d’informations sur la manière de détacher des éléments pour les supprimer de la feuille de temps, passez à l’étape 10.

   <!--(ensure this stays accurate)-->

1. (Facultatif) Cliquez sur les icônes **Réduire** ![](assets/collapse-icon.png) ou **Développer** ![](assets/expand-icon.png) en regard du nom du projet pour afficher ou masquer la liste des tâches et des problèmes du projet.


   >[!TIP]
   >
   >   À l’aide d’un clavier standard, utilisez les raccourcis clavier suivants pour réduire ou développer un projet. Cliquez sur le nom d’un projet dans la feuille de temps, puis procédez comme suit :
   >   * Pour développer le projet et afficher ses éléments de travail :
   >     * Maj+Alt+Touche Haut (sous Windows)
   >     * Maj+Option+Touche Haut (sous Mac)
   >   * Pour réduire le projet et masquer ses éléments de travail :
   >     * Maj+Alt+Touche Bas (sous Windows)
   >     * Maj+Option+Touche Bas (sous Windows)


1. (Facultatif) Pour épingler manuellement un élément qui s’affiche automatiquement sur la feuille de temps, pointez sur le nom de l’élément, puis cliquez sur l’icône **Épingler** ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   À l’aide d’un clavier standard, utilisez le raccourci clavier suivant pour épingler un élément. Cliquez sur un élément, puis procédez comme suit :
   >   * Option+P pour les ordinateurs Windows et Mac.


1. (Facultatif) Cliquez sur l’icône de recherche ![](assets/search-icon.png) et commencez à saisir un mot-clé pour rechercher un projet, une tâche ou un problème dans la feuille de temps.

1. (Facultatif) Si votre administrateur ou administratrice Workfront ou de groupes a activé le paramètre Attribuer manuellement des fonctions aux entrées d’heure, sélectionnez une fonction dans le menu déroulant. **** Le rôle spécifié lors de votre affectation à l’élément de travail s’affiche par défaut. Si aucune fonction ne vous est attribuée sur l’objet, votre rôle principal s’affiche par défaut. Pour plus d’informations sur ce paramètre, consultez l’article [Configurer les préférences de feuille de temps et d’heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![Consignation des heures de plusieurs rôles dans la feuille de temps](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (Facultatif) Cliquez sur l’icône **+** pour ajouter une autre ligne, puis sélectionnez un nouveau type d’heure dans le menu déroulant de la colonne [!UICONTROL Type d’heure] pour consigner des heures d’un autre type d’heure.

   ![Menu déroulant Type d’heure](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)


   >[!TIP]
   >
   >   À l’aide d’un clavier standard et en fonction de votre système d’exploitation ou de votre navigateur, utilisez le raccourci clavier suivant pour ajouter une autre ligne :
   >   * Ctrl+Option+« + »+pour les ordinateurs Windows
   >   * Cmd+Option+« + » pour les ordinateurs Mac

   Les types d’heures sont disponibles en fonction de ce qui a été défini au niveau du système, du projet et de l’utilisateur, comme décrit dans la section [Définition des types d’heures et disponibilité](define-hour-types-and-availability.md).

   Le type d’heure ne peut pas être modifié après la fermeture d’une feuille de temps.

   >[!TIP]
   >
   >Si vous avez précédemment consigné les heures et que le type d’heure sélectionné est maintenant désactivé, la ligne entière des heures consignées est grisée. Si vous sélectionnez un autre type d’heure et actualisez la page, l’option du type d’heure désactivée est supprimée de la liste déroulante. Vous ne pouvez donc pas ajouter d’heures supplémentaires à ce type d’heure.
   >
   >Envisagez d’ajouter une nouvelle ligne pour l’élément de travail pour lequel consigner les heures supplémentaires, puis de sélectionner un nouveau type d’heure pour conserver le type d’heure désactivé associé aux heures consignées dans le passé.

1. Cliquez sur l’icône **Supprimer** ![](assets/delete.png) en regard de la fonction à supprimer. Toutes les heures consignées pour le rôle sont également supprimées.

   >[!TIP]
   >
   >   Selon votre système d’exploitation ou navigateur, sur un clavier standard, appuyez sur l’ensemble de touches suivant pour supprimer une ligne :
   >   * Ctrl+Option+- pour les ordinateurs Windows
   >   * Cmd+Option+- pour les ordinateurs Mac

1. Spécifiez les heures à consigner chaque jour dans dans la section Chronologie de la feuille de temps, puis cliquez en dehors de la zone d’heure pour enregistrer l’entrée d’heure. Les heures sont enregistrées automatiquement. La ligne pour laquelle vous consignez les heures est mise en surbrillance en bleu clair et la zone de saisie de l’heure est indiquée en bleu foncé.

   ![Zone de consignation des heures dans la feuille de temps](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   Le temps consigné est exprimé en heures ou en jours. Ce paramètre est configuré par les utilisateurs et utilisatrices disposant d’une licence Plan, ou encore par l’administrateur ou l’administratrice système, comme décrit dans la section [Configurer la consignation du temps en heures ou en jours](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >Vous devez enregistrer manuellement la feuille de temps si l’un des scénarios suivants se produit :
   >
   >* La fonction associée au temps que vous avez précédemment consigné a changé et le paramètre **Affecter manuellement des fonctions aux entrées d’heure** a été désactivé. Le temps consigné pour les nouvelles dates est associé à une fonction différente.
   >   
   >   Si le rôle a été modifié et que le paramètre **Affecter manuellement des fonctions aux entrées d’heure** est activé, vous pouvez consigner le temps ou mettre à jour le rôle et vos modifications sont enregistrées automatiquement.
   >
   >* La fonction affectée à une tâche ou à un problème est différente de celle avec laquelle la personne propriétaire de la feuille de temps consigne le temps.<!--or assigned to them_ this last  piece came from a Support note but but sure what role it's referring to. Leaving it out for now.-->.
   >
   >La feuille de temps permet de gagner du temps automatiquement lorsqu’il n’y a plus d’entrées en conflit entre les deux rôles.
   >

1. (Facultatif) Indiquez le nombre d’heures supplémentaires dans le champ Heures supplémentaires de l’en-tête de la feuille de temps.

   >[!TIP]
   >
   >Vous ne pouvez pas consigner un nombre d’heures supplémentaires supérieur au nombre total actuel d’heures sur la feuille de temps. Par exemple, si jusqu’à présent, vous avez consigné 7 heures sur la feuille de temps, vous ne pouvez pas consigner 8 heures supplémentaires.

1. (Facultatif) Cliquez sur **Commentaire** pour ajouter un commentaire pour votre entrée d’heure.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Sur un clavier standard, après avoir cliqué sur la zone de saisie de l’heure, appuyez sur l’ensemble de touches suivant pour ouvrir la zone de commentaire :
   >   * Maj+F2 pour les ordinateurs Windows et Mac.

1. Cliquez sur **Terminé** pour enregistrer le commentaire.

   >[!TIP]
   >
   >   Sur un clavier standard, dans la zone de commentaire, appuyez sur l’ensemble de touches suivant pour enregistrer le commentaire :
   >   * Ctrl+Entrée pour les ordinateurs Windows.
   >   * Cmd+Retour pour les ordinateurs Mac.


1. (Facultatif) Cliquez sur **Afficher les commentaires** dans la barre d’outils pour afficher les commentaires d’entrée d’heure sous l’élément de travail.

   ![Commentaires répertoriés sous l’élément dans la feuille de temps](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Toutes les modifications que vous apportez à la feuille de temps sont enregistrées automatiquement.

1. (Facultatif) Cliquez sur la ligne d’une tâche ou d’un problème, puis cliquez sur Ouvrir le résumé dans le coin supérieur droit de la feuille de temps pour ajouter une mise à jour ou mettre à jour des informations sur la tâche ou le problème. **** Le panneau Résumé s’ouvre à droite.

   ![summary-panel-for-task-open-in-timesheet](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   Votre mise à jour s’affiche dans la zone Mises à jour de l’élément de travail associé au temps consigné.

   >[!TIP]
   >
   >Vous ne pouvez pas commenter les projets ni les entrées de durée générale.

1. Cliquez sur [!UICONTROL **Fermer le résumé**] pour fermer le panneau Résumé et revenir à la feuille de temps.

1. (Facultatif) Cliquez sur Mises à jour dans le panneau de gauche, puis ajoutez une mise à jour à la feuille de temps. [!UICONTROL ****] Pour plus d’informations sur les mises à jour de Workfront, voir [Mettre à jour le travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-redesigned-timesheet-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

1. (Facultatif) Revenez à la zone **Feuille de temps** pour fermer ou soumettre votre feuille de temps.

   * **Fermer** : fermez la feuille de temps lorsque vous l’avez mise à jour. Cette option n’est disponible que si votre feuille de temps n’est pas associée à un approbateur ou une approbatrice.

   * **Soumettre à approbation :** cette option est disponible uniquement si la feuille de temps est associée à un approbateur ou une approbatrice. Enregistrez vos modifications et soumettez-les pour approbation. Vous pouvez ouvrir la feuille de temps après l’avoir fermée en cliquant sur Rappeler, si aucune validation n’a encore été effectuée. **** Pour plus d’informations, consultez [Soumettre une feuille de temps à approbation](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **Refuser** : cette option s’affiche lorsque vous approuvez les feuilles de temps et que la feuille de temps vous a été envoyée pour approbation. En cliquant dessus, le statut de la feuille de temps passe à Refusé et la feuille de temps reste ouverte.

   * **Approuver : cette option s’affiche lorsque vous approuvez les feuilles de temps et que la feuille de temps vous a été envoyée pour approbation.** En cliquant dessus, le statut de la feuille de temps passe à Approuvé et ferme la feuille de temps.

   >[!TIP]
   >
   >Les options Refuser et Approuver s’affichent également sur votre feuille de temps lorsque vous êtes administrateur ou administratrice système et que la feuille de temps est associée à un approbateur ou une approbatrice.

1. (Le cas échéant) Si vous avez fermé ou envoyé votre feuille de temps pour approbation, cliquez sur l’une des options suivantes :

   * **Rouvrir : cette option est disponible pour les feuilles de temps que vous avez déjà fermées et qui n’ont pas d’approbateurs ou d’approbatrices, ou les feuilles de temps qui ont déjà été approuvées.** Rouvrez la feuille de temps pour modifier les entrées d’heure.
   * **Rappeler** : cette option est disponible pour les feuilles de temps qui ont été soumises à validation mais qui n’ont pas encore été approuvées ou refusées. Cliquez sur **Rappeler** pour rouvrir la feuille de temps et modifier les entrées d’heure.

#### Supprimer un élément de la feuille de temps

Vous pouvez supprimer une entrée d’heure ou un élément (projet, tâche ou problème) d’une feuille de temps.

Pour supprimer une entrée d’heure d’une feuille de temps :

1. Accédez à la feuille de temps et recherchez l’entrée d’heure à supprimer.
1. Remplacez les heures saisies par 0
ou
supprimez les heures et remplacez-les par 0, puis appuyez sur Entrée.

   Les heures sont supprimées et la feuille de temps est enregistrée automatiquement.

Vous pouvez supprimer un élément (projet, tâche ou problème) de la feuille de temps en l’annulant, si vous ne l’avez pas encore consigné et si vous avez ajouté manuellement l’élément (comme décrit aux étapes 4 à 8 dans la section [Consigner le temps sur une feuille de temps](#log-time-on-a-timesheet) dans cet article). <!--ensure this stays accurate-->

Vous ne pouvez pas supprimer automatiquement les éléments inclus dans la feuille de temps en fonction des préférences de la feuille de temps dans votre système Workfront ou groupe configuré pour préremplir la feuille de temps (comme décrit dans [Configurer des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)). Les éléments cessent de préremplir la feuille de temps lorsque les dates des éléments se trouvent en dehors de la période de la feuille de temps.

Pour supprimer un élément de la feuille de temps qui a été ajouté manuellement :

1. Assurez-vous qu’aucune heure n’est consignée pour l’élément.
1. Cliquez sur l’icône **Détacher** ![Épingler un élément](assets/pin-icon.png) en regard de l’élément pour détacher l’élément de la feuille de temps.

   >[!TIP]
   >
   >   Lors de l’utilisation d’un clavier standard après avoir cliqué sur un élément dans la feuille de temps, appuyez sur l’ensemble de touches suivant pour détacher un élément :
   > * Option+P pour les ordinateurs Windows et Mac.

   L’élément est supprimé de la feuille de temps après avoir actualisé la page.

### Page d’accueil {#home}

Vous pouvez consigner le temps spécifique au projet dans la page d’accueil.

Pour obtenir des informations générales sur l’utilisation de la zone Accueil, reportez-vous aux sections suivantes :

* Pour plus d’informations sur l’utilisation de la zone Accueil héritée, consultez [Utiliser la zone Accueil](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).
* Pour plus d’informations sur l’utilisation de la nouvelle zone Accueil, consultez [Prise en main du nouvel Accueil](../../workfront-basics/using-home/new-home/get-started-with-new-home.md).

#### Consigner le temps sur un élément de travail de la nouvelle zone Accueil

Vous pouvez consigner les heures consacrées aux tâches et aux problèmes dans un widget à l’aide du panneau Résumé de la zone Accueil. Pour plus d’informations, consultez la section [Panneau Résumé](#summary-panel) dans cet article.

En outre, pour enregistrer l’heure d’un élément dans le widget Mon travail :

1. Accédez à la zone **Accueil**.
1. Ajoutez le widget **Mon travail** à votre page Accueil.
1. (Facultatif) Sélectionnez une tâche, un problème ou une demande dans une liste, puis cliquez sur **Travailler dessus**.
1. Passez la souris sur la tâche ou le problème dont vous souhaitez consigner le temps, puis cliquez sur l’icône **Consigner le temps** ![](assets/log-time-icon-in-new-home.png) à droite des informations de la tâche.

   ![](assets/log-time-ui-for-task-from-new-home.png)

1. Cliquez sur **Consigner le temps**.

   Les heures consignées s’affichent dans la section Heures de l’objet, ainsi que dans votre feuille de temps.

#### Consigner le temps sur un élément de travail à partir de la zone Accueil héritée

1. Dans la zone **Liste de travaux**, sélectionnez l’élément sur lequel vous souhaitez consigner le temps.
1. Dans le panneau de droite, cliquez sur **Consigner le temps**.

   ![](assets/log-time-home-350x181.png)

1. Dans le menu déroulant **Saisir les heures**, sélectionnez le type d’heure approprié.\
   Les types d’heures sont disponibles en fonction de ce qui a été défini au niveau du système, du projet et de l’utilisateur, comme décrit dans la section [Définition des types d’heures et disponibilité](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (Facultatif) Si votre administrateur ou administratrice Workfront ou de groupes a activé le paramètre Attribuer manuellement des fonctions aux entrées d’heure, sélectionnez une fonction dans le menu déroulant. **** Le rôle spécifié lors de votre affectation à l’élément de travail s’affiche par défaut. Si aucune fonction ne vous est attribuée sur l’objet, votre rôle principal s’affiche par défaut. Pour plus d’informations sur ce paramètre, consultez l’article [Configurer les préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. Précisez le temps à consigner, puis cliquez sur **Consigner le temps**.

   Les heures consignées s’affichent dans la section Heures de l’objet, ainsi que dans votre feuille de temps.

### Projet, tâche ou problème {#project-task-or-issue}

Vous pouvez enregistrer l’heure spécifique d’un projet, d’une tâche ou d’un problème dans les sections suivantes :

* [Met à jour la section](#updates-section)
* [Section Heures](#hours-section)

#### Met à jour la section{#updates-section}

Pour consigner une heure dans la section Mises à jour d’un projet, d’une tâche ou d’un problème, vous devez disposer des éléments suivants :

* L’accès et les autorisations appropriés, comme décrit dans la section [Exigences d’accès](#access-requirements) de cet article.

* Votre administrateur ou administratrice de Workfront doit activer le paramètre Consigner les heures directement sur les projets sous [!UICONTROL **Feuille de temps et heures**]> [!UICONTROL **Préférences**] dans la zone Système, si vous souhaitez consigner les heures directement dans un projet.

  Pour plus d’informations sur l’autorisation des utilisateurs et utilistarices de consigner des heures directement dans des projets, consultez [Configurer les préférences de feuille de temps et d’heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Pour consigner une heure dans la section Mises à jour d’un projet, d’une tâche ou d’un problème :

1. Accédez à un projet, à une tâche ou à un problème.
1. Dans le panneau de gauche, sélectionnez **Mises à jour**.
1. Cliquez sur **Consigner le temps**. <!-- did Anna B change the casing for this button? If yes and if she changed it for the other areas, update screen shot too-->

   La boîte de dialogue Consigner le temps s’affiche.

   >[!TIP]
   >
   >   Si la préférence de votre profil est définie sur la consignation du temps en jours, la zone Saisir les jours s’affiche.
   >   
   >   Le nombre d’heures incluses dans une journée est indiqué, dans le coin supérieur droit de la zone Saisir les jours.

   ![](assets/log-time-box-in-updates-stream.png)

1. Indiquez les informations suivantes :

   * **Type d’heure** : sélectionnez un type d’heure dans le menu déroulant, s’il est différent de celui affiché par défaut.

     Selon les types d’heures configurés dans votre système, les options disponibles peuvent varier. Pour plus d’informations sur la configuration des types d’heures, voir [Définition des types d’heures et disponibilité](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Fonctions** : (le cas échéant) si votre administrateur ou administratrice Workfront ou de groupes a activé le paramètre **Affecter manuellement des fonctions aux entrées d’heure**, sélectionnez une **Fonction** dans le menu déroulant. La fonction spécifiée lorsque vous êtes la personne affectée à l’objet s’affiche par défaut. Si aucune fonction ne vous est attribuée sur l’objet, votre rôle principal s’affiche par défaut. Pour plus d’informations sur ce paramètre, consultez l’article [Configurer des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   * **Heures** : saisissez le nombre d’heures pour le projet, la tâche ou le problème.

1. Cliquez sur **Consigner le temps**.

   Les heures consignées s’affichent dans la section Heures de l’objet, ainsi que dans votre feuille de temps.

#### Section Heures{#hours-section}

Vous devez être un administrateur ou une administratrice Workfront pour consigner le temps pour les projets, tâches et problèmes dans la section Heures,

Ou

vous devez disposer de tous les éléments suivants :

* Une licence Plan avec accès administratif aux feuilles de temps et aux heures. Pour plus d’informations sur l’octroi de l’accès administratif aux feuilles de temps et aux heures, consultez [Octroyer aux utilisateurs et utilisatrices un accès administratif à certaines zones](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* Autorisations Contribuer ou supérieures pour le projet avec accès aux heures de journal. Pour plus d’informations sur l’octroi d’autorisations sur les projets, consultez [Partager un projet dans Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* Votre administrateur ou administratrice de Workfront doit activer le paramètre Consigner les heures directement sur les projets dans la section Feuille de temps et heures > Préférences de la zone Configuration, si vous souhaitez consigner les heures directement sur un projet. **** Pour plus d’informations sur l’autorisation des utilisateurs et utilisatrices de consigner des heures directement dans des projets, consultez [Configurer les préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Pour consigner du temps dans la section Heures d’un projet, d’une tâche ou d’un problème :

1. Accédez à un projet, à une tâche ou à un problème.
1. Dans le panneau de gauche, cliquez sur **Heures**.
1. Cliquez sur **Consigner le temps**.

   La boîte de dialogue Consigner les heures s’affiche.

1. Indiquez les informations suivantes :

   * **Personne propriétaire :** par défaut, votre nom s’affiche dans ce champ.\
     Si vous consignez les heures pour une autre personne, indiquez son nom.

   * **Type d’heure** : sélectionnez un type d’heure dans le menu déroulant, s’il est différent de celui affiché par défaut.

     Selon les types d’heures configurés dans votre système, les options disponibles peuvent varier. Pour plus d’informations sur la configuration des types d’heures, voir [Définition des types d’heures et disponibilité](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Fonctions** : (le cas échéant) si votre administrateur ou administratrice Workfront ou de groupes a activé le paramètre **Affecter manuellement des fonctions aux entrées d’heure**, sélectionnez une **Fonction** dans le menu déroulant. La fonction spécifiée lorsque vous êtes la personne affectée à l’objet s’affiche par défaut. Si aucune fonction ne vous est attribuée sur l’objet, votre rôle principal s’affiche par défaut. Pour plus d’informations sur ce paramètre, consultez l’article [Configurer des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     ![](assets/log-time-box-in-hours-section-on-task.png)
   * **Heures** : saisissez le nombre d’heures pour le projet, la tâche ou le problème.

1. Cliquez sur **Consigner le temps**.

### Panneau Résumé

Vous pouvez consigner les heures consacrées aux tâches et aux problèmes dans le panneau Résumé. Consultez la [Vue d’ensemble du panneau Résumé](../../workfront-basics/the-new-workfront-experience/summary-overview.md) pour plus d’informations.

![](assets/summary-hour-log.png)

### Panneaux {#boards}

Vous pouvez consigner les heures consacrées aux cartes connectées sur un panorama Workfront. Il s’agit du même processus que la consignation d’heures pour une tâche ou un problème, et les heures enregistrées sur la carte sont enregistrées sur la tâche connectée ou le problème connecté. Pour plus d’informations, consultez [Utiliser des cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### Application mobile {#mobile-app}

Vous pouvez consigner les heures à partir de l’application mobile Workfront. Pour plus d’informations, consultez [Adobe Workfront pour Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) ou [Adobe Workfront pour iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).

## Modification des heures de connexion dans les listes et les rapports

>[!CAUTION]
>
>* Vous ne pouvez pas modifier les entrées d’heure appartenant à une feuille de temps fermée. Vous devez d’abord rouvrir la feuille de temps, puis modifier les informations de saisie de l’heure.
>* Lorsque vous modifiez le type d’heure d’un type qui ne compte pas comme recettes à un autre type qui compte comme recettes, des modifications sont également apportées aux finances du projet. La modification des types Heure d’un type qui comptabilise comme recettes à un type qui ne compte pas comme recettes met également à jour les finances du projet.
>
>Pour plus d’informations, voir [Gestion des types d’heures](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).
>

Vous pouvez modifier les heures enregistrées dans les zones suivantes :

* Toutes les zones où vous avez ajouté des heures, y compris les feuilles de temps ouvertes
* Listes d’heures et rapports.

Vous pouvez modifier les éléments suivants d’une entrée d’heure lorsque vous modifiez une entrée d’heure dans une liste ou un rapport :

* Nombre d&#39;heures
* Type d’heure
* Rôle de tâche associé à l’entrée d’heure

Selon le type d’entrées d’heure que vous modifiez, les champs suivants peuvent être modifiés :

* Lorsque vous modifiez les heures spécifiques au projet :

   * Vous pouvez modifier le nombre d’heures.
   * Vous pouvez modifier le type d’heure uniquement en types spécifiques au projet.
   * Vous ne pouvez modifier l’affectation du rôle de tâche d’heure que si elle a été activée dans Configuration. Pour plus d’informations, voir [Configuration des préférences de feuille de temps et d’heure](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)

* Lorsque vous modifiez les heures générales :

   * Vous pouvez modifier le nombre d’heures.
   * Vous ne pouvez modifier le type d’heure que sur les types généraux.
   * Vous ne pouvez pas modifier l’affectation des rôles de tâche d’heure, car les heures générales ne peuvent pas être associées aux rôles.

* Lorsque vous modifiez un mélange d’heures générales et d’heures spécifiques au projet, en bloc :

   * Vous pouvez modifier le nombre d’heures.
   * Vous ne pouvez pas modifier le type d’heure, car les types d’heure généraux ne peuvent pas être modifiés en types spécifiques au projet et les types d’heure spécifiques au projet ne peuvent pas être modifiés en types généraux.
   * Vous ne pouvez pas modifier l’affectation des rôles de tâche, car les heures générales ne peuvent pas être associées aux rôles.
