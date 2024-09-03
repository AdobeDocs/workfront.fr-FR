---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: '« Exemple de champ personnalisé calculé : afficher la date et l’heure d’un statut dans un formulaire personnalisé »'
description: Le champ calculé suivant affiche la date à laquelle le statut de l’objet est marqué comme étant en cours. Vous pouvez utiliser les mêmes informations des champs personnalisés calculés pour les problèmes, les tâches ou les projets.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 100%

---

# Exemple de champ personnalisé calculé : afficher la date et l’heure d’un statut dans un formulaire personnalisé

Le champ calculé suivant affiche la date à laquelle le statut de l’objet est marqué comme étant en cours. Vous pouvez utiliser les mêmes informations des champs personnalisés calculés pour les problèmes, les tâches ou les projets.

>[!NOTE]
>
>Si le statut de l’objet passe à En cours, puis à un autre statut, puis de nouveau à En cours, Adobe Workfront ne saisit que la date et l’heure du premier passage au status En cours.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Accès en modification à la création de rapports, de tableaux de bord et de calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, consultez <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorisations d’objet</strong> </p> </td> 
   <td> <p>Autorisations de gestion pour l’objet auquel le formulaire est attaché</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.<br>Pour plus d’informations sur les autorisations relatives aux tableaux de bord, consultez la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Partager des rapports, des tableaux de bord et des calendriers </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prérequis

Pour ajouter un champ calculé qui affiche l’historique des modifications d’un champ dans un formulaire personnalisé, vous devez d’abord créer le formulaire personnalisé.

## Afficher la date et l’heure d’un statut dans un formulaire personnalisé

1. Accédez au formulaire personnalisé dans lequel vous souhaitez ajouter le champ.
1. Cliquez sur **Calculé** pour ajouter un champ personnalisé calculé au formulaire.
1. Saisissez un **libellé** pour le champ personnalisé, par exemple *Champ personnalisé Date et heure du statut*.
1. Cliquez sur **Terminé**, puis sur **Enregistrer et fermer**.
1. Rouvrez le formulaire personnalisé, puis sélectionnez le nouveau **Champ personnalisé Date et heure du statut** dans le formulaire.
1. Dans la zone **Calcul**, copiez et collez le calcul suivant pour votre champ personnalisé :

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Ce calcul est identique pour tous les objets et pour tous les statuts. Dans ce calcul, vous devez toujours utiliser la clé à trois lettres et non le nom du statut de l’objet.
   >
   >Pour plus d’informations sur les clés des statuts, consultez la section [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Cliquez sur **Enregistrer + Fermer**.

   Vous pouvez désormais établir des rapports sur le champ personnalisé « Date et heure du statut » ou l’utiliser dans d’autres calculs, des rapports ou des champs personnalisés.
