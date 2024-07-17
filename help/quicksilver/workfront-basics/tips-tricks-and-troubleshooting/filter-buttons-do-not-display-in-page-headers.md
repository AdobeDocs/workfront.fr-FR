---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Absence des boutons de filtre dans les en-têtes de page
description: Lisez cet article pour résoudre les problèmes liés aux boutons de filtrage qui ne s’affichent pas dans les en-têtes de page.
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 20%

---

# Absence des boutons de filtre dans les en-têtes de page

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe de la licence [!DNL Workfront]</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
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
   <td><span>[!UICONTROL Fuseaux horaires]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL Mes approbations de feuille de temps]</span> </p> </li> 
     <li> <p><span>[!UICONTROL Mes feuilles de calcul]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

Les boutons de filtre de la zone [!UICONTROL Projets et feuilles de calcul] ne s’affichent pas, car les filtres correspondants ne sont pas inclus dans le modèle de mise en page appliqué à l’utilisateur. L’administrateur [!DNL Workfront] doit attribuer un modèle de mise en page contenant les filtres.

>[!NOTE]
>
>Parfois, les filtres sont supprimés de la zone [!UICONTROL Contrôles de liste] dans [!UICONTROL Configuration]. L&#39;administrateur [!DNL Workfront] doit les inclure dans les listes de cette zone pour qu&#39;elles soient disponibles dans les modèles de mise en page.

1. Vérifiez que le modèle de mise en page affiche les filtres suivants :

   * [!UICONTROL Projets sur lesquels je suis active] et [!UICONTROL Projets que je possède] dans la zone [!UICONTROL Projets]
   * [!UICONTROL  Mes approbations de feuille de temps ] et [!UICONTROL Mes feuilles de temps] dans la zone [!UICONTROL  de feuille de temps]

   Pour ce faire :

   1. Accédez au modèle de mise en page.
   1. Sélectionnez **[!UICONTROL Listes]** sous **[!UICONTROL Personnaliser ce que voient les utilisateurs]**.
   1. Sélectionnez **[!UICONTROL Projets]** ou **[!UICONTROL Fiches horaires]** sous **[!UICONTROL Sélectionner une liste à personnaliser]**.
   1. Dans la section **[!UICONTROL Filtre]**, vérifiez que les **[!UICONTROL Projets sur lesquels je suis activé]**, **[!UICONTROL Projets que je possède]** (pour les projets) et **[!UICONTROL Mes approbations de feuille de temps]** et **[!UICONTROL Mes feuilles de temps]** (pour les feuilles de temps) sont sélectionnés.
   1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Pour plus d’informations, voir [Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Attribuez le modèle de mise en page aux utilisateurs, aux rôles de tâche, aux équipes ou aux groupes appropriés. Pour plus d’informations, consultez la section [Affecter des personnes à un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
