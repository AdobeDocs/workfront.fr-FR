---
navigation-topic: financials
title: Créer des enregistrements de facturation
description: En plus de définir les revenus et de suivre les dépenses, vous pouvez créer des enregistrements de facturation sur un projet pour les informations qui doivent être facturées.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '1898'
ht-degree: 98%

---

# Créer des enregistrements de facturation

En plus de définir les revenus et de suivre les dépenses, vous pouvez créer des enregistrements de facturation sur un projet pour les informations qui doivent être facturées.

Vous ne pouvez pas créer d’enregistrements de facturation pour les tâches. Vous ne pouvez créer des enregistrements de facturation que pour des projets.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Accès en modification aux projets et aux données financières</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Autorisations de gestion pour le projet avec les autorisations de gestion financière</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vue d’ensemble des enregistrements de facturation

Les enregistrements de facturation sont créés en tant que pièces jointes à un projet et contiennent les données financières du projet ainsi que certaines informations financières pour les tâches d’un projet.

Tenez compte des éléments suivants lorsque vous envisagez d’utiliser les enregistrements de facturation :

* Vous créez un enregistrement de facturation lorsque vous souhaitez facturer une somme d’argent liée au projet à un fournisseur ou à un partenaire externe. Outre la facturation d’un montant fixe à une source externe, il arrive que vous deviez facturer à un fournisseur la quantité de travail sur le projet (à partir des heures consignées), ainsi que les dépenses encourues ou le montant des revenus fixes. Vous pouvez inclure toutes ces informations dans le même enregistrement de facturation.
* Une fois qu’un enregistrement de facturation a été défini comme facturé, il ne peut plus être modifié.

  >[!IMPORTANT]
  >
  >C’est important lorsque vos taux varient et que vous souhaitez verrouiller les informations relatives aux revenus et aux dépenses de votre projet. Le fait de les ajouter à un enregistrement de facturation et de les marquer comme facturées les empêche d’être mises à jour lorsque les taux sont actualisés dans votre système.

* Un projet incluant des enregistrements de facturation marqués comme facturés ne peut pas être supprimé.

## Créer un enregistrement de facturation

1. Accédez à un projet.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.

   Cette section peut être située sous **Afficher plus**.

1. Lorsque l’option **Détails de l’enregistrement de facturation** est sélectionnée dans le panneau de gauche, cliquez sur **Nouvel enregistrement de facturation**.
1. Dans la zone **Nouvel enregistrement de facturation** qui s’affiche, spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Champ obligatoire. Spécifiez une description pour l’enregistrement de facturation afin de traduire l’objectif ou l’intention de cet enregistrement.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Statut de la facturation</td> 
      <td> <p>Sélectionnez <strong>Non facturé</strong>, si cet enregistrement n’a pas encore été facturé.</p> <p>Sélectionnez <strong>Facturé</strong> lorsque l’enregistrement de facturation est facturé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date de facturation</td> 
      <td>Sélectionnez la date à laquelle cet enregistrement de facturation est facturé, en cliquant sur l’icône du calendrier.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Numéro de bon de commande</td> 
      <td>Si un numéro de commande est associé à cet enregistrement de facturation, indiquez-le dans ce champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID de facture</td> 
      <td>Si une facture est associée à cet enregistrement de facturation, indiquez cette information dans ce champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Montant supplémentaire</td> 
      <td>Saisissez le montant fixe de votre enregistrement de facturation. Il s’agit du montant que vous avez l’intention de facturer à un client ou une cliente, un fournisseur ou un partenaire externe pour ce projet. Ce montant ne peut pas être modifié une fois que le statut de l’enregistrement de facturation est passé à Facturé.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Sous **Formulaires personnalisés**, sélectionnez un formulaire personnalisé d’enregistrements de facturation que vous souhaitez ajouter à l’enregistrement de facturation.

   Vous (ou une autre personne ayant accès aux formulaires personnalisés) devez créer un formulaire personnalisé d’enregistrements de facturation avant de pouvoir le sélectionner ici. Seuls les formulaires personnalisés actifs sont affichés dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Vous pouvez répéter cette étape pour ajouter d’autres formulaires personnalisés dont vous avez besoin pour l’enregistrement de facturation.

1. Cliquez sur **Enregistrer**.

   L’enregistrement de facturation est créé. Pour inclure les heures facturables, les dépenses et les revenus fixes dans l’enregistrement de facturation, suivez les étapes décrites dans la sous-section suivante.

## Inclure les heures facturables, les dépenses et les revenus fixes dans un enregistrement de facturation

* [Inclure les heures facturables dans un enregistrement de facturation](#include-billable-hours-in-a-billing-record)
* [Inclure les dépenses facturables dans un enregistrement de facturation](#include-billable-expenses-in-a-billing-record)
* [Inclure les revenus fixes dans un enregistrement de facturation](#include-fixed-revenues-in-a-billing-record)

### Inclure les heures facturables dans un enregistrement de facturation {#include-billable-hours-in-a-billing-record}

Vous pouvez inclure les heures qui ont été consignées sur les tâches, les problèmes ou le projet dans vos enregistrements de facturation.\
Si la personne qui consigne les heures ou sa fonction principale est associée à un taux de facturation horaire, le revenu de ces heures est ajouté à l’enregistrement de facturation.

* [Quelles heures peuvent être ajoutées à un enregistrement de facturation ?](#what-hours-can-be-added-to-a-billing-record)
* [Ajouter des heures à un enregistrement de facturation](#add-hours-to-a-billing-record)

#### Quelles heures peuvent être ajoutées à un enregistrement de facturation ? {#what-hours-can-be-added-to-a-billing-record}

Vous pouvez ajouter des heures à un enregistrement de facturation lorsque les conditions suivantes sont remplies :

* Les tâches, les problèmes ou le projet ont des heures consignées.
* Le type d’heure des heures enregistrées est marqué comme Compte comme revenu.

  Pour plus d’informations sur les types d’heures, voir l’article [Gérer les types d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Toutes les heures consignées pour les problèmes ou pour le projet peuvent être ajoutées à un enregistrement de facturation si la personne qui consigne le temps a un taux de facturation à l’heure associé à elle ou à sa fonction principale.
* Si les heures sont enregistrées sur une tâche, celle-ci doit avoir le type de revenu suivant 

   * Le type de revenu ne peut pas être défini sur Non facturable.
   * Si le type de revenu est défini sur Taux horaire de la personne, la personne qui consigne le temps doit avoir un taux de facturation horaire défini dans son profil.
   * Si le type de revenu est défini sur Taux horaire du rôle, le rôle principal de la personne qui consigne le temps doit avoir un taux de facturation horaire.

     >[!NOTE]
     >
     >Vous pouvez modifier les taux de facturation pour les fonctions au niveau du projet.\
     >Pour plus d’informations sur la substitution des taux de facturation des fonctions, voir la section « Substituer des taux de facturation des fonctions au niveau du projet » dans l’article [Vue d’ensemble de la substitution des taux de facturation des fonctions et du calcul des revenus sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Si l’option **Demander du temps pour avoir l’approbation pour ce projet** est cochée sous Paramètres de projet, la personne propriétaire du projet doit approuver les heures consignées.\
  Pour plus d’informations sur l’obligation d’approuver les heures d’un projet, voir l’article [Exiger que les heures soient approuvées pour un projet](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Ajouter des heures à un enregistrement de facturation {#add-hours-to-a-billing-record}

Pour ajouter des heures facturables à un enregistrement de facturation :

1. Accédez au projet contenant les enregistrements de facturation.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.

   Cette section peut être située sous **Afficher plus**.

1. Cliquez sur **Description** d’un enregistrement de facturation pour ouvrir l’onglet **Détails de l’enregistrement de facturation**.

1. Cliquez sur **Heures facturables** dans le panneau de gauche.
1. Si des heures peuvent être incluses dans un enregistrement de facturation, cliquez sur **Ajouter des heures**.\
   La boîte **Ajouter des heures facturables** s’ouvre.

   >[!NOTE]
   >
   >S’il n’y a pas d’heures consignées ou si les heures consignées ne remplissent pas les conditions requises pour être ajoutées à un enregistrement de facturation, le bouton **Ajouter des heures** ne s’affiche pas. Pour plus d’informations sur les heures qui peuvent être consignées dans un dossier de facturation, voir la section [Quelles heures peuvent être ajoutées à un enregistrement de facturation](#what-hours-can-be-added-to-a-billing-record) dans cet article.

1. Sélectionnez les entrées d’heures que vous souhaitez inclure dans l’enregistrement de facturation et cliquez sur **Ajouter des heures**.\
   Le coût réel des heures est ajouté en tant que montant des **heures facturables** au total de l’**enregistrement de facturation**.

1. (Facultatif) Cliquez sur **Détails des enregistrements de facturation** pour consulter les montants **Heures facturables** et **Total de l’enregistrement de facturation**. Vous pouvez également voir le total de l’enregistrement de facturation dans l’en-tête de l’enregistrement de facturation.


### Inclure les dépenses facturables dans un enregistrement de facturation {#include-billable-expenses-in-a-billing-record}

Si vous ajoutez des dépenses facturables à l’enregistrement de facturation, assurez-vous que les dépenses des tâches et du projet sont marquées comme facturables. Les frais qui ne sont pas marquées comme facturables ne peuvent pas être ajoutés à un enregistrement de facturation. Pour plus d’informations sur l’ajout de frais, consultez l’article [Gérer les dépenses liées à un projet](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Pour ajouter des frais facturables à un enregistrement de facturation, procédez comme suit :

1. Accédez au projet contenant les enregistrements de facturation.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Enregistrements de facturation**.

1. Cliquez sur **Description** pour un enregistrement de facturation afin d’ouvrir l’onglet **Détails de l’enregistrement de facturation**.

1. Cliquez sur **Frais facturables** dans le panneau de gauche.
1. (Le cas échéant) Si vous avez ajouté des frais à vos tâches ou au projet et que vous les avez marqués comme facturables, cliquez sur **Ajouter des frais**.

   >[!NOTE]
   >
   >Si vous avez des frais mais qu’ils ne sont pas marqués comme facturables, le bouton **Ajouter des frais** ne s’affiche pas. Seuls les frais facturables dont le montant réel est supérieur à zéro peuvent être inclus dans un enregistrement de facturation.

1. Sélectionnez les frais facturables qui peuvent être ajoutés à l’enregistrement de facturation, puis cliquez sur **Ajouter des frais**.\
   Le montant réel des frais est ajouté en tant que **Frais facturables** au **Total de l’enregistrement de facturation**.

1. (Facultatif) Cliquez sur **Détails de l’enregistrement de facturation** pour consulter les montants **Frais facturables** et **Total de l’enregistrement de facturation**. Vous pouvez également voir le total de l’enregistrement de facturation dans l’en-tête de l’enregistrement de facturation.

### Inclure les revenus fixes dans un enregistrement de facturation {#include-fixed-revenues-in-a-billing-record}

Vous pouvez ajouter des revenus fixes à vos enregistrements de facturation si vous avez des tâches pour lesquelles des revenus fixes sont disponibles. Aucun autre type de revenu de tâche ou de projet ne peut être ajouté dans un enregistrement de facturation. Pour plus d’informations sur les types de revenus, consultez la section [Vue d’ensemble de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) dans [Vue d’ensemble de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Pour ajouter des revenus fixes à un enregistrement de facturation, procédez comme suit :

1. Accédez au projet contenant les enregistrements de facturation.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Enregistrements de facturation**.

1. Cliquez sur **Description** pour un enregistrement de facturation afin d’ouvrir l’onglet **Détails de l’enregistrement de facturation**.

1. Sélectionnez l’onglet **Revenus fixes**.
1. Si vous avez ajouté des revenus fixes à vos tâches, cliquez sur **Ajouter des revenus fixes**.

   >[!NOTE]
   >
   >Si vous avez des montants de revenus sur les tâches mais qu’ils ne sont pas marqués comme « fixes », le bouton **Ajouter des revenus fixes** ne s’affiche pas.

1. Sélectionnez les tâches pour lesquelles vous souhaitez inclure des revenus fixes dans l’enregistrement de facturation, puis cliquez sur **Ajouter des tâches**.\
   Le montant **Revenus fixes** des tâches est ajouté en tant que montant **Revenus facturables** au **total de l’enregistrement de facturation**.

1. (Facultatif) Cliquez sur **Détails de l’enregistrement de facturation** pour consulter les montants **Revenus facturables** et **Total de l’enregistrement de facturation**. Vous pouvez également voir le total de l’enregistrement de facturation dans l’en-tête de l’enregistrement de facturation.

## Modifier un enregistrement de facturation

Après avoir créé un enregistrement de facturation et inclus les heures, les frais et les revenus dans l’enregistrement de facturation, vous pouvez modifier certaines informations sur l’enregistrement existant, avant qu’il ne soit marqué comme facturé.

1. Accédez à l’enregistrement de facturation.
1. Sélectionnez **Détails de l’enregistrement de facturation** dans le panneau de gauche, modifiez les informations dans les champs disponibles.

   Ou

   Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) dans le coin supérieur droit, puis modifiez les informations dans les champs disponibles.

   Mettez à jour les informations suivantes :

   * **Description**
   * **Statut de la facturation**

     >[!TIP]
     >
     >Si vous sélectionnez **Facturé** pour le statut de facturation, l’enregistrement de facturation ne peut plus être modifié une fois que vous avez enregistré vos modifications.

   * **Date de facturation**
   * **Numéro de bon de commande**
   * **ID de facture**
   * **Montant supplémentaire**

   Les champs suivants ne peuvent pas être modifiés :

   * **Heures facturables :** total des revenus réels des heures incluses dans l’enregistrement de facturation. Pour plus d’informations sur l’inclusion des heures dans un enregistrement de facturation, consultez la section [Inclure les heures facturables dans un enregistrement de facturation](#include-billable-hours-in-a-billing-record) dans cet article.

   * **Dépenses facturables** : total du montant réel des dépenses facturables inclus dans l’enregistrement de facturation. Pour plus d’informations sur l’inclusion des dépenses facturables dans un enregistrement de facturation, consultez la section [Inclure les dépenses facturables dans un enregistrement de facturation](#include-billable-expenses-in-a-billing-record) dans cet article.

   * **Revenus facturables** : le total des revenus fixes des tâches incluses dans l’enregistrement de facturation. Pour plus d’informations sur l’inclusion de revenus fixes dans un enregistrement de facturation, voir la section [Inclure des revenus fixes dans un enregistrement de facturation](#include-fixed-revenues-in-a-billing-record) dans cet article.

   * **Total de l’enregistrement de facturation** : le total de tous les montants facturables. Cela est calculé à l’aide de la formule suivante :

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Cliquez sur **Enregistrer**&#x200B;**les modifications**.
