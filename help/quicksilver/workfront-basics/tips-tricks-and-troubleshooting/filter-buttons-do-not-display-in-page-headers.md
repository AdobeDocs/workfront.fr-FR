---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Les boutons de filtre ne s’affichent pas dans les en-têtes de page
description: Lisez cet article pour résoudre les problèmes liés aux boutons de filtrage qui ne s’affichent pas dans les en-têtes de page.
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# Les boutons de filtre ne s’affichent pas dans les en-têtes de page

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] license</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problème

Les boutons de filtre suivants ne s’affichent pas dans leurs zones respectives :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] area</strong></td> 
   <td><strong>Bouton Filtrer</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projects] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projets sur lesquels je suis connecté]</p> </li> 
     <li> <p>[!UICONTROL Projets que je possède]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Feuilles de calcul]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL Mes approbations de feuille de temps]</span> </p> </li> 
     <li> <p><span>[!UICONTROL Mes feuilles de calcul]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

Les boutons de filtrage du [!UICONTROL Projets et feuilles de temps] ne s’affichent pas, car les filtres correspondants ne sont pas inclus dans le modèle de mise en page appliqué à l’utilisateur. Le [!DNL Workfront] L’administrateur doit attribuer un modèle de mise en page contenant les filtres.

>[!NOTE]
>
>Parfois, les filtres sont supprimés de la variable [!UICONTROL Contrôles de liste] area dans [!UICONTROL Configuration]. Le [!DNL Workfront] L&#39;administrateur doit les inclure dans les listes de cette zone pour qu&#39;elles soient disponibles dans les modèles de mise en page.

1. Vérifiez que le modèle de mise en page affiche les filtres suivants :

   * [!UICONTROL Projets actifs] et [!UICONTROL Projets que je possède] dans le [!UICONTROL Projets] area
   * [!UICONTROL Mes approbations de la feuille de temps] et [!UICONTROL Mes feuilles de calcul] dans le [!UICONTROL Feuille de calcul] area

   Pour ce faire :

   1. Accédez au modèle de mise en page.
   1. Sélectionner **[!UICONTROL Listes]** under **[!UICONTROL Personnalisation des éléments affichés par les utilisateurs]**.
   1. Sélectionner **[!UICONTROL Projets]** ou **[!UICONTROL Feuilles de temps]** under **[!UICONTROL Sélectionner une liste à personnaliser]**.
   1. Dans le **[!UICONTROL Filtrer]** , vérifiez que **[!UICONTROL Projets actifs]**, **[!UICONTROL Projets que je possède]** (pour les projets) et **[!UICONTROL Mes approbations de la feuille de temps]** et **[!UICONTROL Mes feuilles de calcul]** (pour les feuilles de temps) sont sélectionnées.
   1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Pour plus d’informations, voir [Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Attribuez le modèle de mise en page aux utilisateurs, aux rôles de tâche, aux équipes ou aux groupes appropriés. Pour plus d’informations, voir [Affecter des utilisateurs à un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
