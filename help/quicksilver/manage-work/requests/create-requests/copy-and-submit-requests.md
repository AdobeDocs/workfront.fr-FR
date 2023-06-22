---
title: Copie et envoi de requêtes
description: Copie et envoi de requêtes
author: Alina
draft: Probably
feature: Work Management
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: cd059c445d86ed5581e8b2cb01507f18b97954f3
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# Copie et envoi de requêtes

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Lorsque vous envoyez fréquemment des requêtes similaires, vous pouvez copier une requête envoyée existante. Dans ce cas, vous pouvez copier une requête existante, y apporter des modifications minimales et la soumettre à nouveau en tant que nouvelle requête.

## Exigences d’accès

<!--drafted - replace table with P&P:

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
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
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
   <td> <p>Accès à l’ajout de requêtes à une file d’attente de requêtes</p> <p>Afficher ou des autorisations supérieures sur la requête existante</p> <p>Pour plus d’informations sur la configuration d’une file d’attente de requêtes, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Création d’une file d’attente de requête</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Vous devez disposer d’une demande que vous ou une personne de votre organisation avez déjà envoyée pour pouvoir la copier et la soumettre à nouveau. Si la demande appartient à une autre personne, vous devez avoir au moins accès à l’option Afficher pour pouvoir la copier et l’envoyer comme nouveau.

## Considérations relatives à la copie et à l’envoi de requêtes en tant que nouvelles

* Vous pouvez uniquement copier et envoyer des requêtes envoyées. Vous ne pouvez pas copier de requêtes en rédaction.
* Vous pouvez copier et envoyer des requêtes que vous avez envoyées initialement, ou des requêtes que d’autres personnes ont envoyées et vous avez accès à au moins Afficher.
* Vous avez toujours accès à la copie et à l’envoi d’une copie de vos propres requêtes, sauf si quelqu’un leur a retiré vos autorisations.
* L’accès aux demandes de copie et d’envoi envoyées initialement par d’autres peut être accordé automatiquement aux personnes de la même société lorsque le créateur de la file d’attente de demandes active la fonction **Les personnes d’une même société hériteront des mêmes autorisations pour toutes les demandes.** dans les zones Détails de la file d’attente ou Modifier le projet . La désactivation de ce paramètre permet uniquement au demandeur d’origine d’afficher ses propres requêtes.

  Pour plus d’informations, voir les articles suivants :

   * [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md)

* Vous pouvez mettre à jour la copie de la requête d’origine avant de la soumettre à nouveau en tant que nouvelle requête.
* Si les modifications suivantes surviennent après l’envoi de la demande d’origine, vous ne pouvez plus la copier et la soumettre à nouveau :

   * La file d’attente des demandes a été supprimée.
   * La rubrique de file d’attente a été supprimée.

     >[!TIP]
     >
     >Si la rubrique de la file d’attente était la seule dans la file d’attente des demandes, vous pouvez toujours copier et envoyer la demande. Elle sera enregistrée dans la file d’attente des demandes elle-même.

   * La file d’attente des demandes n’est plus publiée en tant que file d’attente des demandes d’aide. Pour plus d’informations, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Si la file d’attente des demandes ne comporte pas de rubrique de file d’attente et que la demande d’origine a été envoyée avant janvier 2022.

   * L’état du projet associé à la file d’attente des demandes n’est plus actuel.

* Vous pouvez copier et envoyer une copie d’une requête convertie si la requête a été conservée dans le processus de conversion. Pour plus d’informations, voir [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >La requête copiée n’est pas liée à un objet de résolution.

## Copie et envoi de requêtes

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Demandes**.
1. (Conditionnel) Si la section Envoyé ne s’affiche pas par défaut, cliquez sur **Envoyé** dans le panneau de gauche.
1. Recherchez la requête que vous souhaitez copier et envoyer comme nouvelle requête, puis effectuez l’une des opérations suivantes :

   * Sélectionnez-le, puis cliquez sur le bouton **Copier et envoyer en tant que nouveau** icon ![](assets/copy-and-submit-as-new-requests-area-nwe.png) dans le coin supérieur gauche de la liste Demandes envoyées . <!--update this icon AND change its name to "Copy" with the 23.3 preview release, or shortly after-->

   <!-- reveal this tip for 23.3 preview release:
   >[!TIP]
   >
   > <span class="preview">If you did not select a request first, the Copy icon is dimmed.</span> 
   -->

   * Cliquez sur le bouton **Plus** menu ![](assets/more-icon.png) à droite du nom de la requête, puis cliquez sur **Copier et envoyer en tant que nouveau** <!--ensure this does not change with the Copy icon improvements with 23.3 preview-->

     Ou

     Cliquez avec le bouton droit de la souris sur la requête sélectionnée, puis cliquez sur **Copier et envoyer en tant que nouveau**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Lorsque vous n’avez pas accès à la création de problèmes, vous recevez un avertissement indiquant que l’administrateur vous a empêché de créer des requêtes.

1. (Facultatif) Mettez à jour les informations suivantes, le cas échéant :

   * **Type de requête**: la file d’attente des demandes dans laquelle la requête copiée est enregistrée. Par défaut, la requête copiée est enregistrée dans la file d’attente des requêtes de la requête d’origine.
   * **Groupes de rubriques** et **Rubriques de file**, s’ils sont sélectionnés. Les noms ou les groupes de rubriques et les rubriques de la file d’attente sont personnalisés pour votre environnement. Par défaut, la requête copiée est enregistrée dans les groupes de rubriques et les rubriques de file d’attente de la requête d’origine.

     >[!TIP]
     >
     >Si le chemin d’accès change à partir du chemin d’accès de la requête d’origine, le créateur de la file d’attente de la requête modifie la file d’attente.

1. (Facultatif) Mettez à jour les informations de la requête copiée. Selon les champs activés par le créateur de la file d’attente de requêtes dans **Nouveaux champs de problème** de la section **Détails de la file** sous-onglet du projet, vous trouverez peut-être l’un des champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Objet</strong> </td> 
      <td>Affiche le nom de la requête d’origine. Mettez-le à jour, si nécessaire. Sinon, Workfront nomme la requête copiée. <b>Copie de &lt;name of="" original="" request=""&gt;</b>. Il s’agit d’un champ obligatoire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Affiche la description de la requête d’origine. Mettez-le à jour, si nécessaire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Affiche l’URL de la requête d’origine. Mettez-le à jour, si nécessaire.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorité</strong> </td> 
      <td> <p>Indiquez la priorité de votre requête. La priorité doit définir la vitesse à laquelle vous pensez que cette requête doit être résolue. Les options par défaut sont les suivantes :</p> 
       <ul> 
        <li>Aucun</li> 
        <li>Faible</li> 
        <li>Normal</li> 
        <li>Élevé</li> 
        <li>Urgent</li> 
       </ul> <p>Votre administrateur Workfront peut modifier les noms des priorités.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gravité</strong> </td> 
      <td> <p>Spécifiez la gravité de votre requête. La gravité doit définir l’impact de cette requête sur votre travail s’il n’est pas résolu à temps. Les options par défaut sont les suivantes :</p> 
       <ul> 
        <li>Décoratif</li> 
        <li>Cause de la confusion</li> 
        <li>Bogue qui a une solution</li> 
        <li>Bogue sans solution</li> 
        <li>Erreur fatale</li> 
       </ul> <p>Votre administrateur Workfront peut modifier les noms des statistiques.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contact principal</strong> </td> 
      <td>Le contact Principal d’une requête vous est transmis par défaut, dans la mesure où vous êtes la personne qui répond à toutes les questions relatives à la requête. Cependant, vous pouvez modifier ce paramètre pour n’importe quel autre utilisateur Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Affectations</strong></span> </td> 
      <td> <p>Indiquez le nom d’un utilisateur, d’un rôle de tâche ou d’une équipe principal auquel la requête doit être affectée. </p> <p> Vous pouvez spécifier plusieurs utilisateurs, rôles de tâche ou équipes. </p> <p>Selon la configuration de la file d’attente des demandes, vous pouvez n’affecter la requête qu’à un ou deux types de ressources, au lieu des trois. </p> <p>Nous vous recommandons d’utiliser des règles de routage pour vos files d’attente de requêtes afin qu’elles puissent être automatiquement acheminées vers les ressources appropriées. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">En fonction de la configuration de la file d’attente des demandes, il se peut que vous ne puissiez affecter qu’un seul type de ressource à la demande (par exemple, les utilisateurs). Si une règle de routage est également associée à la file d’attente des demandes et qu’elle achemine automatiquement la demande vers un autre type de ressource (par exemple, une équipe), votre demande est affectée à la fois à l’entité que vous spécifiez manuellement lors de l’envoi de la demande (utilisateurs) et à la ressource spécifiée dans la règle de routage (l’équipe).</p> <p style="font-weight: normal;">Pour plus d’informations, voir les articles suivants :</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Création d’une file d’attente de requête</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Création de règles de routage</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Heures prévues</strong> </td> 
      <td> <p>Estimez le nombre d’heures nécessaire à l’exécution de cette requête.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Date de début prévue</strong> </td> 
      <td> <p>Date à laquelle le travail sur cette requête doit commencer.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Date d'achèvement prévue</strong> </td> 
      <td>Date à laquelle vous souhaitez que cette requête soit résolue.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Statut</strong> </td> 
      <td>L’état par défaut d’une nouvelle requête est "Nouveau". Votre administrateur Workfront a peut-être modifié le nom de cet état. Vous pouvez également modifier l’état pour autre chose à partir de ce menu déroulant.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documents</strong> </td> 
      <td> <p>Ajoutez des documents à votre requête. Les documents joints à la requête d’origine ne sont pas transférés vers la requête copiée.</p> <p><b>CONSEIL</b>

   Selon la configuration de la file d’attente des demandes, la section Documents peut s’afficher avant ou après les champs personnalisés.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Facultatif) Si nécessaire, mettez à jour les informations contenues dans les formulaires personnalisés joints.

   >[!TIP]
   >
   >* Tous les formulaires personnalisés associés à la requête d’origine et les valeurs incluses dans les champs personnalisés sont transférés vers la requête copiée. Cela inclut les champs qui contiennent de la logique.
   >* Vous ne pouvez pas supprimer des formulaires personnalisés de la requête copiée.

1. Cliquez sur **Envoyer**.

   La requête copiée est envoyée en tant que nouvelle requête dans la file d’attente de requête que vous avez spécifiée.
