---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copier un modèle de projet
description: Au lieu de créer un modèle de projet entièrement nouveau, vous pouvez copier un modèle existant et y apporter des modifications, si nécessaire.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 34%

---

# Copier un modèle de projet

Au lieu de créer un modèle de projet entièrement nouveau, vous pouvez copier un modèle existant et y apporter des modifications, si nécessaire.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux modèles</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures d’un modèle</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.


## Observations relatives à la copie de modèles

Les éléments suivants sont toujours copiés d’un projet existant vers un nouveau :

* Tâches de modèles
* Modèle Tâche Informations par défaut (Processus d’approbation par défaut de la tâche, Tâche par défaut Forms personnalisé)
* Formulaires personnalisés dans mon groupe
* Risques
* Informations sur la configuration de la file
* Portfolio et programme
* Approbations
* Documents
* Les jours des tâches du modèle d’origine sont transférés vers le nouveau modèle. Vous devez modifier le jour de début ou de fin du modèle (en fonction de son mode de planification) pour mettre à jour les jours des tâches du modèle, si nécessaire.

Les éléments suivants ne sont jamais copiés d’un projet existant vers un nouveau :

* Taux de facturation
* Commentaires des utilisateurs

## Copier un modèle

1. Accédez au modèle que vous souhaitez copier.
1. Cliquez sur le menu **Plus** ![](assets/qs-more-icon-on-an-object.png), puis sur **Copier**.
1. Spécifiez un nom pour le modèle dans le champ **Nouveau nom de modèle**.

   Par défaut, le nouveau nom est **Copie de `<original template name>`.**

1. Choisissez si vous souhaitez **Conserver les affectations d’utilisateurs sur les tâches et le modèle** : sélectionnez cette option pour effectuer toutes les affectations de tâche et de modèle du modèle d’origine vers le nouveau modèle.
1. Cliquez sur **Enregistrer** pour créer une copie du modèle.
