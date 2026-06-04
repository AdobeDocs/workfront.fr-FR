---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copier un modèle de projet
description: Outre la création d’un modèle de projet à partir de zéro, vous pouvez également copier un modèle existant et le modifier.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/6d0OXEaAdH-569LF5nuQ8wcJd-Iq7KYz8os3IOyx0yA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 327
ht-degree: 44%

---

# Copier un modèle de projet

<!--Audited: 5/2025-->

Outre la création d’un modèle de projet à partir de zéro, vous pouvez également copier un modèle existant et le modifier dans Adobe Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

Vous devez disposer de l’accès suivant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux modèles</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou de niveau supérieur sur un modèle</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a template</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Remarques relatives à la copie de modèles

Les éléments suivants sont toujours copiés d’un modèle existant vers un nouveau :

* Tâches de modèles
* Informations par défaut sur la tâche de modèle (processus d’approbation par défaut de la tâche, formulaires personnalisés par défaut de la tâche)
* Formulaires personnalisés
* Risques
* Informations sur la configuration de la file d’attente
* Portfolio et programme
* Approbations
* Documents
* Les jours des tâches du modèle d’origine sont transférés vers le nouveau modèle. Vous devez modifier le jour de début ou d’achèvement du modèle (en fonction de son mode de planification) pour mettre à jour les jours des tâches du modèle, si nécessaire.

Les éléments suivants ne sont jamais copiés d’un modèle existant vers un nouveau :

* Taux de facturation
* Commentaires des utilisateurs et des utilisatrices

## Copier un modèle

<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. Accédez au modèle à copier.
1. Cliquez sur le menu **Plus** ![icône Plus](assets/more-icon.png) à droite du nom du modèle dans l’en-tête, puis cliquez sur **Copier**.

   La boîte de dialogue **Copier le modèle** s’ouvre.

   ![Zone Copier le modèle](assets/copy-template-box.png)

1. Spécifiez un nom pour le modèle dans le champ **Nouveau nom du modèle**.

   Par défaut, Workfront définit le nouveau nom au format `Copy of Original template name`.

1. Sélectionnez l&#39;option **Conserver les affectations d&#39;utilisateurs pour les tâches et le modèle** si vous souhaitez transférer toutes les affectations de tâches et de modèles du modèle d&#39;origine vers le nouveau modèle. Les affectations de tâches de modèles, ainsi que le Propriétaire et le Sponsor du modèle sont transférés vers le modèle copié.
1. Cliquez sur **Enregistrer** pour créer une copie du modèle.

   Le nouveau modèle s’affiche dans la liste des modèles de la zone Modèle de Workfront.
