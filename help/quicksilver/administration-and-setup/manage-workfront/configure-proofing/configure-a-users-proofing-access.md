---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configuration de l’accès de vérification de l’utilisateur
description: En tant qu’administrateur Adobe Workfront ou administrateur Workfront BAT, vous pouvez configurer l’accès d’un utilisateur à la création et à l’affichage de BAT dans Workfront et Workfront BAT.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# Configuration de l’accès de vérification de l’utilisateur

En tant qu’administrateur Adobe Workfront ou administrateur Workfront BAT, vous pouvez configurer l’accès d’un utilisateur à la création et à l’affichage de BAT dans Workfront et Workfront BAT.

Pour plus d’informations sur les fonctionnalités de vérification disponibles pour la vérification de base et intégrée, voir [Accès aux fonctionnalités de vérification dans Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un administrateur Workfront ou un administrateur Workfront BAT. Pour plus d’informations sur les administrateurs Workfront, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Activation et désactivation de la vérification pour un utilisateur (plans hérités uniquement) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Si votre entreprise utilise un abonnement Workfront Select ou Premium hérité, en tant qu’administrateur Workfront, vous pouvez activer et désactiver la fonctionnalité de vérification pour l’utilisateur.

Lorsque vous activez la vérification pour un utilisateur, Workfront active l’option de génération automatique de BAT de l’utilisateur.

Bien que vous puissiez activer un utilisateur en tant qu’utilisateur de vérification, il doit disposer des autorisations d’administrateur pour accéder directement à l’interface du bon à tirer Workfront à partir du menu principal de Workfront. Pour plus d’informations sur la manière dont vous pouvez activer cette option pour tous les utilisateurs de la vérification sur votre système Workfront, voir [Configurer l’accès au BAT Workfront via le menu principal de Workfront pour tous les utilisateurs](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. Dans le **Menu Principal**, sélectionnez **Utilisateurs**.

1. Sélectionnez un utilisateur, puis cliquez sur le bouton **Modifier** icône .
1. Dans le **Accès** , sélectionnez ou désélectionnez **L’utilisateur peut générer des BAT**.

## Configuration du profil d’autorisation de BAT d’un utilisateur

Le profil d’autorisation sélectionné est attribué aux utilisateurs pour chaque BAT existant au sein de votre organisation.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png).
1. Sélectionnez un ou plusieurs utilisateurs, puis cliquez sur **Modifier**.

1. Dans le **Accès** Cliquez sur l’une des options d’autorisation de BAT Workfront suivantes dans la section **Profil d’autorisation de preuve** menu déroulant :

   >[!NOTE]
   >
   >Si vous avez souscrit à un plan Workfront hérité, assurez-vous que la variable **L’utilisateur peut générer des BAT** est activée, comme expliqué ci-dessus dans la section . [Activation et désactivation de la vérification pour un utilisateur (plans hérités uniquement)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Superviseur</strong> </td> 
      <td>Les utilisateurs peuvent gérer et afficher tous les bons à tirer créés sur le compte de votre entreprise. Ils peuvent également modifier les opérateurs validants ajoutés à ces BAT. Les utilisateurs disposant de ce profil d’autorisation ne peuvent pas gérer d’utilisateurs ni modifier les paramètres de Bon à tirer de Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gestionnaire</strong> </td> 
      <td> <p> Les utilisateurs peuvent gérer et afficher les bons à tirer créés ou détenus sur le compte de votre entreprise. Ils peuvent afficher les bons à tirer d’autres utilisateurs uniquement lorsqu’ils sont ajoutés en tant que réviseurs. Il s’agit d’un paramètre par défaut. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrateur</strong> </td> 
      <td> Les utilisateurs disposent des autorisations d’administrateur dans le Bon à tirer de Workfront et peuvent modifier les paramètres du compte. Les utilisateurs peuvent gérer et afficher tous les bons à tirer créés sur le compte de votre entreprise. Cela inclut l’ajout et la suppression de réviseurs, de BAT et de commentaires.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personnalisé</strong> </td> 
      <td> <p>Disponible uniquement si vous avez configuré un profil d’autorisation personnalisé dans Workfront BAT.</p> <p><b>NOTE</b>:  <p>Assurez-vous que le profil d’autorisation que vous accordez ici ne fournit pas un accès plus élevé que le paramètre Niveau d’accès de l’utilisateur dans Workfront (voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>). S’il offre un accès supérieur, l’utilisateur peut accéder aux bons à tirer dans le bon à tirer Workfront auxquels il n’a pas accès dans Workfront.</p> <p>Ceci est particulièrement important si vous prévoyez d’autoriser tous les utilisateurs de Workfront à accéder au BAT Workfront directement à partir de Workfront, comme décrit dans la section <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Accès au BAT Workfront à partir d’Adobe Workfront</a>.</p> <p>Par défaut, seuls les administrateurs Workfront ont accès à un lien direct vers le site Workfront Proof à partir de la barre de navigation globale de Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Le profil d’autorisation sélectionné est attribué aux utilisateurs pour chaque BAT existant au sein de votre organisation.

1. Cliquez sur **Enregistrer les modifications** pour terminer la mise à jour des paramètres utilisateur.

   >[!NOTE]
   >
   >Lorsque vous créez ou mettez à jour un utilisateur dans Workfront et que l’adresse électronique Workfront de l’utilisateur correspond à celle d’un utilisateur Workfront Bon à tirer sous licence, le système active la vérification de l’identité de l’utilisateur dans Workfront. Pour plus d’informations, voir [Synchronisation des utilisateurs entre Adobe Workfront et Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considérations

Tenez compte des informations suivantes lors de la définition des autorisations :

* Si vous remplacez le profil d’autorisation d’un utilisateur par un profil avec moins d’autorisations, l’utilisateur risque de perdre de la visibilité sur les bons à tirer existants dans Workfront. Cela peut se produire lorsqu’une personne partage une tâche avec un utilisateur dans Workfront, mais ne partage pas le BAT associé à la tâche (voir [Partage d’un BAT dans Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Partage d’un BAT dans Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* Vous ne pouvez définir des autorisations de BAT Workfront à partir de Workfront que si votre environnement Workfront est intégré à un compte Workfront Proof Premium. Si vous ne pouvez pas utiliser le correctif comme décrit dans cette section, contactez votre administrateur Workfront.
* Au moins un utilisateur de votre environnement Workfront doit disposer des autorisations d’administrateur pour la vérification. Un message d’erreur s’affiche si vous tentez de supprimer les autorisations Administrateur pour la vérification de tous les utilisateurs.
* Lorsque vous définissez le niveau d’accès Workfront d’un utilisateur sur un niveau autre que Administrateur système, le profil d’autorisation Workfront Proof de l’utilisateur prend par défaut la valeur Manager.

* Lorsque vous définissez le niveau d’accès Workfront sur Administrateur système, le profil d’autorisation des BAT passe à Administrateur.

## Configurer l’accès au BAT Workfront via le menu principal de Workfront pour tous les utilisateurs {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Par défaut, seuls les utilisateurs disposant de droits d’administration dans Workfront peuvent accéder au Bon à tirer de Workfront, comme décrit  [Accès au BAT Workfront à partir d’Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Vous pouvez accorder à tous les utilisateurs l’accès au bouton Bon à tirer de Workfront dans le menu principal de Workfront en contactant l’assistance Workfront et en envoyant une demande.

>[!IMPORTANT]
>
> Si vous prévoyez d’autoriser tous les utilisateurs de Workfront à accéder au Bon à tirer de Workfront directement à partir de la barre de navigation globale de Workfront, assurez-vous que le profil d’autorisation de chaque utilisateur ne fournit pas un accès supérieur à celui de l’utilisateur dans Workfront. Cela empêche les utilisateurs d’accéder aux bons à tirer dans Workfront, auxquels ils ne peuvent pas accéder dans Workfront. Pour plus d’informations, voir [Activation et désactivation de la vérification pour un utilisateur (plans hérités uniquement)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configuration de l’accès des utilisateurs à la visionneuse de vérification de l’appli de bureau

Si les utilisateurs de votre entreprise préfèrent utiliser la visionneuse de vérification de l’appli de bureau au lieu de la visionneuse de vérification de l’application web pour passer en revue le contenu interactif, vous pouvez configurer la visionneuse de vérification de l’appli de bureau afin qu’elle soit lancée automatiquement lorsque les utilisateurs ouvrent des bons à tirer du contenu interactif. Pour plus d’informations à ce sujet, voir Visionneuse de vérification de l’appli de bureau et en quoi elle diffère de la visionneuse de vérification de l’appli de bureau Web. [Présentation de la visionneuse de vérification de l’appli de bureau](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) et [Présentation des différences entre la visionneuse de test Web et la visionneuse de test de bureau](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. Dans Workfront, cliquez sur l’icône BAT Workfront de la barre de navigation globale pour accéder au BAT Workfront.

   ![](assets/proof-access-proofhq-350x39.png)

1. Cliquez sur **Paramètres du compte** près du coin supérieur droit du BAT Workfront, puis cliquez sur le bouton **Paramètres** .

1. Sous **Valeurs par défaut des BAT**, à la fin de la variable **Visionneuse de vérification de l’appli de bureau pour la vérification interactive** ligne, cliquez sur **Configuration**.

1. Modifiez les paramètres de la visionneuse de vérification de l’appli de bureau, comme décrit dans la section [Visionneuse de vérification de poste de travail](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) dans l’article [Configuration des paramètres du BAT pour votre organisation](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Cliquer sur **Enregistrer**.

## Configuration de périphériques personnalisés pour les bons à tirer interactifs

Vous pouvez ajouter des appareils personnalisés à votre système, ce qui permet aux utilisateurs de passer en revue le contenu interactif et de simuler l’affichage du contenu sur un appareil spécifique lorsqu’ils utilisent la visionneuse de vérification de l’appli de bureau. (Cette fonctionnalité n’est pas disponible dans la visionneuse de test Web, où les utilisateurs peuvent consulter du contenu interactif, mais uniquement tel qu’il apparaît dans diverses résolutions, et non sur divers appareils.)

Pour plus d’informations, voir [Modification de la résolution du BAT interactif dans la visionneuse de correctifs](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. À partir de Workfront, accédez à l’interface du Bon à tirer de Workfront, comme décrit dans la section [Accès au BAT Workfront à partir d’Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modifiez les paramètres de la visionneuse de vérification de l’appli de bureau, comme décrit dans la section [Configuration de périphériques personnalisés pour les bons à tirer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) dans l’article [Configuration des paramètres du BAT pour votre organisation](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
