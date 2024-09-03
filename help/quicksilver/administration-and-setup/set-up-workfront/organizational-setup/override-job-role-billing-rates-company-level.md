---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Remplacer les taux de facturation des fonctions à l’échelle de l’entreprise
description: Lorsqu’une fonction est créée, vous avez la possibilité de sélectionner un taux de facturation horaire pour cette fonction. Vous pouvez créer un taux de facturation horaire spécifique à une société.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 100%

---

# Remplacer les taux de facturation des fonctions à l’échelle de l’entreprise

Lorsqu’une fonction est créée, vous avez la possibilité de sélectionner un taux de facturation horaire pour cette fonction. Vous pouvez créer plusieurs taux de facturation horaires spécifiques à une société. Chaque taux de facturation est effectif pour une période spécifique.

Au niveau du projet, vous pouvez activer une option pour permettre aux taux de facturation au niveau de la société de remplacer les taux au niveau du projet. Pour plus d’informations, consultez la section [Remplacer les taux de facturation au niveau du projet par les taux de facturation au niveau de l’entreprise](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès administratif aux entreprises si vous n’êtes pas une personne administratrice du système.</p> <p>Accès en [!UICONTROL Edit] aux données financières</p> <p><b>NOTE</b> : si votre accès n’est toujours pas activé, demandez à votre administrateur ou à votre administratrice [!DNL Workfront] si des restrictions supplémentaires au niveau de votre accès ont été définies. Pour plus d’informations sur la manière dont une équipe d’administration [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Remplacer ou modifier un taux de facturation défini utilisé pour une fonction spécifique

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe] Workfront, puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

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
