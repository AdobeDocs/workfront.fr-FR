---
title: Suppression d’utilisateurs
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Lorsqu’un utilisateur quitte votre entreprise, peut le supprimer de Workfront. Nous vous recommandons toutefois de désactiver les utilisateurs au lieu de les supprimer.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Suppression d’utilisateurs

Lorsqu’un utilisateur quitte votre entreprise, vous pouvez le supprimer d’Adobe Workfront.

>[!IMPORTANT]
>
>* La suppression d’un utilisateur du système supprime également les informations associées à l’utilisateur que vous souhaitez peut-être conserver. Il est recommandé de désactiver les utilisateurs au lieu de les supprimer. Pour plus d’informations, voir [Désactivation ou réactivation d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées au Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, vous devez effectuer cette action via Adobe Admin Console.
>
>Suppression d’un utilisateur de l’événement [!DNL Adobe Admin Console] désactive l’utilisateur dans [!DNL Workfront], mais ne les supprime pas de [!DNL Workfront].
>
>  Pour obtenir des instructions sur la suppression d’un utilisateur dans Adobe Admin Console, reportez-vous à la section &quot;Suppression définitive d’utilisateurs&quot; de l’article. [Gérer les utilisateurs individuellement](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) ou contactez votre administrateur Adobe Admin Console.
>
>  Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Admin Console, voir [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez disposer de l’une des options suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
     <li> <p><b>Utilisateurs</b> paramètre de votre niveau d’accès configuré sur <b>Modifier</b> accès, avec <b>Créer</b> et au moins l’une des deux <b>Administration des utilisateurs</b> options activées sous <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>de ces deux options, si Utilisateur <b>Administration (utilisateurs de groupe)</b> est activé, vous devez être administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> <p>Pour plus d’informations sur la variable <b>Utilisateurs</b> paramétrer un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Suppression ou désactivation d’un utilisateur

La désactivation d’un utilisateur entraîne les événements suivants :

* Supprime les licences de l’utilisateur pour Workfront et Workfront BAT si le composant BAT Workfront est associé à votre compte Workfront. Pour plus d’informations sur le BAT Workfront, voir [Bon à tirer Workfront : index de l’article](../../../workfront-proof/workfront-proof.md).
* L’utilisateur ne peut plus se voir attribuer une tâche.
* L’utilisateur ne peut plus être ajouté aux mises à jour.
* L’utilisateur ne peut plus être ajouté à des équipes ou à des groupes.
* Les objets ne peuvent plus être partagés avec l’utilisateur.
* Leur association avec les objets suivants reste intacte :

   * Tâches, problèmes, projets, portfolios
   * Tableaux de bord

     >[!NOTE]
     >
     >Si vous désactivez un utilisateur et ne pouvez plus afficher les rapports ou les tableaux de bord associés à un utilisateur, vous devrez peut-être mettre à jour la variable **Exécutez ce rapport avec les droits d’accès de :** champ .\
     >Pour en savoir plus, voir la section [Pourquoi ne puis-je pas accéder à un rapport détenu par un utilisateur désactivé ?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) de la [FAQ sur les rapports](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

   * Documents
   * Mises à jour
   * Heures

* Si l’utilisateur a extrait des documents, les documents restent extraits lorsque vous les désactivez. Seul un administrateur Workfront peut les archiver à nouveau. Pour plus d’informations sur l’extraction de documents, voir [Extraction de documents](../../../documents/managing-documents/check-out-documents.md).

La suppression d’un utilisateur entraîne les événements suivants :

* Supprime les licences de l’utilisateur pour Workfront et Workfront BAT, si le composant BAT Workfront est associé à votre compte Workfront. Pour plus d’informations sur le BAT Workfront, voir [Bon à tirer Workfront : index de l’article](../../../workfront-proof/workfront-proof.md).
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
     >Pour en savoir plus, voir la section [Comment accéder à un tableau de bord contenant un rapport détenu par un utilisateur supprimé ?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) de la [FAQ sur les rapports](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

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

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Utilisateurs**.
1. Sélectionnez au moins un utilisateur à supprimer, puis cliquez sur le menu Plus . ![](assets/more-icon.png), puis cliquez sur **Supprimer**.
1. Dans la zone qui s’affiche, cliquez sur **Supprimer** pour confirmer la suppression.

   Le processus de suppression d’utilisateurs s’exécute en arrière-plan, de sorte que vous pouvez continuer à utiliser Workfront lorsque l’utilisateur ou les utilisateurs sont supprimés.

   Selon le nombre d’utilisateurs que vous supprimez, le processus peut prendre plusieurs minutes, voire quelques heures.

   Après avoir reçu la confirmation dans Workfront que les utilisateurs ont été supprimés, vous pouvez continuer à les voir dans le système jusqu’à ce que le processus de suppression soit terminé en arrière-plan.

   Si vous découvrez ultérieurement qu’un ou plusieurs utilisateurs n’ont pas été supprimés, essayez de les supprimer un par un.
