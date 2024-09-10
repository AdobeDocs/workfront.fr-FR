---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Remplacer les taux de facturation des rôles de tâche au niveau de l’entreprise
description: Lorsqu’une fonction est créée, vous avez la possibilité de sélectionner un taux de facturation horaire pour cette fonction. Vous pouvez créer un taux de facturation horaire spécifique à une société.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 96%

---

# Remplacer les taux de facturation des fonctions à l’échelle de l’entreprise

Lorsqu’une fonction est créée, vous avez la possibilité de sélectionner un taux de facturation horaire pour cette fonction. Vous pouvez créer plusieurs taux de facturation horaires spécifiques à une société. Chaque taux de facturation est effectif pour une période spécifique.

Au niveau du projet, vous pouvez activer une option pour permettre aux taux de facturation au niveau de la société de remplacer les taux au niveau du projet. Pour plus d’informations, consultez la section [Remplacer les taux de facturation au niveau du projet par les taux de facturation au niveau de l’entreprise](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>
   <p>Nouvelle : [!UICONTROL Standard]</p>
   <p>Ou</p>
   <p>Actuelle : [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès administratif aux entreprises si vous n’êtes pas une personne administratrice du système.</p>
   <p>Modifier l’accès aux données financières</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remplacer ou modifier un taux de facturation défini utilisé pour une fonction spécifique

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Entreprises]**.
1. Localisez l’entreprise à laquelle la fonction est affectée.
1. Cliquez sur le nom de l’entreprise dans la liste.
1. Cliquez sur **[!UICONTROL Taux de facturation]** dans le panneau de gauche.
1. Cliquez sur **[!UICONTROL Ajouter un taux de facturation] > [!UICONTROL Nouveau taux de facturation]**, ou choisissez un taux existant à modifier.
1. Dans la boîte de dialogue [!UICONTROL Nouveau taux de facturation], sélectionnez une [!UICONTROL **fonction**] pour définir son taux de facturation.

   Le [!UICONTROL **Taux de facturation par défaut**] affiche le taux au niveau du système pour cette fonction.

   ![Boîte de dialogue du nouveau taux de facturation](assets/date-effective-billing-rates-for-company.png)

1. Dans le champ [!DNL **Taux de facturation 1**], saisissez le taux de facturation. Cliquez ensuite sur [!UICONTROL **Enregistrer**] pour remplacer une fois le taux de facturation.

   Ou

   Cliquez sur [!UICONTROL **Ajouter un taux**] pour ajouter d’autres taux de facturation avec des dates de validité.

1. (Le cas échéant) Si vous ajoutez plusieurs taux de facturation, saisissez les informations suivantes :

   * **[!UICONTROL Taux de facturation 1], 2, etc.** : valeur du taux de facturation pour la période.
   * **[!UICONTROL Date de début]** : date de début de validité du taux.
   * **[!UICONTROL Date de fin]** : date de fin de validité du taux.

     Le taux de facturation 1 ne comporte pas de date de début de validité et le dernier taux de facturation n’a pas de date de fin de validité. Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de facturation 1 ne comporte pas de date de fin de validité et que vous ajoutez le taux de facturation 2 avec une date de début de validité le 1er mai 2023, une date de fin de validité au 30 avril 2023 est ajoutée au taux de facturation 1 afin qu’il n’y ait pas d’écart.

1. Cliquer sur [!UICONTROL **Enregistrer**].

   >[!NOTE]
   >
   >Les taux modifiés des fonctions sur le projet n’auront d’incidence que sur ce projet. Les taux modifiés au niveau de l’entreprise auront une incidence sur tous les projets. Pour plus d’informations, consultez la section [Vue d’ensemble du remplacement des taux de facturation des fonctions et calcul des revenus sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
