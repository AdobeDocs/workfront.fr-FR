---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Filtre : Rapport d’approbation de BAT pour Omettre les versions de BAT précédentes"
description: Dans un rapport d’approbation d’épreuves, vous pouvez utiliser le filtre Est la version actuelle du document pour inclure uniquement les versions actuelles des épreuves en attente d’approbation.
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 51%

---

# Filtre : relire le rapport d’approbation pour ne pas tenir compte des versions antérieures des épreuves.

<!--Audited: 10/2024-->

Sur un rapport Approbation de BAT, vous pouvez utiliser le filtre **Is Current Document Version** pour inclure uniquement les versions actuelles des BAT en attente de votre approbation.

Ceci est utile, par exemple, si l’on vous a demandé d’approuver des épreuves comportant plusieurs versions. Lorsque vous exécutez le rapport d’approbation d’épreuves avec le filtre Est la version actuelle du document, le rapport ne répertorie que la version actuelle de chaque épreuve en attente d’approbation, en omettant les versions antérieures sur lesquelles vous n’avez plus besoin de travailler.

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
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur à la modification d’un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
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

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrer le rapport d’approbation des épreuves pour ne pas tenir compte des versions antérieures des épreuves

Vous pouvez créer un filtre pour un rapport Approbation de BAT.

1. Si vous disposez déjà d’un rapport d’approbation d’épreuves, ouvrez-le.

   Ou

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Pour créer votre propre rapport d’approbation de BAT, cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit ou sur l’icône **Menu principal** ![](assets/lines-main-menu.png) dans le coin supérieur gauche, le cas échéant, puis cliquez sur **Rapports** ![](assets/reports-in-main-menu.png).

1. Cliquez sur **Nouveau rapport**. La liste des types d’objets s’affiche.
1. Cliquez sur **Approbation de BAT** dans la liste.
Le créateur de rapports s’ouvre.
1. Cliquez sur **Filtres**, puis sur **Ajouter une règle de filtre**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Cliquez dans la zone **Définir les règles de filtrage pour votre rapport**, puis sélectionnez **Approbation de BAT** dans la liste.
1. Cliquez sur **Is Current Document Version** dans la liste sous l’objet **Proof Approval** (Approbation de BAT).
1. Sélectionnez Egal pour votre modificateur de filtre, puis True.
1. Cliquez sur **Enregistrer + Fermer** dans le coin inférieur gauche d’Adobe Workfront, puis cliquez sur **Appliquer** dans la zone qui s’affiche.

   Le rapport Validation du BAT affiche uniquement les BAT associés aux versions actuelles d&#39;un document, si les validations du BAT correspondent à ces critères de filtrage.
