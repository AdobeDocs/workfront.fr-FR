---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Ajouter ou supprimer des membres d’un panorama
description: Les personnes doivent être ajoutées au panorama en tant que membres avant qu’elles ne puissent afficher le panorame et être affectées aux cartes.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: 03768a0d3a63c7f6adcd11a6cd2e4d093b24f214
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 63%

---

# Ajouter ou supprimer des membres d’un panorama

Les personnes et les équipes doivent être ajoutées au panorama en tant que membres avant qu’elles ne puissent afficher le panorama.

Le créateur d’un panorama en est le propriétaire par défaut. Le propriétaire du panorama est la seule personne qui peut supprimer ce panorama ou mettre à jour ses filtres dans le panneau Configurer. Seul un administrateur système ou le propriétaire actuel du panorama peut changer de propriétaire.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> 
   <p>Nouvelle : [!UICONTROL Contributor] ou niveau supérieur</p> 
   <p>ou</p>
   <p>Actuelle : [!UICONTROL Request] ou supérieure</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter des personnes membres à un panorama

{{step1-to-boards}}

1. Créez un panorama ou modifiez un panorama existant. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur l’icône **[!UICONTROL Ajouter une personne membre]** ![Ajouter des personnes membres](assets/boards-addmember-spectrum-25x25.png).
1. Dans la zone **[!UICONTROL Ajouter des personnes membres]**, commencez à saisir un nom, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   Vous pouvez sélectionner une personne membre individuelle ou une équipe. Si vous choisissez une équipe, celle-ci est ajoutée au panorama.

   >[!NOTE]
   >
   >Une personne individuelle doit avoir l’option **[!UICONTROL Afficher]** ou **[!UICONTROL Modifier]** définie dans son niveau d’accès pour les équipes, sinon elle ne pourra pas afficher le panorama.


   ![Ajout de personnes membres au panorama](assets/boards-add-members.png)

## Supprimer des personnes membres d’un panorama

{{step1-to-boards}}

1. Créez un panorama ou modifiez un panorama existant. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur l’icône **[!UICONTROL Ajouter une personne membre]** ![Ajouter des personnes membres](assets/boards-addmember-spectrum-25x25.png).
1. Dans la zone **[!UICONTROL Ajouter des personnes membres]**, cliquez sur le X en regard du nom d’une personne ou d’une équipe pour la supprimer du panorama.

   ![Suppression d’une personne membre du panorama](assets/boards-remove-member-from-board-350x367.png)

   Lorsque vous supprimez une personne membre d’un panorama, elle n’est supprimée d’aucune carte à laquelle elle est affectée. Pour les cartes connectées, les affectations sont également mises à jour dans la tâche ou le problème [!DNL Workfront].

   Les personnes membres ne sont supprimées que de ce panorama. Elles ne sont pas supprimées des autres panoramas auxquels elles appartiennent.

   >[!NOTE]
   >
   >Vous ne pouvez pas supprimer la personne propriétaire du panorama.

## Modifier le propriétaire du panorama

>[!NOTE]
>
>Seul un administrateur système ou le propriétaire actuel du panorama peut changer de propriétaire. Un panorama ne peut avoir qu’un seul propriétaire.
>
>La possibilité de changer le propriétaire du panorama est disponible sur les panoramas de base, rétrospectifs et kanban, mais pas sur les panoramas dynamiques.

1. Accédez au panorama.
1. Cliquez sur le menu **[!UICONTROL Plus]** ![Plus](assets/more-icon-spectrum.png) en regard du nom du panorama, puis choisissez **[!UICONTROL Modifier le propriétaire du panorama]**.
1. Dans la boîte de dialogue Modifier le propriétaire du panorama , recherchez et sélectionnez l’utilisateur dont vous souhaitez faire le propriétaire.

   Vous ne pouvez pas rechercher des utilisateurs qui sont déjà membres du panorama. Pour qu’un membre existant devienne le propriétaire, vous devez d’abord le supprimer du panorama. Le fait de définir un utilisateur comme propriétaire du panorama permet de l’ajouter au panorama.

   Seul un utilisateur peut être le propriétaire du panorama. Une équipe ne peut pas être propriétaire.

1. Cliquez sur [!UICONTROL **Mettre à jour**].
