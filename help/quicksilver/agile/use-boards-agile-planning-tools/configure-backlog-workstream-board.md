---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configuration du journal en souffrance sur un panorama de flux de travail
description: Vous pouvez choisir d’afficher une colonne de journal sur un panorama dans un flux de travail et de définir une requête pour les cartes qui sont extraites dans le journal du panorama depuis la liste des cartes du flux de travail.
author: Lisa
source-git-commit: b58831d50c2be421c666515808091aa4863bb471
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 1%

---

# Configuration du journal en souffrance sur un panorama de flux de travail

Vous pouvez choisir d’afficher une colonne de journal sur un panorama dans un flux de travail et de définir une requête pour les cartes qui sont extraites dans le journal du panorama depuis la liste des cartes du flux de travail. Ces options ne sont pas disponibles sur les panoramas autonomes. Pour plus d’informations sur l’ajout d’une colonne d’entrée à un panorama autonome, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Configuration du journal en souffrance sur un panorama de flux de travail

{{step1-to-boards}}

1. Ouvrez le workflow dans lequel vous souhaitez travailler. Pour ouvrir un workflow, cliquez sur [!UICONTROL **Afficher le flux de travail**].
1. Cliquez sur n’importe quel panorama du processus pour l’ouvrir.
1. Cliquez sur [!UICONTROL **Configurer**] à droite du panorama pour ouvrir le panneau Configurer .
1. Activer [!UICONTROL **Inclure une colonne de journal sur ce panorama**].

   La colonne &quot;journal des travaux&quot; est ajoutée à gauche du panorama. Il reste vide jusqu’à ce que vous lui appliquiez une requête.

1. Développer [!UICONTROL **Requête de journal**].
1. Cliquez sur [!UICONTROL **Ajouter une condition**] et cliquez dans le champ &quot;vide&quot;.
1. Sélectionnez le champ sur lequel effectuer la requête.

   Les champs que vous pouvez choisir sont les champs par défaut d’une carte.

1. Sélectionnez le modificateur de requête.

   Les options sont les suivantes : est égal à, n’est pas égal à, existe et n’existe pas.

   Exemple : Si vous choisissez Échéance et existe, le journal affiche les cartes avec des dates d’échéance désignées. Les cartes sans date d’échéance ne sont pas extraites dans le journal.

1. Sélectionnez la valeur.

   La valeur n’est disponible que si vous utilisez equals ou non comme modificateur.

1. (Facultatif) Cliquez sur [!UICONTROL **Ajouter une condition**] pour ajouter une autre condition à la requête.

   ![Requête de liste d’attente](assets/backlog-query-wrkstrm-board.png)

1. (Facultatif) Cliquez sur [!UICONTROL **Créer un groupe**] pour ajouter un groupe de conditions liées à la première condition avec un opérateur OU.
1. Cliquez sur [!UICONTROL **Enregistrer la requête**].

   La requête est appliquée et les cartes répondant aux critères apparaissent dans la colonne des logs d&#39;attente.
