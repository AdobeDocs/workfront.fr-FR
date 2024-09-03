---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copier un modèle de projet
description: Au lieu de créer entièrement un modèle de projet, vous pouvez copier un modèle existant et y apporter des modifications, si nécessaire.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 100%

---

# Copier un modèle de projet

Au lieu de créer entièrement un modèle de projet, vous pouvez copier un modèle existant et y apporter des modifications, si nécessaire.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux modèles</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou de niveau supérieur sur un modèle</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.


## Remarques relatives à la copie de modèles

Les éléments suivants sont toujours copiés d’un projet existant vers un nouveau :

* Tâches de modèles
* Informations par défaut sur la tâche de modèle (processus d’approbation par défaut de la tâche, formulaires personnalisés par défaut de la tâche)
* Formulaires personnalisés dans mon groupe
* Risques
* Informations sur la configuration de la file d’attente
* Portfolio et programme
* Approbations
* Documents
* Les jours des tâches du modèle d’origine sont transférés vers le nouveau modèle. Vous devez modifier le jour de début ou d’achèvement du modèle (en fonction de son mode de planification) pour mettre à jour les jours des tâches du modèle, si nécessaire.

Les éléments suivants ne sont jamais copiés d’un projet existant vers un nouveau :

* Taux de facturation
* Commentaires des utilisateurs et des utilisatrices

## Copier un modèle

1. Accédez au modèle à copier.
1. Cliquez sur le menu **Plus** ![](assets/qs-more-icon-on-an-object.png), puis sur **Copier**.
1. Spécifiez un nom pour le modèle dans le champ **Nouveau nom du modèle**.

   Par défaut, le nouveau nom est **Copie de `<original template name>`.**

1. Indiquez si vous souhaitez **Conserver les affectations d’utilisateurs et d’utilisatrices sur les tâches et le modèle** : sélectionnez cette option pour transférer toutes les affectations de tâche et de modèle du modèle d’origine vers le nouveau.
1. Cliquez sur **Enregistrer** pour créer une copie du modèle.
