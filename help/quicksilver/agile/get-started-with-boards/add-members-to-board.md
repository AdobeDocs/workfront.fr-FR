---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Ajout ou suppression de membres d’un panorama
description: Les personnes doivent être ajoutées au panorama en tant que membres avant de pouvoir l’afficher et d’être affectées aux cartes.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 24%

---

# Ajouter ou supprimer des personnes membres d’un panorama

Les personnes et les équipes doivent être ajoutées au panorama en tant que membres avant de pouvoir l’afficher.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> 
   <p>Nouvelle : [!UICONTROL Contributor] ou niveau supérieur</p> 
   <p>ou</p>
   <p>Actuel : [!UICONTROL Request] ou supérieure</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajout de membres à un panorama

{{step1-to-boards}}

1. Créez un panorama ou modifiez un panorama existant. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur l&#39;icône **[!UICONTROL Ajouter un membre]** ![Ajouter des membres](assets/boards-addmember-spectrum-25x25.png).
1. Dans la zone **[!UICONTROL Ajouter des membres]**, commencez à saisir un nom, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   Vous pouvez sélectionner un membre individuel ou une équipe. Si vous choisissez une équipe, celle-ci est ajoutée au panorama.

   >[!NOTE]
   >
   >Un utilisateur individuel doit avoir l’option **[!UICONTROL Afficher]** ou **[!UICONTROL Modifier]** définie dans son niveau d’accès pour les équipes, sinon il ne pourra pas afficher le panorama.


   ![Ajouter des membres au panorama](assets/boards-add-members.png)

## Suppression de membres d’un panorama

{{step1-to-boards}}

1. Créez un panorama ou modifiez un panorama existant. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur l&#39;icône **[!UICONTROL Ajouter un membre]** ![Ajouter des membres](assets/boards-addmember-spectrum-25x25.png).
1. Dans la zone **[!UICONTROL Ajouter des membres]**, cliquez sur le X en regard du nom d’une personne ou d’une équipe pour les supprimer du panorama.

   ![Supprimer un membre du panorama](assets/boards-remove-member-from-board-350x367.png)

   Lorsque vous supprimez un membre d’un panorama, il n’est supprimé d’aucune carte à laquelle il est affecté. Pour les cartes connectées, les affectations sont également mises à jour sur la tâche [!DNL Workfront] ou le problème.

   Les membres ne sont supprimés de ce panorama que. Ils ne sont pas supprimés des autres panoramas auxquels ils appartiennent.

   >[!NOTE]
   >
   >Vous ne pouvez pas supprimer le propriétaire du panorama.
