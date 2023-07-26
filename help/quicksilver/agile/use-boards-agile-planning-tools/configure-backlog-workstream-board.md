---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configuration du journal en souffrance sur un panorama de flux de travail
description: Vous pouvez choisir d’afficher une colonne de journal sur un panorama dans un flux de travail et de définir une requête pour les cartes qui sont extraites dans le journal du panorama depuis la liste des cartes du flux de travail.
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Configuration du journal en souffrance sur un panorama de flux de travail

Vous pouvez choisir d’afficher une colonne de journal sur un panorama dans un flux de travail et de définir une requête pour les cartes qui sont extraites dans le journal du panorama depuis la liste des cartes du flux de travail.

>[!NOTE]
>
>Si vous ajoutez une nouvelle carte dans la colonne des logs d&#39;attente qui ne correspond pas aux critères de requête, la carte disparaîtra du journal lors de l&#39;actualisation du panorama et elle ne sera disponible que dans la liste des cartes. Vous pouvez à tout moment modifier la requête pour ajuster les cartes qui apparaissent dans la colonne de journal.

La colonne et la requête du journal en souffrance ne sont pas disponibles sur les panoramas autonomes. Pour plus d’informations sur l’ajout d’une colonne d’entrée à un panorama autonome, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

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

   >[!NOTE]
   >
   >Une requête par défaut peut déjà être appliquée au journal, indiquant toutes les tâches de la liste des cartes ayant un état et dont l’état n’est pas Terminé.

1. Cliquez sur [!UICONTROL **Ajouter une condition**] et cliquez dans le champ &quot;vide&quot;.
1. Sélectionnez le champ sur lequel effectuer la requête.

   Les champs que vous pouvez choisir sont les champs par défaut d’une carte.

1. Sélectionnez le modificateur de requête.

   Les options de modificateur dépendent des champs auxquels elles peuvent s’appliquer. Par exemple, le champ &quot;name&quot; ne comporte pas &quot;supérieur à&quot; ou &quot;inférieur à&quot; comme choix de modificateur, car ces modificateurs s’appliquent uniquement aux nombres.

1. Sélectionnez la valeur.

   La valeur n’est pas disponible lorsque vous utilisez &quot;exists&quot; ou &quot;not exists&quot; comme modificateur.

   Par exemple, si vous sélectionnez &quot;Date d’échéance&quot; et &quot;existe&quot;, le journal affiche les cartes avec des dates d’échéance désignées. Les cartes sans date d’échéance ne sont pas extraites dans le journal.

1. (Facultatif) Cliquez sur [!UICONTROL **Ajouter une condition**] pour ajouter une autre condition à la requête.

   ![Requête de liste d’attente](assets/backlog-query-wrkstrm-board.png)

1. (Facultatif) Cliquez sur [!UICONTROL **Créer un groupe**] pour ajouter un groupe de conditions liées à la première condition avec un opérateur OU.
1. Cliquez sur [!UICONTROL **Enregistrer la requête**].

   La requête est appliquée et les cartes répondant aux critères apparaissent dans la colonne des logs d&#39;attente.
