---
title: Supprimer utilisateurs
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Lorsqu’un utilisateur quitte votre entreprise, peut le supprimer de Workfront. Nous vous recommandons toutefois de désactiver les utilisateurs au lieu de les supprimer.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 15%

---

# Supprimer des utilisateurs et utilisatrices

Lorsqu’un utilisateur quitte votre entreprise, vous pouvez le supprimer d’Adobe Workfront.

>[!IMPORTANT]
>
>La suppression d’un utilisateur du système supprime également les informations associées à l’utilisateur que vous souhaitez peut-être conserver. Il est recommandé de désactiver les utilisateurs au lieu de les supprimer. Pour plus d’informations, voir [Désactivation ou réactivation d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur ou administratrice système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à un utilisateur ou une utilisatrice</a>. </p> </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Parmi ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être administrateur ou administratrice d’un groupe dont l’utilisateur est membre.</p> <p>Pour plus d’informations sur le paramètre <b>Utilisateurs et utilisatrices</b> dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Suppression ou désactivation d’un utilisateur

La désactivation d’un utilisateur entraîne les événements suivants :

* Supprime les licences de l’utilisateur pour Workfront et Workfront Proof si le composant Workfront Proof est associé à votre compte Workfront. Pour plus d’informations sur Workfront Proof, voir [Workfront Proof : article index](../../../workfront-proof/workfront-proof.md).
* L’utilisateur ne peut plus se voir attribuer une tâche.
* L’utilisateur ne peut plus être ajouté aux mises à jour.
* L’utilisateur ne peut plus être ajouté à des équipes ou à des groupes.
* Les objets ne peuvent plus être partagés avec l’utilisateur.
* Leur association avec les objets suivants reste intacte :

   * Tâches, problèmes, projets, portfolios
   * Tableaux de bord

     >[!NOTE]
     >
     >Si vous désactivez un utilisateur et ne pouvez plus afficher les rapports ou les tableaux de bord associés à un utilisateur, vous devrez peut-être mettre à jour le champ **Exécuter ce rapport avec les droits d’accès de :** .\
     >Pour en savoir plus, consultez la section [Pourquoi ne puis-je pas accéder à un rapport détenu par un utilisateur désactivé ?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) de l’article [FAQ sur les rapports](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) .

   * Documents
   * Mises à jour
   * Heures

* Si l’utilisateur a extrait des documents, les documents restent extraits lorsque vous les désactivez. Seul un administrateur Workfront peut les archiver à nouveau. Pour plus d’informations sur l’extraction de documents, voir [Extraction de documents](../../../documents/managing-documents/check-out-documents.md).

La suppression d’un utilisateur entraîne les événements suivants :

* Supprime les licences de l’utilisateur pour Workfront et Workfront Proof, si le composant Workfront Proof est associé à votre compte Workfront. Pour plus d’informations sur Workfront Proof, voir [Workfront Proof : article index](../../../workfront-proof/workfront-proof.md).
* L’utilisateur ne peut plus se voir attribuer une tâche.
* L’utilisateur ne peut plus être ajouté aux mises à jour.
* L’utilisateur ne peut plus être ajouté à des équipes ou à des groupes.
* Les objets ne peuvent plus être partagés avec l’utilisateur.
* Supprime l’association de cet utilisateur avec les objets suivants :

   * Tâches, problèmes, projets, portfolio
   * Tableaux de bord

     >[!NOTE]
     >
     >Vous ne pouvez plus accéder aux sections personnalisées qui contenaient des tableaux de bord associés à l’utilisateur supprimé.\
     >Pour en savoir plus, consultez le [Comment accéder à un tableau de bord contenant un rapport détenu par un utilisateur supprimé ?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) de l’article [FAQ sur les rapports](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) .

   * Mises à jour
   * Heures

     >[!NOTE]
     >
     >Ces objets restent dans Workfront, mais le propriétaire de l’objet est désormais vide.

* Si l’utilisateur a téléchargé des documents dans la zone Documents de la barre de navigation globale, les documents sont également supprimés.
* Si l’utilisateur a extrait les documents qu’il possède et que les documents sont téléchargés dans la zone Documents principale (accessible à partir du menu principal), les documents sont supprimés avec l’utilisateur. Pour plus d’informations sur l’extraction de documents, voir [Extraction de documents](../../../documents/managing-documents/check-out-documents.md).

Pour plus d’informations sur la désactivation des utilisateurs, voir [Désactivation ou réactivation d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Vous pouvez supprimer définitivement des utilisateurs un par un ou supprimer plusieurs utilisateurs simultanément. Lorsque vous supprimez des utilisateurs individuels, vous devez attendre que le processus de suppression soit terminé avant de passer à d’autres activités dans Workfront. Le processus de suppression simultanée de plusieurs utilisateurs s’exécute en arrière-plan, ce qui vous permet de continuer à utiliser Workfront lorsque les utilisateurs sont supprimés.

## Suppression d’un ou plusieurs utilisateurs

{{step-1-to-users}}

1. Sélectionnez au moins un utilisateur à supprimer, cliquez sur le menu Plus ![](assets/more-icon.png), puis sur **Supprimer**.
1. Dans la zone qui s’affiche, cliquez sur **Supprimer** pour confirmer la suppression.

   Le processus de suppression d’utilisateurs s’exécute en arrière-plan, de sorte que vous pouvez continuer à utiliser Workfront lorsque l’utilisateur ou les utilisateurs sont supprimés.

   Selon le nombre d’utilisateurs que vous supprimez, le processus peut prendre plusieurs minutes, voire quelques heures.

   Après avoir reçu la confirmation dans Workfront que les utilisateurs ont été supprimés, vous pouvez continuer à les voir dans le système jusqu’à ce que le processus de suppression soit terminé en arrière-plan.

   Si vous découvrez ultérieurement qu’un ou plusieurs utilisateurs n’ont pas été supprimés, essayez de les supprimer un par un.
