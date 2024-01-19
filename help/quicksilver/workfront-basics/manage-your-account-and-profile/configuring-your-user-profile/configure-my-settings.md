---
product-area: user-management;setup
navigation-topic: configure-your-user-profile
title: Configurer mes paramètres
description: Votre [!DNL Adobe Workfront] Le profil contient des informations vous concernant (par exemple, votre nom, votre adresse électronique, votre adresse, votre numéro de téléphone, votre titre, etc.). Il contient également des informations sur vos interactions avec [!DNL Workfront] et d’autres utilisateurs de votre entreprise.
author: Nolan
feature: Get Started with Workfront
exl-id: 0199bf74-0611-48f0-9c05-da6afac85033
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '3301'
ht-degree: 0%

---

# Configurer mes paramètres

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Edit the job role FTE percentage allocation blurbs when more functionality is released: now, it says that the % is that of the user's schedule, but it will be either the user's schedule or the system schedule.</p>
-->

Votre [!DNL Adobe Workfront] Le profil contient des informations vous concernant (par exemple, votre nom, votre adresse électronique, votre adresse, votre numéro de téléphone, votre titre, etc.). Il contient également des informations sur vos interactions avec [!DNL Workfront] et d’autres utilisateurs de votre entreprise (vos paramètres de notification, par exemple, les onglets que vous souhaitez afficher dans [!DNL Workfront], ou votre rôle professionnel, votre rôle de manager, de groupe et d’équipe).

La plupart de ces informations ont déjà été définies par votre [!DNL Workfront] lorsque votre [!DNL Workfront] compte a été créé.

Selon le niveau d’accès que vous avez dans [!DNL Workfront], vous pouvez modifier certaines de ces informations en configurant votre [!UICONTROL Mes paramètres] zone.

## Comment les niveaux d’accès affectent-ils la modification des [!UICONTROL Mes paramètres] area

Selon le niveau d’accès dont vous disposez, vous pouvez modifier des sections de votre [!UICONTROL Mes paramètres] zone.

Certains champs contenus dans des sections modifiables ne peuvent pas être modifiés, selon d’autres paramètres qui peuvent être configurés ou non dans votre niveau d’accès. Pour plus d’informations sur les accès supplémentaires nécessaires à l’édition de certains champs que vous trouverez dans [!UICONTROL Mes paramètres], reportez-vous aux sections de la section [Configuration du [!UICONTROL Mes paramètres] area](#configuring-the-my-settings-area).

Pour connaître votre niveau d’accès, contactez votre [!DNL Workfront] administrateur.

La grille suivante indique les sections dans la [!UICONTROL Mes paramètres] sont visibles ou modifiables en fonction de votre niveau d’accès :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Zones [!UICONTROL Mes paramètres]</strong> </th> 
   <th><strong>Visible ou modifiable</strong> </th> 
   <th><strong>[!UICONTROL Administrateur système]</strong> </th> 
   <th><strong>[!UICONTROL Planner]</strong> </th> 
   <th><strong>[!UICONTROL Worker]</strong> </th> 
   <th><strong>[!UICONTROL Reviewer]</strong> </th> 
   <th><strong>[!UICONTROL Requestor]</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2">[!UICONTROL Personal Info]</td> 
   <td> <p>Visible</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td> <p>Modifiable</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Preferences]</td> 
   <td> <p>Visible</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>Modifiable</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Notifications]</td> 
   <td> <p>Visible</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>Modifiable</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Access]</td> 
   <td>Visible</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifiable</td> 
   <td> ✔</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Organisation]</td> 
   <td>Visible</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifiable</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Resource Planning]</td> 
   <td>Visible</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifiable</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Forms personnalisé]</td> 
   <td>Visible</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>Modifiable</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Comment]</td> 
   <td>Visible</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>Modifiable</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
 </tbody> 
</table>

## Configuration du [!UICONTROL Mes paramètres] area

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, cliquez sur votre nom d’utilisateur en regard de votre image de profil. Ou (le cas échéant), cliquez sur l’image de profil dans la zone de navigation supérieure, puis cliquez sur **[!UICONTROL Profil Workfront]**.
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![](assets/more-icon.png), puis cliquez sur **[!UICONTROL Modifier]**.

1. Selon votre niveau d’accès, vous pouvez mettre à jour les sections suivantes :

   * [Infos personnelles](#personal-info)
   * [Préférences](#preferences)
   * [Notifications](#notifications)
   * [Accès](#access)
   * [Organisation](#organization)
   * [Planification des ressources](#resource-planning)
   * [Formulaire personnalisé](#custom-form)
   * [Commentaire](#comment)

1. Cliquer sur **[!UICONTROL Enregistrer]**.

### [!UICONTROL Informations personnelles]

Cette section comprend les sous-sections suivantes :

* [Informations de base](#basic-info)
* [Informations sur la tâche](#job-info)
* [Coordonnées](#contact-info)

#### [!UICONTROL Informations de base]

Ces informations doivent déjà être configurées par votre [!DNL Workfront] administrateur. Tous les champs de cette sous-section sont obligatoires.

Vous pouvez modifier les éléments suivants de cette sous-section :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Prénom]</strong></td> 
   <td>Mettez à jour votre prénom. Champ obligatoire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Nom]</strong></td> 
   <td>Mettez à jour votre nom de famille. Champ obligatoire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Adresse électronique]</strong></td> 
   <td> Mettez à jour votre adresse électronique. Il s’agit d’un champ obligatoire. Gardez à l’esprit que votre adresse électronique est également votre nom d’utilisateur pour [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Réinitialiser le mot de passe]</strong></td> 
   <td>Réinitialisez votre mot de passe dans cette section. Pour plus d’informations sur la réinitialisation de votre mot de passe, voir <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Réinitialisation de votre mot de passe</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Conditionnel) &lt;sso configuration=""&gt; [!UICONTROL Username]</strong></td> 
   <td> Si votre [!DNL Workfront] l’administrateur a activé une intégration SSO avec [!DNL Workfront], votre nom d’utilisateur SSO s’affiche dans ce champ. Le type de configuration SSO activé pour votre [!DNL Workfront] est visible dans ce champ.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Conditionnel) [!UICONTROL Autoriser uniquement &lt;sso configuration=""&gt; Authentification]</strong></td> 
   <td> <p> Si votre [!DNL Workfront] l’administrateur a activé une intégration SSO avec [!DNL Workfront] et contient des utilisateurs mis à jour pour SSO, ce champ est sélectionné par défaut. Le type de configuration SSO activé pour votre [!DNL Workfront] est visible dans ce champ.</p> <p>Lorsque ce champ est sélectionné, vous devez vous connecter à [!DNL Workfront] avec vos informations d’identification SSO. Si vous la décochez, vous pourrez vous connecter à [!DNL Workfront] avec votre [!DNL Workfront] informations d’identification.</p> <p>Pour plus d’informations sur la configuration [!DNL Workfront] avec une solution SSO, voir <a href="../../../administration-and-setup/add-users/single-sign-on/single-sign-on.md" class="MCXref xref">Connexion unique [!DNL Adobe Workfront]</a>. Pour plus d’informations sur la mise à jour des utilisateurs pour SSO, voir <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Mise à jour des utilisateurs pour l’authentification unique</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Informations sur la tâche]

Vous pouvez modifier les éléments suivants de cette sous-section :

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Title]</strong></td>
        <td>Indiquez votre titre. Ce n’est pas la même chose que votre rôle professionnel. Votre titre ne fait pas partie de la planification des ressources, alors que votre rôle de tâche l’est. Votre titre s’affiche dans le [!DNL Workfront] partout où votre nom et votre avatar s’affichent. Elle est visible par tous ceux qui ont accès à l’utilisateur.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Me parler de]</strong></td>
        <td>Indiquez vos intérêts professionnels dans ce domaine.</td>
    </tr>
</table>

#### [!UICONTROL Coordonnées]

Vous pouvez modifier les éléments suivants de cette sous-section :

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Numéro de téléphone]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Extension]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Numéro de mobile]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Address]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL City]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL State]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Postal Code]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Country]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Image De Profil]</strong></td>
        <td>Votre image de profil devient votre avatar et elle est visible dans tout le [!DNL Workfront] système, où votre nom s’affiche.</td>
    </tr>
</table>

### [!UICONTROL Préférences]

Indiquez ce que vous souhaitez afficher dans votre [!DNL Workfront] dans cette section.

>[!NOTE]
>
>Utilisateurs avec un [!UICONTROL Demandeur] La licence ne comporte aucun autre élément de panneau de gauche à ajouter à sa [!UICONTROL Menu Principal], en dehors de la fonction [!UICONTROL Demandes] zone. Comme [!DNL Workfront] administrateur, vous pouvez affecter des utilisateurs disposant d’une licence Requestor à un modèle de mise en page qui comprend toutes les autres zones du [!UICONTROL Menu Principal]. Ensuite, ils peuvent sélectionner les zones à afficher dans leur [!UICONTROL Menu Principal] en modifiant leur profil utilisateur.

Vous pouvez modifier les éléments suivants de cette sous-section :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Fuseau horaire]</strong> </td> 
   <td><p>Indiquez votre fuseau horaire. Cela contrôle l’heure affichée dans vos emails sortants.</p>
       <p>Le fuseau horaire affecte également ce qui s’affiche dans un rapport de calendrier PTO.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Paramètres régionaux de l’adresse électronique]</strong> </td> 
   <td>Indiquez ici votre langue préférée. Cela contrôle le format de la langue, de la date et du nombre utilisé dans les emails sortants.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Afficher le pourcentage terminé à la mise à jour de l’état]</strong> </td> 
   <td>Cochez cette option si vous souhaitez afficher une barre de pourcentage complète dans la zone Mises à jour de vos tâches, lors de l’utilisation de l’expérience de commentaire héritée. Pour plus d’informations, voir <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">Nouvelle expérience de commentaire</a>.

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL M’envoyer du travail assigné à mon onglet Travail]</strong> </td> 
   <td>Sélectionnez ce champ pour afficher le travail que vous vous assignez directement sur l’onglet [!UICONTROL Travail sur] au lieu de l’onglet [!UICONTROL Demandes de travail] .</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Conditionnel) Générer automatiquement des bons à tirer lors du téléchargement de documents</strong></td> 
   <td>Sélectionnez ce champ pour commencer à générer un BAT immédiatement après le chargement du document dans [!DNL Workfront]. Ce champ est désactivé par défaut et ne peut être mis à jour que par un administrateur Workfront.<br>Ce champ n’est disponible que si votre société a acheté le composant Bon à tirer de Workfront pour Workfront et si vous êtes activé en tant qu’utilisateur du BAT. Pour plus d’informations sur le BAT Workfront, voir <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md" class="MCXref xref">Gestion des bons à tirer dans Adobe Workfront</a>.
   <p><b>Remarque :</b> Les documents chargés dans une requête ne génèrent pas automatiquement de BAT. </p></td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Notifications]

Spécifiez les notifications que vous souhaitez recevoir. [!DNL Workfront]. Pour plus d’informations sur la configuration des notifications, voir [Modifier vos propres notifications électroniques](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### [!UICONTROL Accès]

Votre accès et les autres composants qui lui sont associés sont configurés par votre [!DNL Workfront] administrateur, lors de la configuration de votre compte.

Uniquement un [!DNL Workfront] l’administrateur peut consulter et modifier tous les champs de cette section.

Vous pouvez modifier les éléments suivants de cette sous-section :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Est Actif]</strong> </td> 
   <td>Ce champ est visible uniquement pour un utilisateur qui est également un [!DNL Workfront] et doit être vérifié par défaut. Cela signifie que l’utilisateur est actif et peut se connecter à [!DNL Workfront]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Niveau d’accès]</strong> </td> 
   <td>Ce champ est visible pour les utilisateurs disposant d’un niveau d’accès [!UICONTROL Plan] ou [!UICONTROL Administrateur Workfront]. Il n’est modifiable que pour [!DNL Workfront] administrateurs. Si vous êtes un [!DNL Workfront] administrateur, gardez à l’esprit de ne pas modifier votre niveau d’accès à un niveau inférieur lorsque vous modifiez ce champ. </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Modèle de mise en page]</strong> </td> 
   <td>Ce champ est visible par les utilisateurs disposant d’un [!UICONTROL Plan] ou [!UICONTROL [!DNL Workfront] niveau d’accès administrateur, et il n’est modifiable que pour [!UICONTROL [!DNL Workfront] administrateurs] ou les utilisateurs disposant d’une licence [!UICONTROL Plan] qui disposent également d’un accès administrateur. Sélectionnez ici un modèle de mise en page pour mettre à jour l’aspect et le champ de votre interface Workfront. Pour plus d’informations sur la configuration des utilisateurs disposant d’un accès administrateur, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurer l’accès des utilisateurs à la modification des utilisateurs à l’aide d’un niveau d’accès personnalisé</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.<br>Pour plus d’informations sur les modèles de mise en page et leur impact sur l’interface, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Création et gestion des modèles de mise en page</a></td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><strong>Log in as</strong> </td> 
    <td> <p><strong>Add access</strong> for a Workfront administrator or group administrator (associated with a group you are in) to log in as you. Select an <strong>Access expiration date</strong> for the login. </p> <p>You can repeat this to grant login access to multiple administrators.</p> <p>The settings you choose in this section are visible only to you.
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <span class="PinkDraftNote">Add a note about this being only for the Enterprise package if they decide to do it that way. Functionality that may come in a later sprint: If you want to be notified when the administrator logs in as you, select Receive an email when this user logs in.</span> 
       </MadCap:conditionalText>
      </p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader"><strong>(Conditionnel) [!UICONTROL L’utilisateur peut générer des BAT (... sur ... licences de BAT restantes)]</strong></td> 
   <td>Ce champ n’est disponible que si votre entreprise utilise un ancien [!DNL Workfront] planifiez et a acheté la variable [!DNL Workfront Proof] composant. Lorsqu’il est sélectionné, vous êtes activé en tant qu’utilisateur de vérification. Il affiche également le nombre de licences de BAT utilisées dans votre système sur le nombre total de licences de BAT achetées. Ce champ est visible et modifiable uniquement pour les utilisateurs qui [!DNL Workfront] administrateurs. Pour plus d’informations sur les options de plan pour la vérification, voir [!DNL Workfront], voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md">Accès aux fonctionnalités de vérification dans [!DNL Workfront]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Conditionnel) [!UICONTROL Profil d’autorisation]</strong></td> 
   <td> <p>Ce champ affiche le niveau d’accès que vous avez dans [!DNL Workfront Proof]. Elle n’est disponible que si :</p> 
    <ul> 
     <li>Votre entreprise utilise un héritage [!DNL Workfront] planifiez et a acheté la variable [!DNL Workfront Proof] ou si vous disposez d’une licence [!UICONTROL Work] ou [!UICONTROL Plan] sur une nouvelle [!DNL Workfront] planifiez.</li> 
     <li>Vous êtes activé en tant qu’utilisateur de BAT.</li> 
    </ul> <p>[!DNL Workfront] Les administrateurs peuvent modifier le champ pour tous les utilisateurs, à l’exception d’eux-mêmes, de sorte que tous les utilisateurs voient le champ comme un affichage uniquement sur leurs propres profils. Pour plus d’informations sur le profil d’autorisation, voir <a href="../../../review-and-approve-work/proofing/proofing-overview/permission-profiles.md" class="MCXref xref">Aperçu du profil d’autorisation de preuve</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Organisation]

Ces informations sont généralement configurées par votre [!DNL Workfront] lorsqu’ils créent votre [!DNL Workfront] compte . Vous pouvez également mettre à jour les informations relatives à votre organisation ou structure d’organisation dans cette section. Uniquement les utilisateurs avec un [!UICONTROL Planifier] ou [!UICONTROL Administrateur système] Le niveau d&#39;accès peut modifier cette section. 

Vous pouvez modifier les éléments suivants de cette sous-section :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Company]</strong></td> 
   <td>Sélectionnez le nom de la société à laquelle vous appartenez dans la liste déroulante.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Conditionnel) [!UICONTROL Rapports À]</strong></td> 
   <td>Après avoir sélectionné une <strong>[!UICONTROL Company]</strong> pour votre profil, vous pouvez également spécifier le nom de votre responsable dans ce champ. Vous ne pouvez spécifier qu’un seul nom ici. Nous vous recommandons de spécifier le nom de votre responsable immédiat. Commencez à saisir leur nom, puis cliquez pour le sélectionner lorsqu’il s’affiche dans la liste.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Conditionnel) [!UICONTROL Rapports directs]</strong></td> 
   <td>Après avoir sélectionné une <strong>[!UICONTROL Company]</strong> pour votre profil, vous pouvez également spécifier le nom de vos rapports directs dans ce champ. Vous pouvez y spécifier autant de rapports directs que nécessaire. Commencez à saisir leurs noms, puis cliquez pour les sélectionner lorsqu’ils apparaissent dans la liste.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Home Team]</strong> </td> 
   <td> <p>Sélectionnez une <strong>[!UICONTROL Home Team]</strong> dans le menu déroulant. Ce champ est visible pour les utilisateurs disposant d’un niveau d’accès [!UICONTROL Plan] ou [!UICONTROL Administrateur système]. Il n’est modifiable que pour [!DNL Workfront] administrateurs ou utilisateurs disposant d’une licence [!UICONTROL Plan] ayant également un accès administrateur. Pour plus d’informations sur la configuration des utilisateurs disposant d’un accès administrateur, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurer l’accès des utilisateurs à la modification des utilisateurs à l’aide d’un niveau d’accès personnalisé</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.<br></p> <p>Votre <strong>Équipe Accueil</strong> peut affecter l’aspect de votre [!DNL Workfront] , si un modèle de mise en page est associé à l’équipe. </p> <p> <br>Pour plus d’informations sur les équipes, voir <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Présentation des équipes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Autres équipes]</strong> </td> 
   <td> <p>Vous pouvez appartenir à plusieurs équipes. Spécifiez les équipes supplémentaires auxquelles vous appartenez dans ce champ en commençant à saisir le nom d’une équipe, puis cliquez pour la sélectionner lorsqu’elle s’affichera dans la liste. Le fait d'appartenir à trop d'équipes peut créer une confusion quant au travail qui est assigné aux équipes. Pour plus d’informations sur les équipes, voir <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Présentation des équipes</a>.</p> <p>Ce champ est visible par les utilisateurs disposant d’une licence [!UICONTROL Plan] ou [!UICONTROL System Administrator], et il n’est modifiable que pour [!DNL Workfront] administrateurs ou utilisateurs disposant d’une licence [!UICONTROL Plan] ayant également un accès administrateur. Pour plus d’informations sur la configuration des utilisateurs disposant d’un accès administrateur, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurer l’accès des utilisateurs à la modification des utilisateurs à l’aide d’un niveau d’accès personnalisé</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Home Group]</strong> </td> 
   <td> <p>Sélectionnez une <strong>[!UICONTROL Home Group]</strong> dans le menu déroulant.</p> <p>Remarque : il s’agit d’un champ obligatoire. Un utilisateur ne peut pas être associé à un groupe.<br></p> <p>Ce champ est visible par les utilisateurs disposant d’un niveau [!UICONTROL Plan] ou [!UICONTROL Administrateur système]. Pour plus d’informations sur les personnes qui peuvent modifier la variable <strong>[!UICONTROL Home Group]</strong> , voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md#prerequisites" class="MCXref xref">Ajout d’utilisateurs</a> dans <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Ajout d’utilisateurs</a>.Your <strong>[!UICONTROL Home Group]</strong> est le groupe par défaut pour tous les projets et la valeur par défaut <strong>[!UICONTROL Home Group]</strong> pour tous les nouveaux utilisateurs que vous créez. Tous les formulaires personnalisés que vous créez sont partagés avec vos <strong>[!UICONTROL Home Group]</strong> par défaut.</p> <p>Pour plus d’informations sur les groupes, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Présentation des groupes</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Autres groupes]</strong> </td> 
   <td> <p>Vous pouvez appartenir à plusieurs groupes. Spécifiez les groupes supplémentaires auxquels vous appartenez dans ce champ en commençant à saisir le nom d’un groupe. Cliquez pour la sélectionner lorsqu’elle s’affiche dans la liste. Ce champ est visible pour les utilisateurs disposant d’un niveau d’accès [!UICONTROL Plan] ou [!UICONTROL Administrateur système]. Pour plus d’informations sur les personnes qui peuvent modifier la variable <strong>[!UICONTROL Autres groupes]</strong> voir la section "Autres groupes" dans <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Ajout d’utilisateurs</a>.</p> <p>Pour plus d’informations sur les groupes, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Présentation des groupes</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Planification des ressources]

Vos informations de planification des ressources affectent la chronologie des affectations de travail, la durée de journalisation, le coût et les recettes des projets que vous utilisez. En règle générale, cette zone est mise à jour par le [!DNL Workfront] administrateur, un chef de projet ou de ressource, ou par votre directeur.

Utilisez l’une des méthodes suivantes de cette section :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Désactivation de la planification]</strong></td> 
   <td>Cochez cette case si vous souhaitez planifier la désactivation de votre compte au bout d’un certain temps. Dans le <p><strong>[!UICONTROL Date de désactivation planifiée]</strong> qui s’affiche, indiquez la date à laquelle votre compte sera désactivé. Pour plus d’informations sur la désactivation des utilisateurs, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planification de la désactivation pour les utilisateurs</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur</a>. </p><p>Vous pouvez modifier les champs de désactivation de votre compte si vous disposez d’une licence Plan ou si vous êtes le [!DNL Workfront] administrateur. </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Rôle de Principal]</strong></td> 
   <td> <p>Il s’agit du rôle de tâche principal que vous pouvez remplir dans Workfront. Par défaut, chaque tâche et problème auquel vous êtes affecté est également affecté à ce rôle de tâche. Les rôles de tâche sont essentiels dans la gestion des ressources. Pour plus d’informations sur les rôles de tâche, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Création et gestion des rôles de tâche</a>.</p> <p>Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence [!UICONTROL Plan] avec accès administrateur ou si vous êtes un utilisateur [!DNL Workfront] administrateur. Pour plus d’informations sur la configuration des utilisateurs disposant d’un accès administrateur, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurer l’accès des utilisateurs à la modification des utilisateurs à l’aide d’un niveau d’accès personnalisé</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Conditionnel) Si vous avez sélectionné un [!UICONTROL Rôle de Principal], le champ [!UICONTROL Pourcentage de disponibilité de l’éditeur de texte enrichi] s’affiche.</strong></td> 
   <td>Indiquez le pourcentage de votre temps planifié attribué à ce rôle de tâche. La valeur par défaut du [!UICONTROL Pourcentage de disponibilité de l’éditeur de texte enrichi] pour le rôle de Principal est de 100 %.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Autres rôles]</strong> </td> 
   <td> <p>Vous pouvez avoir plusieurs rôles de tâche dans [!DNL Workfront]. Les rôles de tâche sont essentiels dans la gestion des ressources. Pour plus d’informations sur les rôles de tâche, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Création et gestion des rôles de tâche</a>.</p> <p>Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence [!UICONTROL Plan] avec accès administrateur ou si vous êtes un utilisateur [!DNL Workfront] administrateur. Pour plus d’informations sur la configuration des utilisateurs disposant d’un accès administrateur, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurer l’accès des utilisateurs à la modification des utilisateurs à l’aide d’un niveau d’accès personnalisé</a> in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Conditionnel) Si vous avez sélectionné un ou plusieurs autres rôles, le champ [!UICONTROL Pourcentage de disponibilité de l’éditeur de texte enrichi] s’affiche pour chaque rôle.</strong></td> 
   <td> <p>Indiquez le pourcentage de votre temps planifié attribué à chaque rôle de tâche. La valeur par défaut du [!UICONTROL Pourcentage de disponibilité de l’éditeur de texte enrichi] pour [!UICONTROL Autres rôles] est de 0 %.</p> <p> <img src="assets/user-settings-roles-and-dte-boxes-rp-story--1--350x224.png" alt="user_settings_tasks_and_dte_boxes_rp_story__1_.png" style="width: 350;height: 224;"> </p> <p>Remarque :  
     <ul> 
      <li>Si [!UICONTROL Autres rôles] disposent d’une disponibilité de l’éditeur de texte enrichi de 0 %, ils ne s’affichent pas dans le [!UICONTROL Resource Planner], sauf si les utilisateurs sont affectés à des tâches dans ces rôles.</li> 
      <li> <p>La somme de tous les <strong>[!UICONTROL Pourcentages de disponibilité de l’éditeur de texte enrichi]</strong> pour tous les rôles, doit être égal à 100 %. Chaque [!UICONTROL Pourcentage de disponibilité de l’éditeur de texte enrichi] calcule les [!UICONTROL Heures disponibles] pour chaque rôle par utilisateur dans le [!UICONTROL Resource Planner]. </p> <p>Les [!UICONTROL Hours disponibles] pour chaque rôle par utilisateur dépendent de l’heure disponible pour l’utilisateur. L’heure disponible pour l’utilisateur est calculée par [!DNL Workfront] selon la méthode sélectionnée par la variable [!DNL Workfront] pour calculer l’éditeur de texte enrichi dans les préférences de [!UICONTROL Resource Management]. Pour plus d’informations sur le calcul de la disponibilité de l’utilisateur, voir <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Présentation du calcul des heures et de l’éditeur de texte enrichi pour les utilisateurs et les rôles dans le planificateur de ressources</a>. Pour plus d’informations sur la configuration des préférences de gestion des ressources, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configuration des préférences de gestion des ressources</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Planning</strong></td> 
   <td> <p>Uniquement [!DNL Workfront] Les administrateurs ou les utilisateurs disposant d’une licence [!UICONTROL Plan] qui disposent également d’un accès administratif pour les feuilles de temps et les heures peuvent mettre à jour ce champ. Pour plus d’informations sur l’accès administratif pour les feuilles de temps et les heures, voir la section "Fiches horaires et heures" dans <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> <p>Sélectionnez la feuille de temps appropriée dans le menu déroulant. Cela garantit que vos feuilles de temps sont générées automatiquement, conformément aux spécifications définies par votre [!DNL Workfront] administrateur. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Type d’heure par défaut]</strong> </td> 
   <td>Sélectionnez votre type d’heure par défaut. Il s’agit du type d’heure que le système utilise par défaut chaque fois que vous connectez l’heure dans Workfront.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Types d’heure disponibles]</strong> </td> 
   <td>Sélectionnez les types d’heures dans lesquels vous pouvez sélectionner l’heure de journal. Les types d’heures de ce menu déroulant sont mis à votre disposition par votre [!DNL Workfront] administrateur.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Pool de ressources]</strong> </td> 
   <td>Sélectionnez un pool de ressources auquel vous appartenez. Ce champ est destiné uniquement à des fins de création de rapports et d’information, il n’a aucune incidence sur la planification ou la planification des ressources.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL FTE]</strong> </td> 
   <td> <p>Le nombre que vous indiquez ici est pris en compte pour calculer votre disponibilité en fonction du planning par défaut uniquement lorsque les [!UICONTROL Resource Management Preferences] au niveau du système sont définies sur <strong>[!UICONTROL La Planification Par Défaut]</strong>.</p> <p>Par exemple, si la valeur de l’éditeur de texte enrichi est 0,5 et que la planification par défaut [!UICONTROL] est de 40 heures, vous pouvez travailler 20 heures par semaine.</p> <p>Si les [!UICONTROL Resource Management Preferences] au niveau du système sont définies sur <strong>[!UICONTROL Planification de l’utilisateur]</strong>, la valeur que vous indiquez ici est ignorée et vous pouvez travailler en fonction de ce qui est spécifié dans votre planning. Dans ce cas, l’éditeur de texte enrichi pour le [!UICONTROL Resource Planner] est calculé à l’aide de la formule suivante : </p> <p><code style="font-style: normal;">[!UICONTROL User Available FTE] = [!UICONTROL Hours from the Schedule of the User/ Default Schedule Hours]</code> </p> <p>Pour plus d’informations sur le calcul de l’éditeur de texte enrichi, voir <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Présentation du calcul des heures et de l’éditeur de texte enrichi pour les utilisateurs et les rôles dans le planificateur de ressources</a>.</p> <p>Pour plus d’informations sur la création de planifications dans [!DNL Workfront], voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Création d’un planning</a>.</p> <p>Pour plus d’informations sur la configuration des préférences de gestion des ressources, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configuration des préférences de gestion des ressources</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Coût par heure]</strong> </td> 
   <td>Indiquez le coût horaire de votre utilisateur. Pour plus d’informations sur le suivi des coûts dans [!DNL Workfront], voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivi des coûts</a>. Vous ne pouvez pas mettre à jour ces informations, sauf si vous avez accès aux données financières de votre niveau d’accès ou si vous êtes un [!DNL Workfront] administrateur. Pour plus d’informations sur l’accès financier, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Accorder l'accès aux données financières</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Facturation par heure]</strong> </td> 
   <td>Indiquez le montant de la facturation par heure pour votre utilisateur. Pour plus d’informations sur le suivi de la facturation et des recettes, voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Présentation de la facturation et des recettes</a>. Vous ne pouvez pas mettre à jour ces informations si vous n’avez pas accès aux données financières de votre niveau d’accès ou si vous êtes un [!DNL Workfront] administrateur. Pour plus d’informations sur l’accès financier, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Accorder l'accès aux données financières</a>.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Formulaire personnalisé]

Vous pouvez associer un formulaire personnalisé à votre profil utilisateur. Cela vous permet de stocker des informations supplémentaires pour votre utilisateur qui ne peuvent pas être stockées autrement dans la variable [!DNL Workfront] champs natifs décrits ci-dessus.\
Pour joindre un formulaire personnalisé à votre utilisateur, vous devez disposer de l’un des accès ou autorisations suivants :

* Vous êtes un [!DNL Workfront] administrateur.
* Vous êtes un [!UICONTROL Planifier] l’utilisateur de licence et le formulaire personnalisé de l’utilisateur sont partagés avec l’un de vos groupes.

Tous les utilisateurs peuvent voir des formulaires personnalisés qui ont été associés à leurs utilisateurs.

Votre [!DNL Workfront] L’administrateur doit configurer des formulaires personnalisés pour l’objet utilisateur afin que vous puissiez joindre un formulaire personnalisé à votre profil utilisateur. Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### [!UICONTROL Commentaire]

Vous pouvez enregistrer un commentaire sur votre profil utilisateur qui est stocké dans la variable [!UICONTROL Mises à jour] de votre utilisateur.

Vous pouvez cliquer sur le bouton [!UICONTROL personnes] pour inclure d’autres personnes dans la mise à jour.

Vous pouvez cliquer sur le bouton [!UICONTROL lock] pour rendre cette mise à jour privée aux utilisateurs de la même société que vous.
