---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configuration de l'accès à la relecture d'un utilisateur
description: En tant qu’administrateur ou administratrice Adobe Workfront ou Workfront Proof, vous pouvez configurer l’accès d’un utilisateur ou d’une utilisatrice à la création et à l’affichage des épreuves dans Workfront et Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
TQID: 'https://experienceleague.adobe.com/L-AMDvQYgtXJwxmtwekimbEA9OQQN72QHIcoQ2iKzGU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4ea8bc003ce17978be5e5a6fd838012dfcfeae78
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 98%
---
# Configurer l’accès à la relecture pour une personne

En tant qu’administrateur ou administratrice Adobe Workfront ou Workfront Proof, vous pouvez configurer l’accès d’un utilisateur ou d’une utilisatrice à la création et à l’affichage des épreuves dans Workfront et Workfront Proof.

Pour plus d’informations sur les fonctionnalités de relecture disponibles pour la relecture de base et intégrée, consultez la section [Accès aux fonctionnalités de relecture dans Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront ou Workfront Proof. Pour plus d’informations sur l’administration Workfront, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à un utilisateur ou une utilisatrice</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

<!--

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

{{step-1-to-users}}
 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile** drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only). 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Users can manage and view all proofs created on your organization's account. They can also edit reviewers added to these proofs. Users with this permission profile can't manage users or edit Workfront Proof settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Users can manage and view proofs created or owned on your organization's account. They can view other users' proofs only when added as a reviewer. This is a default setting. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Users are given Administrator permissions in Workfront Proof and can edit account settings. Users can manage and view all proofs created on your organization's account. This includes adding and removing reviewers, proofs, and comments.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom</strong> </td> 
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p><b>NOTE</b>:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's Access Level setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes** to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront. For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront. This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

-->

## Configurer l’accès à Workfront Proof via le menu principal de Workfront pour tous les utilisateurs et utilisatrices {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Par défaut, seules les personnes disposant de droits d’administration dans Workfront peuvent accéder à Workfront Proof, comme décrit dans [Accéder à Workfront Proof à partir d’Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Vous pouvez accorder à toutes les personnes l’accès au bouton Workfront Proof dans le menu principal de Workfront en contactant le support Workfront et en envoyant une demande.

>[!IMPORTANT]
>
> Si vous prévoyez d’autoriser tous les utilisateurs et utilisatrices de Workfront à accéder à Workfront Proof directement à partir de la barre de navigation globale de Workfront, assurez-vous que le profil d’autorisation de chaque personne ne fournit pas un accès supérieur à celui de cette personne dans Workfront. Cela empêche les personnes d’accéder à des épreuves dans Workfront Proof auxquelles elles ne peuvent pas accéder dans Workfront. Pour plus d’informations, voir [Activer et désactiver la relecture pour une personne (plans hérités uniquement)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configurer l’accès des personnes à la visionneuse de relecture de bureau

Si les personnes de votre entreprise préfèrent utiliser la visionneuse de relecture de bureau au lieu de la visionneuse de relecture web pour passer en revue le contenu interactif, vous pouvez configurer la visionneuse de relecture de bureau afin qu’elle soit lancée automatiquement lorsque les personnes ouvrent des épreuves du contenu interactif. Pour plus d’informations concernant la visionneuse de relecture de bureau et en quoi elle diffère de la visionneuse de relecture web, voir [Présentation de la visionneuse de relecture de bureau](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) et [Vue d’ensemble des différences entre la visionneuse de relecture web et la visionneuse de relecture de bureau](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. Dans Workfront, cliquez sur l’icône Workfront Proof de la barre de navigation globale pour accéder à Workfront Proof.

   ![Icône de BAT](assets/proof-access-proofhq-350x39.png)

1. Cliquez sur **Paramètres du compte** près du coin supérieur droit de Workfront Proof, puis cliquez sur l’onglet **Paramètres**.

1. Sous **Valeurs par défaut des épreuves**, à la fin de la ligne **Visionneuse de relecture de bureau pour la relecture interactive**, cliquez sur **Configuration**.

1. Modifiez les paramètres de la visionneuse de relecture de bureau, comme décrit dans la section [Visionneuse de relecture de bureau](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) dans l’article [Configurer les paramètres des épreuves pour votre organisation](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Cliquer sur **Enregistrer**.

## Configurer les appareils personnalisés pour les épreuves interactives

Vous pouvez ajouter des appareils personnalisés à votre système, ce qui permet aux personnes de passer en revue le contenu interactif et de simuler l’affichage du contenu sur un appareil spécifique lorsqu’elles utilisent la visionneuse de relecture de bureau. (Cette fonctionnalité n’est pas disponible dans la visionneuse de relecture web, où les personnes peuvent consulter du contenu interactif, mais uniquement tel qu’il apparaît dans diverses résolutions, et non sur divers appareils.)

Pour plus d’informations, voir [Modifier la résolution des épreuves interactives dans la visionneuse de relecture](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. À partir de Workfront, accédez à l’interface de Workfront Proof, comme décrit dans [Accéder à Workfront Proof à partir d’Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modifiez les paramètres de la visionneuse de relecture de bureau, comme décrit dans [Configurer des appareils personnalisés pour les épreuves](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) dans l’article [Configurer les paramètres des épreuves pour votre organisation](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
