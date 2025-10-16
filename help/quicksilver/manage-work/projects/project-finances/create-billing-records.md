---
navigation-topic: financials
title: Créer des enregistrements de facturation
description: En plus de définir les revenus et de suivre les dépenses, vous pouvez créer des enregistrements de facturation sur un projet pour les informations qui doivent être facturées.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 38%

---

# Créer des enregistrements de facturation

<!-- Audited: 6/2025 -->

En plus de définir les revenus et de suivre les dépenses, vous pouvez créer des enregistrements de facturation sur un projet pour les informations qui doivent être facturées.

Vous ne pouvez pas créer d&#39;enregistrements de facturation pour les tâches ; vous pouvez uniquement créer des enregistrements de facturation pour les projets.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Accès en modification aux projets et aux données financières</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Autorisations de gestion pour le projet avec les autorisations de gestion financière</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vue d’ensemble des enregistrements de facturation

Les enregistrements de facturation sont créés en tant que pièces jointes à un projet et contiennent des données financières du projet ainsi que les informations financières des tâches du projet.

Tenez compte des éléments suivants lorsque vous envisagez d’utiliser les enregistrements de facturation :

* Vous créez un enregistrement de facturation lorsque vous souhaitez facturer une somme d’argent liée au projet à un fournisseur ou à un partenaire externe. Outre la facturation d’un montant fixe à une source externe, il arrive que vous deviez facturer à un fournisseur la quantité de travail sur le projet (à partir des heures consignées), ainsi que les dépenses encourues ou le montant des revenus fixes. Vous pouvez inclure toutes ces informations dans le même enregistrement de facturation.
* Une fois qu’un enregistrement de facturation est défini sur Facturé, il ne peut pas être modifié.

  >[!IMPORTANT]
  >
  >C’est important lorsque vos taux varient et que vous souhaitez verrouiller les informations relatives aux revenus et aux dépenses de votre projet. Le fait de les ajouter à un enregistrement de facturation et de les marquer comme facturées les empêche d’être mises à jour lorsque les taux sont actualisés dans votre système.

* Impossible de supprimer un projet dont les enregistrements de facturation ont été marqués comme Facturés.

## Créer un enregistrement de facturation

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.
1. Cliquez sur **Nouvel enregistrement de facturation**.
1. Dans la zone **Nouvel enregistrement de facturation** qui s&#39;affiche, saisissez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>(Obligatoire) Saisissez une description pour l’enregistrement de facturation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Statut de la facturation</td> 
      <td> <p>Sélectionnez <strong>Non facturé</strong> si cet enregistrement n'a pas encore été facturé.</p> <p>Sélectionnez <strong> Facturé </strong> si l’enregistrement de facturation a été facturé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date de facturation</td> 
      <td>Sélectionnez la date à laquelle cet enregistrement de facturation a été facturé en cliquant sur l’icône de calendrier.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Numéro de bon de commande</td> 
      <td>Saisissez le numéro de bon de commande associé à cet enregistrement de facturation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID de facture</td> 
      <td>Saisissez la facture associée à cet enregistrement de facturation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Montant supplémentaire</td> 
      <td>Saisissez le montant fixe de votre enregistrement de facturation. Il s'agit du montant que vous avez l'intention de facturer à un client, un entrepreneur ou un partenaire externe pour ce projet. Ce montant ne peut pas être modifié une fois que le statut de l’enregistrement de facturation est passé à Facturé.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Sous **Forms personnalisé**, sélectionnez un formulaire personnalisé d’enregistrements de facturation que vous souhaitez ajouter à l’enregistrement.

   Un formulaire personnalisé d’enregistrements de facturation doit être créé avant de pouvoir le sélectionner ici. Seuls les formulaires personnalisés actifs sont affichés dans la liste. Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Cliquez sur **Enregistrer.** L’enregistrement de facturation est créé.

## Inclure les heures facturables, les dépenses et les revenus fixes dans un enregistrement de facturation

### Inclure les heures facturables dans un enregistrement de facturation {#include-billable-hours-in-a-billing-record}

Vous pouvez inclure les heures qui ont été consignées sur les tâches, les problèmes ou le projet dans vos enregistrements de facturation.

Si l’utilisateur ou l’utilisatrice qui enregistre les heures ou sa fonction principale est associé à un taux de facturation par heure, le chiffre d’affaires généré par ces heures est ajouté à l’enregistrement de facturation.

* [Quelles heures peuvent être ajoutées à un enregistrement de facturation ?](#what-hours-can-be-added-to-a-billing-record)
* [Ajouter des heures à un enregistrement de facturation](#add-hours-to-a-billing-record)

#### Quelles heures peuvent être ajoutées à un enregistrement de facturation ? {#what-hours-can-be-added-to-a-billing-record}

Vous pouvez ajouter des heures à un enregistrement de facturation lorsque les conditions suivantes sont remplies :

* Des heures ont été consignées pour les tâches, les événements ou le projet.
* Le type d’heure des heures enregistrées est marqué comme Compte comme revenu.

  Pour plus d’informations, consultez l’article [Gestion des types d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Toutes les heures enregistrées pour les événements du projet peuvent être ajoutées à un enregistrement de facturation si l&#39;utilisateur qui enregistre les heures a un taux de facturation par heure qui lui est associé ou qui est associé à sa fonction principale.
* Si les heures sont enregistrées sur une tâche, celle-ci doit avoir le type de revenu suivant 

   * Impossible de définir le type de revenus sur Non facturable.
   * Si le type de revenu est défini sur Taux horaire de la personne, la personne qui consigne le temps doit avoir un taux de facturation horaire défini dans son profil.
   * Si le Type de revenu est défini sur Rôle par heure, le rôle principal de l’utilisateur qui enregistre le temps doit avoir un taux de facturation par heure.

     >[!NOTE]
     >
     >Vous pouvez modifier les taux de facturation pour les fonctions au niveau du projet.\
     >Pour plus d’informations, reportez-vous à la section « Remplacement des taux de facturation des fonctions au niveau du projet » de l’article [Présentation du remplacement des taux de facturation des fonctions et du calcul du revenu sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Si l’option Exiger que le temps soit approuvé pour ce projet est sélectionnée sous Paramètres du projet, le propriétaire du projet doit approuver les heures consignées.\
  Pour plus d’informations, voir [L’approbation d’un projet demande du temps](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Ajouter des heures à un enregistrement de facturation {#add-hours-to-a-billing-record}

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.
1. Cliquez sur l’enregistrement de facturation **Description** pour ouvrir l’onglet **Détails de l’enregistrement de facturation**.
1. Cliquez sur **Heures facturables** dans le panneau de gauche.
1. Si des heures peuvent être incluses dans un enregistrement de facturation, cliquez sur **Ajouter des heures**. La zone **Ajouter des heures facturables** s’ouvre.

   >[!NOTE]
   >
   >Si aucune heure n&#39;est consignée ou si les heures consignées ne remplissent pas les conditions requises pour être ajoutées à un enregistrement de facturation, le bouton **Ajouter des heures** ne s&#39;affiche pas. Pour plus d’informations, reportez-vous à la section suivante de cet article : [quelles heures peuvent être ajoutées à un enregistrement de facturation &#x200B;](#what-hours-can-be-added-to-a-billing-record).

1. Sélectionnez les entrées d&#39;heures à inclure dans l&#39;enregistrement de facturation, puis cliquez sur **Ajouter des heures**. Le coût réel des heures est ajouté en tant que montant des **heures facturables** au total de l’**enregistrement de facturation**.

1. (Facultatif) Cliquez sur **Détails des enregistrements de facturation** pour consulter les montants **Heures facturables** et **Total de l’enregistrement de facturation**, ainsi que le total de l’enregistrement de facturation dans l’en-tête de l’enregistrement de facturation.

### Inclure les dépenses facturables dans un enregistrement de facturation {#include-billable-expenses-in-a-billing-record}

Si vous ajoutez des dépenses facturables à l&#39;enregistrement de facturation, assurez-vous que les dépenses des tâches et du projet sont marquées comme facturables. Les frais qui ne sont pas marquées comme facturables ne peuvent pas être ajoutés à un enregistrement de facturation. Pour plus d’informations sur l’ajout de frais, consultez l’article [Gérer les dépenses liées à un projet](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Pour ajouter des frais facturables à un enregistrement de facturation, procédez comme suit :

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.
1. Cliquez sur l’enregistrement de facturation **Description** pour ouvrir l’onglet **Détails de l’enregistrement de facturation**.
1. Cliquez sur **Frais facturables** dans le panneau de gauche.
1. (Conditionnel) Si vous avez ajouté des dépenses à vos tâches ou au projet et que vous les avez marquées comme facturables, cliquez sur **Ajouter des dépenses**.

   >[!NOTE]
   >
   >Si vous avez des dépenses mais qu&#39;elles ne sont pas marquées comme facturables, le bouton **Ajouter des dépenses** ne s&#39;affiche pas. Seuls les frais facturables dont le montant réel est supérieur à zéro peuvent être inclus dans un enregistrement de facturation.

1. Sélectionnez les dépenses facturables qui peuvent être ajoutées à l&#39;enregistrement de facturation, puis cliquez sur **Ajouter des dépenses**.  Le montant réel des frais est ajouté en tant que **Frais facturables** au **Total de l’enregistrement de facturation**.

1. (Facultatif) Cliquez sur **Détails des enregistrements de facturation** pour consulter les montants **Dépenses facturables** et **Total de l’enregistrement de facturation**, ainsi que le total de l’enregistrement de facturation dans l’en-tête de l’enregistrement de facturation.

### Inclure les revenus fixes dans un enregistrement de facturation {#include-fixed-revenues-in-a-billing-record}

Vous pouvez ajouter des revenus fixes à vos enregistrements de facturation si certaines tâches disposent de revenus fixes. Aucun autre type de revenu de tâche ou de projet ne peut être ajouté à un enregistrement de facturation. Pour plus d&#39;informations sur les types de revenus, reportez-vous à la section Présentation de la facturation et des revenus de l&#39;article [Présentation de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.
1. Cliquez sur le **Description** de l’enregistrement de facturation pour ouvrir l’onglet **Détails de l’enregistrement de facturation**.
1. Sélectionnez l’onglet **Revenus fixes**.
1. Si vous avez ajouté des revenus fixes à vos tâches, cliquez sur **Ajouter des revenus fixes**.

   >[!NOTE]
   >
   >Si des montants de revenus sont associés à des tâches mais qu&#39;ils ne sont pas marqués comme fixes, le bouton **Ajouter un revenu fixe** ne s&#39;affiche pas.

1. Sélectionnez les tâches dont vous souhaitez inclure les revenus fixes dans l&#39;enregistrement de facturation, puis cliquez sur **Ajouter des tâches**.  Le montant **Revenus fixes** des tâches est ajouté en tant que montant **Revenus facturables** au **total de l’enregistrement de facturation**.

1. (Facultatif) Cliquez sur **Détails des enregistrements de facturation** pour consulter les montants **Revenus facturables** et **Total de l’enregistrement de facturation**, ainsi que le total de l’enregistrement de facturation dans l’en-tête de l’enregistrement de facturation.

## Modifier un enregistrement de facturation

Après avoir créé un enregistrement de facturation et y avoir ajouté des heures, des dépenses et des revenus, vous pouvez modifier certaines informations de l&#39;enregistrement existant avant qu&#39;il ne soit marqué comme Facturé.

1. Accédez à l’enregistrement de facturation.
1. Sélectionnez **Détails de l’enregistrement de facturation** dans le panneau de gauche.
1. Modifiez les informations dans les champs disponibles.

   Ou

   Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) dans le coin supérieur droit, puis modifiez les informations dans les champs disponibles.

   Mettez à jour les informations suivantes :

   * **Description**
   * **Date de facturation**
   * **Statut de la facturation**

     >[!TIP]
     >
     >Si vous sélectionnez **Facturé** pour le statut de facturation, l’enregistrement de facturation ne peut pas être modifié après l’enregistrement de vos modifications.

   * **ID de facture**
   * **Numéro de bon de commande**
   * **Montant supplémentaire**

   Les champs suivants ne peuvent pas être modifiés :

   * **Heures facturables :** total des revenus réels des heures incluses dans l’enregistrement de facturation. Pour plus d’informations, reportez-vous à la section suivante de cet article : [Inclure des heures facturables dans un enregistrement de facturation](#include-billable-hours-in-a-billing-record).

   * **Dépenses facturables** : total du montant réel des dépenses facturables inclus dans l’enregistrement de facturation. Pour plus d’informations, reportez-vous à la section suivante de cet article : [Inclure les dépenses facturables dans un enregistrement de facturation](#include-billable-expenses-in-a-billing-record).

   * **Revenus facturables** : le total des revenus fixes des tâches incluses dans l’enregistrement de facturation. Pour plus d&#39;informations, reportez-vous à la section suivante de cet article : [Inclure les revenus fixes dans un enregistrement de facturation](#include-fixed-revenues-in-a-billing-record).

   * **Total de l’enregistrement de facturation** : le total de tous les montants facturables. Cela est calculé à l’aide de la formule suivante :

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Cliquez sur **Enregistrer les modifications**.
