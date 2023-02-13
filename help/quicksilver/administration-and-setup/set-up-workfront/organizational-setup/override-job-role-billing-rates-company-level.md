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
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Remplacer les taux de facturation des rôles de tâche au niveau de l’entreprise

Lorsqu’un rôle de tâche est créé, vous avez la possibilité de sélectionner un taux de facturation horaire pour ce rôle. Vous pouvez créer un taux de facturation horaire spécifique à une société.

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
1. Cliquez sur **[!UICONTROL Modifier la société]** dans le coin supérieur droit.
1. Dans le **[!UICONTROL Taux de facturation]** , sélectionnez le rôle de tâche à modifier, puis saisissez le nouveau taux de facturation pour ce rôle dans la section **[!UICONTROL Taux de facturation de l’entreprise]** de la boîte.

   >[!NOTE]
   >
   >Les taux de rôle des tâches modifiés sur le projet n’auront une incidence que sur ce projet. Les taux modifiés au niveau de l’entreprise auront une incidence sur tous les projets. Pour plus d’informations, voir [Présentation du remplacement des taux de facturation des rôles de tâche et calcul des recettes sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
