---
navigation-topic: financials
title: Créer des enregistrements de facturation
description: Outre la configuration des recettes et des dépenses de suivi, vous pouvez créer des enregistrements de facturation sur un projet pour obtenir des informations à facturer.
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 6%

---

# Créer des enregistrements de facturation

Outre la configuration des recettes et des dépenses de suivi, vous pouvez créer des enregistrements de facturation sur un projet pour obtenir des informations à facturer.

Vous ne pouvez pas créer d’enregistrements de facturation pour les tâches. Vous pouvez uniquement créer des enregistrements de facturation pour les projets.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets et aux données financières</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations du projet avec les autorisations de gestion financière</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Présentation des enregistrements de facturation

Les enregistrements de facturation sont créés en tant que pièces jointes à un projet et contiennent des données financières du projet ainsi que des informations financières pour les tâches d’un projet.

Tenez compte des points suivants lorsque vous envisagez d’utiliser des enregistrements de facturation :

* Vous créez un enregistrement de facturation lorsque vous souhaitez facturer une somme d’argent liée au projet à un fournisseur ou à un partenaire externe. Outre la facturation d’un montant fixe à une source externe, il peut arriver que vous deviez facturer le montant des travaux sur le projet (des heures consignées) à un prestataire externe, ainsi que les dépenses encourues ou le montant des revenus fixes. Vous pouvez inclure toutes ces informations dans le même enregistrement de facturation.
* Une fois qu&#39;un enregistrement de facturation est défini sur Facturé, il ne peut plus être modifié.

  >[!IMPORTANT]
  >
  >Ceci est important lorsque vos taux varient et que vous souhaitez verrouiller les informations de recettes et de dépenses sur votre projet. L’ajouter à un enregistrement de facturation et le marquer comme Facturé empêche sa mise à jour lors de la mise à jour des taux dans votre système.

* Un projet dont les enregistrements de facturation ont été marqués comme Facturés ne peut pas être supprimé.

## Création d’un enregistrement de facturation

1. Accédez à un projet.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.

   Cette section peut se trouver sous **Afficher plus**.

1. Lorsque **Informations sur l’enregistrement de facturation** est sélectionné dans le panneau de gauche, cliquez sur **Nouvel enregistrement de facturation**.
1. Dans la zone **New Billing Record** qui s’affiche, spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Il s’agit d’un champ obligatoire. Spécifiez une description pour l’enregistrement de facturation, afin de refléter l’objectif ou l’intention de cet enregistrement.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Statut de la facturation</td> 
      <td> <p>Sélectionnez <strong>Non facturé</strong> si cet enregistrement n'a pas encore été facturé.</p> <p>Sélectionnez <strong>Facturé</strong> lorsque l’enregistrement de facturation est facturé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date de facturation</td> 
      <td>Sélectionnez la date de facturation de cet enregistrement de facturation en cliquant sur l'icône de calendrier.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Numéro de bon de commande</td> 
      <td>Si un numéro de bon de commande est associé à cet enregistrement de facturation, indiquez ces informations dans ce champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID de facture</td> 
      <td>Si une facture est associée à cet enregistrement de facturation, indiquez ces informations dans ce champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Montant supplémentaire</td> 
      <td>Saisissez le montant fixe de votre enregistrement de facturation. Il s’agit du montant que vous avez l’intention de facturer à un client, à un entrepreneur ou à un partenaire externe pour ce projet. Ce montant ne peut pas être modifié une fois que l'état de l'enregistrement de facturation a été modifié en Facturé.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Sous **Forms personnalisée**, sélectionnez un formulaire personnalisé d’enregistrements de facturation à ajouter à l’enregistrement de facturation.

   Vous (ou un autre utilisateur ayant accès à des formulaires personnalisés) devez créer un formulaire personnalisé d’enregistrement de facturation avant de pouvoir le sélectionner ici. Seuls les formulaires personnalisés actifs sont affichés dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, voir [Concevoir un formulaire avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Vous pouvez répéter cette étape pour ajouter d’autres formulaires personnalisés dont vous avez besoin pour l’enregistrement de facturation.

1. Cliquez sur **Enregistrer.**

   L&#39;enregistrement de facturation est créé. Pour inclure les Heures facturables, Dépenses et Revenus fixes dans l&#39;enregistrement de facturation, suivez les étapes décrites dans la sous-section suivante.

## Inclure les heures facturables, les dépenses et les recettes fixes dans un enregistrement de facturation

* [Inclure les heures facturables dans un enregistrement de facturation](#include-billable-hours-in-a-billing-record)
* [Inclure les dépenses facturables dans un enregistrement de facturation](#include-billable-expenses-in-a-billing-record)
* [Inclure les recettes fixes dans un enregistrement de facturation](#include-fixed-revenues-in-a-billing-record)

### Inclure les heures facturables dans un enregistrement de facturation {#include-billable-hours-in-a-billing-record}

Vous pouvez inclure dans vos enregistrements de facturation les heures qui ont été enregistrées pour des tâches, des problèmes ou le projet.\
Si l’utilisateur qui consigne les heures ou son rôle de tâche Principal est associé à un taux de facturation par heure, les recettes de ces heures sont ajoutées à l’enregistrement de facturation.

* [Quelles heures peuvent être ajoutées à un enregistrement de facturation](#what-hours-can-be-added-to-a-billing-record)
* [Ajout d’heures à un enregistrement de facturation](#add-hours-to-a-billing-record)

#### Quelles heures peuvent être ajoutées à un enregistrement de facturation {#what-hours-can-be-added-to-a-billing-record}

Vous pouvez ajouter des heures à un enregistrement de facturation lorsque les conditions suivantes sont remplies :

* Les tâches, les problèmes ou le projet ont des heures enregistrées.
* Le type d’heure des heures consignées est marqué comme Comptage comme Recettes.

  Pour plus d’informations sur les types d’heure, consultez l’article [Gérer les types d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Toutes les heures consignées pour des problèmes ou pour le projet peuvent être ajoutées à un enregistrement de facturation si l’utilisateur qui consigne l’heure est associé à un taux de facturation par heure ou à son rôle de tâche Principal.
* Si les heures sont connectées sur une tâche, celle-ci doit avoir le type de revenu suivant :

   * Le type de revenu ne peut pas être défini sur Non facturable.
   * Si le type de revenu est défini sur Heure de l’utilisateur, un taux de facturation par heure doit être défini dans le profil de l’utilisateur qui consigne l’heure.
   * Si le type de revenu est défini sur Rôle horaire, le rôle de Principal de l’utilisateur qui consigne l’heure doit avoir un taux de facturation par heure.

     >[!NOTE]
     >
     >Vous pouvez remplacer les taux de facturation pour les rôles de tâche au niveau du projet.\
     >Pour plus d’informations sur le remplacement des taux de facturation des rôles de tâche, voir la section &quot;Remplacement des taux de facturation des rôles de tâche au niveau du projet&quot; dans l’article [Présentation du remplacement des taux de facturation des rôles de tâche et calcul des recettes sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Si **l’heure requise pour approuver ce projet** est cochée sous Paramètres du projet, le propriétaire du projet doit approuver les heures consignées.\
  Pour plus d’informations sur la nécessité d’une approbation sur les heures de projet, consultez l’article [Exiger du temps pour l’approbation d’un projet](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Ajout d’heures à un enregistrement de facturation {#add-hours-to-a-billing-record}

Pour ajouter des heures facturables à un enregistrement de facturation :

1. Accédez au projet avec les enregistrements de facturation.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.

   Cette section peut se trouver sous **Afficher plus**.

1. Cliquez sur la **Description** d’un enregistrement de facturation pour ouvrir l’onglet **Informations sur l’enregistrement de facturation** .

1. Cliquez sur **Billable Hours** dans le panneau de gauche.
1. Si des heures peuvent être incluses dans un enregistrement de facturation, cliquez sur **Ajouter des heures**.\
   La zone **Ajouter des heures facturables** s’ouvre.

   >[!NOTE]
   >
   >Si aucune heure n’est consignée ou si les heures consignées ne répondent pas aux conditions requises pour être ajoutées à un enregistrement de facturation, le bouton **Ajouter des heures** ne s’affiche pas. Pour plus d’informations sur les heures pouvant être enregistrées dans un enregistrement de facturation, reportez-vous à la section [Quelles heures peuvent être ajoutées à un enregistrement de facturation](#what-hours-can-be-added-to-a-billing-record) de cet article.

1. Sélectionnez les entrées d’heure que vous souhaitez inclure dans l’enregistrement de facturation, puis cliquez sur **Ajouter des heures**.\
   Le coût réel des heures est ajouté comme le montant **Heures facturables** au **Total des enregistrements de facturation**.

1. (Facultatif) Cliquez sur **Détails des enregistrements de facturation** pour passer en revue les **Heures facturables** et les **Total des enregistrements de facturation**. Vous pouvez également voir le total de l’enregistrement de facturation dans l’en-tête de l’enregistrement de facturation.

### Inclure les dépenses facturables dans un enregistrement de facturation {#include-billable-expenses-in-a-billing-record}

Si vous ajoutez des Dépenses facturables à l&#39;enregistrement de facturation, assurez-vous que les dépenses sur les tâches et le projet sont marqués comme Facturables. Les dépenses qui ne sont pas marquées comme facturables ne peuvent pas être ajoutées dans un enregistrement de facturation. Pour plus d’informations sur l’ajout de dépenses, consultez l’article [Gérer les dépenses de projet](../../../manage-work/projects/project-finances/manage-project-expenses.md).

Pour ajouter des dépenses facturables à un enregistrement de facturation :

1. Accédez au projet avec les enregistrements de facturation.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Enregistrements de facturation**.

1. Cliquez sur la **Description** d’un enregistrement de facturation pour ouvrir l’onglet **Informations sur l’enregistrement de facturation** .

1. Cliquez sur **Dépenses facturables** dans le panneau de gauche.
1. (Conditionnel) Si vous avez ajouté des dépenses à vos tâches ou au projet et que vous les avez marquées comme facturables, cliquez sur **Ajouter des dépenses**.

   >[!NOTE]
   >
   >Si vous avez des dépenses mais qu&#39;elles ne sont pas marquées comme facturables, le bouton **Ajouter des dépenses** ne s&#39;affiche pas. Seules les dépenses facturables dont le montant réel est supérieur à zéro peuvent être incluses dans un enregistrement de facturation.

1. Sélectionnez les dépenses facturables qui peuvent être ajoutées à l&#39;enregistrement de facturation, puis cliquez sur **Ajouter des dépenses**.\
   Le montant réel des dépenses est ajouté comme le montant **Dépenses facturables** au **Total de l’enregistrement de facturation**.

1. (Facultatif) Cliquez sur **Détails des enregistrements de facturation** pour passer en revue les **Dépenses facturables** et les **Total des enregistrements de facturation**. Vous pouvez également voir le total de l’enregistrement de facturation dans l’en-tête de l’enregistrement de facturation.

### Inclure les recettes fixes dans un enregistrement de facturation {#include-fixed-revenues-in-a-billing-record}

Vous pouvez ajouter des recettes fixes à vos enregistrements de facturation si des tâches dont les recettes fixes sont disponibles. Aucun autre type de recettes de tâche ou de projet ne peut être ajouté dans un enregistrement de facturation. Pour plus d’informations sur les types de recettes, consultez la section [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) dans [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Pour ajouter des recettes fixes à un enregistrement de facturation :

1. Accédez au projet avec les enregistrements de facturation.
1. Cliquez sur **Enregistrements de facturation** dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Enregistrements de facturation**.

1. Cliquez sur la **Description** d’un enregistrement de facturation pour ouvrir l’onglet **Informations sur l’enregistrement de facturation** .

1. Sélectionnez l’onglet **Recettes fixes** .
1. Si vous avez ajouté des recettes fixes à vos tâches, cliquez sur **Ajouter des recettes fixes**.

   >[!NOTE]
   >
   >Si des recettes sont affectées à des tâches mais qu’elles ne sont pas marquées comme &quot;fixes&quot;, le bouton **Ajouter des recettes fixes** ne s’affiche pas.

1. Sélectionnez les tâches dont vous souhaitez inclure les recettes fixes dans l&#39;enregistrement de facturation, puis cliquez sur **Ajouter des tâches**.\
   Le **montant des recettes fixes** des tâches est ajouté lorsque le **montant des recettes facturables** correspond au **total des enregistrements de facturation**.

1. (Facultatif) Cliquez sur **Détails des enregistrements de facturation** pour passer en revue les **recettes facturables** et les **totaux des enregistrements de facturation**. Vous pouvez également voir le total de l’enregistrement de facturation dans l’en-tête de l’enregistrement de facturation.

## Modification d’un enregistrement de facturation

Après avoir créé un enregistrement de facturation et inclus les heures, les dépenses et les revenus dans l’enregistrement de facturation, vous pouvez modifier certaines informations de l’enregistrement existant avant qu’il ne soit marqué comme Facturé.

1. Accédez à l’enregistrement de facturation.
1. Lorsque les **détails de l’enregistrement de facturation** sont sélectionnés dans le panneau de gauche, modifiez les informations dans tous les champs disponibles.

   Ou

   Cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) dans le coin supérieur droit, puis modifiez les informations dans les champs disponibles.

   Mettez à jour les éléments suivants :

   * **Description**
   * **État de facturation**

     >[!TIP]
     >
     >Si vous sélectionnez **Facturé** pour l’état de facturation, l’enregistrement de facturation ne peut pas être modifié une fois vos modifications enregistrées.

   * **Date de facturation**
   * **Numéro de bon de commande**
   * **ID de facture**
   * **Montant supplémentaire**

   Les champs suivants ne peuvent pas être modifiés :

   * **Heures facturables :** total des recettes réelles des heures incluses dans l’enregistrement de facturation. Pour plus d’informations sur l’inclusion d’heures dans un enregistrement de facturation, reportez-vous à la section [Inclure des heures facturables dans un enregistrement de facturation](#include-billable-hours-in-a-billing-record) de cet article.

   * **Dépenses facturables** : total du montant réel des dépenses facturables inclus dans l’enregistrement de facturation. Pour plus d’informations sur l’inclusion des dépenses facturables dans un enregistrement de facturation, reportez-vous à la section [Inclure les dépenses facturables dans un enregistrement de facturation](#include-billable-expenses-in-a-billing-record) de cet article.

   * **Recettes facturables** : total des recettes fixes des tâches incluses dans l’enregistrement de facturation. Pour plus d’informations sur l’inclusion des revenus fixes dans un enregistrement de facturation, reportez-vous à la section [ Inclusion des revenus fixes dans un enregistrement de facturation](#include-fixed-revenues-in-a-billing-record) de cet article.

   * **Total des enregistrements de facturation** : total de tous les montants facturables. Elle est calculée par la formule suivante :

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Cliquez sur **Save****Changes**.
