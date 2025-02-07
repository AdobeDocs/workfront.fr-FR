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
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 99%

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

## Activer et désactiver la relecture pour un utilisateur ou une utilisatrice (plans hérités uniquement) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Si votre entreprise dispose d’une formule Workfront Select ou Premium héritée, en tant qu’administrateur ou administratrice Workfront, vous pouvez activer et désactiver la fonctionnalité de relecture pour l’utilisateur ou l’utilisatrice.

Lorsque vous activez la relecture pour un utilisateur ou une utilisatrice, Workfront active l’option de génération automatique d’épreuves de l’utilisateur ou de l’utilisatrice.

Vous pouvez accorder un accès en relecture à un utilisateur ou une utilisatrice, mais pour que cette personne puisse accéder directement à l’interface de Workfront Proof à partir du menu principal de Workfront, elle doit également disposer d’autorisations d’administration. Pour plus d’informations sur la manière de procéder à l’échelle de votre système Workfront, consultez la section [Configurer l’accès à Workfront Proof à partir du menu principal de Workfront pour tous les utilisateurs et utilisatrices](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. Dans le **Menu principal**, sélectionnez **Utilisateurs et utilisatrices**.

1. Sélectionnez une personne, puis cliquez sur l’icône **Modifier**.
1. Dans la section **Accès**, sélectionnez ou désélectionnez **L’utilisateur ou l’utilisatrice peut générer des épreuves**.

## Configurer le profil d’autorisation d’épreuve d’un utilisateur ou d’une utilisatrice

Le profil d’autorisation que vous sélectionnez est attribué aux personnes pour chaque épreuve existante au sein de votre organisation.

{{step-1-to-users}}

1. Sélectionnez une ou plusieurs personnes, puis cliquez sur **Modifier**.

1. Dans la section **Accès**, cliquez sur l’une des options d’autorisation de Workfront Proof suivantes dans le menu déroulant **Profil d’autorisation d’épreuve** :

   >[!NOTE]
   >
   >Si vous avez souscrit à un plan Workfront hérité, assurez-vous d’activer l’option **L’utilisateur ou l’utilisatrice peut générer des épreuves**, comme décrit ci-dessus dans la section [Activer et désactiver la relecture pour un utilisateur ou une utilisatrice (plans hérités uniquement)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Superviseur ou superviseuse</strong> </td> 
      <td>Les utilisateurs et utilisatrices peuvent gérer et afficher toutes les épreuves créées sur le compte de votre entreprise. Ils peuvent également modifier les personnes réviseuses ajoutées à ces épreuves. Les utilisateurs et utilisatrices disposant de ce profil d’autorisation ne peuvent pas gérer d’utilisateurs et d’utilisatrices ni modifier les paramètres de Workfront Proof.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personne gestionnaire</strong> </td> 
      <td> <p> Les utilisateurs et utilisatrices peuvent gérer et afficher les épreuves créées ou détenues sur le compte de votre entreprise. Ils peuvent afficher les épreuves d’autres utilisateurs et utilisatrices uniquement lorsqu’ils sont ajoutés en tant que personnes réviseuses. Il s’agit du paramètre par défaut. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrateur ou administratrice</strong> </td> 
      <td> Les utilisateurs et utilisatrices disposent d’autorisations d’administration dans Workfront Proof et peuvent modifier les paramètres du compte. Les utilisateurs et utilisatrices peuvent gérer et afficher toutes les épreuves créées sur le compte de votre entreprise. Cela inclut l’ajout et la suppression de personnes réviseuses, d’épreuves et de commentaires.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personnalisé</strong> </td> 
      <td> <p>Disponible uniquement si vous avez configuré un profil d’autorisation personnalisé dans Workfront Proof.</p> <p><b>NOTE</b> :  <p>Assurez-vous que le profil d’autorisation que vous accordez ici ne fournit pas un accès plus élevé que le paramètre Niveau d’accès de l’utilisateur ou de l’utilisatrice dans Workfront (consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>). Si le profil offre un accès supérieur, la personne peut accéder aux épreuves dans Workfront Proof auxquelles elle n’a pas accès dans Workfront.</p> <p>Tenez-en compte si vous prévoyez d’autoriser tous les utilisateurs et utilisatrices Workfront à accéder à Workfront Proof directement à partir de Workfront, comme décrit dans la section <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Accéder à Workfront Proof à partir d’Adobe Workfront</a>.</p> <p>Par défaut, seule l’administration Workfront a accès à un lien direct vers le site Workfront Proof à partir de la barre de navigation globale de Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Le profil d’autorisation que vous sélectionnez est attribué aux personnes pour chaque épreuve existante au sein de votre organisation.

1. Cliquez sur **Enregistrer les modifications** pour terminer la mise à jour des paramètres utilisateur.

   >[!NOTE]
   >
   >Lorsque vous créez ou mettez à jour une personne dans Workfront et que l’adresse e-mail Workfront de cette personne correspond à celle d’un utilisateur ou d’une utilisatrice de Workfront Proof sous licence, le système active la vérification de l’identité de la personne dans Workfront. Pour plus d’informations, voir [Synchronisation des utilisateurs et utilisatrices entre Adobe Workfront et Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considérations

Tenez compte des informations suivantes lors du paramétrage des autorisations :

* Si vous remplacez le profil d’autorisation d’une personne par un profil avec moins d’autorisations, la personne risque de perdre de la visibilité sur les épreuves existantes dans Workfront. Cela peut se produire lorsqu’une personne partage une tâche avec un utilisateur ou une utilisatrice dans Workfront, mais ne partage pas l’épreuve associée à la tâche (voir [Partager une épreuve dans Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) dans [Partager une épreuve dans Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* Vous ne pouvez définir des autorisations d’épreuves Workfront à partir de Workfront que si votre environnement Workfront est intégré à un compte Workfront Proof Premium. Si vous ne pouvez pas utiliser la relecture comme décrit dans cette section, contactez votre équipe d’administration Workfront.
* Au moins un utilisateur ou une utilisatrice de votre environnement Workfront doit disposer des autorisations d’administration pour la relecture. Un message d’erreur s’affiche si vous tentez de supprimer les autorisations d’administration pour la vérification de tous les utilisateurs et utilisatrices.
* Lorsque vous définissez le niveau d’accès Workfront d’une personne sur un niveau autre qu’administration système, le profil d’autorisation Workfront Proof de la personne prend par défaut la valeur de responsable.

* Lorsque vous définissez le niveau d’accès Workfront sur Administrateur ou administratrice système, le profil d’autorisation des épreuves passe à Administrateur ou administratrice.

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
