---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuration des paramètres de BAT pour votre organisation
description: En tant qu’administrateur Adobe Workfront ou administrateur Workfront Proof, vous pouvez personnaliser les paramètres de BAT par défaut de votre entreprise. Ces paramètres comprennent les options de partage par défaut, la valorisation de marque, etc.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '1221'
ht-degree: 3%

---

# Configuration des paramètres du BAT pour votre organisation

En tant qu’administrateur Adobe Workfront ou administrateur Workfront Proof, vous pouvez personnaliser les paramètres de BAT par défaut de votre entreprise. Ces paramètres comprennent les options de partage par défaut, la valorisation de marque, etc.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : Premium ou Sélectionner</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>L’administrateur doit être sélectionné dans votre profil d’autorisation de BAT. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configuration de l’accès de vérification de l’utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Configuration des actions

Pour plus d’informations sur l’utilisation des actions dans la visionneuse de vérification, voir [Utilisation d’actions sur les commentaires de BAT](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md).

Vous pouvez configurer des actions pour votre organisation comme suit :

* [Ajouter ou renommer une action](#add-or-rename-an-action)
* [Désactiver ou réactiver une action](#deactivate-or-reactivate-an-action)
* [Réorganiser les actions](#reorder-actions)

### Ajouter ou renommer une action {#add-or-rename-an-action}

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte** dans le coin supérieur droit de l’interface de Workfront Proof, puis cliquez sur l’onglet **Paramètres** .

1. Effectuez l’une des opérations suivantes :

   * Pour créer une action, dans la section **Actions**, cliquez sur **Nouvelle action**.

     Le nombre d’actions que vous pouvez configurer dans votre compte n’est pas limité.

   * Pour renommer une action existante, cliquez sur **Configuration** en regard de l’action.

1. Saisissez le nom de l’action, puis cliquez sur **Enregistrer**.
1. Cliquez sur **Enregistrer.**

### Désactivation ou réactivation d’une action {#deactivate-or-reactivate-an-action}

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte** dans le coin supérieur droit de l’interface de Workfront Proof, puis cliquez sur l’onglet **Paramètres** .

1. Cliquez sur **Configuration** en regard de l’action que vous souhaitez désactiver ou réactiver.
1. Sélectionnez **Activer** ou **Désactiver**, puis cliquez sur **Enregistrer**.

### Réorganiser les actions {#reorder-actions}

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte** dans le coin supérieur droit de l’interface de Workfront Proof, puis cliquez sur l’onglet **Paramètres** .

1. Cliquez sur les flèches Haut et Bas bleues en regard de **Configuration** pour réorganiser les actions.

   ![Re-order_actions.png](assets/re-order-actions-350x103.png)

## Configuration de périphériques personnalisés pour les bons à tirer

Vous pouvez ajouter n’importe quel appareil personnalisé à votre système, ce qui permet aux utilisateurs de passer en revue le contenu interactif et de simuler l’affichage du contenu sur un appareil spécifique.

Pour plus d’informations sur la façon dont les utilisateurs peuvent sélectionner les appareils lors de la révision du contenu interactif, voir [Modification de la résolution du BAT interactif dans la visionneuse de vérification de l’orthographe](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)

Pour ajouter un appareil personnalisé :

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte** dans le coin supérieur droit de l’interface de Workfront Proof, puis cliquez sur l’onglet **Paramètres** .

1. Dans la section **Périphériques personnalisés pour les bons à tirer**, cliquez sur **Ajouter un nouvel appareil**.

1. Dans la zone **Ajouter un nouvel appareil** qui s’affiche, spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td>Le nom que les utilisateurs voient lors de la sélection de l’appareil dans la visionneuse de vérification de l’appli de bureau, comme décrit dans la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">Modification de la résolution du BAT interactif dans la visionneuse de vérification de l’orthographe</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensions</td> 
      <td>Spécifiez les dimensions à utiliser pour cet appareil. Les utilisateurs voient les dimensions affichées sous le nom de l’appareil.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ratio</td> 
      <td>Spécifiez le rapport pour l’appareil.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type</td> 
      <td>Indiquez si l’appareil est mobile, tablette ou bureau.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chaîne de l’agent utilisateur</td> 
      <td>Saisissez l’agent utilisateur de l’appareil pour fournir des informations qui permettent à notre logiciel de s’exécuter et de s’afficher comme prévu pour l’appareil.<p>Vous pouvez obtenir l’agent utilisateur en accédant à <a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a> à partir de l’appareil.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Désactivé</td> 
      <td>Si cette option est sélectionnée, l’appareil n’est pas disponible pour que les utilisateurs puissent le sélectionner lors de la révision des BAT interactifs.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Créer**.

## Configuration de messages contextuels pour les bons à tirer

Vous pouvez configurer des messages contextuels sur les bons à tirer pour communiquer des informations générales à tous les réviseurs de votre organisation.

Vous pouvez paramétrer l&#39;affichage des messages dans les cas suivants :

* **Message au chargement** : s’affiche à la première ouverture du BAT. Utile pour expliquer aux utilisateurs comment réviser un BAT ou fournir une clause de non-responsabilité ou tout autre texte juridique.
* **Au message de décision** : s’affiche lorsqu’un utilisateur sélectionne une décision sur un BAT. Utile pour fournir des listes de contrôle à vos utilisateurs pour des éléments tels que la conformité à la marque ou la réglementation. Pour plus d’informations sur les décisions, voir [Prise d’une décision sur un BAT dans la visionneuse de correctifs](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

* **Texte du bouton Confirmer** : libellé qui s’affiche sur le bouton dans le message contextuel On load expliqué ci-dessus.

Pour créer des messages contextuels pour les bons à tirer :

1. Cliquez sur **Modifier** à droite du message que vous souhaitez personnaliser.
1. Spécifiez un message et incluez la mise en forme appropriée, puis cliquez sur **Enregistrer**.
1. (Facultatif) Si vous avez personnalisé le message Au chargement et que vous souhaitez également personnaliser l’étiquette du bouton de confirmation, cliquez sur **Modifier** à droite de **Confirmer le texte du bouton**, spécifiez une étiquette, puis cliquez sur **Enregistrer**.

## Configuration des paramètres par défaut du BAT

Pour plus d’informations sur la configuration des paramètres par défaut du BAT pour votre organisation, voir [Configuration des paramètres par défaut du BAT](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).


## Configuration des paramètres de partage par défaut

Vous pouvez spécifier avec qui les bons à tirer de votre entreprise peuvent être partagés, les versions disponibles pour les réviseurs et le moment où les bons à tirer avec un workflow automatisé sont visibles pour les utilisateurs associés à une étape donnée.

Pour plus d’informations sur le partage des paramètres dans Workfront Proof, voir [Configuration des paramètres de partage pour vos utilisateurs](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md).

## Effectuer le branding du site de l’épreuve Workfront

Si vous utilisez Workfront Proof, vous pouvez configurer la valorisation de marque pour les zones suivantes du site :

* Page de démarrage qui s’affiche au chargement du BAT
* Écrans de connexion et de déconnexion
* Notifications par e-mail

Pour plus d’informations sur la manière de personnaliser le site Workfront Proof, voir [Marquer le site Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).

## Configuration des paramètres de mot de passe avancés

>[!IMPORTANT]
>
>Cette option est disponible uniquement pour les forfaits Workfront hérités. Si vous utilisez un forfait Pro, Entreprise ou Enterprise Workfront, vous ne pouvez plus configurer de paramètres avancés de mot de passe.

Sous **Paramètres avancés du mot de passe**, vous pouvez améliorer la sécurité du mot de passe de vos utilisateurs.

1. Cliquez sur **Configuration** à droite du paramètre que vous souhaitez configurer :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Longueur minimale du mot de passe</td> 
      <td>La longueur du mot de passe Workfront Proof par défaut est de six caractères. Vous pouvez augmenter le nombre en fonction des stratégies de votre entreprise.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Combinaison de caractères</strong> </td> 
      <td>Vous pouvez forcer les utilisateurs à utiliser un mélange de minuscules, de majuscules, de nombres et de symboles dans leurs mots de passe. Vous décidez du nombre de caractères que doit contenir le mot de passe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Nombre maximal de caractères répétés</strong> </td> 
      <td>Vous pouvez spécifier le nombre de caractères à répéter dans le mot de passe de chaque utilisateur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mot de passe automatique</td> 
      <td>Force les utilisateurs à changer régulièrement leur mot de passe. Vous décidez de la fréquence à laquelle ils le feront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Nombre de répétitions de mot de passe non autorisées</strong> </td> 
      <td>Configurez le nombre de répétitions de mot de passe non autorisées dans votre compte.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Verrouillage de profil</strong> </td> 
      <td>Verrouille vos utilisateurs hors du compte après plusieurs tentatives de connexion infructueuses que vous avez spécifiées. Vous pouvez également spécifier la durée pendant laquelle ils doivent attendre avant de pouvoir accéder à nouveau à leur compte.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’utilisateur si le mot de passe n’est pas réinitialisé après 30 jours</td> 
      <td>Si votre utilisateur ne modifie pas son mot de passe initial dans les 30 jours suivant l’activation de son profil, il est bloqué hors du compte.<br><p>Les administrateurs de compte peuvent déverrouiller (réactiver) les utilisateurs qui sont automatiquement verrouillés par le système. Cela leur donnera sept jours supplémentaires pour modifier leur mot de passe.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller le compte utilisateur s’il est inactif pendant 120 jours</td> 
      <td>Si votre utilisateur ne se connecte pas à Workfront Proof ou qu’il dispose d’un BAT pour se connecter pendant 120 jours, il est bloqué hors du compte.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modifier le mot de passe après la première connexion</strong> </td> 
      <td>Nécessite que les utilisateurs modifient leur mot de passe temporaire après leur première connexion.<p>Les administrateurs de compte peuvent déverrouiller (réactiver) les utilisateurs qui sont automatiquement verrouillés par le système.</p><p>Pour plus d’informations sur le mot de passe, voir <a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">Connexion et modification de votre mot de passe et de votre adresse électronique pour Workfront Proof</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>
