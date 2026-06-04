---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Les boutons de filtre ne s’affichent pas dans les en-têtes de page.
description: Cet article permet de résoudre le problème des boutons de filtre qui ne s’affichent pas dans les en-têtes de page.
feature: Get Started with Workfront
author: Courtney
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
TQID: https://experienceleague.adobe.com/36hMJKo4unpIxvUOmBk79XlhFvFL5TgqUaoQXxrPd7c
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 100%

---

# Les boutons de filtre ne s’affichent pas dans les en-têtes de page.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table>
  <tr>
   <td>Package Adobe Workfront
   </td>
   <td>Tous</td>
  </tr>
  <tr>
   <td>Licences Adobe Workfront
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td>Vous devez être administrateur ou administratrice [!DNL Workfront].
   </td>
  </tr>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Problème

Les boutons de filtre suivants ne s’affichent pas dans leurs zones respectives :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] Zone</strong></td> 
   <td><strong>Boutons de filtre</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projects] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects I'm On]</p> </li> 
     <li> <p>[!UICONTROL Projects I Own]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Timesheets]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL My Timesheet Approvals]</span> </p> </li> 
     <li> <p><span>[!UICONTROL My Timesheets]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

Les boutons de filtre dans la zone [!UICONTROL Projets et feuilles de temps] ne s’affichent pas, car les filtres correspondants ne sont pas inclus dans le modèle de mise en page appliqué à la personne. L’administration [!DNL Workfront] doit affecter un modèle de mise en page qui inclut les filtres.

>[!NOTE]
>
>Parfois, les filtres sont supprimés de la zone [!UICONTROL Contrôles de listes] dans [!UICONTROL Configuration]. L’administration [!DNL Workfront] doit les inclure dans les listes de cette zone pour qu’ils soient disponibles dans les modèles de mise en page.

1. Vérifiez que le modèle de mise en page affiche les filtres suivants :

   * [!UICONTROL Projets auxquels je participe] et [!UICONTROL Projets dont je suis propriétaire] dans la zone [!UICONTROL Projets]
   * [!UICONTROL Mes approbations de feuille de temps] et [!UICONTROL Mes feuilles de temps] dans la zone [!UICONTROL Feuille de temps]

   Pour ce faire :

   1. Accédez au modèle de mise en page.
   1. Sélectionnez **[!UICONTROL Listes]** sous **[!UICONTROL Personnaliser ce que les clientes et clients voient]**.
   1. Sélectionnez **[!UICONTROL Projets]** ou **[!UICONTROL Feuilles de temps]** sous **[!UICONTROL Sélectionner une liste à personnaliser]**.
   1. Dans la section **[!UICONTROL Filtre]**, vérifiez que les filtres **[!UICONTROL Projets auxquels je participe]**, **[!UICONTROL Projets dont je suis propriétaire]** (pour les projets), **[!UICONTROL Mes approbations de feuille de temps]** et **[!UICONTROL Mes feuilles de temps]** (pour les feuilles de temps) sont sélectionnés.
   1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Pour plus d’informations, voir [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Attribuez le modèle de mise en page aux personnes, fonctions, équipes ou groupes appropriés. Pour plus d’informations, consultez la section [Affecter des personnes à un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
