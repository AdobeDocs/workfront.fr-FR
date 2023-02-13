---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '''Filtre : Rapport Approbation de BAT pour omettre les versions de BAT précédentes'
description: Dans un rapport d’approbation de BAT, vous pouvez utiliser le filtre Est la version actuelle du document pour inclure uniquement les versions actuelles des BAT en attente de votre approbation.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Filtre : rapport Approbation du BAT pour omettre les versions précédentes du BAT

Dans un rapport d’approbation de BAT, vous pouvez utiliser la variable **Is Current Document Version** filtre pour inclure uniquement les versions actuelles des bons à tirer en attente de votre approbation.

Cela s’avère utile, par exemple, si vous avez été invité à approuver des bons à tirer qui comportent plusieurs versions. Lorsque vous exécutez le rapport Approbation de BAT avec le filtre Is Current Document Version , il répertorie uniquement la version actuelle de chaque BAT en attente de votre approbation, omettant les versions antérieures sur lesquelles vous n’avez plus besoin de travailler. 

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Filtrer le rapport Approbation de BAT pour omettre les versions précédentes du BAT

1. Si vous disposez déjà d’un rapport d’approbation de BAT, ouvrez-le.

   Ou

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Pour créer votre propre rapport Validation du BAT, cliquez sur le menu principal ![](assets/main-menu-icon.png), puis cliquez sur **Rapports** ![](assets/reports-in-main-menu.png). Cliquez sur **Nouveau rapport**. Dans la liste qui s’affiche, faites défiler l’écran jusqu’à et cliquez sur **Approbation du BAT**. Cliquez sur **Enregistrer + Fermer**, saisissez une **Nom du rapport** (facultatif), puis cliquez sur **Enregistrer le rapport**.

1. Cliquez sur **Actions de rapport > Modifier**.
1. Cliquez sur **Filtres**, puis cliquez sur **Ajouter une règle de filtre**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Cliquez sur **Approbation du BAT**.
1. Dans la liste qui s’affiche, cliquez sur **Is Current Document Version**.
1. Cliquez sur **Enregistrer + Fermer** dans le coin inférieur gauche d’Adobe Workfront, puis cliquez sur **Enregistrer le rapport** dans la zone qui s’affiche.
