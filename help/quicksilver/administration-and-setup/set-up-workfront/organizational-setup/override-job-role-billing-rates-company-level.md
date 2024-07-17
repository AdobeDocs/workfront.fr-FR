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
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 33%

---

# Remplacer les taux de facturation des rôles de tâche au niveau de l’entreprise

Lorsqu’un rôle de tâche est créé, vous avez la possibilité de sélectionner un taux de facturation horaire pour ce rôle. Vous pouvez créer plusieurs taux de facturation horaires spécifiques à une entreprise. Chaque taux de facturation est effectif pour une période spécifique.

Au niveau du projet, vous pouvez activer une option pour permettre aux taux de facturation au niveau de l’entreprise de remplacer les taux au niveau du projet. Pour plus d’informations, voir [Remplacement des taux de facturation au niveau du projet par des taux de facturation au niveau de l’entreprise](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès administratif aux entreprises si vous n’êtes pas administrateur système</p> <p>Accès à [!UICONTROL Modifier] aux données financières</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Remplacer ou modifier un taux de facturation défini utilisé pour un rôle de tâche spécifique

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe] Workfront, puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Entreprises]**.
1. Localisez la société dans laquelle le rôle de tâche est affecté.
1. Cliquez sur le nom de la société dans la liste.
1. Cliquez sur **[!UICONTROL Taux de facturation]** dans le panneau de gauche.
1. Cliquez sur **[!UICONTROL Ajouter le taux de facturation] > [!UICONTROL Nouveau taux de facturation]** ou choisissez un taux existant à modifier.
1. Dans la boîte de dialogue [!UICONTROL New Billing Rate] (Nouveau taux de facturation), sélectionnez un [!UICONTROL **rôle de tâche**] pour définir le taux de facturation.

   Le [!UICONTROL **taux de facturation par défaut**] affiche le taux au niveau du système pour ce rôle de tâche.

   ![Boîte de dialogue Nouveau taux de facturation](assets/date-effective-billing-rates-for-company.png)

1. Dans le champ [!DNL **Taux de facturation 1**] , saisissez le taux de facturation. Cliquez ensuite sur [!UICONTROL **Enregistrer**] pour remplacer le taux de facturation une fois.

   Ou

   Cliquez sur [!UICONTROL **Ajouter le taux**] pour ajouter d’autres taux de facturation avec des dates d’entrée en vigueur.

1. (Conditionnel) Si vous ajoutez plusieurs taux de facturation, saisissez les informations suivantes :

   * **[!UICONTROL Taux de facturation 1], 2, etc.** : valeur du taux de facturation pour la période.
   * **[!UICONTROL Date de début]** : date à laquelle le taux prend effet.
   * **[!UICONTROL Date de fin]** : date de fin du taux.

     Le taux de facturation 1 ne comporte pas de date de début et le dernier taux de facturation n’a pas de date de fin. Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de facturation 1 n’a pas de date de fin et que vous ajoutez le taux de facturation 2 avec une date de début le 1er mai 2023, une date de fin le 30 avril 2023 est ajoutée au taux de facturation 1 afin qu’il n’y ait pas d’écart.

1. Cliquer sur [!UICONTROL **Enregistrer**].

   >[!NOTE]
   >
   >Les taux de rôle des tâches modifiés sur le projet n’auront une incidence que sur ce projet. Les taux modifiés au niveau de l’entreprise auront une incidence sur tous les projets. Pour plus d’informations, voir [Présentation du remplacement des taux de facturation des rôles de tâche et calcul des recettes sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
