---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Personnalisation des types de problème par défaut
description: Vous pouvez personnaliser les étiquettes pour chaque type de problème par défaut afin de mieux correspondre à la terminologie utilisée dans votre entreprise. Les types de problème sont utiles pour personnaliser les états de problème et créer des files d’attente de requête.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 15%

---

# Personnalisation des types de problèmes par défaut

Les types de problèmes sont utiles dans les cas suivants :

* Lors de la personnalisation des états de problème, comme décrit dans [Créer ou modifier un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* Lors de la création d’une file d’attente de requêtes, comme décrit dans [Création d’une file d’attente de requêtes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Vous pouvez personnaliser les étiquettes pour chaque type de problème par défaut afin de mieux correspondre à la terminologie utilisée dans votre entreprise.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
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

+++

## Types de problèmes par défaut

Si vous disposez de l’accès [!DNL Adobe Workfront] [!UICONTROL administrateur], vous pouvez configurer et renommer quatre types de problèmes par défaut :

* **[!UICONTROL Rapport de bogues]** Utilisé pour effectuer le suivi des bogues signalés dans le système.
* **[!UICONTROL Modifier l’ordre]** Utilisé pour effectuer le suivi des problèmes qui doivent être mis à jour ou modifiés.
* **[!UICONTROL Problème]** Objet dans [!DNL Workfront] qui communique un travail non planifié, un problème qui survient ou quelque chose qui doit être résolu pour continuer une tâche.
* **[!UICONTROL Requête]** Type de problème qui s’applique à une file d’attente de requêtes dans laquelle les utilisateurs effectuent des requêtes dans Workfront.

![](assets/default-issue-types.png)

## Personnalisation d’un type de problème

Tenez compte des points suivants concernant la personnalisation des types de problèmes :

* Vous pouvez modifier le libellé d’un type de problème, mais pas sa fonction.
* Vous ne pouvez pas créer d’autres types de problèmes.
* Vous ne pouvez pas modifier les valeurs de filtre pour le nom d’un type de problème. Ainsi, si vous créez un filtre sur un rapport de problème, la valeur du filtre (clé) ne reflète pas le nom personnalisé du type de problème.
* Trois états par défaut sont associés à chaque type de problème : [!UICONTROL New], [!UICONTROL In Progress] et [!UICONTROL Closed]. Vous ne pouvez pas supprimer ces états ou les supprimer d’un type de problème, mais vous pouvez les renommer.
* Vous pouvez réorganiser les options qui s’affichent dans le menu déroulant pour chaque type de problème.

Pour personnaliser un type de problème :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL États]**.

1. Cliquez sur l’onglet **[!UICONTROL Problèmes]** .
1. Effectuez l’une des opérations suivantes :

   * Passez la souris sur le type de problème à personnaliser, cliquez sur l’icône [!UICONTROL Modifier] ![](assets/edit-icon.png) qui s’affiche à l’extrême droite, puis saisissez un nouveau nom pour le type de problème.

     ![](assets/customize-issue-type.png)

   * Cliquez sur un [!UICONTROL type de problème] pour répertorier les états associés, puis faites glisser les poignées qui apparaissent lorsque vous les survolez et déposez-les dans l’ordre dans lequel vous souhaitez qu’elles apparaissent dans le menu déroulant **[!UICONTROL État]** de la question de vos utilisateurs.
