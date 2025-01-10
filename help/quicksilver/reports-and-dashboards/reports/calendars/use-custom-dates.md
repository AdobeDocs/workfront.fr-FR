---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utilisation de champs de date personnalisés dans un rapport de calendrier
description: Un rapport de calendrier est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez utiliser des champs de date personnalisés dans un rapport de calendrier pour les tâches, les problèmes et les projets.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: d90459cb4f6fb1960552f0ab174e963582312b5c
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 92%

---

# Utiliser les champs de date personnalisés dans un rapport de calendrier

Un rapport de [!UICONTROL calendrier] est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez afficher les champs de date personnalisés dans un rapport de calendrier pour les objets suivants :

* Tâches
* Problèmes
* Projets

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès [!UICONTROL Edit] aux [!UICONTROL Reports], [!UICONTROL Dashboards] et [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>[!UICONTROL Manage] l’accès au rapport de calendrier</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

1. Vous devez disposer de champs de date personnalisés et d’une valeur dans le champ disponible dans votre instance [!DNL Workfront]. Si vous n’avez pas configuré de formulaire personnalisé avec des dates personnalisées, suivez les instructions de la section [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Joignez le formulaire personnalisé à un projet, à une tâche ou à un problème que vous prévoyez d’ajouter au calendrier, puis indiquez une date. Pour plus d’informations, voir [Ajouter un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Configurer le groupe d’éléments

Vous pouvez choisir la manière dont le groupe d’éléments doit s’afficher sur votre calendrier.

{{step1-to-calendars}}

1. Sélectionnez le calendrier auquel vous souhaitez ajouter un nouveau groupe d&#39;éléments.
Ou
Cliquez sur **[!UICONTROL + Nouveau calendrier]** puis saisissez le nom du calendrier.

   >[!NOTE]
   >
   >Vous devez avoir un accès en [!UICONTROL modification] à [!UICONTROL Rapports], [!UICONTROL Tableaux de bord], et [!UICONTROL Calendriers] dans votre niveau d’accès pour créer un rapport de calendrier.

1. Sur la gauche, cliquez sur **[!UICONTROL Ajouter au calendrier]**, puis sur **[!UICONTROL Ajouter des éléments avancés]**.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Saisissez un nom pour le groupe d’éléments.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Sélectionnez une couleur pour le groupe d’éléments. Tous les éléments s’affichent dans la couleur sélectionnée sur le rapport du calendrier.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td>Choisissez <strong>[!UICONTROL Custom dates]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>Choisissez le mode d’affichage des dates :</p>
       <ul>
        <li><strong>[!UICONTROL Date unique]</strong>: le calendrier affiche l’objet à une seule date.</li>
        <li><strong>[!UICONTROL Duration] (du début à la fin)</strong> : le calendrier affiche l’objet sur une période de plusieurs jours.<br><p>Note : si vous choisissez <strong>[!UICONTROL Duration]</strong>, la date de fin indiquée doit être postérieure à la date de début, sinon l’élément ne s’affichera pas dans le calendrier.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Custom Dates]</strong></td>
      <td><p>Saisissez le nom de date personnalisé associé à l’objet dont vous souhaitez effectuer le suivi.</p><p><strong>NOTE :</strong> la recherche du nom de date personnalisé est limitée à 50 résultats pour éviter des problèmes de performances.</td>
     </tr>
    </tbody>
   </table>

1. Passez à la section suivante.

## Ajouter des objets au groupe d’éléments

Après avoir défini le mode d’affichage des éléments, vous devez ajouter au regroupement les objets que vous souhaitez voir apparaître sur le calendrier.

1. Dans la section **[!UICONTROL Que souhaitez-vous ajouter au calendrier ?]**, sélectionnez

   * **[!UICONTROL Tâches]**
   * **[!UICONTROL Projets]**
   * **[!UICONTROL Événements]**

1. Cliquez sur **[!UICONTROL Ajouter des tâches]**, **[!UICONTROL Ajouter des projets]** ou **[!UICONTROL Ajouter des problèmes]**, selon le type d’objet que vous ajoutez au calendrier.
   ![Sélection d’un objet pour le calendrier](assets/field-name.png)

1. Dans le menu déroulant, commencez à saisir le nom du champ, puis sélectionnez la source du champ de l’objet que vous souhaitez afficher dans le calendrier (par exemple, **[!UICONTROL Tâches en retard]**).
1. Définissez une condition pour le regroupement de calendrier.

   ![Instruction de condition](assets/condition-statement-calendar.png)

   Pour en savoir plus sur la définition de conditions, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Facultatif) Spécifiez des objets supplémentaires pour le groupe de calendriers en répétant les étapes 1 à 4.
1. Dans le champ **[!UICONTROL Définissez les libellés des Tâches/Projets/Problèmes sur ...]**, sélectionnez le libellé des objets de ce regroupement de calendrier.

   >[!NOTE]
   >
   >Si les options relatives aux libellés par défaut ne sont pas disponibles pour un objet donné, le nom de l’objet est affiché à la place. Par exemple, lorsque le libellé [!UICONTROL Tâche parent] est sélectionné et qu’aucune tâche parent n’est associée à l’objet, [!DNL Adobe Workfront] affiche le nom de l’objet affiché dans le calendrier.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
