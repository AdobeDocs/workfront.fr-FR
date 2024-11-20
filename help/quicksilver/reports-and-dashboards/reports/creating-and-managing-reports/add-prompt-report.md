---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Ajouter une invite à un rapport
description: Les filtres et les invites sont similaires dans la mesure où ils limitent tous deux la quantité d’informations que vous affichez dans un rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 9396cd2ac073a57b7d99618cdf09e54ddcf95130
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 83%

---

# Ajouter une invite à un rapport

<!-- Audited: 11/2024 -->

## Différence entre les invites et les filtres

Les filtres et les invites sont similaires dans la mesure où ils limitent tous deux la quantité d’informations que vous affichez dans un rapport.

Vous créez un filtre afin que les informations affichées dans le rapport soient filtrées selon les mêmes critères à chaque exécution du rapport. Les filtres sont créés une seule fois et codés en dur dans le rapport. Pour plus d’informations sur la création de filtres, voir l’article [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Les invites sont des filtres ouverts qui peuvent être personnalisés et appliqués différemment chaque fois que vous exécutez un rapport.

Lorsque vous ajoutez des invites à votre rapport, vous pouvez personnaliser les informations de filtrage en modifiant les critères d’invite à chaque exécution du rapport. Le rapport s’exécute avec un filtre différent à chaque fois, selon les modificateurs que vous choisissez, au lieu de coder en dur les modificateurs une fois dans le filtre du rapport.

Les invites agissent comme un filtre personnalisable sur les rapports qui peuvent être mis à jour juste avant l’exécution du rapport. Vous pouvez créer des rapports génériques, puis affiner les résultats en fonction des informations que vous souhaitez afficher pour cette journée ou des informations pertinentes pour un ensemble de critères qui vous sont propres. Par exemple, si vous disposez d’un rapport Heures et que vous souhaitez modifier les informations du rapport en fonction des critères suivants :

* Dates auxquelles les heures ont été consignées
* Utilisateurs et utilisatrices qui ont renseigné les heures
* Nombre d’heures renseignées

Vous allez créer trois invites où les conditions sont les critères requis et le rapport sera différent chaque fois que vous l’exécuterez, selon les informations que vous choisirez pour vos invites.

Un filtre peut indiquer à Adobe Workfront de n’afficher que les heures renseignées entre juin et août de cette année. Toutefois, vous pouvez utiliser une période différente chaque fois que vous exécutez le rapport (par exemple, entre janvier et février ou entre octobre et décembre).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
    <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et regroupements</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet*</td> 
   <td> <p>Gérer les autorisations d’un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Vous devez créer un rapport avant d’y ajouter une invite.

Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Créer une invite

1. Accédez au rapport auquel vous souhaitez ajouter une invite.
1. Développez **Actions de rapport**, puis cliquez sur **Modifier**.

1. Cliquez sur le bouton **Paramètres de rapport** .
1. Cliquez sur l’onglet **Report Invite** , puis sur **Ajouter une invite**.\
   ![](assets/create-report-prompt-tab.png)

1. (Le cas échéant) Sélectionnez le champ sur lequel vous souhaitez que l’invite soit basée. Commencez à saisir le nom du champ, puis cliquez pour le sélectionner lorsqu’il apparaît dans la liste.\
   Les options disponibles pour les utilisateurs et les utilisatrices qui exécutent le rapport varient en fonction du champ sélectionné.\
   Par exemple, si vous sélectionnez un champ de date tel que Date d’achèvement effective dans un rapport de tâche, « Date d’achèvement effective » est le nom de l’invite. Lorsque vous modifiez cette invite pendant l’exécution de ce rapport, vous pouvez choisir parmi un ensemble de modificateurs pour créer votre instruction de filtrage. Ce processus est identique à la création d’un filtre. Pour plus d’informations sur les modificateurs, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Le cas échéant) Cliquez sur **Invite personnalisée** pour créer une invite personnalisée.

   Une invite personnalisée est une invite prédéfinie dans laquelle vous codez en dur les critères de filtrage avant d’exécuter le rapport. En ce sens, une invite personnalisée est plus proche d’un filtre que d’une invite.

   Cependant, l’invite reste aussi flexible qu’une invite ordinaire, car vous pouvez choisir parmi plusieurs instructions prédéfinies, au lieu de ne disposer que d’un seul filtre codé en dur dans le rapport.

   Renseignez les informations suivantes pour l’invite personnalisée : la condition d’une invite personnalisée ne peut être modifiée qu’en mode texte. Cela permet d’appliquer plusieurs conditions dans un seul champ.

   * **Nom du champ :** il s’agit du nom de l’invite tel qu’il s’affiche avant l’exécution du rapport.
   * **Libellé de l’élément de liste déroulante :** Il s’agit du nom de l’une des options de l’invite telle qu’elle s’affiche avant l’exécution du rapport.
   * **Condition :** saisissez une condition qui définit l’invite.
   * **Par défaut :** Vous pouvez sélectionner un élément pour être l’option par défaut de cette invite.

   Utilisez la même syntaxe que celle que vous utiliseriez lors de la saisie d’un filtre de mode texte et joignez vos instructions par « &amp; ». Pour plus d’informations sur la modification d’un filtre en mode texte, voir [Modifier un filtre à l’aide du mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   Par exemple, le champ **Condition** de l’invite personnalisée pour les scénarios suivants peut se présenter comme suit :

   * Toutes les tâches sur les projets futurs pour lesquels le statut du projet est Idée, Demandé, Prévu et Actuel :

     ```
     project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
     ```

   * Toutes les tâches des projets terminés (précédents) pour lesquels le statut du projet est Terminé ou Inactif :

     ```
     project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
     ```

   Pour plus d’informations sur les modificateurs de mode texte, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Vous ne pouvez pas modifier les conditions d’une invite personnalisée lors de l’exécution du rapport comme vous le feriez avec une invite standard. Vous pouvez avoir autant de conditions prédéfinies pour une invite personnalisée que nécessaire.

1. (Facultatif) Répétez l’étape 4 ou 5 pour créer autant d’invites que nécessaire.
1. Cliquez sur **Terminé**, puis sur **Enregistrer et fermer** pour enregistrer le rapport.

## Appliquer une invite à un rapport

Lorsqu’une invite est ajoutée à un rapport, l’onglet par défaut du rapport est toujours l’onglet Invites.

Pour exécuter un rapport avec une invite :

1. Accédez au rapport à l’aide de l’invite.

   ![](assets/run-report-prompts.png)

1. Choisissez une condition pour l’une ou toutes les invites affichées dans l’onglet **Invites**.\
   (Facultatif) Vous pouvez laisser les invites vides et ne pas filtrer le rapport selon les conditions d’invite.

1. Cliquez sur **Exécuter le rapport**.\
   (Le cas échéant) Si vous avez renseigné les invites, le rapport est filtré selon les conditions que vous avez choisies pour vos invites.\
   (Le cas échéant) Si vous laissez les invites vides, le rapport n’est pas filtré selon les conditions d’invite. Le rapport s’affiche comme s’il n’avait pas été filtré.

   >[!NOTE]
   >
   >Un rapport qui contient un filtre en plus d’une invite filtre les résultats en fonction à la fois des critères définis dans le filtre et de l’invite.

## Limites du partage des rapports contenant des invites

>[!CAUTION]
>
>Lorsque vous partagez un rapport invité, les utilisateurs connectés et non connectés qui visualisent le rapport à l’aide du lien de partage public ne peuvent pas exécuter le rapport à l’aide de ses invites. Dans ce cas, les résultats du rapport s’affichent sans appliquer d’invites. Les informations affichées seront alors basées sur le niveau d’accès et les autorisations de l’utilisateur, ou sur le niveau d’accès et les autorisations Exécuter en tant qu’utilisateur du rapport, si un niveau est défini.

Les restrictions suivantes s’appliquent au partage de rapports contenant des invites à partir de Workfront :

* Lorsque vous partagez un rapport publiquement, les utilisateurs ne peuvent pas exécuter le rapport avec des invites appliquées, sauf s’ils disposent : des informations d’identification Workfront, se connectent en premier et accèdent directement au rapport dans Workfront (et non via le lien de partage public).

  Pour plus d’informations sur le partage de rapports, consultez l’article [Partager un rapport dans Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

* Lorsque vous planifiez la remise d’un rapport invité, le rapport en pièce jointe inclut les données du rapport sans invite. Lorsque la personne clique sur le lien contenu dans l’e-mail pour accéder au rapport, elle doit d’abord se connecter pour afficher le rapport et lancer l’invite.

  Pour plus d’informations sur la planification d’une remise de rapport, voir [Planifier la remise automatique d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).
