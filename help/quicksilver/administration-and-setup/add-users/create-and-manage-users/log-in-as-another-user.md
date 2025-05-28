---
title: Se connecter en tant qu'utilisateur différent
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur ou administratrice Adobe Workfront, il peut arriver que vous deviez accéder à Workfront au nom d’une autre personne.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 6068c9c53568d3ebec9fae294bfee1cbd365714b
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 62%

---

# Se connecter sous une autre identité

<!--Audited: 5/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

En tant qu’administrateur Adobe Workfront, vous devrez peut-être parfois accéder à Workfront au nom d’un autre utilisateur. Ou, en tant qu’administrateur ou administratrice de groupe, vous pouvez avoir besoin d’accéder à Workfront au nom d’une personne membre d’un groupe que vous gérez.

Par exemple, si une tâche ne peut pas progresser tant qu’une personne en vacances n’a pas effectué une certaine action, vous pouvez vous connecter en tant que cette personne et effectuer l’action à sa place.

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
>Étant donné qu&#39;une intégration de documents peut se connecter à des fichiers personnels privés, les administrateurs et administratrices ne peuvent pas accéder aux intégrations de documents tout en ayant une connexion en tant qu’autre utilisateur ou utilisatrice.
>
>Pour plus d’informations sur les intégrations de documents, voir [Configuration des intégrations de documents](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard</p>
   <p>Ou</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Avec le niveau d'accès Administrateur système, vous pouvez vous connecter en tant que personne.</p> <p>Avec un niveau d’accès Standard ou Planificateur, vous pouvez vous connecter en tant qu’utilisateur avec un niveau de licence inférieur si le paramètre Utilisateurs du niveau d’accès est configuré sur Modifier l’accès, avec l’option Créer et au moins l’une des deux options d’administration des utilisateurs activées sous Affiner vos paramètres <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p>REMARQUE : de ces deux options, si l’option Administration des utilisateurs (utilisateurs du groupe) est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Se connecter et effectuer des actions en tant qu’un autre utilisateur ou qu’une autre utilisatrice

1. Connectez-vous à Workfront en tant qu’administrateur ou administratrice Workfront ou de groupe.

   >[!NOTE]
   >
   >* Si vous êtes administrateur ou administratrice de groupe, vous ne pouvez vous connecter qu’en tant qu’utilisateur ou utilisatrice des groupes que vous gérez. En outre, l’autorisation Administration des utilisateurs et utilisatrices (utilisateurs et utilisatrices de groupe) doit être activée dans votre niveau d’accès :
   >   
   >  ![Utilisateur administrateur de groupe](assets/group-admin-user.png)
   >   
   >  Ce paramètre est désactivé par défaut. Pour plus d’informations, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Vous ne pouvez pas réinitialiser le mot de passe d’un administrateur ou d’une administratrice Workfront.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Se connecter en tant que**.

1. Dans la zone **Commencer à saisir le nom...** de l&#39;onglet **Se connecter en tant que**, commencez à saisir le nom de l&#39;utilisateur, puis cliquez sur le nom lorsqu&#39;il apparaît dans la liste déroulante.


   >[!NOTE]
   >* Un niveau d’accès doit être défini dans Workfront pour l’utilisateur ou l’utilisatrice que vous sélectionnez. Vous ne pouvez pas vous connecter au système Workfront en tant que personne n’ayant pas les droits de connexion.
   >* Les administrateurs et administratrices de groupe ne peuvent se connecter qu’en tant que personnes membres des groupes gérés. Ils et elles ne peuvent pas se connecter en tant qu’administrateur ou administratrice Workfront.

1. Cliquez sur **Connexion**. Vous êtes connecté en tant qu’autre utilisateur et une notification s’affiche en haut de l’écran pour l’indiquer.

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



1. Une fois que vous avez effectué les actions nécessaires en tant qu’utilisateur, cliquez sur **Déconnexion** dans la partie supérieure de l’écran.

## Suivre et réaliser un audit de l’activité lorsqu’un administrateur ou une administratrice se connecte en tant qu’un autre utilisateur ou qu’une autre utilisatrice

Workfront fournit des mécanismes de suivi et de réalisation d’audit des activités qui ont lieu lorsque l’administrateur se connecte en tant qu’un autre utilisateur ou qu’une autre utilisatrice.

Lorsque vous vous connectez en tant qu’autre utilisateur, la date de dernière connexion de cet utilisateur est remplacée par la date de connexion de l’administrateur système ou de l’administrateur de groupe en tant qu’utilisateur en question.

* [Visualiser les indicateurs sur les éléments](#view-indicators-on-items)
* [Afficher les informations d’audit](#view-audit-information)

### Visualiser les indicateurs sur les éléments {#view-indicators-on-items}

Lorsque vous vous connectez à Workfront en tant qu’autre utilisateur ou utilisatrice et exécutez une action, Workfront indique clairement que toute action que vous effectuez est effectuée par vous au nom de l’utilisateur ou l’utilisatrice sous lequel ou laquelle vous êtes connecté.

Par exemple, si vous commentez un élément lors de votre connexion en tant qu’autre utilisateur ou utilisatrice, une instruction indique que vous avez commenté pour le compte de l’utilisateur ou de l’utilisatrice lors de l’affichage de la section Mises à jour d’un objet.

### Afficher des informations sur l’audit {#view-audit-information}

1. Connectez-vous à Workfront en tant qu’administrateur ou administratrice Workfront ou de groupe.
   {{step-1-to-setup}}
   <!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

1. Dans le panneau de gauche, cliquez sur **Connexion en tant que** puis sur l’onglet **Journal d’accès**.

   >[!NOTE]
   >
   >Chaque fois qu’un administrateur ou une administratrice système ou de groupe se connecte à Workfront en tant qu’un autre utilisateur ou qu’une autre utilisatrice, l’événement est enregistré dans le journal d’audit. En outre, toutes les actions vérifiables qui ont lieu lorsque l’administrateur ou administratrice se connecte en tant qu’un autre utilisateur ou qu’une autre utilisatrice sont enregistrées dans le journal d’audit.

1. (Facultatif) Vous pouvez filtrer les résultats qui s’affichent dans le journal d’audit des manières suivantes :

   * Par personne qui s’est connectée
   * Par personne qui s’est connectée en tant que
   * Par date et heure
