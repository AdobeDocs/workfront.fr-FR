---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Personnaliser les types d'événements par défaut
description: Vous pouvez personnaliser les libellés de chaque type de problème par défaut afin qu’ils correspondent mieux à la terminologie utilisée dans votre organisation. Les types de problème sont utiles pour personnaliser les statuts des problèmes et créer des files d’attente des demandes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 90%

---

# Personnaliser les types de problèmes par défaut

Les types de problème sont utiles dans les circonstances suivantes :

* Lorsque vous personnalisez les statuts des problèmes, comme décrit dans [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* Lorsque vous créez une file d’attente des demandes, comme décrit dans [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Vous pouvez personnaliser les libellés de chaque type de problème par défaut afin qu’ils correspondent mieux à la terminologie utilisée dans votre organisation.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Types de problème par défaut

Si vous disposez d’un accès [!UICONTROL administrateur ou administratrice] [!DNL Adobe Workfront], vous pouvez configurer et renommer quatre types de problème par défaut :

* **[!UICONTROL Rapport sur les bugs]** Utilisé pour suivre les bugs signalés dans le système.
* **[!UICONTROL Ordre de modification]** Utilisé pour suivre les problèmess qui doivent être mis à jour ou révisés.
* **[!UICONTROL Problème]** Objet dans [!DNL Workfront] qui communique un travail non planifié, un problème qui se pose ou quelque chose qui doit être résolu afin de poursuivre une tâche.
* **[!UICONTROL Demande]** Type de problème qui s’applique à une file d’attente des demandes dans laquelle les personnes font des demandes dans Workfront.

![Types de problème par défaut](assets/default-issue-types.png)

## Personnaliser un type de problème

Tenez compte de ce qui suit pour la personnalisation des types de problème :

* Vous pouvez modifier le libellé d’un type de problème, mais vous ne pouvez pas modifier sa fonction.
* Vous ne pouvez pas créer d’autres types de problème.
* Vous ne pouvez pas modifier les valeurs du filtre pour le nom d’un type de problème. Ainsi, si vous créez un filtre sur un rapport de problèmes, la valeur du filtre (clé) ne reflète pas le nom personnalisé du type de problème.
* Trois statuts par défaut sont associés à chaque type de problème : [!UICONTROL Nouveau], [!UICONTROL En cours] et [!UICONTROL Fermé]. Vous ne pouvez pas supprimer ces statuts ou les retirer d’un type de problème, mais vous pouvez les renommer.
* Vous pouvez réorganiser les options qui apparaissent dans le menu déroulant pour chaque type de problème.

Pour personnaliser un type de problème :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Statuts]**.

1. Cliquez sur l’onglet **[!UICONTROL Problèmes]**.
1. Effectuez l’une des opérations suivantes :

   * Pointez sur le type d’événement à personnaliser, cliquez sur l’icône [!UICONTROL Modifier] ![Icône Modifier](assets/edit-icon.png) qui s’affiche à l’extrémité droite, puis saisissez un nouveau nom pour le type d’événement.

     ![Personnaliser le type d&#39;événement](assets/customize-issue-type.png)

   * Cliquez sur un [!UICONTROL type de problème] pour afficher la liste des statuts associés, puis faites glisser les poignées qui apparaissent lorsque vous pointez sur eux et déposez-les dans l’ordre dans lequel vous souhaitez qu’ils apparaissent dans le menu déroulant du **[!UICONTROL Statut]** des problèmes de vos utilisateurs et utilisatrices.
