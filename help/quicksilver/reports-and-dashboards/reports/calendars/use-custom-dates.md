---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Utiliser des champs de date personnalisés dans un rapport de calendrier
description: Un rapport Calendrier est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez utiliser des champs de date personnalisés dans un rapport de calendrier pour les tâches, les problèmes et les projets.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 13%

---

# Utiliser des champs de date personnalisés dans un rapport de calendrier

Un rapport [!UICONTROL calendar] est un rapport dynamique qui fournit une représentation visuelle de votre travail. Vous pouvez utiliser des champs de date personnalisés dans un rapport de calendrier pour les objets suivants :

* Tâches
* Problèmes
* Projets

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>Accès à [!UICONTROL Modifier] aux [!UICONTROL Rapports], aux [!UICONTROL Tableaux de bord] et aux [!UICONTROL Calendriers]</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Gérer] l’accès au rapport Calendrier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

1. Vous devez avoir des champs de date personnalisés et une valeur dans le champ disponible dans votre instance [!DNL Workfront]. Si vous ne disposez pas d’un formulaire personnalisé configuré avec des dates personnalisées, suivez les instructions des deux premières sections de [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Joignez le formulaire personnalisé à un projet, à une tâche ou à un problème que vous prévoyez d’ajouter au calendrier, puis spécifiez une date. Pour plus d’informations, voir [Ajout d’un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Configurer le groupe d’éléments

Vous pouvez choisir le mode d’affichage du groupe d’éléments dans votre calendrier.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Calendriers]**.

1. Sélectionnez le calendrier auquel vous souhaitez ajouter un nouveau groupe d’éléments.\
   Ou\
   Cliquez sur **[!UICONTROL + Nouveau calendrier]** et saisissez le nom du calendrier.

   >[!NOTE]
   >
   >Pour créer un rapport de calendrier, vous devez disposer de l’accès [!UICONTROL Modifier] aux [!UICONTROL  rapports], [!UICONTROL tableaux de bord] et [!UICONTROL calendriers] dans votre niveau d’accès.

1. Sur la gauche, cliquez sur **[!UICONTROL Ajouter au calendrier]**, puis sur **[!UICONTROL Ajouter des éléments avancés]**.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nommer ce groupe d’éléments]</strong></td>
      <td>Saisissez le nom du groupe d’éléments.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Sélectionnez une couleur pour le groupe d’éléments. Tous les éléments s’affichent dans la couleur sélectionnée sur le rapport du calendrier.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Champ de date]</strong></td>
      <td>Sélectionnez <strong>[!UICONTROL Dates personnalisées]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Sur le calendrier, afficher]</strong></td>
      <td><p>Choisissez le mode d’affichage des dates :</p>
       <ul>
        <li><strong>[!UICONTROL Date unique]</strong> : le calendrier affiche l’objet à une seule date.</li>
        <li><strong>[!UICONTROL Durée] (du début à la fin)</strong> : le calendrier affiche l’objet sur une période de plusieurs jours.<br><p>Remarque : Si vous choisissez <strong>[!UICONTROL Durée]</strong>, la date de fin spécifiée doit être postérieure à la date de début, sinon l’élément ne s’affichera pas dans le calendrier.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Dates personnalisées]</strong></td>
      <td><p>Saisissez le nom de date personnalisé associé à l’objet dont vous souhaitez effectuer le suivi.</p><p><strong>REMARQUE :</strong> La recherche du nom de date personnalisé est limitée à 50 résultats pour éviter des problèmes de performances.</td>
     </tr>
    </tbody>
   </table>

1. Passez à la section suivante.

## Ajouter des objets au groupe d’éléments

Une fois que vous avez configuré l’affichage des éléments, vous devez ajouter au regroupement les objets que vous souhaitez voir sur le calendrier.

1. Dans le **[!UICONTROL , que souhaitez-vous ajouter au calendrier ?section]**, sélectionnez

   * **[!UICONTROL Tâches]**
   * **[!UICONTROL Projets]**
   * **[!UICONTROL Événements]**

1. Cliquez sur **[!UICONTROL Ajouter des tâches]**, **[!UICONTROL Ajouter des projets]** ou **[!UICONTROL Ajouter des problèmes]**, selon le type d’objet que vous ajoutez au calendrier.\
   ![Sélectionner un objet pour le calendrier](assets/field-name.png)

1. Dans le menu déroulant, commencez à saisir le nom du champ, puis sélectionnez la source du champ de l’objet que vous souhaitez afficher dans le calendrier (par exemple, **[!UICONTROL Tâches en retard]**).
1. Définissez une instruction de condition pour le regroupement de calendrier.

   ![Instruction de condition](assets/condition-statement-calendar.png)

   Pour en savoir plus sur la définition des conditions, voir [modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Facultatif) Spécifiez d’autres objets pour le regroupement de calendrier en répétant les étapes 1 à 4.
1. Dans le champ **[!UICONTROL Définir les étiquettes Tâches/Projets/Problèmes comme...]**, sélectionnez le libellé des objets de ce groupe de calendrier dans le calendrier.

   >[!NOTE]
   >
   >Si les options d’étiquette par défaut ne sont pas disponibles pour un certain objet, le nom de l’objet s’affiche à la place. Par exemple, lorsque l’étiquette [!UICONTROL Tâche parente] est sélectionnée et qu’aucune tâche parente n’est associée à l’objet, [!DNL Adobe Workfront] affiche le nom de l’objet que vous affichez dans le calendrier.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
