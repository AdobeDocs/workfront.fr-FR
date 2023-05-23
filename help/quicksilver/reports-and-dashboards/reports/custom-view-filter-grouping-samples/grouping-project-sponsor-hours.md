---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Groupement : Parrain du projet pour les heures'
description: Ce regroupement d’heures organise les heures par le parrain du projet où les heures sont consignées. L’interface du créateur de rapports standard pour les groupements d’heures ne fournit pas de mappage au champ Parrain de projet . Vous devez utiliser l’interface Mode texte pour accéder à ce champ.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Regroupement : Parrain du projet pour les heures

Ce regroupement d’heures organise les heures par le parrain du projet où les heures sont consignées. L’interface du créateur de rapports standard pour les groupements d’heures ne fournit pas de mappage au champ Parrain de projet . Vous devez utiliser l’interface Mode texte pour accéder à ce champ.

![hour_report_group_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demande de modification d’un groupement </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification d’un rapport</p> <p>Editer l'accès aux Filtres, Vues, Groupements pour modifier un groupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Groupe par responsable de projet pour les heures

Pour appliquer ce groupement :

1. Accédez à une liste d&#39;heures.
1. Dans la **Regroupement** menu déroulant, sélectionnez **Nouveau groupement**.

1. Cliquez sur **Passer en mode Texte**.
1. Supprimez le texte de la section **Regrouper votre rapport** zone.

1. Remplacez le texte par le code suivant :

   <pre>group.0.linkedname=project:sponsor:name<br>group.0.name=<br>group.0.valuefield=project:sponsor:name<br>group.0.valueformat=HTML<br>textmode=true<br></pre>

1. Cliquez sur **Enregistrer le groupement**.
