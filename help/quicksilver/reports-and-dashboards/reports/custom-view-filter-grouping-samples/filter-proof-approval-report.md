---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filtrer : rapport d’approbation d’épreuve pour omettre les versions d’épreuve précédentes'
description: Dans un rapport d’approbation d’épreuves, vous pouvez utiliser le filtre Est la version actuelle du document pour inclure uniquement les versions actuelles des épreuves en attente d’approbation.
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 47%

---

# Filtre : relire le rapport d’approbation pour ne pas tenir compte des versions antérieures des épreuves.

<!--Audited: 10/2024-->

Sur un rapport Approbation d’épreuve , vous pouvez utiliser le filtre **Est la version actuelle du document** pour inclure uniquement les versions actuelles des épreuves en attente de votre approbation.

Ceci est utile, par exemple, si l’on vous a demandé d’approuver des épreuves comportant plusieurs versions. Lorsque vous exécutez le rapport d’approbation d’épreuves avec le filtre Est la version actuelle du document, le rapport ne répertorie que la version actuelle de chaque épreuve en attente d’approbation, en omettant les versions antérieures sur lesquelles vous n’avez plus besoin de travailler.

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
   <p>Contributeur ou demande de modification d’un filtre </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrer le rapport d’approbation des épreuves pour ne pas tenir compte des versions antérieures des épreuves

Vous pouvez créer un filtre pour un rapport Approbation de l&#39;épreuve.

1. Si vous disposez déjà d’un rapport d’approbation d’épreuves, ouvrez-le.

   Ou

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Pour créer votre propre rapport Approbation de l&#39;épreuve, cliquez sur l&#39;icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit, ou sur l&#39;icône **Menu principal** ![Lignes du menu principal](assets/lines-main-menu.png) dans le coin supérieur gauche, si disponible, puis cliquez sur **Rapports** ![Icône de rapports](assets/reports-in-main-menu.png).

1. Cliquez sur **Nouveau rapport**. La liste des types d’objet s’affiche.
1. Cliquez sur **Approbation de l&#39;épreuve** dans la liste.
Report Builder s’ouvre.
1. Cliquez sur **Filtres**, puis sur **Ajouter une règle de filtre**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Cliquez dans la zone **Définir des règles de filtrage pour votre rapport**, puis sélectionnez **Approbation de l’épreuve** dans la liste.
1. Cliquez sur **Est la version actuelle du document** dans la liste sous l&#39;objet **Approbation de l&#39;épreuve**.
1. Choisissez Égal pour votre modificateur de filtre, puis sélectionnez Vrai.
1. Cliquez sur **Enregistrer + Fermer** dans le coin inférieur gauche d’Adobe Workfront, puis cliquez sur **Appliquer** dans la zone qui s’affiche.

   Le rapport Approbation de l’épreuve affiche uniquement les épreuves associées aux versions actuelles d’un document, si l’une des validations d’épreuve répond à ce critère de filtrage.
