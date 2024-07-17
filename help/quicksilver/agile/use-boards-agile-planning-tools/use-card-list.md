---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Utiliser la liste des cartes
description: Vous pouvez créer une liste de cartes sur un workflow et ajouter les cartes aux itérations.
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: d44eb048103e469bc072cc5287947fea471668b3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 6%

---

# Utiliser la liste des cartes

>[!IMPORTANT]
>
>Les flux de travail ne sont pas disponibles pour tous les clients.

Vous pouvez créer une liste de cartes sur un workflow et ajouter les cartes aux itérations.

La liste de cartes peut fonctionner comme un journal de travail en retard pour le flux de travail.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ajout de cartes à la liste

{{step1-to-boards}}

1. Pour ouvrir un workflow, cliquez sur [!UICONTROL **Afficher le workflow**].
1. Cliquez sur l’onglet [!UICONTROL **Liste de cartes**] .
1. Cliquez sur [!UICONTROL **Ajouter une carte**].
1. Dans la boîte de dialogue [!UICONTROL **Créer/Modifier la carte**], ajoutez les informations suivantes :

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>Nom de la carte.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Description]</strong></td> 
      <td>Description de la carte.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimation]</strong></td> 
      <td>Nombre estimé d’heures pour la carte à remplir. Il s’agit d’une entrée manuelle uniquement.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Sélectionnez l’état de la carte.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Itérations]</strong></td> 
      <td>Sélectionnez une itération à laquelle attribuer la carte.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Assigents]</strong></td> 
      <td><p>Pour attribuer la carte, commencez à saisir un nom dans le champ de recherche, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Vous pouvez ajouter des individus et des équipes et affecter plusieurs personnes ou équipes à une carte.</p><p>Les personnes désignées doivent être membres du workflow ou elles n’apparaîtront pas dans la liste de sélection.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Cliquer sur [!UICONTROL **Enregistrer**].
1. Continuez à ajouter des cartes jusqu’à ce que vous ayez créé la liste des cartes.

## Afficher les cartes

Pour afficher toutes les cartes du flux de travail dans une seule liste, cliquez sur [!UICONTROL **Mode Liste**] dans l’onglet Liste de cartes.

Pour afficher toutes les cartes du workflow regroupées par itération, cliquez sur [!UICONTROL **Iteration view**]. Les cartes non planifiées s’affichent dans leur propre groupe.

Pour modifier une carte existante, sélectionnez-la dans la liste et cliquez sur [!UICONTROL **Modifier**].

Pour supprimer une carte, sélectionnez-la dans la liste et cliquez sur [!UICONTROL **Supprimer**].

### Filtrer les cartes

Les cartes ne peuvent être archivées que depuis la carte d’itération. Lorsqu’une carte est archivée, elle n’est pas affichée dans la liste des cartes, sauf si vous filtrez pour afficher les cartes archivées. Pour plus d’informations sur l’archivage d’une carte, voir [Suppression ou archivage d’une carte à partir d’un panorama](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Accédez à la liste des cartes du flux de travail.
1. Cliquez sur [!UICONTROL **Filtrer**] et sélectionnez [!UICONTROL **Toutes**], [!UICONTROL **Cartes actives**] ou [!UICONTROL **Cartes archivées**].

   Lorsqu’un filtre autre que le filtre par défaut est appliqué sur la liste des cartes, un indicateur s’affiche sur l’icône de filtre ![Filtre appliqué](assets/boards-filterapplied-30x30.png).

### Recherche dans la liste des cartes

1. Accédez à la liste des cartes du flux de travail.
1. Cliquez sur [!UICONTROL **Rechercher**] et saisissez un terme de recherche. Ensuite, appuyez sur Entrée.

   Toutes les cartes qui contiennent le terme de recherche s’affichent.
Cliquez sur le X pour effacer la recherche.

   ![Recherche de cartes dans un panorama](assets/boards-searchbox.png)

## Ajout de cartes à une itération

>[!NOTE]
>
>Vous devez créer une itération avant de pouvoir y ajouter des cartes. Pour plus d’informations, voir [Création d’une itération dans un workflow](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Accédez à la liste des cartes du flux de travail.
1. Sélectionnez la [!UICONTROL **vue Itération**] pour voir les cartes qui sont affectées à une itération et celles qui ne sont pas planifiées.
1. Sélectionnez une carte non planifiée dans la liste et cliquez sur [!UICONTROL **Modifier**].
1. Sélectionnez une itération dans le champ [!UICONTROL **Itérations**] .
1. Si vous utilisez des points d’article, saisissez une valeur dans le champ [!UICONTROL **Estimation**] .
1. Cliquer sur [!UICONTROL **Enregistrer**].

   La carte est déplacée vers l’itération et les mesures d’itération reflètent le nombre de cartes et de points.

   Vous pouvez également faire glisser et déposer une carte du groupe Cartes non planifiées dans l’itération, ou cliquer sur [!UICONTROL **Ajouter une carte**] pour ajouter une nouvelle carte à l’itération.

>[!TIP]
>
>Si vous avez créé une carte de processus d’itération, toutes les cartes non planifiées de la liste de cartes apparaissent dans la colonne [!UICONTROL Backlog]. Lorsqu’une carte est déplacée dans une autre colonne, elle fait partie de l’itération active. Les cartes que vous ajoutez à l’itération dans la liste des cartes sont ajoutées à une colonne en fonction de leur état.
