---
title: Rapport sur la zone Mises à jour
description: Rapport sur la zone Mises à jour
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '2686'
ht-degree: 3%

---

# Rapport sur la zone Mises à jour

Le rapport Entrée de journal répertorie les mises à jour système de la zone Mises à jour des projets, tâches, problèmes et autres objets qui n’étaient auparavant disponibles que par le biais de l’API Adobe Workfront. Bien qu’il s’agisse d’un rapport avancé destiné à des cas d’utilisation spécifiques, le format plus digestible facilite la création de rapports sur l’activité de projet et les mises à jour système dans Workfront.

>[!TIP]
>
>Le rapport Entrée de journal contient uniquement des mises à jour système de la zone Mises à jour des objets. Pour signaler les commentaires laissés dans la zone Mises à jour, vous devez utiliser le rapport Remarque .\
>Pour plus d’informations sur le rapport Remarque, voir [Afficher toutes les mises à jour d’un rapport Remarque](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md)‍

Le rapport Entrée de journal peut afficher :

* Nombre de modifications d’état survenues
* Lorsqu’une tâche ou un problème a été supprimé
* Modification des valeurs de champs personnalisés importants au cours du cycle de vie d’un projet
* Quelles dates importantes ont changé au cours du cycle de vie d’un projet ?
* Si le propriétaire d’un projet a changé

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
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
   <td> <p>Afficher les autorisations pour les objets qui contiennent les entrées de journal que vous affichez dans le rapport</p> <p>Une fois le rapport créé, vous obtiendrez les autorisations de gestion .</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant d’effectuer les actions décrites dans cet article, vous devez vous assurer des éléments suivants :

* Tous les champs sur lesquels vous souhaitez créer des rapports sont suivis dans Workfront. Vous pouvez uniquement générer des rapports sur les données de la zone Mises à jour qui est suivie.

  Pour savoir comment ajouter des champs dont Workfront doit effectuer le suivi, voir [Configuration des mises à jour du système](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* Tout champ personnalisé sur lequel vous souhaitez créer des rapports comporte le paramètre . **Afficher les modifications de champ dans les flux de mise à jour** activée.

  Pour savoir comment activer ce paramètre pour un champ personnalisé, consultez la section [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) dans l’article [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Rapport d’entrée de journal - Aperçu

Comme le système de requêtes de saisie du journal est mis à jour, il peut renvoyer un nombre important de résultats. C’est pourquoi il est recommandé de filtrer des objets spécifiques (projets, programmes, portefeuilles, groupes, etc.) lors de la création du rapport.

Pour en savoir plus sur les différents types d’objets dans Workfront, voir [Présentation des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Le rapport Entrée de journal renvoyant une telle quantité de données, l’exportation et la remise de rapports planifiés ne sont pas prises en charge.

La vue par défaut de ce rapport contient les colonnes suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>champ</th> 
   <th>Explication</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Nom du champ</strong> </td> 
   <td> <p><span style="font-weight: normal;">Nom du champ affecté. Selon la configuration du rapport, cette colonne peut contenir État, ID de propriétaire, Nom de la tâche, Date d’achèvement prévue ou d’autres champs.</span> </p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> s’affiche dans cette colonne, ce qui indique que le champ répertorié est un champ personnalisé.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>Type de modification</strong> </td> 
   <td> <p>Type de modification apportée au champ concerné. Selon les règles de filtrage que vous configurez et les actions entreprises par les utilisateurs, les éléments suivants peuvent apparaître dans ce champ :</p> 
    <ul> 
     <li> <p>Ajouter</p> </li> 
     <li> <p>Audit</p> </li> 
     <li> <p>Supprimer</p> </li> 
     <li> <p>Synthèse</p> </li> 
     <li> <p>Modifier</p> </li> 
     <li> <p>Restaurer</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Code Obj supérieur</strong> </td> 
   <td> <p>Objet parent le plus élevé de la hiérarchie.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Portée</strong> </td> 
   <td> <p>Le type d’objet qui a été modifié.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Date d’entrée</strong> </td> 
   <td> <p>Date à laquelle le champ a été modifié.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Modifié par nom</strong> </td> 
   <td> <p>L’utilisateur qui a modifié le champ.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour organiser les informations de ce rapport, vous pouvez utiliser le regroupement intégré Projet. Le regroupement Projet vous donne un regroupement principal Nom du projet et un regroupement secondaire Date d’entrée. Vous pouvez appliquer ce groupement existant lors de la création du rapport ou l&#39;appliquer lors de la consultation du rapport.

Pour savoir comment configurer les vues, les filtres et les regroupements que vous souhaitez pour votre rapport, reportez-vous à la section correspondante :

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [Afficher les modifications d’état](#see-what-status-changes-occurred)
* [Afficher le moment où une tâche ou un problème a été supprimé](#see-when-a-task-or-issue-was-deleted)
* [Découvrez comment les champs personnalisés ont changé au cours du cycle de vie d’un projet](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [Afficher la modification de la date d’achèvement prévue au cours du cycle de vie d’un projet](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [Vérification de la modification du propriétaire d’un projet](#see-if-the-owner-of-a-project-changed)

## Afficher les modifications d’état {#see-what-status-changes-occurred}

Vous pouvez configurer le rapport Entrée de journal pour qu’il affiche :

* Nombre de modifications d’état apportées à un projet, à une tâche ou à un problème

* Quel était l’état précédent avant la modification ?
* Qui a modifié l’état
* Lorsque le changement d’état a eu lieu

Si vous souhaitez afficher l’intégrité d’un projet, vous pouvez également configurer le rapport afin d’afficher les mêmes informations à l’aide du projet. **Condition** champ .

Ces informations peuvent être utilisées pour faciliter les audits et pour illustrer la planification effectuée par vous-même et votre organisation.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>Si vous souhaitez comparer la différence en jours entre les modifications de condition, vous pouvez utiliser l’analyse améliorée.\
>Pour en savoir plus sur les analyses améliorées, voir [Présentation des analyses améliorées](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Entrée du journal**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Le créateur de rapports se charge.

1. Dans le **Colonnes (affichage)** , ajoutez les colonnes suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Colonnes</th> 
      <th>Explication</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nom de champ</p> </td> 
      <td> <p>Nom du champ affecté. Dans ce cas, <strong>status</strong> doit s’afficher dans cette colonne.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modifier le type</p> </td> 
      <td> <p>Le type de modification apportée au champ affecté, par exemple <strong>Ajouter</strong>, <strong>Supprimer</strong>, ou <strong>Modifier</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modifié par nom</p> </td> 
      <td> <p>Nom de l’utilisateur qui a mis à jour l’état.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Date d’entrée</p> </td> 
      <td> <p>Date à laquelle l’état a été modifié.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ancienne valeur du texte</p> </td> 
      <td> <p>Clé du statut précédent. Voici les clés d’état des états du projet par défaut :</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: actuel</p> </li> 
        <li> <p><strong>DED</strong>: Mort</p> </li> 
        <li> <p><strong>ONH</strong>: actif</p> </li> 
        <li> <p><strong>PLN</strong>: planification</p> </li> 
        <li> <p><strong>CPL</strong>: terminé</p> </li> 
        <li> <p><strong>REQ</strong>: demandé</p> </li> 
        <li> <p><strong>APR</strong>: Approuvé</p> </li> 
        <li> <p><strong>REJ</strong>: refusé</p> </li> 
        <li> <p><strong>IDA</strong>: Idée</p> </li> 
       </ul> <p>Si votre organisation a configuré des états personnalisés, d’autres clés d’état peuvent apparaître dans cette colonne. Pour savoir quel état personnalisé est associé à une clé d’état, contactez votre administrateur Workfront ou votre administrateur de groupe.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nouvelle valeur de texte</p> </td> 
      <td> <p>Clé du statut mis à jour.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Code objet supérieur</p> </td> 
      <td> <p>Objet parent le plus élevé pour le champ dont l’état a été modifié.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Étendue</p> </td> 
      <td> <p>Type d’objet dont l’état a changé.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nom du problème<br>(Facultatif)</p> </td> 
      <td> <p>Nom du problème qui a été modifié.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Task Name<br>(Facultatif)</p> </td> 
      <td> <p>Nom de la tâche qui a changé d’état.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Pour plus d’informations sur l’ajout de colonnes, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Dans le **Filtres** , cliquez sur **Ajouter une règle de filtre**, puis ajouter la règle de filtrage **Nom du champ** > **Égal** > **status**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >Pour créer des rapports sur les modifications de condition, vous pouvez ajouter la règle de filtrage. **Nom du champ** > **Égal** > **Condition**.

   Pour plus d’informations sur l’ajout de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facultatif) Pour cibler davantage le rapport et réduire les temps de chargement, ajoutez une invite.

   Ou

   Créez des règles de filtrage supplémentaires pour inclure des projets, des tâches ou des problèmes spécifiques.

   >[!IMPORTANT]
   >
   >Création d’une règle de filtrage qui utilise le modificateur **Contient** peut augmenter les temps de chargement. Pour cette raison, nous vous recommandons d’utiliser un autre modificateur, comme **Égal** si possible, filtrez pour un projet spécifique ou un identifiant d’objet de niveau supérieur.

   Pour savoir comment ajouter une invite, voir [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Dans le **Groupements** , cliquez sur **Appliquer un groupement existant**, puis sélectionnez **Projet**.

   Pour plus d’informations sur l’ajout de groupements, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Cliquez sur **Enregistrer + Fermer**.

   Votre nouveau rapport se charge.

## Afficher le moment où une tâche ou un problème a été supprimé {#see-when-a-task-or-issue-was-deleted}

Vous pouvez configurer le rapport Entrée de journal pour qu’il affiche :

* Tâches ou problèmes supprimés
* Qui a supprimé une tâche ou un problème

Pour savoir quand une tâche ou un problème a été supprimé :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Entrée du journal**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Le créateur de rapports se charge.

1. Dans le **Colonnes (affichage)** , ajoutez les colonnes suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Colonnes</th> 
      <th>Explication</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Étendue</p> </td> 
      <td> <p>Type d’objet qui a été supprimé.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modifier le type</p> </td> 
      <td> <p>Le type de changement qui s’est produit. La variable <strong>Supprimer</strong> change s’affiche dans cette colonne.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Date d’entrée</p> </td> 
      <td> <p>Date à laquelle la tâche ou le problème a été supprimé.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modifié par nom</p> </td> 
      <td> <p>Nom de l’utilisateur qui a supprimé la tâche ou le problème.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nom du projet</p> </td> 
      <td> <p>Nom du projet pour lequel des tâches ou des problèmes ont été supprimés.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Pour plus d’informations sur l’ajout de colonnes, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Dans le **Filtres** , cliquez sur **Ajouter une règle de filtre**, puis ajoutez ce qui suit :

   * **Type de modification** > **Égal** > **Supprimer**
   * **Identifiant de projet** > **Égal** > **`<project>`**

     <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   Pour plus d’informations sur l’ajout de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facultatif) Pour cibler davantage le rapport et réduire les temps de chargement, ajoutez une invite.

   Ou

   Créez des règles de filtrage supplémentaires pour inclure des projets, des tâches ou des problèmes spécifiques.

   >[!IMPORTANT]
   >
   >Création d’une règle de filtrage qui utilise le modificateur **Contient** peut augmenter les temps de chargement. Pour cette raison, nous vous recommandons d’utiliser un autre modificateur, comme **Égal** si possible, filtrez pour un projet spécifique ou un identifiant d’objet de niveau supérieur.

   Pour savoir comment ajouter une invite, voir [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Facultatif) Dans la variable **Groupements** , cliquez sur **Appliquer un groupement existant**, puis sélectionnez **Projet**.

   Pour plus d’informations sur l’ajout de groupements, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Cliquez sur **Enregistrer + Fermer**.

   Votre nouveau rapport se charge.

## Découvrez comment les champs personnalisés ont changé au cours du cycle de vie d’un projet {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

Vous pouvez effectuer le suivi des modifications importantes apportées aux champs au cours du projet. Pour ce faire, vous pouvez configurer l’entrée du journal pour effectuer le suivi :

* Si certains champs personnalisés ont été ajoutés, mis à jour ou modifiés
* Lorsque ces modifications se sont produites
* Qui a apporté les modifications

Pour découvrir comment les champs personnalisés ont changé au cours du cycle de vie d’un projet :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Entrée du journal**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Le créateur de rapports se charge.

1. Dans le **Colonnes (affichage)** , ajoutez les colonnes suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Colonnes</th> 
      <th>Explication</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nom de champ</p> </td> 
      <td> <p>Nom du champ personnalisé affecté.</p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> s’affiche dans cette colonne, ce qui indique que le champ répertorié est un champ personnalisé.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modifier le type</p> </td> 
      <td> <p>Le type de modification apportée au champ affecté, par exemple <strong>Ajouter</strong>, <strong>Supprimer</strong>, ou <strong>Modifier</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modifié par nom</p> </td> 
      <td> <p>Nom de l’utilisateur qui a mis à jour le champ personnalisé.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Date d’entrée</p> </td> 
      <td> <p>Date à laquelle la valeur du champ personnalisé a changé.</p> <p>Vous devez trier par ce champ dans l’ordre décroissant.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ancienne valeur numérique</p> </td> 
      <td> <p>La valeur du nombre précédent dans le champ personnalisé.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nouvelle valeur numérique</p> </td> 
      <td> <p>La valeur du nombre actuel dans le champ personnalisé.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ancienne valeur de la date</p> </td> 
      <td> <p>La valeur de date précédente dans le champ personnalisé.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nouvelle valeur de date</p> </td> 
      <td> <p>La valeur de date actuelle dans le champ personnalisé.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ancienne valeur du texte</p> </td> 
      <td> <p>La valeur de texte précédente dans le champ personnalisé.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nouvelle valeur de texte</p> </td> 
      <td> <p>La valeur de texte actuelle dans le champ personnalisé.</p> <p>Si le champ personnalisé est un champ de saisie anticipée, la variable <strong>Nouvelle valeur de texte</strong> affiche l’identifiant de l’objet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Pour plus d’informations sur l’ajout de colonnes, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Dans le **Filtres** , cliquez sur **Ajouter une règle de filtre**, puis ajoutez ce qui suit :

   * **Nom du champ d’entrée du journal** > **Contient** > **DE**

     >[!TIP]
     >
     >Pour limiter ce rapport à des champs personnalisés spécifiques, ajoutez la règle de filtrage **Nom du champ d’entrée du journal** > **Égal** > **`<custom field>`**.

   * **Identifiant de projet** > **Égal** > **`<project>`**

     ![](assets/qs-custom-form-changes-filter-350x92.png)

   Pour plus d’informations sur l’ajout de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facultatif) Pour cibler davantage le rapport et réduire les temps de chargement, ajoutez une invite.

   Ou

   Créez des règles de filtrage supplémentaires pour inclure des projets, des tâches ou des problèmes spécifiques.

   >[!IMPORTANT]
   >
   >Création d’une règle de filtrage qui utilise le modificateur **Contient** peut augmenter les temps de chargement. Pour cette raison, nous vous recommandons d’utiliser un autre modificateur, comme **Égal** si possible, filtrez pour un projet spécifique ou un identifiant d’objet de niveau supérieur.

   Pour savoir comment ajouter une invite, voir [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Dans le **Groupements** , cliquez sur **Appliquer un groupement existant**, puis sélectionnez **Projet**.

   Pour plus d’informations sur l’ajout de groupements, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Cliquez sur **Enregistrer + Fermer**.

   Votre nouveau rapport se charge.

## Afficher la modification de la date d’achèvement prévue au cours du cycle de vie d’un projet {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

Vous pouvez configurer le rapport Entrée de journal pour qu’il indique à quelle fréquence la date d’achèvement planifiée change au cours de la vie d’un projet.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Entrée du journal**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Le créateur de rapports se charge.

1. Dans le **Colonnes (affichage)** , ajoutez les colonnes suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Colonnes</th> 
      <th>Explication</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nom de champ</p> </td> 
      <td> <p>Nom du champ affecté.</p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> s’affiche dans cette colonne, ce qui indique que le champ répertorié est un champ personnalisé.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modifier le type</p> </td> 
      <td>Le type de modification qui s’est produit, par exemple <strong>Ajouter</strong>, <strong>Supprimer</strong>, ou <strong>Modifier</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modifié par nom</p> </td> 
      <td> <p>Nom de l’utilisateur qui a mis à jour la date d’achèvement prévue du projet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Date d’entrée</p> </td> 
      <td> <p>Date à laquelle la date d’achèvement prévue du projet a été modifiée.</p> <p>Vous devez trier par ce champ dans l’ordre décroissant.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Code objet supérieur</p> </td> 
      <td> <p>Objet parent le plus élevé pour le champ dont la date de fin planifiée a été modifiée.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Étendue</p> </td> 
      <td> <p>Objet dont la date de fin planifiée a été modifiée.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Ancienne valeur de la date</p> </td> 
      <td> <p>Valeur précédente de la date d’achèvement planifiée.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nouvelle valeur de date</p> </td> 
      <td> <p>Valeur actuelle de la date d’achèvement planifiée.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nom du projet</p> <p>(Facultatif)</p> </td> 
      <td> <p>Nom du projet pour lequel la date d’achèvement planifiée a été modifiée.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nom de la tâche</p> <p>(Facultatif)</p> </td> 
      <td> <p>Nom des tâches du projet pour lesquelles la date d’achèvement planifiée a été modifiée.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nom de l'événement</p> <p>(Facultatif)</p> </td> 
      <td>Nom des problèmes du projet pour lesquels la date d’achèvement planifiée a été modifiée.</td> 
     </tr> 
    </tbody> 
   </table>

   Pour plus d’informations sur l’ajout de colonnes, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Dans le **Filtres** , cliquez sur **Ajouter une règle de filtre**, puis ajoutez ce qui suit :

   * **Nom du champ** > **Égal** > **Date**
   * **Identifiant de projet** > **Égal** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   Pour plus d’informations sur l’ajout de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facultatif) Pour cibler davantage le rapport et réduire les temps de chargement, ajoutez une invite.

   Ou

   Créez des règles de filtrage supplémentaires pour inclure des projets, des tâches ou des problèmes spécifiques.

   >[!IMPORTANT]
   >
   >Création d’une règle de filtrage qui utilise le modificateur **Contient** peut augmenter les temps de chargement. Pour cette raison, nous vous recommandons d’utiliser un autre modificateur, comme **Égal** si possible, filtrez pour un projet spécifique ou un identifiant d’objet de niveau supérieur.

   Pour savoir comment ajouter une invite, voir [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Dans le **Groupements** , cliquez sur **Appliquer un groupement existant**, puis sélectionnez **Projet**.

   Pour plus d’informations sur l’ajout de groupements, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Cliquez sur **Enregistrer + Fermer**.

   Votre nouveau rapport se charge.

## Vérification de la modification du propriétaire d’un projet {#see-if-the-owner-of-a-project-changed}

Vous pouvez configurer le rapport Entrée de journal pour qu’il indique le nombre de fois où le propriétaire du projet (ou le responsable de projet) change au cours de la vie d’un projet.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Entrée du journal**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Le créateur de rapports se charge.

1. Dans le **Colonnes (affichage)** , ajoutez les colonnes suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Colonnes</th> 
      <th>Explication</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">Nom de champ</p> </td> 
      <td>Nom du champ affecté. La variable <strong>ownerID</strong> s’affiche dans cette colonne.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modifier le type</p> </td> 
      <td> <p>Le type de modification qui s’est produit, par exemple <strong>Ajouter</strong>, <strong>Supprimer</strong>, ou <strong>Modifier</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Code objet supérieur</p> </td> 
      <td> <p>Objet parent le plus élevé du projet auquel le propriétaire du projet a été mis à jour.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Date d’entrée</p> </td> 
      <td>Date à laquelle le propriétaire du projet a été modifié.<br>Vous devez trier par ce champ dans l’ordre décroissant.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Modifié par nom</p> </td> 
      <td> <p>Nom de l’utilisateur qui a mis à jour le propriétaire du projet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Infos supplémentaires 1</p> </td> 
      <td> <p>Propriétaire actuel du projet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Infos supplémentaires 2</p> </td> 
      <td> <p>Propriétaire précédent du projet sur le projet.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">Nom du projet</p> </td> 
      <td> <p>Le champ Propriétaire du projet a été mis à jour.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Pour plus d’informations sur l’ajout de colonnes, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Dans le **Filtres** , cliquez sur **Ajouter une règle de filtre**, puis ajoutez ce qui suit :

   * **Nom du champ** > **Égal** > **ownerID**
   * **Identifiant de projet** > **Égal** > **`<project name>`**

     ![](assets/qs-owner-changes-filter-350x94.png)

   Pour plus d’informations sur l’ajout de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facultatif) Pour cibler davantage le rapport et réduire les temps de chargement, ajoutez une invite.

   Ou

   Créez des règles de filtrage supplémentaires pour inclure des projets, des tâches ou des problèmes spécifiques.

   >[!IMPORTANT]
   >
   >Création d’une règle de filtrage qui utilise le modificateur **Contient** peut augmenter les temps de chargement. Pour cette raison, nous vous recommandons d’utiliser un autre modificateur, comme **Égal** si possible, filtrez pour un projet spécifique ou un identifiant d’objet de niveau supérieur.

   Pour savoir comment ajouter une invite, voir [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (Facultatif) Dans la variable **Groupements** , cliquez sur **Appliquer un groupement existant**, puis sélectionnez **Projet**.

   Pour plus d’informations sur l’ajout de groupements, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Cliquez sur **Enregistrer + Fermer**.

   Votre nouveau rapport se charge.
