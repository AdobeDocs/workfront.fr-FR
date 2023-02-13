---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Ajout d’une invite à un rapport
description: Les filtres et les invites sont similaires dans la mesure où ils limitent tous deux la quantité d’informations que vous affichez dans un rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# Ajout d’une invite à un rapport

## Différence entre les invites et les filtres

Les filtres et les invites sont similaires dans la mesure où ils limitent tous deux la quantité d’informations que vous affichez dans un rapport.

Vous créez un filtre afin que les informations affichées dans le rapport soient filtrées selon les mêmes critères à chaque exécution du rapport. Les filtres sont créés une seule fois et codés en dur dans le rapport. Pour plus d’informations sur la création de filtres, voir l’article [Présentation des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Les invites sont des filtres ouverts qui peuvent être personnalisés et appliqués différemment chaque fois que vous exécutez un rapport.

Lorsque vous ajoutez des invites à votre rapport, vous pouvez personnaliser les informations de filtrage en éditant les critères d’invite à chaque exécution du rapport. Le rapport s’exécute avec un filtre différent à chaque fois, selon les modificateurs que vous choisissez, au lieu de coder en dur les modificateurs une fois dans le filtre du rapport.

Les invites agissent comme un filtre personnalisable sur les rapports qui peuvent être mis à jour juste avant l’exécution du rapport. Vous pouvez créer des rapports génériques, puis affiner les résultats en fonction des informations que vous souhaitez afficher pour cette journée ou des informations pertinentes pour un ensemble de critères qui vous sont propres. Par exemple, si vous disposez d’un rapport Heures et que vous souhaitez modifier les informations du rapport en fonction des critères suivants :

* Les dates auxquelles les heures ont été consignées
* Les utilisateurs qui ont participé aux heures
* Le nombre d’heures saisies

Vous allez créer trois invites où les conditions sont les critères requis et le rapport sera différent chaque fois que vous l’exécutez, selon les informations que vous choisissez pour vos invites.

Un filtre peut indiquer à Adobe Workfront de n’afficher que les heures entrées entre juin et août de cette année. Toutefois, vous pouvez utiliser une période différente chaque fois que vous exécutez le rapport (par exemple, entre janvier et février ou octobre et décembre).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Vous devez créer un rapport avant d’y ajouter une invite.

Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## Création d’une invite

1. Accédez au rapport dans lequel vous souhaitez ajouter une invite.
1. Développer **Actions de rapport**, puis cliquez sur **Modifier**.

1. Cliquez sur **Paramètres des rapports**.
1. Dans le **Invite de rapports** zone, cliquez sur **Ajouter une invite**.\
   ![](assets/qs-add-a-prompt-350x216.png)

1. (Conditionnel) Sélectionnez le champ sur lequel vous souhaitez que l’invite soit basée. Commencez à saisir le nom du champ, puis cliquez pour le sélectionner lorsqu’il apparaît dans la liste.\
   Les options disponibles pour les utilisateurs qui exécutent le rapport varient en fonction du champ sélectionné.\
   Par exemple, si vous sélectionnez un champ de date tel que Date de fin réelle dans un rapport de tâche, &quot;Date de fin réelle&quot; est le nom de l’invite. Lorsque vous modifiez cette invite pendant l’exécution de ce rapport, vous pouvez choisir parmi un ensemble de modificateurs pour créer votre instruction de filtrage. Ce processus est identique à la création d’un filtre. Pour plus d’informations sur les modificateurs, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Conditionnel) Cliquez sur **Invite personnalisée** pour créer une invite personnalisée.

   Une invite personnalisée est une invite prédéfinie dans laquelle vous codez en dur les critères de filtrage avant d’exécuter le rapport. En ce sens, une invite personnalisée est plus proche d’un filtre que d’une invite.

   Cependant, l’invite reste aussi flexible qu’une invite ordinaire, car vous pouvez choisir parmi plusieurs instructions prédéfinies, contrairement à un seul filtre codé en dur dans le rapport.

   Spécifiez les informations suivantes pour l’invite personnalisée : La condition d’une invite personnalisée ne peut être modifiée qu’en mode texte. Cela permet d’appliquer plusieurs conditions dans un seul champ.

   * **Nom du champ :** Il s’agit du nom de l’invite, comme vous le voyez avant d’exécuter le rapport.
   * **Libellé :** Il s’agit du nom d’une des options de l’invite telles qu’elle s’affiche avant l’exécution du rapport.
   * **Condition :** Saisissez une condition qui définit l’invite.

   Utilisez la même syntaxe que celle que vous utiliseriez lors de la saisie d’un filtre de mode texte et joignez vos instructions par &quot;&amp;&quot;. Pour plus d’informations sur la modification d’un filtre en mode texte, voir [Modification d’un filtre à l’aide du mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   Par exemple, la variable **Condition** de l’invite personnalisée pour les scénarios suivants peut se présenter comme suit :

   * toutes les tâches sur les projets futurs pour lesquels l’état du projet est Idée, Demandée, Planifiée et Actuelle :

      ```
      project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
      ```

   * toutes les tâches des projets terminés (précédents) pour lesquels l’état du projet est Terminé ou Mort :

      ```
      project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
      ```
   Pour plus d’informations sur les modificateurs de mode texte, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Vous ne pouvez pas modifier les conditions d’une invite personnalisée lors de l’exécution du rapport, comme vous le feriez avec une invite standard. Vous pouvez avoir autant de conditions prédéfinies pour une invite personnalisée que nécessaire.

1. (Facultatif) Répétez l’étape 4 ou 5 pour créer autant d’invites que nécessaire.
1. Cliquez sur **Terminé**, puis cliquez sur **Enregistrer + Fermer** pour enregistrer le rapport.

## Application d’une invite à un rapport

Lorsqu&#39;une invite est ajoutée à un rapport, l&#39;onglet par défaut du rapport est toujours l&#39;onglet Invite .

Pour exécuter un rapport avec une invite :

1. Accédez au rapport à l’aide de l’invite .

   ![](assets/qs-prompt-drop-downs-350x229.png)

1. Sélectionnez une condition pour l’un ou tous les messages affichés sur la page **Invitations** .\
   (Facultatif) Vous pouvez laisser les invites vides et ne pas filtrer le rapport selon les conditions d’invite.

1. Cliquez sur **Exécuter le rapport**.\
   (Conditionnel) Si vous avez renseigné les invites, le rapport est filtré selon les conditions que vous avez choisies pour vos invites.\
   (Conditionnel) Si vous laissez les invites vides, le rapport n’est pas filtré selon les conditions d’invite. Le rapport s’affiche comme s’il n’avait pas été filtré.

   >[!NOTE]
   >
   >Un rapport qui contient un filtre en plus d’une invite filtre les résultats en fonction des critères définis dans le filtre et de l’invite combinée.

## Limites du partage des rapports demandés

>[!CAUTION]
>
>Lorsque vous partagez un rapport invité en dehors de Workfront, l’utilisateur qui le consulte doit être connecté à Workfront pour exécuter le rapport à l’aide de l’invite. Si l’utilisateur qui consulte le rapport n’est pas connecté, tous les résultats du rapport s’affichent sans application de l’invite.

Les restrictions suivantes s’appliquent au partage de rapports générés à partir de Workfront :

* Lorsque vous partagez un rapport publiquement, les utilisateurs ne peuvent pas l’exécuter en appliquant l’invite, sauf s’ils disposent des informations d’identification Workfront et se connectent d’abord pour afficher le rapport dans Workfront.

   Pour plus d’informations sur le partage de rapports, reportez-vous à l’article [Partage d’un rapport dans Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
* Lorsque vous planifiez la remise d’un rapport invité, le rapport en pièce jointe inclut les données du rapport demandées. Lorsque l&#39;utilisateur clique sur le lien contenu dans l&#39;email pour accéder au rapport, il doit d&#39;abord se connecter pour afficher le rapport et lancer lui-même l&#39;invite.

   Pour plus d’informations sur la planification d’un rapport remis, voir [Planifier la remise automatique d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).
