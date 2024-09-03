---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Utilisation de la liste de cartes
description: Vous pouvez créer une liste de cartes sur un flux de travail et ajouter les cartes aux itérations.
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 99%

---

# Utiliser la liste des cartes

>[!IMPORTANT]
>
>Les flux de travail ne sont pas disponibles pour toute la clientèle.

Vous pouvez créer une liste de cartes sur un flux de travail et ajouter les cartes aux itérations.

La liste des cartes peut servir de liste d’attente des travaux pour le flux de travail.

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

## Ajouter des cartes à la liste des cartes

{{step1-to-boards}}

1. Pour ouvrir un flux de travail, cliquez sur [!UICONTROL **Afficher le flux de travail**].
1. Cliquez sur l’onglet [!UICONTROL **Liste des cartes**].
1. Cliquez sur [!UICONTROL **Ajouter une carte**].
1. Dans la boîte de dialogue [!UICONTROL **Créer/Modifier une carte**], ajoutez les informations suivantes :

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
      <td>Le nombre d’heures estimé pour la réalisation de la carte. L’entrée ne peut être que manuelle.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>Sélectionnez le statut de la carte.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterations]</strong></td> 
      <td>Sélectionnez une itération à laquelle attribuer la carte.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Assignees]</strong></td> 
      <td><p>Pour attribuer la carte, commencez à saisir un nom dans le champ de recherche, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Vous pouvez ajouter des personnes et des équipes ainsi qu’en affecter plusieurs à une carte.</p><p>Les personnes cessionnaires doivent être membres du flux de travail ou elles n’apparaîtront pas dans la liste de sélection.</p></td> 
     </tr>
    </tbody> 
   </table>

1. Cliquer sur [!UICONTROL **Enregistrer**].
1. Continuez à ajouter des cartes jusqu’à ce que vous ayez créé la liste des cartes.

## Afficher les cartes

Pour afficher toutes les cartes du flux de travail dans une seule liste, cliquez sur [!UICONTROL **Vue Liste**] dans l’onglet Liste des cartes.

Pour afficher toutes les cartes du flux de travail regroupées par itération, cliquez sur [!UICONTROL **Vue Itération**]. Les cartes non prévues s’affichent dans leur propre groupe.

Pour modifier une carte existante, sélectionnez-la dans la liste, puis cliquez sur [!UICONTROL **Modifier**].

Pour supprimer une carte, sélectionnez-la dans la liste, puis cliquez sur [!UICONTROL **Supprimer**].

### Filtrer les cartes

Les cartes ne peuvent être archivées qu’à partir du panorama d’itération. Lorsqu’une carte est archivée, elle n’est pas affichée dans la liste des cartes, sauf si vous filtrez pour afficher les cartes archivées. Pour plus d’informations sur l’archivage d’une carte, voir [Supprimer ou archiver une carte d’un panorama](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. Accédez à la liste des cartes du flux de travail.
1. Cliquez sur [!UICONTROL **Filtrer**] et sélectionnez [!UICONTROL **Toutes**], [!UICONTROL **Cartes actives**], ou [!UICONTROL **Cartes archivées**].

   Lorsqu’un filtre autre que celui par défaut est appliqué sur la liste des cartes, un indicateur s’affiche sur l’icône de filtre ![Filtre appliqué](assets/boards-filterapplied-30x30.png).

### Rechercher dans la liste des cartes

1. Accédez à la liste des cartes du flux de travail.
1. Cliquez sur [!UICONTROL **Rechercher**] et saisissez un terme de recherche. Appuyez ensuite sur Entrée.

   Toutes les cartes qui contiennent le terme de recherche s’affichent.
Cliquez sur le X pour effacer la recherche.

   ![Rechercher des cartes dans un panorama](assets/boards-searchbox.png)

## Ajouter des cartes à une itération

>[!NOTE]
>
>Vous devez créer une itération avant de pouvoir y ajouter des cartes. Pour plus d’informations, voir [Créer une itération dans un flux de travail](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Accédez à la liste des cartes du flux de travail.
1. Sélectionnez la [!UICONTROL **Vue Itération**] pour voir quelles cartes sont affectées à une itération et lesquelles ne sont pas prévues.
1. Sélectionnez une carte non prévue dans la liste et cliquez sur [!UICONTROL **Modifier**].
1. Sélectionnez une itération dans le champ [!UICONTROL **Itérations**].
1. Si vous utilisez des points de l’histoire, saisissez une valeur dans le champ [!UICONTROL **Estimation**].
1. Cliquer sur [!UICONTROL **Enregistrer**].

   La carte est déplacée vers l’itération et les mesures d’itération reflètent le nombre de cartes et de points.

   Vous pouvez également faire glisser et déposer une carte à partir du groupe Cartes non prévues dans l’itération, ou cliquer sur [!UICONTROL **Ajouter une carte**] pour ajouter une nouvelle carte à l’itération.

>[!TIP]
>
>Si vous avez créé un panorama de processus d’itération, toutes les cartes non prévues de la liste apparaissent dans la colonne [!UICONTROL Liste d’attente]. Lorsqu’une carte est déplacée dans une autre colonne, elle fait partie de l’itération active. Les cartes que vous ajoutez à l’itération dans la liste des cartes sont ajoutées à une colonne en fonction de leur statut.
