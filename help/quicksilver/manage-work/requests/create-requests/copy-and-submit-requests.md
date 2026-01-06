---
title: Copie et envoi de demandes
description: Lorsque vous soumettez fréquemment des demandes similaires, vous pouvez copier une demande déjà soumise. Dans ce cas, vous pouvez copier une demande existante, y apporter des modifications minimes et la soumettre à nouveau en tant que nouvelle demande.
author: Becky
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 85%

---

# Copier et soumettre les demandes


<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

Lorsque vous soumettez fréquemment des demandes similaires, vous pouvez copier une demande déjà soumise. Dans ce cas, vous pouvez copier une demande existante, y apporter des modifications minimes et la soumettre à nouveau en tant que nouvelle demande.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Contributeur ou version ultérieure</p>
   <p>Requête ou supérieure</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader">Autorisations d’objet</td> 
   <td><p>Accès à l’ajout de demandes à une file d’attente</p> <p>Autorisation en affichage ou supérieure sur la demande existante</p> <p>Pour plus d’informations sur la configuration d’une file d’attente des demandes, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Créer une file d’attente des demandes</a>. </p> </td> 
  </tr>
  <tr> 
   <td role="rowheader"> Produit</td> 
   <td> <ul><li>Adobe Workfront</li><li>Vous devez disposer d’Adobe Workfront Planning pour afficher les demandes Planning ou les formulaires de demande</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Vous devez avoir une demande que vous ou une personne membre de votre organisation avez déjà soumise pour pouvoir la copier et la soumettre à nouveau. Si la demande appartient à quelqu’un d’autre, vous devez au moins avoir accès à son affichage pour pouvoir la copier et la soumettre comme nouvelle.

## Considérations relatives à la copie et à la soumission des demandes en tant que nouvelles demandes

* Vous ne pouvez copier et soumettre que les demandes soumises. Vous ne pouvez pas copier les brouillons de demandes.
* Vous pouvez copier et soumettre des demandes que vous avez initialement soumises, ou des demandes que d’autres ont soumises et auxquelles vous avez accès au moins à l’affichage.
* Vous avez toujours la possibilité de copier et de soumettre une copie de vos propres demandes, à moins que quelqu’un ne vous ait retiré l’autorisation d’y accéder.
* L’accès à la copie et à la soumission des demandes initialement soumises par d’autres personnes peut être accordé automatiquement aux personnes de la même entreprise lorsque le créateur ou la créatrice de la file d’attente des demandes active l’option **Les personnes appartenant à la même entreprise hériteront d’autorisations identiques pour toutes les demandes** dans les zones Détails de la file d’attente ou Modifier le projet. La désactivation de ce paramètre permet uniquement au demandeur ou à la demandeuse initial d’afficher ses propres demandes.

  Pour plus d’informations, consultez les articles suivants :

   * [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md)

* Vous pouvez mettre à jour la copie de la demande originale avant de la soumettre à nouveau en tant que nouvelle demande.
* Si les changements suivants interviennent après la soumission de la demande initiale, vous ne pouvez plus la copier et la soumettre à nouveau :

   * La file d’attente des demandes a été supprimée.
   * La rubrique de file d’attente a été supprimée.

     >[!TIP]
     >
     >Si la rubrique de file d’attente était la seule dans la file d’attente des demandes, vous pouvez toujours copier et soumettre la demande et elle sera enregistrée sous la file d’attente des demandes.

   * La file d’attente des demandes n’est plus publiée en tant que file d’attente des demandes d’aide. Pour plus d’informations, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Si la file d’attente des demandes n’a pas de rubrique de file d’attente et que la demande originale a été soumise avant janvier 2022.

   * Le statut du projet associé à la file d’attente des demandes n’est plus en cours.

* Vous pouvez copier et soumettre une copie d’une demande convertie si la demande a été conservée lors du processus de conversion. Pour plus d’informations, voir [Vue d’ensemble de la conversion des problèmes dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >La demande copiée n’est pas liée à un objet de résolution.

## Copier et envoyer des requêtes dans l’expérience de requête héritée

{{step1-to-requests}}

1. (Le cas échéant) Si la section Soumis ne s’affiche pas par défaut, cliquez sur **Soumis** dans le panneau de gauche.

   >[!TIP]
   >
   >   Votre administrateur ou administratrice Workfront ou de groupes peut personnaliser votre modèle de mise en page et supprimer des zones du menu principal ou du panneau de gauche dans votre environnement. Dans ce cas, il se peut que vous ne puissiez pas en bénéficier.

1. Localisez la demande que vous souhaitez copier et soumettre en tant que nouvelle demande, puis effectuez l’une des opérations suivantes :

   * Sélectionnez-la, puis cliquez sur **Copier** ![](assets/copy-and-submit-as-new-requests-area-nwe.png) dans le coin supérieur gauche de la liste des demandes soumises.

   >[!TIP]
   >
   > Si vous n’avez pas sélectionné d’abord une demande, l’icône Copier est grisé.

   * Cliquez sur le menu **Plus** ![](assets/more-icon.png) à droite du nom de la demande, puis cliquez sur **Copier et soumettre comme nouveau**.

     Ou

     Cliquez avec le bouton droit de la souris sur la demande sélectionnée, puis sur **Copier et soumettre comme nouveau**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Lorsque vous n’avez pas accès à la création des problèmes, vous recevez un avertissement indiquant que votre administrateur ou administratrice vous a interdit de créer des demandes.

1. (Facultatif) Mettez à jour les informations suivantes, si nécessaire :

   * **Type de demande** : la file d’attente des demandes où la demande copiée est enregistrée. Par défaut, la demande copiée est enregistrée dans la file d’attente des demandes de la demande originale.
   * **Groupes de rubriques** et **Rubriques de file d’attente**, s’ils sont sélectionnés. Les noms des groupes de sujets et des rubriques de file d’attente sont personnalisés en fonction de votre environnement. Par défaut, la demande copiée est enregistrée dans les groupes de sujets et les rubriques de file d’attente de la demande originale.

     >[!TIP]
     >
     >Si le chemin d’accès change par rapport à celui de la demande initiale, cela signifie que le créateur ou la créatrice de la file d’attente des demandes l’a modifiée.

1. (Facultatif) Mettez à jour les informations de la demande copiée. Selon les champs activés par le créateur de la file d’attente des demandes dans la section **Nouveaux champs de problème** du sous-onglet **Détails de la file d’attente** du projet, vous pouvez trouver l’un des champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Objet</strong> </td> 
      <td>Affiche le nom de la demande originale. Mettez-le à jour, si nécessaire. Sinon, Workfront nomme la demande copiée <b>Copie de &lt;Nom de la demande d’origine&gt;</b>. Champ obligatoire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Affiche la description de la demande originale. Mettez-le à jour, si nécessaire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Affiche l’URL de la demande originale. Mettez-le à jour, si nécessaire.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorité</strong> </td> 
      <td> <p>Précisez la priorité de votre demande. La priorité doit définir la vitesse à laquelle vous estimez que cette demande doit être résolue. Les options par défaut sont les suivantes :</p> 
       <ul> 
        <li>Aucun</li> 
        <li>Faible</li> 
        <li>Normal</li> 
        <li>Élevé</li> 
        <li>Urgent</li> 
       </ul> <p>Votre administrateur ou administratrice Workfront peut modifier les noms des priorités.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gravité</strong> </td> 
      <td> <p>Précisez la gravité de votre demande. La gravité doit définir l’impact de cette demande sur votre travail si elle n’est pas résolue à temps. Les options par défaut sont les suivantes :</p> 
       <ul> 
        <li>Décoratif</li> 
        <li>Cause de la confusion</li> 
        <li>Bogue qui a une solution</li> 
        <li>Bogue sans solution</li> 
        <li>Erreur fatale</li> 
       </ul> <p>Votre administrateur ou administratrice Workfront peut modifier les noms des gravités.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contact principal</strong> </td> 
      <td>Le contact principal d’une demande vous est attribué par défaut, car vous êtes la personne de référence pour répondre à toute question relative à la demande. Cependant, vous pouvez l’attribuer à tout autre utilisateur ou toute autre utilisatrice de Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Affectations</strong></span> </td> 
      <td> <p>Indiquez le nom d’une personne active, d’une fonction ou d’une équipe à qui la demande doit être affectée. </p> <p> Vous pouvez spécifier plus d’une personne, d’une fonction ou d’une équipe. </p> <p>En fonction de la configuration de la file d’attente des demandes, il se peut que vous ne puissiez attribuer la demande qu’à un ou deux types de ressources, et non aux trois. </p> <p>Nous vous recommandons d’utiliser des règles de transmission pour vos files d’attente des demandes afin que celles-ci puissent être automatiquement acheminées vers les ressources appropriées. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">En fonction de la configuration de la file d’attente, il se peut que vous ne puissiez attribuer qu’un seul type de ressource à la demande (par exemple, des personnes). Si une règle de transmission est également associée à la file d’attente des demandes et qu’elle achemine automatiquement la demande vers un autre type de ressource (par exemple, une équipe), votre demande est affectée à la fois à l’entité que vous avez spécifiée manuellement lors de la soumission de la demande (les personnes) et à la ressource spécifiée dans la règle de transmission (l’équipe).</p> <p style="font-weight: normal;">Pour plus d’informations, consultez les articles suivants :</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Créer une file d’attente des demandes</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Créer des règles de transmission</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Nombre d’heures prévues</strong> </td> 
      <td> <p>Estimer le nombre d’heures nécessaires à la réalisation de cette demande.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Date de début prévue</strong> </td> 
      <td> <p>Date à laquelle le travail sur cette demande devrait commencer.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Date d’achèvement prévue</strong> </td> 
      <td>Date à laquelle cette demande doit être résolue.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Statut</strong> </td> 
      <td>Le statut par défaut d’une nouvelle demande est « Nouveau ». Il se peut que votre équipe d’administration Workfront ait modifié le nom de ce statut. Vous pouvez également modifier le statut à partir de ce menu déroulant.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documents</strong> </td> 
      <td> <p>Ajoutez des documents à votre demande. Les documents joints à la demande originale ne sont pas transférés vers la demande copiée.</p> <p><b>CONSEIL</b>

   En fonction de la configuration de la file d’attente des demandes, la section Documents peut s’afficher avant ou après les champs personnalisés.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Facultatif) Mettez à jour les informations contenues dans les formulaires personnalisés joints, si nécessaire.

   >[!TIP]
   >
   >* Tous les formulaires personnalisés joints à la demande originale et les valeurs incluses dans les champs personnalisés sont transférés à la demande copiée. Cela inclut les champs qui contiennent une logique.
   >* Vous ne pouvez pas supprimer les formulaires personnalisés de la demande copiée.

1. Cliquez sur **Soumettre**.

   La demande copiée est soumise en tant que nouvelle demande dans la file d’attente des demandes que vous avez spécifiée.

<div class="preview">

## Copiez et envoyez des demandes dans la nouvelle expérience de demande

Vous pouvez copier et envoyer des requêtes dans la zone des Requêtes de Workfront, ou à partir du widget Mes requêtes dans l’Accueil.

{{step1-to-requests}}

1. Pour accéder au widget Mes requêtes dans l’Accueil :

   {{step1-to-home}}

   1. Recherchez le widget Mes requêtes .

      Pour plus d’informations sur le widget Mes requêtes, voir [Utiliser le widget Mes requêtes](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Dans la liste des Demandes ou le widget Mes demandes , placez le pointeur de la souris sur la demande à copier.

   Un menu Plus à trois points s’affiche.
   ![](assets/more-menu.png)

1. Cliquez sur le menu **Plus** à droite du nom de la requête, puis cliquez sur **Copier**.

   Ou

   Cliquez avec le bouton droit sur la demande sélectionnée, puis cliquez sur **Copier**.

   >[!TIP]
   >
   >Lorsque vous n’avez pas accès à la création des problèmes, vous recevez un avertissement indiquant que votre administrateur ou administratrice vous a interdit de créer des demandes.

1. (Facultatif) Mettez à jour les informations de la demande copiée. Les champs disponibles dépendent de la file d’attente des demandes ou du formulaire de demande utilisé pour la demande.

   Lorsque vous saisissez ou modifiez des valeurs de champ dans la demande copiée, elle est enregistrée en tant que brouillon.

1. Cliquez sur **Soumettre**.

   La demande copiée est envoyée en tant que nouvelle demande.

</div>

