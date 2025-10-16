---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configurer la liste d’attente sur un tableau de flux de travail
description: Vous pouvez choisir d’afficher une colonne de liste d’attente sur un panorama dans un flux de travail et définir une requête pour les cartes qui sont ajoutées à la liste d’attente du panorama depuis la liste des cartes du flux de travail.
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 97%

---

# Configurer la liste d’attente sur un panorama de flux de travail

>[!IMPORTANT]
>
>Les flux de travail ne sont disponibles que pour un groupe spécifique de clientes et de clients.

Vous pouvez choisir d’afficher une colonne de liste d’attente sur un panorama dans un flux de travail et définir une requête pour les cartes qui sont ajoutées à la liste d’attente du panorama depuis la liste des cartes du flux de travail.

>[!NOTE]
>
>Si vous ajoutez une nouvelle carte dans la colonne de liste d’attente qui ne correspond pas aux critères de requête, la carte disparaîtra de la liste d’attente lors de l’actualisation du panorama et elle ne sera disponible que dans la liste des cartes. Vous pouvez à tout moment modifier la requête pour ajuster les cartes qui apparaissent dans la colonne de liste d’attente.

La colonne de liste d’attente et la requête ne sont pas disponibles sur les panoramas autonomes. Pour plus d’informations sur l’ajout d’une colonne de saisie à un panorama autonome, voir [Ajouter une colonne de saisie à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou version ultérieure</p> 
   <p>Requête ou supérieure</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer la liste d’attente sur un panorama de flux de travail

{{step1-to-boards}}

1. Ouvrez le flux de travail dans lequel vous souhaitez travailler. Pour ouvrir un flux de travail, cliquez sur [!UICONTROL **Afficher le flux de travail**].
1. Cliquez sur n’importe quel panorama du flux de travail pour l’ouvrir.
1. Cliquez sur [!UICONTROL **Configurer**] à droite du panorama pour ouvrir le panneau Configurer.
1. Activez [!UICONTROL **Inclure une colonne de liste d’attente sur ce panorama**].

   La colonne de liste d’attente est ajoutée à gauche du panorama. Elle reste vide jusqu’à ce que vous lui appliquiez une requête.

1. Développez [!UICONTROL **Requête de liste d’attente**].

   >[!NOTE]
   >
   >Une requête par défaut peut déjà être appliquée à la liste d’attente, indiquant tous les éléments de travail de la liste des cartes ayant un statut et dont le statut n’est pas Terminé.

1. Cliquez sur [!UICONTROL **Ajouter une condition**] et cliquez dans le champ « vide ».
1. Sélectionnez le champ sur lequel effectuer la requête.

   Les champs que vous pouvez choisir sont les champs par défaut d’une carte.

1. Sélectionnez le modificateur de requête.

   Les options du modificateur dépendent des champs auxquels ils peuvent s’appliquer. Par exemple, le champ « nom » n’accepte pas « supérieur à » ou « inférieur à » comme choix de modificateur, car ces modificateurs s’appliquent uniquement aux nombres.

1. Sélectionnez la valeur.

   La valeur n’est pas disponible lorsque vous utilisez « existe » ou « n’existe pas » comme modificateur.

   Par exemple, si vous sélectionnez « Date d’échéance » et « existe », la liste d’attente affiche les cartes avec des dates d’échéance assignées. Les cartes sans date d’échéance ne sont pas ajoutées à la file d’attente.

1. (Facultatif) Cliquez sur [!UICONTROL **Ajouter une condition**] pour ajouter une autre condition à la requête.

   ![Requête de liste d’attente](assets/backlog-query-wrkstrm-board.png)

1. (Facultatif) Cliquez sur [!UICONTROL **Créer un groupe**] pour ajouter un groupe de conditions liées à la première condition avec un opérateur OU.
1. Cliquez sur [!UICONTROL **Enregistrer la requête**].

   La requête est appliquée et les cartes répondant aux critères apparaissent dans la colonne de file d’attente.
