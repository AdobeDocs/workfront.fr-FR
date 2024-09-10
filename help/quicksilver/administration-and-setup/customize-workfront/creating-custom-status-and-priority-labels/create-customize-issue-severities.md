---
title: Création ou personnalisation des gravité de problème
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Vos utilisateurs et utilisatrices peuvent utiliser des gravités pour définir la sévérité d’un problème. Vous pouvez personnaliser l’une des cinq gravités par défaut d’Adobe Workfront ou créer une gravité pour vos utilisateurs et utilisatrices.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 99%

---

# Créer ou personnaliser la gravité des problèmes

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Vos utilisateurs et utilisatrices peuvent utiliser des gravités pour définir la sévérité d’un problème. Vous pouvez personnaliser l’une des cinq gravités par défaut d’Adobe Workfront ou créer une gravité pour vos utilisateurs et utilisatrices.

>[!NOTE]
>
>Les tâches et les projets ne disposent pas de cette option.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
     <p>Nouveau : Standard</p>
     <p>ou</p>
     <p>Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gravités des problèmes intégrées

Workfront comporte cinq gravités de problème intégrées :

* Décoratif
* Cause de la confusion
* Bogue qui a une solution
* Bogue sans solution
* Erreur fatale

<p>Vous pouvez modifier les éléments suivants pour ces gravités :</p>

* Nom
* Couleur

  La couleur d’une gravité est conservée dans un rapport graphique si vous regroupez vos résultats par gravité de problème. Pour plus d’informations sur les rapports sous forme de graphiques, voir [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Gravité par défaut

  Pour plus d’informations sur les gravités par défaut, voir [Créer ou modifier une gravité de problème](#create-or-edit-an-issue-severity) dans cet article.
* Description
* Gravité masquée ou non dans Workfront

  Pour plus d’informations sur le masquage d’une gravité, voir [Créer ou modifier une gravité de problème](#create-or-edit-an-issue-severity")

* Supprimer une gravité

  Pour ce faire, vous devez sélectionner une gravité de remplacement.

## Créer ou modifier une gravité de problème {#create-or-edit-an-issue-severity}

En tant qu’administrateur ou administratrice de Workfront, vous pouvez créer et modifier des gravités de problème en fonction des besoins de vos utilisateurs et utilisatrices.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Préférences du projet** > **Gravités**.

1. Si vous créez une gravité, cliquez sur **Ajouter une nouvelle gravité**.
1. Configurez les options suivantes pour la nouvelle gravité ou modifiez-les pour une gravité existante :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom de la gravité</td> 
      <td>Saisir le nom de la gravité</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importance</td> 
      <td>Augmentez ou diminuez le degré de sévérité, initialement attribué par Workfront, pour la gravité.
      <p>Le numéro d’importance pour chaque gravité doit être unique. Le nombre le plus élevé correspond au niveau de gravité le plus sévère.</p> <p>Vous ne pouvez pas modifier ce nombre après avoir enregistré la gravité.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Couleur</td> 
      <td> <p>Choisissez une couleur pour la gravité.</p> 
      <p>La couleur de la gravité est utilisée dans les rapports graphiques lorsque vous regroupez vos résultats par gravité de problème. Pour plus d’informations sur les rapports sous forme de graphique, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Ajouter un graphique à un rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gravité par défaut</td> 
      <td>Sélectionnez la gravité que vous souhaitez que Workfront sélectionne automatiquement pour tous les problèmes nouvellement créés.</p>
      <p>Décoratif est la gravité par défaut des problèmes dans Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Saisissez une description de la gravité pour expliquer sa fonction.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Masquer</td> 
      <td> Masquez une gravité qui n’est plus nécessaire. 
      <p>Une gravité masquée ne s’affiche nulle part dans Workfront, de sorte que les utilisateurs et utilisatrices ne peuvent pas la choisir pour leurs problèmes.</p> 
      <p><b>IMPORTANT</b> : au lieu de supprimer les gravités que vous ne souhaitez plus utiliser, nous vous suggérons de les masquer. De cette façon, vous conservez toutes vos données historiques sur les objets déjà terminés avec leurs gravités, tout en empêchant les personnes d’utiliser ces gravités à l’avenir.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Modifiez l’ordre de classement de vos gravités en les faisant glisser et en les déposant dans l’ordre souhaité.

   Cela modifie l’ordre dans lequel elles s’affichent pour les problèmes. Cela ne modifie pas le numéro d’**Importance**.

1. Cliquer sur **Enregistrer**.

Pour plus d’informations sur l’utilisation des gravités dans le cadre du travail sur les problèmes, consultez la section [Mettre à jour les gravités des problèmes](../../../manage-work/issues/issue-information/update-issue-severity.md).
