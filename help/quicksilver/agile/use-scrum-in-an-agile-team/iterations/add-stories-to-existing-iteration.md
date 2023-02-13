---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Ajouter des articles à une itération existante
description: Vous pouvez ajouter des articles à une itération de plusieurs façons.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Ajouter des articles à une itération existante

Vous pouvez ajouter des articles à une itération de l’une des manières suivantes :

* Depuis le journal des travaux après la création de l’itération, comme décrit dans la section [Déplacer des articles du journal vers une itération ou [!UICONTROL Kanban] board](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) dans [Gestion du journal en souffrance agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Dans la [!UICONTROL Détails] page de la tâche ou du problème individuel
* À partir d’une tâche ou d’une liste de problèmes
* À partir d’un rapport
* Depuis un tableau de bord

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Gérer] Accès au projet sur lequel se trouve l’article</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Comprendre comment l’ajout d’articles affecte les dates des tâches

Par défaut, lorsque vous ajoutez une tâche existante à une itération, la tâche [!UICONTROL Date de début planifiée] et [!UICONTROL Date d’achèvement prévue] sont définies comme suit :

### Tâche [!UICONTROL Date de début planifiée]

* La tâche utilise la Date de début de l&#39;itération lorsque :

   * Le projet n’a pas de [!UICONTROL Date de début planifiée] définie.
   * Le projet [!UICONTROL Date de début planifiée] is *before* ou *on* date de début de l’itération.

* La tâche utilise le [!UICONTROL Date de début planifiée] lorsque :

   * Le projet [!UICONTROL Date de début planifiée] is *after* date de début de l’itération.

### Tâche [!UICONTROL Date d’achèvement prévue]

* La tâche utilise la Date de fin de l’itération lorsque :

   * Le projet n’a pas de [!UICONTROL Date d’achèvement prévue] définie.
   * Le projet [!UICONTROL Date de début planifiée] is *avant ou après* Date de début de l’itération ou du projet [!UICONTROL Date d’achèvement prévue] is *avant ou après* Date de fin de l’itération.

* La tâche utilise le [!UICONTROL Date d’achèvement prévue] lorsque :

   * Le projet [!UICONTROL Date de début planifiée] is *after* la date de début de l’itération et celle du projet ; [!UICONTROL Date d’achèvement prévue] is *after* Date de fin de l’itération.

Vous pouvez configurer des équipes Scrum individuelles pour utiliser les dates du projet par défaut plutôt que les dates d’itération. Pour plus d’informations, voir la section [Configurer l’application des dates lors de l’ajout d’éléments de travail à une itération](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) dans l’article [Configuration de Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Ajouter un article à une itération existante

Pour ajouter des articles à une itération directement à partir de la tâche ou du problème :

>[!IMPORTANT]
>
>Une fois que la tâche est déplacée vers l’itération, vous ne pouvez pas mettre à jour la variable [!UICONTROL Type de durée] ou [!UICONTROL Contrainte de tâche]. [!UICONTROL Type de durée] est défini sur [!UICONTROL Simple] et [!UICONTROL Contrainte de tâche] est défini sur [!UICONTROL Dates fixes] afin que la chronologie de la tâche reste cohérente avec la chronologie de l’itération.

### Dans l’onglet Tâches ou problèmes

Vous pouvez ajouter n’importe quelle tâche ou problème à n’importe quelle itération si vous disposez de l’option Gérer pour accéder au projet. Gardez les éléments suivants à l’esprit lorsque vous déplacez une tâche ou un problème vers une itération :

* Si vous ajoutez plusieurs équipes, la tâche ou le problème ne peut s’afficher que sur l’itération d’une équipe. Il s’agit de l’itération choisie à l’étape 3 ci-dessous.
* Si la tâche ou le problème est assigné à une équipe agile et déplacé vers l’itération d’une autre équipe, l’affectation de l’équipe ne change pas.
* Si la tâche ou le problème n’est pas assigné à une équipe, la tâche ou le problème est assigné à l’équipe propriétaire de l’itération.
* Vous ne pouvez pas ajouter de tâches parents à l’itération. Si vous ajoutez des tâches enfants, la tâche parente apparaît sur le panneau Scrum sous la forme d’un couloir.

1. Accédez au projet, au rapport ou au tableau de bord qui contient la tâche ou le problème que vous souhaitez ajouter à une itération.
1. Sélectionnez une ou plusieurs tâches ou problèmes.
1. Cliquez sur **[!UICONTROL Plus]** ![](assets/more-icon.png) > **[!UICONTROL Ajouter à l’itération]**.\
   Vous ne pouvez pas affecter de tâches ou de problèmes affectés à des équipes non agiles.

1. Dans le **[!UICONTROL Ajouter des articles]** saisissez le nom de l’itération.

   >[!NOTE]
   >
   >Vous pouvez déplacer un article d’une itération existante vers une nouvelle itération.

1. Si vous ajoutez des tâches, cliquez sur **[!UICONTROL Ajouter des articles]**.\
   Ou\
   Si vous ajoutez des problèmes, cliquez sur **[!UICONTROL Ajout de problèmes]**.
