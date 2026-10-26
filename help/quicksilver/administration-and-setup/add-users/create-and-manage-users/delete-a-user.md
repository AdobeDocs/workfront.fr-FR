---
title: Supprimer utilisateurs
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Lorsqu’une personne quitte votre entreprise, vous pouvez la supprimer de Workfront. Nous vous recommandons toutefois de désactiver les personnes au lieu de les supprimer.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
TQID: 'https://experienceleague.adobe.com/T5iSq2SOJEQrlvLNiQ5l69OncRMYvEs4uf6QosY9vq8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 6275fff5d615a8db678f16d99c38c96319a57155
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 77%
---
# Supprimer des utilisateurs et utilisatrices

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas été intégrées à Admin Console. Étant donné que votre organisation a été intégrée à Adobe Admin Console, vous devez effectuer cette action via Adobe Admin Console.
>
>  Pour obtenir des instructions sur la suppression d’un utilisateur dans Adobe Admin Console, reportez-vous à la section « Supprimer définitivement des utilisateurs » de l’article [Gérer les utilisateurs individuellement](https://helpx.adobe.com/fr/enterprise/using/manage-users-individually.html) ou contactez votre administrateur Adobe Admin Console.

Lorsqu’une personne quitte votre entreprise, vous pouvez la supprimer d’Adobe Workfront.

La suppression d’un utilisateur ou d’une utilisatrice doit être effectuée via Adobe Admin Console. Pour obtenir des instructions, reportez-vous à la section « Supprimer définitivement des utilisateurs » de l’article [Gérer les utilisateurs individuellement](https://helpx.adobe.com/fr/enterprise/using/manage-users-individually.html) ou contactez votre administrateur Adobe Admin Console.

>[!IMPORTANT]
>
>La suppression d’une personne du système entraîne également la suppression des informations associées que vous pourriez souhaiter conserver. Nous recommandons de désactiver les personnes plutôt que de les supprimer. Pour plus d’informations, voir [Désactiver ou réactiver un utilisateur ou une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être administrateur sur le Adobe Admin Console.</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
    >Pour en savoir plus, consultez le [Pourquoi ne puis-je pas accéder à un rapport détenu par un utilisateur désactivé ?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) de l’article [FAQ sur les rapports](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

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
     >
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


<!--

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![More icon](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.

   -->
