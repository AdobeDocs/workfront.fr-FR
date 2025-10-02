---
title: Créer ou personnaliser des gravités de problèmes
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Vos utilisateurs et utilisatrices peuvent utiliser des gravités pour définir la sévérité d’un problème. Vous pouvez personnaliser l’une des cinq gravités par défaut d’Adobe Workfront ou créer une gravité pour vos utilisateurs et utilisatrices.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 7cb1eed72b0f5ce4abd83013b7a2f224dbb2c229
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 66%

---

# Créer ou personnaliser la gravité des problèmes

{{highlighted-preview}}

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

Vous pouvez modifier les éléments suivants pour ces gravités :

* Nom
* Couleur

  La couleur d’une gravité est conservée dans un rapport graphique si vous regroupez vos résultats par gravité de problème. Pour plus d’informations sur les rapports sous forme de graphiques, voir [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Gravité par défaut

  Pour plus d’informations sur les gravités par défaut, voir [Créer ou modifier une gravité de problème](#create-or-edit-an-issue-severity) dans cet article.

* Description
* Gravité masquée ou non dans Workfront

  Pour plus d’informations sur le masquage d’une gravité, voir [Création ou modification d’une gravité de problème](#create-or-edit-an-issue-severity) dans cet article.

* Supprimer une gravité

  Pour ce faire, vous devez sélectionner une gravité de remplacement.

## Créer ou modifier une gravité de problème {#create-or-edit-an-issue-severity}

En tant qu’administrateur ou administratrice de Workfront, vous pouvez créer et modifier des gravités de problème en fonction des besoins de vos utilisateurs et utilisatrices.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Préférences du projet** > **Gravités**.

1. Si vous créez une nouvelle gravité, cliquez sur <span class="preview">**Nouvelle ligne** au bas du tableau</span> ou **Ajouter une nouvelle gravité**.
1. Configurez les options suivantes pour la nouvelle gravité ou modifiez-les pour une gravité existante :

   * **Nom de la gravité** : saisissez un nom pour la gravité.
   * **Importance** : augmente ou réduit le niveau de gravité attribué initialement par Workfront à la gravité.

     Le numéro d’importance pour chaque gravité doit être unique. Le nombre le plus élevé correspond au niveau de gravité le plus sévère.

     Vous ne pouvez pas modifier ce nombre après avoir enregistré la gravité.

   * **Couleur** : choisissez une couleur pour la gravité.

     La couleur de la gravité est utilisée dans les rapports graphiques lorsque vous regroupez vos résultats par gravité de problème. Pour plus d’informations sur les rapports sous forme de graphiques, voir [Ajouter un graphique à un rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

   * **Gravité par défaut** : sélectionnez la gravité que Workfront doit appliquer automatiquement à tous les problèmes nouvellement créés.

     **Cosmétique** est la gravité par défaut des problèmes dans Workfront.

     Vous ne pouvez pas définir une gravité masquée comme gravité par défaut.

     <div class="preview">

     La gravité par défaut est indiquée par une icône ![Icône de gravité par défaut](assets/default-icon.png). Pour choisir une nouvelle valeur par défaut, effectuez l’une des opérations suivantes :

      * Cochez la case en regard du nom de la gravité et sélectionnez **Rendre par défaut** dans la barre d’actions située en bas de l’écran.
      * Passez la souris sur le nom de la gravité et cliquez sur le menu **Plus** qui s’affiche. Sélectionnez ensuite **Rendre par défaut**.

        La nouvelle gravité par défaut est étiquetée avec l’icône .

     </div>

   * **Description** : saisissez une description de la gravité pour expliquer sa fonction.
   * <span class="preview">**Masquer le choix**</span> ou **Masquer** : <span class="preview">Sélectionnez **Oui**</span> ou cochez la case pour masquer une gravité qui n’est plus nécessaire.

     Une gravité masquée ne s’affiche nulle part dans Workfront, de sorte que les utilisateurs et utilisatrices ne peuvent pas la choisir pour leurs problèmes.

     >[!IMPORTANT]
     >
     >Au lieu de supprimer les gravités que vous ne souhaitez plus utiliser, nous vous suggérons de les masquer. De cette façon, vous conservez toutes vos données historiques sur les objets déjà terminés avec leurs gravités, tout en empêchant les personnes d’utiliser ces gravités à l’avenir.

1. (Facultatif) Modifiez l’ordre de classement de vos gravités en les faisant glisser et en les déposant dans l’ordre souhaité.

   Cela modifie l’ordre dans lequel elles s’affichent pour les problèmes. Cela ne modifie pas le numéro d’**Importance**.

1. Cliquer sur **Enregistrer**.

Pour plus d’informations sur l’utilisation des gravités dans le cadre du travail sur les problèmes, consultez la section [Mettre à jour les gravités des problèmes](../../../manage-work/issues/issue-information/update-issue-severity.md).
