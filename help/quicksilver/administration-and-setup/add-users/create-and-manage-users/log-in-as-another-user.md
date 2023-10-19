---
title: Connexion en tant qu’autre utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur d’Adobe Workfront, vous devrez parfois accéder à Workfront au nom d’un autre utilisateur.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: bc7039bc4b8b257fc55e71e73f72327fdb417837
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# Connexion en tant qu’autre utilisateur


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées à Adobe Admin Console. Si votre entreprise a été intégrée à Adobe Admin Console, cette action n’est pas disponible.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Admin Console, voir [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

En tant qu’administrateur d’Adobe Workfront, vous devrez parfois accéder à Workfront au nom d’un autre utilisateur.

En tant qu’administrateur de groupe, vous devrez peut-être accéder à Workfront au nom d’un utilisateur membre d’un groupe que vous gérez.

Par exemple, si une tâche ne peut pas progresser tant qu’un utilisateur en vacances n’a pas effectué une certaine action, vous pouvez vous connecter en tant qu’utilisateur et effectuer l’action à la place.

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>Comme une intégration de document peut se connecter à des fichiers personnels privés, les administrateurs ne peuvent pas accéder aux intégrations de document lorsqu’ils sont connectés en tant qu’autre utilisateur.
>
>Pour plus d’informations sur les intégrations de documents, voir [Configuration des intégrations de documents](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Avec le niveau d’accès Administrateur système, vous pouvez vous connecter comme n’importe qui. Pour plus d’informations sur ce niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> <p>Avec un niveau d’accès Planificateur, vous pouvez vous connecter en tant qu’utilisateur avec un niveau de licence inférieur si la variable <b>Utilisateurs</b> au niveau d’accès est configuré sur <b>Modifier</b> accès, avec <b>Créer</b> et au moins l’une des deux <b>Administration des utilisateurs</b> options activées sous <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>REMARQUE</b>: de ces deux options, si Utilisateur <b>Administration (utilisateurs de groupe)</b> est activé, vous devez être administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> 
   <p>Pour plus d’informations sur la variable <b>Utilisateurs</b> paramétrer un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Connexion et actions en tant qu’autre utilisateur

1. Connectez-vous à Workfront en tant qu’administrateur Workfront ou administrateur de groupe.

   >[!NOTE]
   >
   >* Si vous êtes administrateur de groupe, vous ne pouvez vous connecter qu’en tant qu’utilisateurs dans les groupes que vous gérez. En outre, l’autorisation Administrateur utilisateur (utilisateurs de groupe) doit être activée dans votre niveau d’accès :
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  Ce paramètre est désactivé par défaut. Pour plus d’informations, voir [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Vous ne pouvez pas réinitialiser le mot de passe d’un administrateur Workfront.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Connexion en tant que**.

1. Dans le **Utilisateurs** sur la zone **Connexion en tant que** , commencez à saisir le nom de l’utilisateur, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   L’utilisateur doit disposer d’un niveau d’accès défini dans Workfront. Vous ne pouvez pas vous connecter au système Workfront en tant qu’utilisateur ne disposant pas des droits de connexion.

   >[!NOTE]
   >
   >Les administrateurs de groupe peuvent se connecter uniquement en tant qu’utilisateurs membres des groupes qu’ils gèrent. Ils ne peuvent pas se connecter en tant qu’administrateur Workfront.

1. Cliquez sur **Connectez-vous.**

   <!--
   <p> Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->

   Lorsque vous êtes connecté en tant qu’autre utilisateur, une notification s’affiche en haut de l’écran pour l’indiquer.

1. Après avoir effectué les actions nécessaires en tant qu’utilisateur, cliquez sur **Déconnectez-vous.**

## Tracking et contrôle des activités lorsqu’un administrateur est connecté en tant qu’autre utilisateur

Workfront fournit des mécanismes pour le suivi et le contrôle des activités qui ont lieu lorsque l’administrateur est connecté en tant qu’autre utilisateur.

Lorsque vous vous connectez en tant qu’autre utilisateur, la date de dernière connexion de cet utilisateur est modifiée à la date à laquelle l’administrateur système ou groupe se connecte en tant qu’utilisateur.

* [Affichage des indicateurs sur les éléments](#view-indicators-on-items)
* [Affichage des informations d’audit](#view-audit-information)

### Affichage des indicateurs sur les éléments {#view-indicators-on-items}

Lorsque vous vous connectez à Workfront en tant qu’autre utilisateur et exécutez une action, Workfront indique clairement que toute action que vous effectuez est effectuée par vous au nom de l’utilisateur sous lequel vous êtes connecté.

Par exemple, si vous commentez un élément lors de votre connexion en tant qu’autre utilisateur, une instruction indique que vous avez fait ce commentaire pour le compte de l’utilisateur.

### Affichage des informations d’audit {#view-audit-information}

1. Connectez-vous à Workfront en tant qu’administrateur Workfront ou administrateur de groupe.
1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Connectez-vous en tant que,** puis cliquez sur le bouton **Journal d’accès** .

   Chaque fois qu’un administrateur système ou de groupe se connecte à Workfront en tant qu’autre utilisateur, l’événement est consigné dans le journal d’audit. En outre, toutes les actions pouvant être vérifiées qui ont lieu pendant que l’administrateur est connecté en tant qu’autre utilisateur sont consignées dans le journal d’audit.

1. (Facultatif) Vous pouvez filtrer les résultats affichés dans le journal d’audit comme suit :

   * Par l’utilisateur qui s’est connecté
   * Par l’utilisateur connecté en tant que
   * Par date
