---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Désactiver ou supprimer une équipe
description: Vous pouvez désactiver les équipes que vous n’utilisez plus tout en conservant les données historiques associées. Les administrateurs et administratrices d’Adobe Workfront peuvent réactiver une équipe à tout moment à partir de la zone Équipes dans Configuration.
author: Jenny
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 68%

---

# Désactiver ou supprimer une équipe

Vous pouvez désactiver les équipes que vous n’utilisez plus tout en conservant les données historiques associées. Les administrateurs et administratrices d’[!DNL Adobe Workfront] peuvent réactiver une équipe à tout moment à partir de la zone Équipes de Configuration. Si vous désactivez une équipe, celle-ci ne s’affiche plus dans les zones suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Champs de saisie semi-automatique dans les formulaires personnalisés</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Boîte de dialogue de partage des objets</p> </li> 
     <li> <p>[!UICONTROL User Profile]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Menu déroulant de la sélection principale dans la zone [!UICONTROL Teams].</p> </li> 
     <li> <p>Saisie semi-automatique pour [!UICONTROL Assignments]</p> </li> 
     <li> <p>Boîte de dialogue du tableau [!UICONTROL Add to Kanban] dans un projet</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Les équipes désactivées n’apparaissent pas lorsque vous recherchez une équipe, mais s’affichent toujours dans [!UICONTROL &#x200B; Équipe interne &#x200B;] et Autres équipes si l’utilisateur a été affecté à l’équipe avant la désactivation.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Package Adobe Workfront</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr>
   <td>Configurations des niveaux d’accès</td>
   <td><p>Pour désactiver une équipe, aucune configuration n'est nécessaire.</p>
   <p>Pour supprimer une équipe, vous devez être administrateur système.</p></td>
  </tr>
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Désactiver une équipe

Tout travail affecté à l’équipe avant la désactivation reste assigné. Nous vous recommandons de réaffecter le travail avant de désactiver l’équipe.

>[!TIP]
>
>Vous pouvez créer un rapport pour filtrer les tâches ou les problèmes auxquels l’équipe désactivée est encore affectée.

Lorsque vous utilisez des files d’attente de demandes, si vous désactivez une équipe affectée comme équipe par défaut dans une règle de transmission, l’équipe est maintenue et les demandes sont toujours acheminées vers l’équipe désactivée. Nous vous recommandons de mettre à jour les règles de transmission avec des équipes actives avant de désactiver l’équipe.

{{step1-to-team}}

1. Cliquez sur l’icône **[!DNL Switch team]**, puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Modifier]**.

   ![](assets/edit-team-settings.png)

1. Désélectionnez la case **[!UICONTROL Est actif]** dans les paramètres de l’équipe.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Limites connues de la désactivation d’une équipe

Les équipes désactivées s’affichent dans les zones suivantes :

* Le champ Personne propriétaire dans [!DNL Workfront Goals]. Cela nécessite une licence supplémentaire pour [!DNL Adobe Workfront Goals]. Pour plus d’informations, consultez [Commencer avec  [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Supprimer une équipe

Seul un administrateur système peut supprimer une équipe. Si vous êtes le propriétaire d&#39;une équipe (mais pas un administrateur) et que vous essayez de supprimer une équipe, un message d&#39;erreur s&#39;affiche.

Pour supprimer une équipe :

{{step1-to-team}}

1. Cliquez sur l’icône **[!DNL Switch team]**, puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Supprimer]**.

   ![](assets/edit-team-settings.png)

1. Cliquez sur [!UICONTROL **Confirmer**] dans le message de confirmation pour supprimer définitivement l’équipe. Les équipes supprimées ne peuvent pas être récupérées.
