---
title: Supprimer utilisateurs
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Lorsqu’une personne quitte votre entreprise, vous pouvez la supprimer de Workfront. Nous vous recommandons toutefois de désactiver les personnes au lieu de les supprimer.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 58567104d88e7e1363d4196aec8a36ee0566b95a
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 89%

---

# Supprimer des utilisateurs et utilisatrices

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore intégré Adobe Business Platform. Si vous avez intégré Adobe Business Platform, vous devez supprimer les utilisateurs dans Adobe Admin Console.
>
>Pour obtenir une liste de procédures qui diffèrent selon que votre entreprise a été intégrée ou non à Adobe Business Platform, voir [Différences d’administration en fonction de la plateforme (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Lorsqu’une personne quitte votre entreprise, vous pouvez la supprimer d’Adobe Workfront.

>[!IMPORTANT]
>
>La suppression d’une personne du système entraîne également la suppression des informations associées que vous pourriez souhaiter conserver. Nous recommandons de désactiver les personnes plutôt que de les supprimer. Pour plus d’informations, voir [Désactiver ou réactiver un utilisateur ou une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
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
   <td><p>Nouveau : Standard</p><p>Ou</p><p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès de l’administrateur système. </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Suppression ou désactivation d’une personne

La désactivation d’une personne entraîne les événements suivants :

* Supprime les licences de l’utilisateur ou l’utilisatrice pour Workfront et Workfront Proof si le composant Workfront Proof est associé à votre compte Workfront. Pour plus d’informations sur Workfront Proof, voir [Workfront Proof : index des articles](../../../workfront-proof/workfront-proof.md).
* La personne ne peut plus se voir affecter du travail.
* La personne ne peut plus être ajoutée aux mises à jour.
* La personne ne peut plus être ajoutée à des équipes ou à des groupes.
* Les objets ne peuvent plus être partagés avec la personne.
* Leur association avec les objets suivants reste intacte :

   * Tâches, problèmes, projets, portfolios
   * Tableaux de bord

     >[!NOTE]
     >
     >Si vous désactivez une personne et ne pouvez plus afficher les rapports ou les tableaux de bord associés à une personne, vous devrez peut-être mettre à jour le champ **Exécuter ce rapport avec les droits d’accès suivants :**.\
     >Pour en savoir plus, voir la section [Pourquoi ne puis-je pas accéder à un rapport détenu par une personne désactivée ?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) de l’article [Questions fréquentes sur les rapports](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

   * Documents
   * Mises à jour
   * Heures

* Si la personne a extrait des documents, les documents restent extraits lorsque vous les désactivez. Seul un administrateur ou une administratrice Workfront peut les réenregistrer. Pour plus d’informations sur l’extraction de documents, voir [Extraire des documents](../../../documents/managing-documents/check-out-documents.md).

La suppression d’une personne entraîne les événements suivants :

* Supprime les licences de l’utilisateur ou de l’utilisatrice pour Workfront et Workfront Proof, si le composant Workfront Proof est associé à votre compte Workfront. Pour plus d’informations sur Workfront Proof, voir [Workfront Proof : index des articles](../../../workfront-proof/workfront-proof.md).
* La personne ne peut plus se voir affecter du travail.
* La personne ne peut plus être ajoutée aux mises à jour.
* La personne ne peut plus être ajoutée à des équipes ou à des groupes.
* Les objets ne peuvent plus être partagés avec la personne.
* Supprime l’association de cette personne avec les objets suivants :

   * Tâches, problèmes, projets, portfolio
   * Tableaux de bord

  <!--
     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.
     -->

   * Mises à jour
   * Heures

     >[!NOTE]
     >
     >Ces objets restent dans Workfront mais la mention de leur personne propriétaire reste vide.

* Lorsque des documents sont ajoutés à la section des documents de la barre de navigation globale par un utilisateur ou une utilisatrice, ils sont également supprimés.
* Quand un utilisateur ou une utilisatrice extrait ses documents pour les charger dans la zone principale des documents, accessible par le menu principal, ces documents sont supprimés lors de la suppression de cet utilisateur ou de cette utilisatrice. Pour plus d’informations sur l’extraction de documents, consultez la section [Extraire des documents](../../../documents/managing-documents/check-out-documents.md).

Pour plus d’informations sur la désactivation des utilisateurs et des utilisatrices, consultez la section [Désactiver ou réactiver un utilisateur ou une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Vous pouvez supprimer définitivement des utilisateurs et des utilisatrices soit séparément, soit simultanément. Lorsque vous supprimez des utilisateurs ou des utilisatrices séparément, vous devez attendre que le processus de suppression soit terminé avant de passer à d’autres activités dans Workfront. Vous pouvez continuer à travailler sur Workfront pendant que le système supprime simultanément plusieurs utilisateurs et utilisatrices en arrière-plan.

## Supprimer séparément ou simultanément des utilisateurs ou des utilisatrices

{{step-1-to-users}}

1. Sélectionnez au moins un utilisateur à supprimer, cliquez sur le menu Plus ![icône Plus](assets/more-icon.png), puis sur **Supprimer**.
1. Dans la zone qui s’affiche, cliquez sur **Supprimer** pour confirmer la suppression.

   Le processus de suppression séparée ou simultanée s’exécute en arrière-plan, de sorte que vous pouvez continuer à utiliser Workfront lorsque la suppression s’effectue.

   Selon le nombre d’utilisateurs et d’utilisatrices que vous supprimez, le processus peut prendre plusieurs minutes, voire quelques heures.

   Bien que Workfront vous informe de la réussite de la suppression des utilisateurs et des utilisatrices, il se peut que vous continuiez à les voir dans le système jusqu’à ce que le processus en arrière-plan soit entièrement finalisé.

   Si vous constatez plus tard que certaines suppressions n’ont pas été correctement effectuées, faites les séparément.
