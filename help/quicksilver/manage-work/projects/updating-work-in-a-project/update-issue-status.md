---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mettre à jour le statut du problème
description: Vous pouvez mettre à jour l’état d’un problème afin d’informer les autres personnes de son état et de son état d’avancement.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 3%

---

# Mettre à jour le statut du problème

Vous pouvez mettre à jour l’état d’un problème afin d’informer les autres personnes de son état et de son état d’avancement.

## Exigences d’accès

<!--drafted for P&P;

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations liées au problème</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Statuts des problèmes

Voici les états par défaut des problèmes dans Workfront :

* Nouveau
* En cours
* Réaction en attente
* Suspendu
* Impossible de résoudre
* Rouvert
* Fermé
* Résolu

Votre administrateur Adobe Workfront peut ajouter des états personnalisés pour les problèmes de votre entreprise. Ils peuvent également rendre les états disponibles en fonction du type de problème.

Pour plus d’informations sur les états personnalisés et les types de problèmes, consultez les articles suivants :

* [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [Création de problèmes](../../../manage-work/issues/manage-issues/create-issues.md)

Vous pouvez mettre à jour manuellement les statuts des problèmes ou laisser Workfront les mettre à jour automatiquement lorsque certaines actions ont lieu.

## Mise à jour manuelle de l’état des problèmes

Lorsque vous mettez à jour un état de problème, vous pouvez également ajouter une explication sur le nouveau statut et modifier d’autres informations de problème telles que la date de validation.

1. Accédez à un problème auquel vous êtes affecté et pour lequel vous souhaitez mettre à jour l’état.
1. Cliquez sur le bouton **État** dans l’en-tête du problème et sélectionnez un nouvel état.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. Pour fournir une indication visuelle de la fin du problème, faites glisser ou double-cliquez sur la bulle sous **Pourcentage terminé** dans l’en-tête du problème.

   Ou

   Cliquez à l’intérieur de la bulle dans l’en-tête de la question pour entrer un pourcentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Facultatif) Pour fournir des informations supplémentaires sur la mise à jour, effectuez l’une des opérations suivantes, puis cliquez sur **Mettre à jour** ou, si le statut du problème correspond à Terminé, cliquez sur **Terminé :**

   * Pour ajouter une note à propos de la mise à jour, accédez au **Mises à jour** et cliquez sur **Démarrer une nouvelle mise à jour**, puis saisissez votre note.

      ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Pour avertir certains utilisateurs de la mise à jour, saisissez leurs noms dans le champ **Notifier** qui s’affiche lorsque vous saisissez une note à propos de la mise à jour. Pour plus d’informations, voir [Balisage des autres sur les mises à jour](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Pour mettre à jour la condition du problème, cliquez sur **Condition**, puis sélectionnez la condition qui reflète le mieux la condition actuelle du problème. Sélectionnez l’une des options suivantes :

      * Tout est en ordre
      * Certaines inquiétudes
      * Obstacles majeurs
   * Pour mettre à jour la date de validation du problème, développez la variable **Date de validation** du calendrier déroulant, puis sélectionnez une nouvelle date.


## Mettre automatiquement à jour le statut des problèmes

Workfront met automatiquement à jour l’état existant d’un problème à un état différent lorsque les actions répertoriées dans le tableau ci-dessous se produisent.

>[!NOTE]
>
>Les états dans le tableau suivant sont les états système par défaut. Votre administrateur Workfront ou un administrateur de groupe peut renommer les états de votre instance de Workfront. Pour plus d’informations sur la création et la gestion des états dans Workfront, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Action</td> 
   <td>État d’origine</td> 
   <td>Nouveau statut</td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le pourcentage de problèmes terminé à 100 %</td> 
   <td>Nouveau ou en cours</td> 
   <td>Fermé</td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le pourcentage de problèmes terminé de 100 % à un nombre inférieur</td> 
   <td>Fermé </td> 
   <td>En cours</td> 
  </tr> 
  <tr> 
   <td>Mettre à jour l’état d’un objet de résolution associé au problème</td> 
   <td>Divers statuts</td> 
   <td> <p>Divers statuts</p> <p>Pour plus d’informations sur la résolution des objets et sur leur impact sur l’état des problèmes, voir la section "Synchronisation de l’état de l’objet résolvable avec celui de l’objet résolvable" dans l’article . <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et des objets résolvables </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Cliquez sur le bouton Démarrer le problème pour accepter de travailler sur un problème qui vous est assigné.</span> </td> 
   <td><span>Nouveau</span> </td> 
   <td> <p>Tout état associé au bouton Démarrer le problème dans les paramètres de votre équipe d’accueil. </p> <p>Pour plus d’informations sur le remplacement du bouton Travailler dessus par un bouton Démarrer le problème, voir <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Remplacez le bouton Travailler dessus par un bouton Démarrer</a></span><span>.</span> </p> <p>Conseil : Cliquer <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">Bouton Annuler</span> après avoir cliqué sur Démarrer le problème, l’état devient Nouveau. </p> </td> 
  </tr> 
 </tbody> 
</table>
