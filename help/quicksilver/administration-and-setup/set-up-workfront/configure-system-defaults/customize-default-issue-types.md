---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Personnalisation des types de problèmes par défaut
description: Vous pouvez personnaliser les étiquettes pour chaque type de problème par défaut afin de mieux correspondre à la terminologie utilisée dans votre entreprise. Les types de problème sont utiles pour personnaliser les états de problème et créer des files d’attente de requête.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Personnalisation des types de problèmes par défaut

Les types de problèmes sont utiles dans les cas suivants :

* Lors de la personnalisation des états de problème, comme décrit dans la section [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* Lors de la création d’une file d’attente de demandes, comme décrit dans [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Vous pouvez personnaliser les étiquettes pour chaque type de problème par défaut afin de mieux correspondre à la terminologie utilisée dans votre entreprise.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Types de problèmes par défaut

Si vous avez [!DNL Adobe Workfront] [!UICONTROL administrator] , vous pouvez configurer et renommer quatre types de problèmes par défaut :

* **[!UICONTROL Rapport de bogues]** Utilisé pour effectuer le suivi des bogues signalés dans le système.
* **[!UICONTROL Modifier l’ordre]** Utilisé pour effectuer le suivi des problèmes qui doivent être mis à jour ou modifiés.
* **[!UICONTROL Problème]** Un objet dans [!DNL Workfront] qui communique un travail non planifié, un problème qui survient ou quelque chose qui doit être résolu pour continuer une tâche.
* **[!UICONTROL Requête]** Type de problème qui s’applique à une file d’attente de requêtes dans laquelle les utilisateurs effectuent des requêtes dans Workfront.

![](assets/default-issue-types.png)

## Personnalisation d’un type de problème

Tenez compte des points suivants concernant la personnalisation des types de problèmes :

* Vous pouvez modifier le libellé d’un type de problème, mais vous ne pouvez pas en modifier la fonction.
* Vous ne pouvez pas créer d’autres types de problèmes.
* Vous ne pouvez pas modifier les valeurs de filtre pour le nom d’un type de problème. Ainsi, si vous créez un filtre sur un rapport de problème, la valeur du filtre (clé) ne reflète pas le nom personnalisé du type de problème.
* Trois statuts par défaut sont associés à chaque type de problème : [!UICONTROL Nouveau], [!UICONTROL En cours], et [!UICONTROL Fermé]. Vous ne pouvez pas supprimer ces états ou les supprimer d’un type de problème, mais vous pouvez les renommer.
* Vous pouvez réorganiser les options qui s’affichent dans le menu déroulant pour chaque type de problème.

Pour personnaliser un type de problème :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Statuts]**.

1. Cliquez sur le bouton **[!UICONTROL Problèmes]** .
1. Effectuez l’une des opérations suivantes :

   * Passez la souris sur le type de problème que vous souhaitez personnaliser, puis cliquez sur le bouton [!UICONTROL Modifier] icon ![](assets/edit-icon.png) qui s’affiche à l’extrême droite, puis saisissez un nouveau nom pour le type de problème.

      ![](assets/customize-issue-type.png)

   * Cliquez sur un [!UICONTROL type de problème] pour répertorier les états associés, faites glisser les poignées qui s’affichent lorsque vous pointez dessus, puis déposez-les dans l’ordre dans lequel vous souhaitez qu’elles apparaissent dans le problème de vos utilisateurs. **[!UICONTROL État]** menu déroulant.
