---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Afficher : objets résolvables dans un rapport de tâche ou de projet"
description: Vous pouvez afficher une liste de tous les objets résolvables dans un affichage de projet ou de tâche ou un rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 75%

---

# Vue : objets résolvables dans un rapport de tâche ou de projet

<!--Audited: 11/2024-->

Vous pouvez afficher une liste de tous les objets résolvables dans un affichage de projet ou de tâche ou un rapport.

Pour plus d’informations sur les objets résolvables, voir l’article [Vue d’ensemble des objets de résolution et résolvables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

L’application de cette vue est identique pour les tâches et les projets.

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
   <td> <p> Actuel : 
   <ul>
   <li>Demander la modification d’un affichage</li> 
   <li>Prévoir de modifier un rapport</li>
   </ul>
     </p>
     <p> Nouveau : 
   <ul>
   <li>Contributeur à la modification d’une vue</li> 
   <li>Standard pour modifier un rapport</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
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

## Afficher les objets résolvables dans un rapport de tâche ou de projet

1. Accédez à la liste des tâches ou des projets qui ont été convertis à partir de problèmes.
1. Dans le menu déroulant de la **Vue**, cliquez sur **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, cliquez sur **Ajouter une colonne**.

1. Cliquez sur l’en-tête de la nouvelle colonne, puis sur **Passer en mode Texte** > **Modifier le mode Texte**.
1. Supprimez le texte que vous trouvez dans la zone **Edit Text Mode** et remplacez-le par le code suivant :

   ```
   displayname=Resolvables
   listdelimiter=<br>
   listmethod=nested(resolvables).lists
   textmode=true
   type=iterate
   valuefield=name
   valueformat=HTML
   ```

1. Cliquez sur **Terminé** > **Enregistrer la vue**.\
   Une liste de tous les objets résolvables s’affiche dans la nouvelle colonne. Les noms des objets de la liste ne peuvent pas être directement liés aux objets.
