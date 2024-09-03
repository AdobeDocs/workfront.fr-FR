---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '« Filtre : le rapport d’approbation d’épreuves ne tient pas compte des versions antérieures des épreuves. »'
description: Dans un rapport d’approbation d’épreuves, vous pouvez utiliser le filtre Est la version actuelle du document pour inclure uniquement les versions actuelles des épreuves en attente d’approbation.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 100%

---

# Filtre : le rapport d’approbation d’épreuves ne tient pas compte des versions antérieures des épreuves.

Dans un rapport d’approbation d’épreuves, vous pouvez utiliser le filtre **Est la version actuelle du document** pour n’inclure que les versions actuelles des épreuves en attente d’approbation.

Ceci est utile, par exemple, si l’on vous a demandé d’approuver des épreuves comportant plusieurs versions. Lorsque vous exécutez le rapport d’approbation d’épreuves avec le filtre Est la version actuelle du document, le rapport ne répertorie que la version actuelle de chaque épreuve en attente d’approbation, en omettant les versions antérieures sur lesquelles vous n’avez plus besoin de travailler. 

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demande de modification d’un filtre </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Filtrer le rapport d’approbation des épreuves pour ne pas tenir compte des versions antérieures des épreuves

1. Si vous disposez déjà d’un rapport d’approbation d’épreuves, ouvrez-le.

   Ou

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Pour créer votre propre rapport d’approbation d’épreuves, cliquez sur le menu principal ![](assets/main-menu-icon.png), puis sur **Rapports** ![](assets/reports-in-main-menu.png). Cliquez sur **Nouveau rapport**. Dans la liste qui s’affiche, trouvez et cliquez sur **Approbation d’épreuve**. Cliquez sur **Enregistrer et Fermer**, saisissez un **Nom de rapport** (facultatif), puis cliquez sur **Enregistrer le rapport**.

1. Cliquez sur **Actions de rapport > Modifier**.
1. Cliquez sur **Filtres**, puis sur **Ajouter une règle de filtre**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Cliquez sur **Approbation d’épreuve**.
1. Dans la liste qui s’affiche, cliquez sur **Est la version actuelle du document**.
1. Cliquez sur **Enregistrer et Fermer** dans le coin inférieur gauche d’Adobe Workfront, puis cliquez sur **Enregistrer le rapport** dans la boîte qui s’affiche.
