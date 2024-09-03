---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuration des paramètres de BAT pour votre organisation
description: En tant qu’administrateur ou administratrice Adobe Workfront ou Workfront Proof, vous pouvez personnaliser les paramètres des épreuves par défaut pour votre organisation. Ces paramètres comprennent les options de partage par défaut, l’image de marque, etc.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '1221'
ht-degree: 99%

---

# Configurer les paramètres des épreuves pour votre organisation

En tant qu’administrateur ou administratrice Adobe Workfront ou Workfront Proof, vous pouvez personnaliser les paramètres des épreuves par défaut pour votre organisation. Ces paramètres comprennent les options de partage par défaut, l’image de marque, etc.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Plan actuel : Pro ou version supérieure</p> <p>ou</p> <p>Formule héritée : Premium ou Select</p> <p>Pour plus d’informations sur la relecture de l’accès avec les différents plans, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Plan hérité : n’importe lequel (la relecture doit être activée pour l’utilisateur ou l’utilisatrice)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>L’option d’administration doit être sélectionnée dans votre profil d’autorisation d’épreuve. Pour plus d’informations, voir la section <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurer l’accès à la relecture d’un utilisateur ou d’une utilisatrice</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Configurer des actions

Pour plus d’informations sur l’utilisation des actions dans l’affichage de relecture, voir la section [Utiliser des actions sur les commentaires des épreuves](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md).

Vous pouvez configurer des actions pour votre organisation comme suit :

* [Ajouter ou renommer une action](#add-or-rename-an-action)
* [Désactiver ou réactiver une action](#deactivate-or-reactivate-an-action)
* [Réorganiser les actions](#reorder-actions)

### Ajouter ou renommer une action {#add-or-rename-an-action}

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte** en haut à droite de l’interface Workfront Proof, puis cliquez sur l’onglet **Paramètres**.

1. Utilisez l’une des méthodes suivantes :

   * Pour créer une action, cliquez sur **Nouvelle action** dans la section **Actions**.

     Le nombre d’actions que vous pouvez configurer dans votre compte n’est pas limité.

   * Pour renommer une action existante, cliquez sur **Configuration** en regard de l’action.

1. Saisissez le nom de l’action, puis cliquez sur **Enregistrer**.
1. Cliquez sur **Enregistrer**.

### Désactiver ou réactiver une action {#deactivate-or-reactivate-an-action}

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte** en haut à droite de l’interface de Workfront Proof, puis cliquez sur l’onglet **Paramètres**.

1. Cliquez sur **Configuration** en regard de l’action à désactiver ou à réactiver.
1. Sélectionnez **Activer** ou **Désactiver**, puis cliquez sur **Enregistrer**.

### Réorganiser les actions {#reorder-actions}

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte** en haut à droite de l’interface de Workfront Proof, puis cliquez sur l’onglet **Paramètres**.

1. Cliquez sur les flèches bleues vers le haut et le bas en regard de **Configuration** pour réorganiser les actions.

   ![Re-order_actions.png](assets/re-order-actions-350x103.png)

## Configurer des appareils personnalisés pour les épreuves

Vous pouvez ajouter n’importe quel appareil personnalisé à votre système, ce qui permet aux utilisateurs et utilisatrices de réviser le contenu interactif et de simuler l’affichage du contenu sur un appareil spécifique.

Pour plus d’informations sur la manière dont les utilisateurs et utilisatrices peuvent sélectionner des appareils lors de la révision d’un contenu interactif, voir la section [Modifier la résolution d’épreuves interactives dans la visionneuse de relecture](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

Pour ajouter un appareil personnalisé :

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte** en haut à droite de l’interface de Workfront Proof, puis cliquez sur l’onglet **Paramètres**.

1. Dans la section **Appareils personnalisés pour les épreuves**, cliquez sur **Ajouter un nouvel appareil**.

1. Dans le **Ajouter un nouvel appareil** qui s’affiche, indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td>Nom que les utilisateurs et utilisatrices voient lors de la sélection de l’appareil dans la visionneuse de relecture de l’application de bureau, comme décrit dans la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">Modifier la résolution d’épreuve interactive dans la visionneuse de relecture</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensions</td> 
      <td>Spécifiez les dimensions à utiliser pour cet appareil. Les utilisateurs et utilisatrices voient les dimensions affichées sous le nom de l’appareil.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rapport</td> 
      <td>Spécifiez le rapport pour l’appareil.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type</td> 
      <td>Indiquez si l’appareil est de catégorie Mobile, Tablette ou Bureau.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chaîne de l’agent utilisateur</td> 
      <td>Saisissez l’agent utilisateur de l’appareil pour fournir des informations qui permettent à notre logiciel de s’exécuter et de s’afficher comme prévu pour l’appareil.<p>Vous pouvez obtenir l’agent utilisateur en accédant à <a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a> à partir de l’appareil.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Désactivé</td> 
      <td>Si cette option est sélectionnée, l’appareil n’est pas disponible à la sélection pour les utilisateurs et utilisatrices lors de la révision des épreuves interactives.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Créer**.

## Configurer le messages contextuels pour les épreuves

Vous pouvez configurer des messages contextuels sur les épreuves pour communiquer des informations générales à tous les réviseurs et réviseuses de votre organisation.

Vous pouvez paramétrer l’affichage des messages dans les cas suivants :

* **Au message de chargement** : s’affiche lors de la première ouverture de l’épreuve. Utile pour expliquer aux utilisateurs et utilisatrices comment réviser une épreuve ou fournir une clause de non-responsabilité ou tout autre texte juridique.
* **Message de décision** : s’affiche lorsqu’un utilisateur ou une utilisatrice sélectionne une décision sur une épreuve. Utile pour fournir des listes de contrôle à vos utilisateurs et utilisatrices pour des éléments tels que la conformité à la marque ou la réglementation. Pour plus d’informations sur les décisions, voir [Prendre une décision sur une épreuve dans la visionneuse de relecture](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

* **Confirmer le texte du bouton** : libellé qui s’affiche sur le bouton dans le message pop-up Au chargement expliqué ci-dessus.

Pour créer des messages pop-up pour les épreuves :

1. Cliquez sur **Modifier** à droite du message que vous souhaitez personnaliser.
1. Spécifiez un message et incluez la mise en forme appropriée, puis cliquez sur **Enregistrer**.
1. (Facultatif) Si vous avez personnalisé le message Au chargement et que vous souhaitez également personnaliser le libellé du bouton de confirmation, cliquez sur **Modifier** à droite de **Confirmer le texte du bouton**, spécifiez un libellé, puis cliquez sur **Enregistrer**.

## Configurer les paramètres par défaut des épreuves

Pour plus d’informations sur la configuration des paramètres par défaut de l’épreuve pour votre organisation, voir [Configuration des paramètres d’épreuve par défaut](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).


## Configurer les paramètres de partage par défaut

Vous pouvez spécifier avec qui les épreuves de votre entreprise peuvent être partagées, les versions disponibles pour les réviseurs et réviseuses et le moment où les épreuves avec un workflow automatisé sont visibles pour les utilisateurs et utilisatrices associés à une étape donnée.

Pour plus d’informations sur le partage des paramètres dans Workfront Proof voir [Configuration des paramètres de partage pour vos utilisateurs et utilisatrices](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md).

## Effectuer le branding du site de Workfront Proof

Si vous utilisez Workfront Proof, vous pouvez configurer le branding pour les zones suivantes du site :

* Page de démarrage qui s’affiche au chargement de l’épreuve
* Écrans de connexion et de déconnexion
* Notifications par e-mail

Pour plus d’informations sur la manière d’effectuer le branding du site Workfront Proof, voir [Effectuer le branding du site de Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).

## Configurer les paramètres de mot de passe avancés

>[!IMPORTANT]
>
>Cette option est disponible uniquement pour les formules Workfront héritées. Si vous utilisez une formule Pro, Business ou Entreprise de Workfront, vous ne pouvez plus configurer de paramètres avancés de mot de passe.

Sous **Paramètres de mot de passe avancés**, vous pouvez améliorer la sécurité des mots de passe de vos utilisateurs et utilisatrices.

1. Cliquez sur **Configuration** à droite du paramètre que vous souhaitez configurer :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Longueur minimale du mot de passe</td> 
      <td>La longueur par défaut du mot de passe Workfront Proof est de six caractères. Vous pouvez augmenter le nombre en fonction des politiques de votre entreprise.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Combinaison de caractères</strong> </td> 
      <td>Vous pouvez forcer les utilisateurs et utilisatrices à utiliser une combinaison de minuscules, de majuscules, de nombres et de symboles dans leurs mots de passe. Vous décidez du nombre de caractères que doit contenir le mot de passe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Répétition maximale des caractères</strong> </td> 
      <td>Vous pouvez spécifier le nombre de caractères pouvant se répéter dans le mot de passe de chaque personne.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Expiration automatique de mot de passe</td> 
      <td>Oblige les utilisateurs et utilisatrices à changer régulièrement leur mot de passe. Vous décidez de la fréquence à laquelle ils le feront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Nombre de répétitions de mot de passe non autorisées</strong> </td> 
      <td>Configurez le nombre de répétitions de mot de passe non autorisées dans votre compte.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Verrouillage du profil</strong> </td> 
      <td>Empêche les utilisateurs et utilisatrices d’accéder à leur compte après un nombre de tentatives de connexion infructueuses que vous avez spécifié. Vous pouvez également spécifier la durée pendant laquelle ils doivent attendre avant de pouvoir accéder à nouveau à leur compte.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’utilisateur ou l’utilisatrice si le mot de passe n’est pas réinitialisé après 30 jours.</td> 
      <td>Si la personne ne modifie pas son mot de passe initial dans les 30 jours suivant l’activation de son profil, elle ne peut plus accéder à son compte.<br><p>Les équipes d’administration de compte peuvent déverrouiller (réactiver) les personnes dont l’accès est automatiquement bloqué par le système. Cela leur laissera sept jours supplémentaires pour modifier leur mot de passe.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller le compte d’utilisateur ou d’utilisatrice s’il est inactif pendant 120 jours</td> 
      <td>Si votre utilisateur ou utilisatrice ne se connecte pas à Workfront Proof ou à une épreuve nécessitant une connexion pendant 120 jours, la personne ne peut plus accéder au compte.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Changer de mot de passe après la première connexion</strong> </td> 
      <td>Nécessite que les utilisateurs et utilisatrices modifient leur mot de passe temporaire après leur première connexion.<p>Les équipes d’administration de compte peuvent déverrouiller (réactiver) les personnes qui sont automatiquement bloquées par le système.</p><p>Pour plus d’informations sur les mots de passe, voir <a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">Se connecter et changer le mot de passe et l’e-mail pour Workfront Proof</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>
