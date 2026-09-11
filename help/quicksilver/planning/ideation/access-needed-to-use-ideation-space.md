---
title: Accès nécessaire pour utiliser l’espace d’idéation
description: Adobe Workfront Planning offre désormais une fonctionnalité supplémentaire pour identifier avant de lancer vos campagnes. Tirez parti de la puissance de l’IA pour transformer les données et orienter les entrées en plans tangibles et donner aux équipes un point de départ éclairé au lieu d’une page vierge avec l’espace Adobe Idéation.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 3%

---


# Accès nécessaire pour utiliser l’espace Idéation

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Il est disponible uniquement dans le cadre du programme **Ideation space Beta**. </span>

<span class="preview">Pour plus d’informations, voir [Prise en main de l’espace d’idéation pour Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>


{{planning-important-intro}}

Adobe Workfront Planning offre désormais une fonctionnalité supplémentaire pour identifier avant de lancer vos campagnes. Tirez parti de la puissance de l’IA pour transformer les données et orienter les entrées en plans tangibles et donner aux équipes un point de départ éclairé au lieu d’une page vierge avec l’espace Adobe Idéation.

Cet article décrit l’accès et les autorisations dont vous devez disposer pour accéder à l’espace d’idéation à partir de Workfront Planning.

Pour obtenir des informations générales sur l’espace d’idée, consultez [Prise en main de l’espace d’idée pour Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).

## Exigences du produit

L&#39;espace Idéation n&#39;est pas un produit autonome. Il nécessite un package Workfront Planning et il n’est accessible qu’à partir de Workfront Planning. Il nécessite également des produits supplémentaires.

Votre entreprise doit acheter un package pour les produits suivants afin d&#39;accéder à l&#39;espace d&#39;idéation :

* Un package de workflow Adobe Workfront en plus d’un package Planning

  Ou

  Un planning Adobe Workfront acheté en tant que produit autonome.
* Une licence Adobe GenStudio for Performance Marketing

  >[!TIP]
  >
  >GenStudio for Performance Marketing est nécessaire pour avoir accès aux droits corrects sur les polices.


<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Exigences de niveau d’accès pour la planification Workfront

L’accès à l’emplacement est configuré dans Workfront.

Votre niveau d’accès Workfront doit inclure les éléments suivants pour accéder à l’espace d’idéation :

* Une licence Workflow standard, lorsque votre société a acheté un package Workflow en plus d’un package Planning.
* Une licence Planning standard, lorsque votre société a acheté avec un package Workflow et Planning, ou un Planning Workfront en tant que produit autonome.
* Le paramètre Désactiver l’espace d’idéation dans la section Définir une restriction supplémentaire de votre niveau d’accès doit être désélectionné. <!--***********check the UI for this***********-->

## Exigences d’autorisations pour Workfront Planning

Chaque enregistrement Planning est associé à un brief dans l&#39;espace Idéation .

Les autorisations brèves de l’espace d’idéation sont héritées des autorisations d’enregistrement de Workfront Planning. <!--not sure if this is right, because now you can share the ideation with others??-->

Vous devez disposer des autorisations de niveau Gérer pour un type d&#39;enregistrement dans Planning afin de créer ou de modifier un enregistrement dans l&#39;espace d&#39;idéation.

Les utilisateurs de Planning disposant d&#39;autorisations d&#39;affichage sur les enregistrements peuvent afficher l&#39;espace d&#39;idéation d&#39;un enregistrement.

Le tableau suivant montre le lien entre les autorisations d’enregistrement de Workfront Planning et les autorisations de courte durée de l’espace d’idéation :

| Autorisation au niveau des enregistrements Planning | Autorisations de court niveau de l’espace d’idéation |
|---|---|
| Gérer les autorisations pour un enregistrement | Peut créer un brief dans l’Espace idéation de l’enregistrement |
| Afficher les autorisations pour un enregistrement | Peut lire le brief de cet enregistrement dans l’espace Idéation, mais ne peut pas le modifier |

## Autorisations de l’emplacement

<!--this is also duplicated in the intro of the Share an ideation space article-->

Les autorisations Planning sont transférées vers l’espace d’idéation d’un enregistrement.

En outre, vous pouvez accorder à d’autres utilisateurs les autorisations nécessaires pour utiliser l’espace d’idéation et y ajouter des idées.

Tenez compte des points suivants :

* Les créateurs d’idées disposent toujours des autorisations d’éditeur sur leurs propres idées.

* Vous devez disposer des autorisations d’éditeur sur un espace d’idéation pour créer des résumés et les exporter vers d’autres applications.

Vous trouverez ci-dessous les autorisations d’espace d’idéation et les fonctionnalités qu’elles offrent :

| Autorisation de l’emplacement | Fonctionnalités |
|---|---|
| Éditeur | Peut modifier, télécharger et partager l’espace d’idéation |
| Commentateur | Peut afficher et commenter l’espace d’idéation |
| Observateur | Peut afficher l’espace d’idéation |

Pour plus d&#39;informations sur le partage d&#39;un espace d&#39;idéation, voir [Partager un espace d&#39;idéation](/help/quicksilver/planning/ideation/share-the-ideation-space.md).

<!--there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users-->


<!-- 
Not sure if this is needed. Maybe all orgs have IMS for all Adobe?? - asking Becky: 

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Ideation space experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use the Ideation space directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for the Ideation space, not just assumed via GenS.
-->



<!--
From Claude: Internal information, not customer-facing: 

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If the Coworker integration inside the Ideation space is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
-->

<!--

Original Claude write-up, in addition to the info above:

## Baseline product requirement

The Ideation space isn't a standalone purchase — you need **Workfront Planning** to access it, through either:

- Adobe Workfront Workflow with a Workfront Planning package, or
- Adobe Workfront Planning as a standalone product

If your org has Workfront Planning, it has the Ideation space too. The Ideation space can't exist without Planning.

For the Closed Beta and Open Beta, the Ideation space is available only to Planning and GenStudio (GenS) customers.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:

- An active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist or ideation user who will be the primary Ideation space user

## Org- and user-level enablement

- Workfront surfaces the Ideation space integration to users only after a Workfront administrator enables the **strategic ideation** product at the org level.
- During the Closed Beta, a user-level feature flag also controls access, so org-level enablement alone isn't enough.
- For Open Beta, access is expected to move to an opt-in model, where customers actively configure themselves in, rather than opt-out.

## Record-level permissions

Your Ideation space permissions come from your Workfront Planning record permissions — there's no separate permission system layered on top:

- If you can create a record in Planning, you can also create a canvas in the Ideation space. Any Planning license is sufficient for this.
- If you have read-only access to a record, you have read-only access to the canvas connected to that record.
- If you only have view access to an existing record, you can't open the Ideation space from it. Workfront shows an "Insufficient permissions" message instead.
- Each canvas is related to exactly one record.

>[!NOTE]
>As of August 2026, the team was still defining discrete access levels for the Ideation space. These are expected to include, at minimum, Can read, Can view, and Can create.

## Org and IMS-level entitlements

Beyond Planning access, your organization's IMS Org needs specific entitlements for the Ideation space to work fully.

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | A missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform or document storage entitlement | Entitlement | Users may be able to reach Ideation space entry points but fail during actual use if storage-related entitlements are missing |

>[!IMPORTANT]
>When you provision a customer, confirm that both the Planning and GenStudio PEM entitlements are set up specifically for the Ideation space. Don't assume that GenStudio (GenS) provisioning alone includes Ideation space access.

## Content-sharing and abuse controls

Because the Ideation space lets you create content and share it with other users through Adobe systems, a **Report Abuse** capability is planned as a requirement before General Availability (GA). Workfront needs this roughly one month ahead of GA to support Adobe's platform license agreement process. This capability may reuse the existing Report Abuse functionality from Adobe Horizon rather than being built from scratch.

## Coworker (conversational AI) access

Access to the **Coworker** integration inside the Ideation space, the conversational right-rail assistant, is being rolled out separately from core Ideation space and Planning access:

- As of mid-August 2026, Coworker access wasn't yet generally available for customer testing.
- By August 17, 2026, Coworker was available inside the Ideation space for internal use, but still being refined.
- If you're documenting or testing the Coworker integration inside the Ideation space specifically, verify current availability separately. Don't assume it's included automatically with standard Planning or Ideation space provisioning.

For more information, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

-->
