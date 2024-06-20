---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gérer les types d’heures
description: Vous pouvez associer des types d’heures à vos entrées d’heures. Les types d’heures sont des libellés que vous utilisez pour définir vos entrées d’heure.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: ht
source-wordcount: '812'
ht-degree: 100%

---

# Gérer les types d’heures

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Vous pouvez associer des types d’heures à vos entrées d’heures. Les types d’heures sont des libellés que vous utilisez pour définir vos entrées d’heure.

Il existe deux jeux de types d’heures :

* **Types d’heures spécifiques au projet** : il s’agit des heures consignées pour les projets, les tâches et les problèmes. Les types d’heures spécifiques au projet peuvent être associés à des entrées d’heures n’importe où dans [!DNL Adobe Workfront], où vous pouvez consigner des heures pour les projets, les tâches et les problèmes.

  Lorsque vous consignez des heures dans [!DNL Workfront], les types d’heures spécifiques au projet disponibles dépendent des options de configuration définies au niveau du système, du projet et de l’utilisateur ou utilisatrice.

  Les types d’heures par défaut spécifiques au projet suivants sont toujours disponibles :

   * Durée du projet
   * Durée de la tâche
   * Heure de l’événement

  L’administrateur ou l’administratrice [!DNL Workfront] détermine les types d’heures spécifiques au projet qui sont disponibles, comme décrit dans la section [Définir les types d’heures et la disponibilité pour les feuilles de temps](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Si vous activez des types d’heures spécifiques à un projet dans votre système [!DNL Workfront], au moins un type d’heure spécifique au projet doit être activé sur chaque projet de votre système. Vous ne pouvez pas activer de type d’heure spécifique au projet au niveau du système et ne disposez pas de types d’heures spécifiques au projet au niveau du projet.

* **Types d’heures générales** : les heures générales ne peuvent pas être associées à un projet, une tâche ou un problème et sont consignées directement dans une feuille de temps. Pour plus d’informations sur la consignation des heures, voir [Consigner les heures](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan [!UICONTROL Adobe Workfront]</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Types d’heures intégrés

Workfront est fourni avec un ensemble de types d’heures intégrés. Ces types d’heures ne peuvent pas être modifiés ni masqués.

Les types d’heures fournis avec [!DNL Workfront] sont les suivants :

* **[!UICONTROL Congés maladie]** : type d’heure général qui ne peut pas être associé aux entrées d’heures pour un projet, une tâche ou un problème. Les congés maladie ne peuvent pas être comptabilisés comme des revenus.
* **[!UICONTROL Congés]** : type d’heure général qui ne peut pas être associé aux entrées d’heures pour un projet, une tâche ou un problème. Les congés ne peuvent pas être comptabilisés comme des revenus.
* **[!UICONTROL Frais généraux]** : type d’heure général qui ne peut pas être associé aux entrées d’heure pour un projet, une tâche ou un problème. Cependant, ils peuvent être comptabilisés comme des revenus dans la planification de votre projet.
* **[!UICONTROL Durée du projet]** : type d’heure général qui ne peut être associé qu’aux entrées d’heures pour un projet.
* **[!UICONTROL Durée de la tâche]** : type d’heure général qui ne peut être associé qu’aux entrées d’heures pour une tâche.
* **[!UICONTROL Durée du problème]** : type d’heure général qui ne peut être associé qu’aux entrées d’heures pour un problème.

## Créer des types d’heures

En tant qu’administrateur ou administratrice [!DNL Workfront], vous pouvez créer de nouveaux types d’heures pour votre organisation, tant au niveau du système que du projet. Une fois que vous avez créé les types d’heures au niveau du système et du projet, les utilisateurs et utilisatrices peuvent définir quels sont les types d’heures disponibles pour des projets et des personnes spécifiques. Pour plus d’informations, voir [Définir les types d’heures et la disponibilité pour les feuilles de temps](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

Pour créer de nouveaux types d’heures :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe] Workfront, puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Feuille de temps et heures]** > **[!UICONTROL Types d’heures]**.

1. Cliquez sur **[!UICONTROL Nouveau type d’heure].**
1. Indiquez les informations suivantes sur le formulaire **[!UICONTROL Nouveau type d’heure]** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Donnez à votre nouveau type d’heure un nom facilement reconnaissable dans le système.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Ajoutez une description pour votre type d’heure.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Définissez si le type d’heure est un type d’heure général ou spécifique à un projet en sélectionnant la portée correcte dans le menu déroulant.</p> <p>Les types d’heures généraux sont visibles uniquement dans les feuilles de temps et ne peuvent pas être associés à des projets, des tâches ou des problèmes.</p> <p><b>IMPORTANT</b> : si vous avez un type d’heure personnalisé qui est [!UICONTROL Project Specific], puis que vous le remplacez par [!UICONTROL General], l’ensemble des tâches, des problèmes et des heures du projet existant sont définis sur leurs types par défaut système.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count As Revenue]</td> 
      <td><p>Sélectionnez cette option si vous souhaitez que l’entrée d’heure associée à ce type d’heure affecte le calcul du revenu.</p>
      <p>Les congés maladie et les congés ne peuvent pas être comptabilisés comme revenu.</p>
      <p><b>NOTE</b></p>
      <p>Lorsque les types d’heures généraux sont comptabilisés comme revenu, le taux de dépenses associé au profil de la personne qui consigne les heures est associé au coût horaire.  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Comptabiliser comme revenu]** : sélectionnez cette option si vous souhaitez que l’entrée d’heure associée à ce type d’heure affecte le calcul de votre revenu.

1. Cliquez sur **[!UICONTROL Créer un type d’heure].**

## Désactiver les types d’heures

Si les types d’heure deviennent obsolètes et que vous ne souhaitez plus que les personnes leur associent leurs entrées d’heure, vous pouvez désactiver les types d’heure.

La désactivation des types d’heures masque les types d’heures dans toutes les zones de [!DNL Workfront] où les types d’heures sont visibles.

Pour désactiver un type d’heure, procédez comme suit :

1. Cliquez sur **[!UICONTROL Configuration]** près du coin supérieur droit d’[!DNL Adobe Workfront] dans la barre de navigation globale.

1. Développer les **[!UICONTROL Préférences en matière de feuille de temps et d’heures]**, puis cliquez sur **[!UICONTROL Types d’heure]**.

1. Sélectionnez le type d’heure à désactiver.

1. Cliquez sur **[!UICONTROL Désactiver]**.
