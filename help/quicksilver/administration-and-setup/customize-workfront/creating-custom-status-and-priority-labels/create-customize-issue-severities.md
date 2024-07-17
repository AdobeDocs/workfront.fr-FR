---
title: Création ou personnalisation des gravité de problème
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Vos utilisateurs peuvent utiliser des statistiques pour définir la gravité d’un problème. Vous pouvez personnaliser l’une des cinq gravité par défaut d’Adobe Workfront ou créer une nouvelle gravité pour vos utilisateurs.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 18%

---

# Création ou personnalisation des gravité de problème

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Vos utilisateurs peuvent utiliser des statistiques pour définir la gravité d’un problème. Vous pouvez personnaliser l’une des cinq gravité par défaut d’Adobe Workfront ou créer une nouvelle gravité pour vos utilisateurs.

>[!NOTE]
>
>Les tâches et les projets n’ont pas de gravité.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Séparations des problèmes intégrés

Workfront comporte cinq ruptures de problème intégrées :

* Décoratif
* Cause de la confusion
* Bogue qui a une solution
* Bogue sans solution
* Erreur fatale

<p>Vous pouvez modifier les éléments suivants pour ces gravité :</p>

* Nom
* Couleur

  La couleur d’une gravité est conservée dans un rapport graphique si vous regroupez vos résultats par gravité de problème. Pour plus d’informations sur les rapports de graphique, voir [Ajout d’un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Quelle gravité est la valeur par défaut ?

  Pour plus d’informations sur les gravité par défaut, voir [Création ou modification d’une gravité de problème](#create-or-edit-an-issue-severity) dans cet article.
* Description
* Si une gravité est masquée dans Workfront

  Pour plus d’informations sur le masquage d’une gravité, voir [Créer ou modifier une gravité de problème](#create-or-edit-an-issue-severity")

* Supprimer une gravité

  Pour ce faire, vous devez sélectionner une gravité de remplacement.

## Création ou modification d’une gravité de problème {#create-or-edit-an-issue-severity}

En tant qu’administrateur de Workfront, vous pouvez créer et modifier des statistiques de problèmes en fonction des besoins de vos utilisateurs.

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Préférences du projet** > **Gravités**.

1. Si vous créez une nouvelle gravité, cliquez sur **Ajouter une nouvelle gravité**.
1. Configurez les options suivantes pour la nouvelle gravité ou modifiez-les pour une autre :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom de la gravité</td> 
      <td>Saisissez le nom de la gravité.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importance</td> 
      <td>Augmenter ou diminuer le niveau de gravité, initialement attribué par Workfront, pour la gravité.
      <p>Le numéro d'importance pour chaque gravité doit être unique. Le nombre le plus élevé correspond au niveau de gravité le plus élevé.</p> <p>Vous ne pouvez pas modifier ce nombre après avoir enregistré la gravité.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Couleur</td> 
      <td> <p>Choisissez une couleur pour la gravité.</p> 
      <p>La couleur de la gravité est utilisée dans les rapports graphiques lorsque vous regroupez vos résultats par gravité de problème. Pour plus d’informations sur les rapports de graphique, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Ajout d’un graphique à un rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gravité par défaut</td> 
      <td>Sélectionnez la gravité que vous souhaitez que Workfront sélectionne automatiquement tous les problèmes nouvellement créés.</p>
      <p>La mesure est la gravité par défaut des problèmes dans Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Saisissez une description de la gravité pour expliquer sa fonction.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Masquer</td> 
      <td> Masquez une gravité qui n’est plus nécessaire. 
      <p>Une gravité masquée ne s’affiche nulle part dans Workfront, de sorte que les utilisateurs ne peuvent pas la choisir pour leurs problèmes.</p> 
      <p><b>IMPORTANT</b> : au lieu de supprimer des statistiques que vous ne souhaitez plus utiliser, nous vous suggérons de les masquer. Ainsi, vous conservez toutes vos données historiques sur les objets déjà atteints avec la gravité, tout en empêchant les personnes d’utiliser la gravité à l’avenir.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Modifiez l’ordre de classement de vos statistiques en les faisant glisser et en les déposant dans l’ordre souhaité.

   Cela modifie l’ordre dans lequel ils s’affichent pour les problèmes. Il ne modifie pas le numéro **Importance**.

1. Cliquer sur **Enregistrer**.

Pour plus d’informations sur l’utilisation des gravité lors de l’utilisation des problèmes, voir [Mise à jour de la gravité des problèmes](../../../manage-work/issues/issue-information/update-issue-severity.md).
