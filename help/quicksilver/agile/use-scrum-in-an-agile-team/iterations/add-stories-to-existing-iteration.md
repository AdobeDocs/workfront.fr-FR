---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Ajouter des utilisateurs et utilisatrices à une itération existante
description: Vous pouvez ajouter des articles à une itération de plusieurs façons.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 11%

---

# Ajouter des utilisateurs et utilisatrices à une itération existante

Vous pouvez ajouter des articles à une itération de l’une des manières suivantes :

* À partir du journal après la création de l’itération, comme décrit dans la section [Déplacer des articles du journal vers une itération ou [!UICONTROL panorama Kanban]](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) de [Gérer le journal agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Sur la page [!UICONTROL Détails] de la tâche ou du problème individuel
* À partir d’une tâche ou d’une liste de problèmes
* À partir d’un rapport
* Depuis un tableau de bord

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Gérer] Accès au projet sur lequel se trouve l’article</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Comprendre comment l’ajout d’articles affecte les dates des tâches

Par défaut, lorsque vous ajoutez une tâche existante à une itération, les [!UICONTROL Date de début planifiée] et [!UICONTROL Date de fin planifiée] de la tâche sont définies comme suit :

### Tâche [!UICONTROL Date de début planifiée]

* La tâche utilise la Date de début de l&#39;itération lorsque :

   * Le projet n’a pas de [!UICONTROL Date de début planifiée] définie.
   * La [!UICONTROL date de début planifiée] du projet est *avant* ou *le* date de début de l’itération.

* La tâche utilise la [!UICONTROL date de début planifiée] du projet lorsque :

   * La [!UICONTROL date de début planifiée] du projet est *après* la date de début de l’itération.

### Tâche [!UICONTROL Date d’achèvement planifiée]

* La tâche utilise la Date de fin de l’itération lorsque :

   * Le projet n’a pas de [!UICONTROL Date d’achèvement planifiée] définie.
   * La [!UICONTROL date de début planifiée] du projet est *avant ou le* la date de début de l’itération ou la [!UICONTROL date d’achèvement planifiée] du projet est *avant ou le* la date de fin de l’itération.

* La tâche utilise la [!UICONTROL date d’achèvement planifiée] du projet lorsque :

   * La [!UICONTROL date de début planifiée] du projet est *après* la date de début de l’itération et la [!UICONTROL date d’achèvement planifiée] du projet est *après* la date de fin de l’itération.

Vous pouvez configurer des équipes Scrum individuelles pour utiliser les dates du projet par défaut plutôt que les dates d’itération. Pour plus d’informations, reportez-vous à la section [Configuration de la manière dont les dates sont appliquées lors de l’ajout d’éléments de travail à une itération](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) dans l’article [Configurer le graphique](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Ajouter un article à une itération existante

Pour ajouter des articles à une itération directement à partir de la tâche ou du problème :

>[!IMPORTANT]
>
>Une fois que la tâche est déplacée vers l’itération, vous ne pouvez pas mettre à jour le [!UICONTROL type de durée] ou la [!UICONTROL contrainte de tâche]. [!UICONTROL Le type de durée] est défini sur [!UICONTROL Simple] et [!UICONTROL Contrainte de tâche] est défini sur [!UICONTROL Dates fixes] pour conserver la chronologie de la tâche cohérente avec la chronologie de l’itération.

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

1. Dans la zone **[!UICONTROL Ajouter des articles]**, saisissez le nom de l’itération.

   >[!NOTE]
   >
   >Vous pouvez déplacer un article d’une itération existante vers une nouvelle itération.

1. Si vous ajoutez des tâches, cliquez sur **[!UICONTROL Ajouter des articles]**.\
   Ou\
   Si vous ajoutez des problèmes, cliquez sur **[!UICONTROL Ajouter des problèmes]**.
