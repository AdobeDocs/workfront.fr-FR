---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gestion des types d’heures
description: Vous pouvez associer des types d’heure à vos entrées d’heure. Les types d’heure sont des libellés que vous utilisez pour définir vos entrées d’heure.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Gestion des types d’heures

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Vous pouvez associer des types d’heure à vos entrées d’heure. Les types d’heure sont des libellés que vous utilisez pour définir vos entrées d’heure.

Il existe deux types d’heure :

* **Types d’heure spécifiques au projet**: il s’agit de l’heure à laquelle les projets, tâches et problèmes sont consignés. Les types d’heures spécifiques au projet peuvent être associés à des entrées d’heure n’importe où dans [!DNL Adobe Workfront] où vous pouvez consigner du temps pour les projets, les tâches et les problèmes.

  Lors de la connexion [!DNL Workfront], les types d’heures spécifiques au projet disponibles dépendent des options de configuration définies au niveau du système, du projet et de l’utilisateur.

  Les types d’heures suivants par défaut spécifiques au projet sont toujours disponibles :

   * Durée du projet
   * Durée de la tâche
   * Heure de l’événement

  La variable [!DNL Workfront] L’administrateur détermine les types d’heures spécifiques au projet qui sont disponibles, comme décrit dans la section [Définition des types d’heures et de la disponibilité des feuilles de temps](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Si vous activez des types d’heures spécifiques à un projet dans votre [!DNL Workfront] système, au moins un type d’heure spécifique au projet doit être activé sur chaque projet de votre système. Vous ne pouvez pas activer un type d’heure spécifique au projet au niveau du système et ne disposez pas de types d’heure spécifique au projet au niveau du projet.

* **Types d’heure généraux**: les heures générales ne peuvent pas être associées à un projet, une tâche ou un problème et sont connectées directement à une feuille de temps. Pour plus d’informations sur la durée de journalisation, voir [Temps de connexion](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule [!UICONTROL Adobe Workfront]</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Types d’heure intégrés

Workfront est fourni avec un ensemble de types d’heure intégrés. Ces types d’heure ne peuvent pas être modifiés et ne peuvent pas être masqués.

Types d’heure fournis avec [!DNL Workfront] sont :

* **[!UICONTROL Temps de malade]**: type d’heure général qui ne peut pas être associé aux entrées d’heure sur un projet, une tâche ou un problème. Les heures de malade ne peuvent pas être comptabilisées comme recettes.
* **[!UICONTROL Durée du déplacement]**: type d’heure général qui ne peut pas être associé aux entrées d’heure sur un projet, une tâche ou un problème. Le temps de déplacement ne peut pas être compté comme recettes.
* **[!UICONTROL Dépassement général]**: type d’heure général qui ne peut pas être associé aux entrées d’heure sur un projet, une tâche ou un problème. Cependant, il peut être comptabilisé comme recettes dans le processus de planification de votre projet.
* **[!UICONTROL Heure du projet]**: type d’heure général qui ne peut être associé qu’aux entrées d’heure sur un projet.
* **[!UICONTROL Heure de tâche]**: type d’heure général qui ne peut être associé qu’aux entrées d’heure sur une tâche.
* **[!UICONTROL Heure de publication]**: type d’heure général qui ne peut être associé qu’aux entrées d’heure pour un problème.

## Création de types d’heure

Comme [!DNL Workfront] administrateur, vous pouvez créer de nouveaux types d’heures pour votre entreprise, tant au niveau du système que du projet. Une fois que vous avez créé les types d’heures au niveau du système et du projet, les utilisateurs peuvent définir les types d’heures disponibles pour des projets et des utilisateurs spécifiques. Pour plus d’informations, voir [Définition des types d’heures et de la disponibilité des feuilles de temps](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Pour créer de nouveaux types d’heures :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe] Workfront, puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Frise chronologique et heures]** > **[!UICONTROL Types d’heure]**.

1. Cliquez sur **[!UICONTROL Nouveau type d’heure].**
1. Indiquez les informations suivantes sur la variable **[!UICONTROL Nouveau type d’heure]** form :

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
      <td> <p>Définissez si le type d’heure est un type d’heure général ou spécifique au projet en sélectionnant la portée correcte dans le menu déroulant.</p> <p>Les types d’heures généraux sont visibles uniquement dans les feuilles de temps et ne peuvent pas être associés à des projets, des tâches ou des problèmes.</p> <p><b>IMPORTANT</b>: si vous avez un type d’heure personnalisé qui est [!UICONTROL Spécifique au projet], puis que vous le remplacez par [!UICONTROL Général], toutes les tâches, tous les problèmes et toutes les heures du projet existants sont définis sur leurs types par défaut système.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Compter Comme Recettes]</td> 
      <td><p>Sélectionnez cette option si vous souhaitez que l’entrée d’heure associée à ce type d’heure affecte le calcul des recettes.</p>
      <p>Les heures de malade et de vacances ne peuvent pas être comptabilisées comme des recettes.</p>
      <p><b>NOTE</b></p>
      <p>Lorsque les types d’heures généraux sont comptabilisés comme des recettes, le Taux de coût associé au profil de l’utilisateur qui consigne l’heure est associé au Coût de l’heure.  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Compter comme recettes]**: sélectionnez cette option si vous souhaitez que l’entrée d’heure associée à ce type d’heure affecte le calcul des recettes.

1. Cliquez sur **[!UICONTROL Créer un type d’heure].**

## Désactivation des types d’heures

Si les types d’heure deviennent obsolètes et que vous ne souhaitez plus que les utilisateurs leur associent leurs entrées d’heure, vous pouvez désactiver les types d’heure.

La désactivation des types d’heures masque les types d’heures n’importe où dans [!DNL Workfront] où les types d’heures sont visibles.

Pour désactiver un type d’heure :

1. Cliquez sur **[!UICONTROL Configuration]** près du coin supérieur droit de [!DNL Adobe Workfront] dans la barre de navigation globale.

1. Développer **[!UICONTROL Préférences de la feuille de temps et des heures]**, puis cliquez sur **[!UICONTROL Types d’heure]**.

1. Sélectionnez le type d’heure à désactiver.

1. Cliquez sur **[!UICONTROL Désactiver]**.
