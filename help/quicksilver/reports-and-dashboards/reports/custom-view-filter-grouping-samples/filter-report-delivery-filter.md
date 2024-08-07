---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : afficher les rapports planifiés pour la diffusion'
description: Ce filtre affiche tous les rapports planifiés pour être livrés automatiquement dans Adobe Workfront. Il est préférable de l’utiliser avec la vue standard.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 53%

---

# Filtre : afficher les rapports dont la diffusion est prévue

Ce filtre affiche tous les rapports planifiés pour être livrés automatiquement dans Adobe Workfront. Il est préférable de l’utiliser avec la vue standard.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demande de modification d’un filtre </p>
   <p>Prévoir la modification d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier un filtre</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Filtre de diffusion de rapport

Pour appliquer ce filtre :

1. Accédez à une liste de rapports.
1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.

1. Cliquez sur **Passer en mode Texte**.
1. Dans la zone **Définir des règles de filtrage pour votre rapport**, copiez et collez le code suivant :

   ```
   scheduledReportID=0<br>scheduledReportID_Mod=notnull
   ```

1. Cliquez sur **Enregistrer le filtre**.
