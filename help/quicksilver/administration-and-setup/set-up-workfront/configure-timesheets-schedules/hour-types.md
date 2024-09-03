---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gérer les types d’heure
description: Vous pouvez associer des types d’heures à vos entrées d’heures. Les types d’heures sont des libellés que vous utilisez pour définir vos entrées d’heures.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 90%

---

# Gérer les types d’heures

<!--Audited: 07/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Vous pouvez associer des types d’heures à vos entrées d’heures. Les types d’heures sont des libellés que vous utilisez pour définir vos entrées d’heures.

Il existe deux types d’heures :

* **Types d’heures spécifiques au projet** : il s’agit du temps consigné sur les projets, les tâches et les problèmes. Les types d’heures spécifiques au projet peuvent être associés à des entrées d’heures n’importe où dans [!DNL Adobe Workfront] où vous pouvez consigner du temps pour les projets, les tâches et les problèmes.

  Lors de la consignation du temps dans [!DNL Workfront], les types d’heures spécifiques au projet disponibles dépendent des options de configuration définies au niveau du système, du projet et de l’utilisateur ou utilisatrice.

  Les types d’heures suivants par défaut spécifiques au projet sont toujours disponibles :

   * Durée du projet
   * Durée de la tâche
   * Heure de l’événement

  L’administrateur [!DNL Workfront] détermine les types d’heures spécifiques au projet disponibles, comme décrit dans la section [Définition des types d’heures et disponibilité](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Si vous activez des types d’heures spécifiques au projet dans votre système [!DNL Workfront], au moins un type d’heure spécifique au projet doit être activé sur chaque projet de votre système. Vous ne pouvez pas activer un type d’heure spécifique au projet au niveau du système et ne disposez pas de types d’heures spécifiques au projet au niveau du projet.

* **Types d’heure généraux** : les heures générales ne peuvent pas être associées à un projet, une tâche ou un problème et sont connectées directement à une feuille de temps.

Pour plus d’informations sur les heures de journalisation et leur association aux types d’heures, voir [Temps du journal](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan [!UICONTROL Adobe Workfront]</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p>
   <p>Actuelle : [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Vous devez être administrateur ou administratrice [!DNL Workfront].</p> <p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Types d’heures intégrés

Workfront est fourni avec un ensemble de types d’heures intégrés. Ces types d’heures ne peuvent pas être modifiés et ni masqués.

Les types d’heures fournis avec [!DNL Workfront] sont les suivants :

* **[!UICONTROL Congés maladie]** : type d’heure général qui ne peut pas être associé aux entrées d’heures pour un projet, une tâche ou un problème. Les congés maladie ne peuvent pas être comptabilisés comme des revenus.
* **[!UICONTROL Congés]** : type d’heure général qui ne peut pas être associé aux entrées d’heures pour un projet, une tâche ou un problème. Les congés ne peuvent pas être comptabilisés comme des revenus.
* **[!UICONTROL Frais généraux]** : type d’heure général qui ne peut pas être associé aux entrées d’heure pour un projet, une tâche ou un problème. Cependant, il peut être comptabilisé comme un revenu dans le processus de planification de projet.
* **[!UICONTROL Heure de projet]** : type d’heure général qui ne peut être associé qu’aux entrées d’heures sur un projet.
* **[!UICONTROL Heure de tâche]** : type d’heure général qui ne peut être associé qu’aux entrées d’heures sur une tâche.
* **[!UICONTROL Heure de problème]** : type d’heure général qui ne peut être associé qu’aux entrées d’heures pour un problème.

## Créer des types d’heures

En tant qu’administrateur ou administratrice [!DNL Workfront], vous pouvez créer de nouveaux types d’heures pour votre entreprise, tant au niveau du système que du projet. Une fois que vous avez créé les types d’heures au niveau du système et du projet, les utilisateurs et utilisatrices peuvent définir les types d’heures disponibles pour des projets et des personnes spécifiques. Pour plus d’informations, voir la [définition des types d’heures et de la disponibilité](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Pour créer des types d’heures :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Feuille de temps et heures]** > **[!UICONTROL Types d’heures]**.

1. Cliquez sur **[!UICONTROL Nouveau type d’heure].**
1. Indiquez les informations suivantes sur le formulaire **[!UICONTROL Nouveau type d’heure]** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Donnez un nom à votre nouveau type d’heure qui soit facilement reconnaissable dans le système.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Ajoutez une description à votre type d’heure.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Définissez si le type d’heure est un type d’heure général ou spécifique au projet en sélectionnant la portée correcte dans le menu déroulant.</p> <p>Les types d’heures généraux sont visibles uniquement sur les feuilles de temps et ne peuvent pas être associés à des projets, des tâches ou des problèmes.</p> <p><b>IMPORTANT</b> : si vous avez un type d’heure personnalisé qui est [!UICONTROL Project Specific], puis que vous le remplacez par [!UICONTROL General], toutes les tâches, problèmes et heures du projet existants sont définis sur leurs types par défaut du système.</p> </td> 
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

Si les types d’heures deviennent obsolètes et que vous ne souhaitez plus que les utilisateurs et utilisatrices leur associent leurs entrées d’heure, vous pouvez désactiver les types d’heures.

La désactivation des types d’heures masque les types d’heures n’importe où dans [!DNL Workfront] où les types d’heures sont visibles.

Pour désactiver un type d’heure :

{{step-1-to-setup}}

1. Développez **[!UICONTROL Préférences de la feuille de temps et des heures]**, puis cliquez sur **[!UICONTROL Types d’heures]**.

1. Sélectionnez le type d’heure à désactiver.

1. Cliquez sur **[!UICONTROL Désactiver]**.
