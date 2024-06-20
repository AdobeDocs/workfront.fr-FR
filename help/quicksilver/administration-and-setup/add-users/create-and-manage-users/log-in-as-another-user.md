---
title: Se connecter sous une autre identité
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous devrez parfois accéder à Workfront au nom d’un autre utilisateur ou d’une autre utilisatrice.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: ht
source-wordcount: '814'
ht-degree: 100%

---

# Se connecter sous une autre identité

<!--Audited: April, 2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux entreprises qui n’ont pas encore été intégrées à Adobe Admin Console. Si votre entreprise a été intégrée à Adobe Admin Console, cette action n’est pas disponible.
>
>Pour obtenir une liste de procédures qui varient selon que votre organisation a été intégrée ou non à Adobe Admin Console, voir [Différences d’administration en fonction de la plateforme (Adobe Workfront Fusion/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

En tant qu’administrateur ou administratrice Adobe Workfront, vous devrez parfois accéder à Workfront au nom d’un autre utilisateur ou d’une autre utilisatrice.

Ou bien, en tant qu’administrateur ou administratrice de groupe, vous devrez peut-être accéder à Workfront au nom d’un utilisateur ou d’une utilisatrice membre d’un groupe que vous gérez.

Par exemple, si une tâche ne peut pas progresser tant qu’un utilisateur ou une utilisatrice en vacances n’a pas effectué une certaine action, vous pouvez vous connecter en tant que cet utilisateur ou cette utilisatrice et effectuer l’action à sa place.

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
>Une intégration de document pouvant se connecter à des fichiers personnels privés, les administrateurs et administratrices ne peuvent pas accéder aux intégrations de document lorsqu’ils sont connectés en tant qu’autre utilisateur ou autre utilisatrice.
>
>Pour plus d’informations sur les intégrations de documents, voir [Configurer les intégrations de documents](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouvelle : standard</p>
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Avec le niveau d’accès Administrateur ou administratrice système, vous pouvez vous connecter comme n’importe qui. Pour plus d’informations sur ce niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif complet à une personne</a>. </p> <p>Avec un niveau d’accès Planificateur, vous pouvez vous connecter en tant qu’utilisateur ou utilisatrice avec un niveau de licence inférieur si le paramètre <b>Utilisateurs et utilisatrices</b> du niveau d’accès est configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>Remarque</b> : parmi ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être administrateur ou administratrice d’un groupe dont l’utilisateur ou l’utilisatrice est membre.</p> 
   <p>Pour plus d’informations sur le paramètre <b>Utilisateurs et utilisatrices</b> dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Se connecter et effectuer des actions en tant qu’autre utilisateur ou utilisatrice

1. Connectez-vous à Workfront en tant qu’administrateur ou administratrice Workfront ou administrateur ou administratrice de groupe.

   >[!NOTE]
   >
   >* Si vous êtes administrateur ou administratrice de groupe, vous ne pouvez vous connecter qu’en tant qu’utilisateurs ou utilisatrices dans les groupes que vous gérez. En outre, l’autorisation Administration des utilisateurs (utilisateurs du groupe) doit être activée dans votre niveau d’accès :
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  Ce paramètre est désactivé par défaut. Pour plus d’informations, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Vous ne pouvez pas réinitialiser le mot de passe d’un administrateur ou d’une administratrice Workfront.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Connexion en tant que**.

1. Dans la zone **Utilisateurs** de l’onglet **Connexion en tant que**, commencez à saisir le nom de l’utilisateur ou de l’utilisatrice, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   L’utilisateur ou l’utilisatrice doit disposer d’un niveau d’accès défini dans Workfront. Vous ne pouvez pas vous connecter au système Workfront en tant qu’utilisateur ou utilisatrice ne disposant pas de droits de connexion.

   >[!NOTE]
   >
   >Les administrateurs et administratrices de groupe peuvent se connecter uniquement en tant qu’utilisateurs et utilisatrices membres des groupes qu’ils gèrent. Ils ne peuvent pas se connecter en tant qu’administrateur ou administratrice Workfront.

1. Cliquez sur **Connexion**.

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

   Lorsque vous êtes connecté en tant qu’autre utilisateur ou utilisatrice, une notification s’affiche en haut de l’écran pour l’indiquer.

1. Après avoir effectué les actions nécessaires en tant qu’utilisateur ou utilisatrice, cliquez sur **Déconnexion**.

## Suivre et réaliser un audit de l’activité lorsqu’un administrateur ou une administratrice est connecté en tant qu’autre utilisateur ou utilisatrice

Workfront fournit des mécanismes pour suivre et réaliser un audit de l’activité lorsque l’administrateur ou l’administratrice est connecté en tant qu’autre utilisateur ou autre utilisatrice.

Lorsque vous vous connectez en tant qu’autre utilisateur ou utilisatrice, la date de dernière connexion de cet utilisateur ou de cette utilisatrice prend la date à laquelle l’administrateur ou l’administratrice système ou de groupe se connecte en tant que cet utilisateur ou cette utilisatrice.

* [Afficher des indicateurs sur les éléments](#view-indicators-on-items)
* [Afficher des informations sur l’audit](#view-audit-information)

### Afficher des indicateurs sur les éléments {#view-indicators-on-items}

Lorsque vous vous connectez à Workfront en tant qu’autre utilisateur ou utilisatrice et exécutez une action, Workfront indique clairement que toute action que vous effectuez est effectuée par vous au nom de l’utilisateur ou l’utilisatrice sous lequel ou laquelle vous êtes connecté.

Par exemple, si vous commentez un élément lors de votre connexion en tant qu’autre utilisateur ou utilisatrice, une instruction indique que vous avez commenté pour le compte de l’utilisateur ou de l’utilisatrice lors de l’affichage de la section Mises à jour d’un objet.

### Afficher des informations sur l’audit {#view-audit-information}

1. Connectez-vous à Workfront en tant qu’administrateur ou administratrice Workfront ou administrateur ou administratrice de groupe.
1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Connexion en tant que**, puis sur l’onglet **Journal d’accès** .

   Chaque fois qu’un administrateur ou une administratrice système ou de groupe se connecte à Workfront en tant qu’autre utilisateur ou autre utilisatrice, l’événement est consigné dans le journal d’audit. En outre, toutes les actions pouvant être auditées alors que l’administrateur ou l’administratrice est connecté en tant qu’autre utilisateur ou autre utilisatrice sont consignées dans le journal d’audit.

1. (Facultatif) Vous pouvez filtrer les résultats affichés dans le journal d’audit de la manière suivante :

   * Par l’utilisateur ou l’utilisatrice qui s’est connecté.
   * Par l’utilisateur ou l’utilisatrice qui s’est connecté en tant que.
   * Par date.
