---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Afficher : masquer le contenu d’une colonne"
description: Vous pouvez masquer les informations dans la colonne d’une vue. Pour ce faire, modifiez le mode texte de la colonne.
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 82%

---

# Vue : masquer le contenu d’une colonne

<!--Audited: 11/2024-->

Vous pouvez masquer les informations dans la colonne d’une vue. Pour ce faire, modifiez le mode texte de la colonne.

>[!NOTE]
>
>* Vous pouvez utiliser des colonnes masquées pour trier selon un certain objet que vous ne souhaitez pas afficher dans la vue.\
>  Par exemple, vous pouvez trier par numéro de tâche dans une vue de tâche et masquer le numéro de tâche. Dans ce cas, l’objet référencé dans la colonne permet de trier la vue, mais les informations de cet objet ne s’affichent pas dans la vue.
>* Lorsque vous masquez une colonne, notez que les informations qu’elle contient sont masquées, mais que la colonne existe toujours dans la vue.
>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau :<ul><li>Contributeur à la modification d’une vue</li><li>Standard pour modifier un rapport</li></ul></p><p>Ou</p>Actuel :<ul><li>Demander la modification d’un affichage</li><li>Prévoir de modifier un rapport</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exemple : triez et masquez la colonne Numéro de tâche dans une vue de tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne** et commencez à saisir « Numéro de la tâche » dans le champ **Afficher dans cette colonne** puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Cliquez sur **Passer en mode Texte**, puis **Modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Edit Text Mode** et remplacez-le par le code suivant :

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
   * `valuefield=` : a été remplacé par `value` et doit être vide.
   * `width=` : selon le champ, il doit avoir la valeur **0** ou **1**.

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.
