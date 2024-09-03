---
product-area: projects
navigation-topic: use-lists
title: Éléments de modification en ligne dans une liste dans  [!DNL Adobe Workfront]
description: Vous pouvez modifier des objets en ligne lorsqu’ils s’affichent dans une liste ou un rapport. Lorsque vous modifiez les informations sur les objets affichés dans une liste ou un rapport, l’objet est immédiatement mis à jour.
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 97%

---

# Éléments de modification en ligne dans une liste dans [!DNL Adobe Workfront]

Vous pouvez modifier des objets en ligne lorsqu’ils s’affichent dans une liste ou un rapport. Lorsque vous modifiez les informations sur les objets affichés dans une liste ou un rapport, l’objet est immédiatement mis à jour.

Lorsque vous modifiez en ligne un champ contenu dans un formulaire personnalisé qui n’est pas joint à l’objet, le formulaire personnalisé est automatiquement ajouté à l’objet. Si le champ existe sur plusieurs formulaires personnalisés, le formulaire personnalisé qui a été mis à jour le plus récemment est joint à l’objet.

Pour plus d’informations sur les listes, voir [Commencer avec les listes dans  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Bien que la plupart des objets affichés dans les listes ou les rapports soient modifiables en ligne dans [!DNL Adobe Workfront], il existe certaines limites, notamment :

* Vous ne pouvez pas modifier les champs calculés ou les champs [!DNL Workfront] intégrés qui correspondent à des calculs.
* Vous ne pouvez modifier que les champs associés directement aux objets de la liste. Vous ne pouvez pas modifier des champs appartenant à des objets associés aux objets de la liste.\
   Par exemple, vous pouvez modifier le statut d’une tâche dans un rapport de tâche, mais vous ne pouvez pas modifier le nom du projet auquel la tâche est associée dans le même rapport. Vous ne pouvez modifier le nom du projet que dans un rapport de projet.
* Vous ne pouvez pas modifier de champs en ligne lorsque la vue d’une liste n’affiche pas la devise par défaut.\
   Pour plus d’informations sur l’affichage de la devise par défaut, voir la section [Modifier des rapports avec des devises uniques](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) dans l’article [Créer des rapports de données financières avec des taux de change uniques](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).
* Vous ne pouvez pas modifier les indicateurs et les icônes affichés dans une liste.
* Vous ne pouvez pas modifier en ligne des champs de rapport issus d’autres rapports.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] formule*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Accès en [!UICONTROL Edit] à la zone dans laquelle se trouve la liste</p> <p>Par exemple, pour modifier des tâches en ligne dans un projet, vous avez besoin de l’accès en [!UICONTROL Edit] aux projets.</p> <p>Note : si vous n’avez toujours pas d’accès, demandez à votre administrateur ou administratrice [!DNL Workfront] si des restrictions supplémentaires ont été définies dans votre niveau d’accès.<br>Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Manage]</p> <p>Vous devez également disposer des autorisations nécessaires pour modifier certains champs, tels que les champs personnalisés, le statut, etc.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Modifier des objets en ligne

1. Accédez à la liste des objets que vous souhaitez modifier en ligne.

   La liste doit afficher les champs appartenant aux objets ou les champs appartenant aux objets associés aux objets de la liste.

1. Recherchez l’objet à modifier, puis cliquez dans n’importe quel champ de la liste.

   >[!TIP]
   >
   >Si vous disposez de plusieurs pages, vous pouvez localiser un objet à l’aide des éléments suivants :
   >
   >   
   >   
   >   * **Pagination** : cliquez sur les flèches vers l’arrière et vers l’avant pour naviguer entre les pages.\
   >     Située dans le coin inférieur droit de la liste, la zone [!UICONTROL pagination] reste visible lorsque vous faites défiler la liste.
   >   * **Filtre rapide** : cliquez sur l’icône de filtre ou tapez Alt+F pour ouvrir le filtre rapide, puis saisissez du texte pour n’afficher que les éléments qui contiennent le texte saisi.\
   >     Le filtre rapide se trouve dans la barre d’outils de la liste. Pour plus d’informations, voir [Appliquer le filtre rapide à une liste](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).


   Si le champ peut être modifié, lui et tous les autres champs affichés dans la liste sont alors transformés en cellules modifiables.

   ![](assets/nwe-editable-cells-350x131.png)

1. Modifiez les informations dans cette cellule, puis appuyez sur [!UICONTROL Entrée].

   >[!NOTE]
   >
   >Si un champ personnalisé a été configuré pour autoriser le formatage, vous pouvez mettre du texte en gras, en italique ou souligné lorsque vous modifiez le champ en ligne dans une liste mise à jour.
   >Pour plus d’informations sur la configuration du formatage pour un champ personnalisé, voir [Concevoir un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
   >Pour plus d’informations sur les listes mises à jour, voir la section « Différence entre les listes mises à jour et héritées » de l’article [Commencer avec les listes dans  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Appuyez sur la touche [!UICONTROL Tabulation] pour passer à la cellule modifiable suivante.
1. (Le cas échéant) Si vous ne parvenez pas à enregistrer vos modifications et que la cellule est indiquée en rouge, cliquez dans le champ pour examiner le message de validation qui s’affiche en regard de la cellule et effectuer les mises à jour appropriées.

   Cela se produit généralement lorsque le mauvais format est utilisé ou qu’un champ obligatoire a été laissé vide.

1. Une fois les cellules modifiées, appuyez sur [!UICONTROL Entrée] pour enregistrer vos modifications.
