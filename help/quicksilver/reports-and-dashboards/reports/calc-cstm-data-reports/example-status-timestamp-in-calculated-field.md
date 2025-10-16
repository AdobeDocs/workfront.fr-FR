---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Exemple de champ personnalisé calculé : afficher la date et l’heure d’un statut dans un formulaire personnalisé'
description: Le champ calculé suivant affiche la date à laquelle l'état de l'objet est marqué comme étant En cours (INP). Vous pouvez utiliser les mêmes informations des champs personnalisés calculés pour les problèmes, les tâches ou les projets.
author: Jenny
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 85%

---

# Exemple de champ personnalisé calculé : afficher la date et l’heure d’un statut dans un formulaire personnalisé

Le champ calculé suivant affiche la date à laquelle l&#39;état de l&#39;objet est marqué comme étant En cours (INP). Vous pouvez utiliser les mêmes informations des champs personnalisés calculés pour les problèmes, les tâches ou les projets.

>[!NOTE]
>
>Si le statut de l’objet passe à En cours, puis à un autre statut, puis de nouveau à En cours, Adobe Workfront ne saisit que la date et l’heure du premier passage au status En cours.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Package Adobe Workfront</p> </td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Configurations des niveaux d’accès</p></td> 
   <td> <p>Accès en modification à la création de rapports, de tableaux de bord et de calendriers</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorisations d’objet</p> </td> 
   <td> <p>Autorisations de gestion pour l’objet auquel le formulaire est attaché</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prérequis

Pour ajouter un champ calculé qui affiche l’historique des modifications d’un champ dans un formulaire personnalisé, vous devez d’abord créer le formulaire personnalisé.

## Afficher la date et l’heure d’un statut dans un formulaire personnalisé

1. Accédez au formulaire personnalisé dans lequel vous souhaitez ajouter le champ.
1. Cliquez sur **Calculé** pour ajouter un champ personnalisé calculé au formulaire.
1. Saisissez un **Libellé** pour le champ personnalisé. Par exemple, « Champ personnalisé Horodatage de statut ».
1. Cliquez sur **Enregistrer et fermer**.
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
