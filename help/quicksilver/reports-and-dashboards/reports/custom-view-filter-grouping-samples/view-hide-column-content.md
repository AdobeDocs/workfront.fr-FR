---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : masquer le contenu d’une colonne'
description: Vous pouvez masquer les informations dans la colonne d’une vue. Pour ce faire, modifiez le mode texte de la colonne.
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 76%

---

# Vue : masquer le contenu d’une colonne

<!--Audited: 11/2024-->

Vous pouvez masquer les informations dans la colonne d’une vue. Pour ce faire, modifiez le mode texte de la colonne.

>[!NOTE]
>
>* Vous pouvez utiliser des colonnes masquées pour trier selon un certain objet que vous ne souhaitez pas afficher dans la vue.\
>  Par exemple, vous pouvez trier par numéro de tâche dans une vue de tâche et masquer le numéro de tâche. Dans ce cas, l’objet référencé dans la colonne permet de trier la vue, mais les informations de cet objet ne s’affichent pas dans la vue.
>* Lorsque vous masquez une colonne, notez que les informations qu’elle contient sont masquées, mais que la colonne existe toujours dans la vue.

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
   <p>Contributeur ou demande de modification d’une vue </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Exemple : triez et masquez la colonne Numéro de tâche dans une vue de tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne** et commencez à saisir « Numéro de la tâche » dans le champ **Afficher dans cette colonne** puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Cliquez sur **Basculer en mode texte**, puis **Modifier le mode texte**.
1. Supprimez le texte de la zone **Modifier le mode texte** et remplacez-le par le code suivant :

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   Les modifications importantes apportées à ce code pour masquer la colonne sont les suivantes :

   * `displayname=` : cette ligne doit être vide.
   * `valuefield=` : cette ligne doit être remplacée par `value=`, qui doit être vide.
   * `width=` : selon le champ, la valeur doit être **0** ou **1**.

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.
