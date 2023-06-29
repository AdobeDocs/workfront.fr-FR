---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Remplacer les taux de facturation des rôles de tâche au niveau de l’entreprise
description: Lorsqu’un rôle de tâche est créé, vous avez la possibilité de sélectionner un taux de facturation horaire pour ce rôle. Vous pouvez créer un taux de facturation horaire spécifique à une société.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# Remplacer les taux de facturation des rôles de tâche au niveau de l’entreprise

{{highlighted-preview}}

Lorsqu’un rôle de tâche est créé, vous avez la possibilité de sélectionner un taux de facturation horaire pour ce rôle. <span class="preview">Vous pouvez créer plusieurs taux de facturation horaires spécifiques à une entreprise. Chaque taux de facturation est effectif pour une période spécifique.</span>

Au niveau du projet, vous pouvez activer une option pour permettre aux taux de facturation au niveau de l’entreprise de remplacer les taux au niveau du projet. Pour plus d’informations, voir [Remplacer les taux de facturation au niveau du projet par les taux de facturation au niveau de l’entreprise](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux entreprises si vous n’êtes pas administrateur système</p> <p>Accès à [!UICONTROL Modifier] aux données financières</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Remplacer ou modifier un taux de facturation défini utilisé pour un rôle de tâche spécifique

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe] Workfront, puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Entreprises]**.
1. Localisez la société dans laquelle le rôle de tâche est affecté.
1. <span class="preview">Cliquez sur le nom de la société dans la liste.</span>
1. <span class="preview">Cliquez sur **[!UICONTROL Taux de facturation]** dans le panneau de gauche.</span>
1. <span class="preview">Cliquez sur **[!UICONTROL Ajouter le taux de facturation] > [!UICONTROL Nouveau taux de facturation]** ou choisissez un taux existant à modifier.</span>
1. <span class="preview">Dans le [!UICONTROL Nouveau taux de facturation] , sélectionnez une [!UICONTROL **Rôle de tâche**] pour définir le taux de facturation.</span>

   <span class="preview">Le [!UICONTROL **Taux de facturation par défaut**] affiche le taux au niveau du système pour ce rôle de tâche.</span>

   <span class="preview">![Boîte de dialogue Nouveau taux de facturation](assets/date-effective-billing-rates-for-company.png)</span>

1. <span class="preview">Dans le [!DNL **Taux de facturation 1**] , saisissez le taux de facturation. Cliquez ensuite sur [!UICONTROL **Enregistrer**] pour remplacer le taux de facturation une fois.</span>

   <span class="preview">Ou</span>

   <span class="preview">Cliquez sur [!UICONTROL **Taux d’ajout**] pour ajouter d’autres taux de facturation avec des dates d’entrée en vigueur.</span>

1. <span class="preview">(Conditionnel) Si vous ajoutez plusieurs taux de facturation, saisissez les informations suivantes :</span>

   * <span class="preview">**[!UICONTROL Taux de facturation 1], 2, etc.**: Valeur du taux de facturation pour la période.</span>
   * <span class="preview">**[!UICONTROL Date de début ]**: Date à laquelle le taux devient effectif.</span>
   * <span class="preview">**[!UICONTROL Date de fin ]**: Date à laquelle le taux se termine.</span>

     <span class="preview">Le taux de facturation 1 ne comporte pas de date de début et le dernier taux de facturation n’a pas de date de fin. Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de facturation 1 ne comporte pas de date de fin et que vous ajoutez le taux de facturation 2 avec une date de début le 1er mai 2023, une date de fin du 30 avril 2023 est ajoutée au taux de facturation 1 afin qu’il n’y ait pas d’écart.</span>

1. <span class="preview">Cliquer sur [!UICONTROL **Enregistrer**].</span>

   >[!NOTE]
   >
   >Les taux de rôle des tâches modifiés sur le projet n’auront une incidence que sur ce projet. Les taux modifiés au niveau de l’entreprise auront une incidence sur tous les projets. Pour plus d’informations, voir [Présentation du remplacement des taux de facturation des rôles de tâche et calcul des recettes sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
