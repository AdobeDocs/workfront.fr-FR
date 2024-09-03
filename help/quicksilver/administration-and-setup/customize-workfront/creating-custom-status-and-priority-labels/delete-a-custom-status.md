---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Suppression d’un état personnalisé
description: Vous pouvez supprimer un statut système personnalisé s’il n’est plus utile à votre organisation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 99%

---

# Modifier un statut personnalisé

Vous pouvez supprimer un statut système personnalisé s’il n’est plus utile à votre organisation.

Le fait que le statut soit verrouillé ou déverrouillé détermine s’il est supprimé pour tous les groupes du système :

* Lorsque vous supprimez un statut système actuellement verrouillé, celui-ci est supprimé pour tous les groupes du système, qu’ils aient été renommés ou non.
* À l’inverse, lorsque vous supprimez un statut système actuellement déverrouillé, celui-ci est conservé pour tous les groupes du système.


>[!NOTE]
>
>Vous ne pouvez pas supprimer les éléments suivants :
>
>* Statut système verrouillé ou déverrouillé utilisé dans un processus d’approbation système en attente d’approbation pour au moins un objet de votre système.
>
>  Cependant, vous pouvez supprimer un statut système déverrouillé utilisé dans un processus d’approbation à usage unique ou au niveau d’un groupe qui est en attente d’approbation.
>
>  Vous pouvez exécuter un rapport pour rechercher les objets et résoudre les approbations en attente, puis réessayer de supprimer le statut. Pour obtenir des instructions, voir la section [Lister des objets dont l’approbation est en attente avec un certain statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Statuts utilisés dans les processus d’approbation en attente d’approbation pour au moins un objet de votre système.

Pour plus d’informations sur la suppression d’un statut de groupe, voir la section [Supprimer un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Supprimer un statut système personnalisé

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Préférences du projet** > **Statuts**.

1. Pour supprimer le statut de l’ensemble du système (y compris pour les groupes individuels), placez le pointeur de la souris dessus, cliquez sur **Modifier**, puis assurez-vous que l’option **Verrouiller pour tous les groupes** est sélectionnée. Cliquer sur **Enregistrer**.

   Ou

   Pour supprimer le statut système, mais le conserver pour des groupes spécifiques, placez le pointeur de la souris dessus, cliquez sur **Modifier**, puis assurez-vous que l’option **Verrouiller pour tous les groupes** n’est pas sélectionnée. Cliquer sur **Enregistrer**.

1. Pointez sur le statut que vous souhaitez supprimer, puis cliquez sur **Supprimer**.
1. Dans le message qui apparaît, cliquez sur **Supprimer le statut**.
1. Dans la zone **Supprimer le statut** qui s’affiche, sélectionnez un statut dans le champ intitulé **Définir tous les projets ayant actuellement ce statut sur**.

   Les projets qui utilisaient le statut que vous supprimez sont définis sur celui que vous sélectionnez.

   Les statuts ne sont disponibles dans la liste déroulante que s’ils correspondent au même statut que celui que vous supprimez.

   Par exemple, si vous supprimez un statut qui correspond à Actuel, seuls les statuts correspondant également à Actuel peuvent être sélectionnés.

1. Cliquez sur **Supprimer le statut**.
