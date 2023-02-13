---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Suppression d’un état personnalisé
description: Vous pouvez supprimer un état système personnalisé s’il n’est plus utile à votre entreprise.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# Suppression d’un état personnalisé

Vous pouvez supprimer un état système personnalisé s’il n’est plus utile à votre entreprise.

Le statut est verrouillé ou déverrouillé détermine si l’état est supprimé pour tous les groupes du système :

* Lorsque vous supprimez un état système actuellement verrouillé, il est supprimé pour tous les groupes du système, qu’ils aient été renommés ou non.
* A l’inverse, lorsque vous supprimez un état système actuellement déverrouillé, l’état est conservé pour tous les groupes du système.


>[!NOTE]
>
>Vous ne pouvez pas supprimer les éléments suivants :
>
>* État du système verrouillé ou déverrouillé utilisé dans un processus d’approbation du système en attente d’approbation pour au moins un objet de votre système.
>
>  Cependant, vous pouvez supprimer un état système déverrouillé utilisé dans un processus d’approbation unique ou au niveau d’un groupe en attente d’approbation.
>
>  Vous pouvez exécuter un rapport pour rechercher les objets et résoudre les validations en attente, puis réessayer de supprimer le statut. Pour obtenir des instructions, voir [Liste des objets dont le traitement de validation est en attente avec un certain état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Statuts utilisés dans les processus d’approbation en attente d’approbation pour au moins un objet de votre système.


Pour plus d’informations sur la suppression d’un état de groupe, voir [Suppression d’un état de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Suppression d’un état de système personnalisé

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Préférences du projet** > **Statuts**.

1. Pour supprimer l’état sur l’ensemble du système (y compris pour les groupes individuels), placez le pointeur de la souris sur l’état, cliquez sur **Modifier**, puis assurez-vous que **Verrouillage de tous les groupes** est sélectionnée. Cliquer sur **Enregistrer**.

   Ou

   Pour supprimer l’état du système, mais le conserver pour des groupes spécifiques, placez le pointeur de la souris sur l’état, cliquez sur **Modifier**, puis assurez-vous que **Verrouillage de tous les groupes** n’est pas sélectionnée. Cliquer sur **Enregistrer**.

1. Pointez sur l’état que vous souhaitez supprimer, puis cliquez sur **Supprimer**.
1. Dans le message qui s’affiche, cliquez sur **État de la suppression**.
1. Dans le **État de la suppression** qui s’affiche, sélectionnez un état dans le champ intitulé **Définissez tous les projets actuellement avec cet état sur**.

   Les projets qui utilisaient le statut que vous supprimez sont définis sur celui que vous sélectionnez.

   Les états ne sont disponibles dans la liste déroulante que s’ils correspondent au même état que celui que vous supprimez.

   Par exemple, si vous supprimez un état qui correspond à Actuel, seuls les états qui correspondent également à Actuel peuvent être sélectionnés.

1. Cliquez sur **État de la suppression**.
