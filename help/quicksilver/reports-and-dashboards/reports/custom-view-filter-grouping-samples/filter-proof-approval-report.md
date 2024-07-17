---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filtre : rapport Approbation du BAT pour omettre les versions précédentes du BAT'
description: Dans un rapport d’approbation de BAT, vous pouvez utiliser le filtre Est la version actuelle du document pour inclure uniquement les versions actuelles des BAT en attente de votre approbation.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 31%

---

# Filtre : rapport Approbation du BAT pour omettre les versions précédentes du BAT

Sur un rapport Approbation de BAT, vous pouvez utiliser le filtre **Is Current Document Version** pour inclure uniquement les versions actuelles des BAT en attente de votre approbation.

Cela s’avère utile, par exemple, si vous avez été invité à approuver des bons à tirer qui comportent plusieurs versions. Lorsque vous exécutez le rapport Approbation de BAT avec le filtre Is Current Document Version , il répertorie uniquement la version actuelle de chaque BAT en attente de votre approbation, omettant les versions antérieures sur lesquelles vous n’avez plus besoin de travailler. 

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

## Filtrer le rapport Approbation de BAT pour omettre les versions précédentes du BAT

1. Si vous disposez déjà d’un rapport d’approbation de BAT, ouvrez-le.

   Ou

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Pour créer votre propre rapport d’approbation de BAT, cliquez sur le menu principal ![](assets/main-menu-icon.png), puis sur **Rapports** ![](assets/reports-in-main-menu.png). Cliquez sur **Nouveau rapport**. Dans la liste qui s’affiche, faites défiler l’écran jusqu’à et cliquez sur **Approbation de BAT**. Cliquez sur **Enregistrer + Fermer**, saisissez un **Nom du rapport** (facultatif), puis cliquez sur **Enregistrer le rapport**.

1. Cliquez sur **Actions de rapport > Modifier**.
1. Cliquez sur **Filtres**, puis sur **Ajouter une règle de filtre**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Cliquez sur **Approbation de BAT**.
1. Dans la liste qui s’affiche, cliquez sur **Is Current Document Version**.
1. Cliquez sur **Enregistrer + Fermer** dans le coin inférieur gauche d’Adobe Workfront, puis cliquez sur **Enregistrer le rapport** dans la zone qui s’affiche.
