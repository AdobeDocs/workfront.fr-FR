---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Exemple de champ personnalisé calculé : afficher un horodatage d’état dans un formulaire personnalisé"
description: Le champ calculé suivant affiche la date à laquelle l’état de l’objet est marqué comme En cours (INP). Vous pouvez utiliser les mêmes informations pour les champs personnalisés calculés pour les problèmes, les tâches ou les projets.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 20%

---

# Exemple de champ personnalisé calculé : affichage d’un horodatage d’état dans un formulaire personnalisé

Le champ calculé suivant affiche la date à laquelle l’état de l’objet est marqué comme En cours (INP). Vous pouvez utiliser les mêmes informations pour les champs personnalisés calculés pour les problèmes, les tâches ou les projets.

>[!NOTE]
>
>Si l’état de l’objet passe à INP, puis à un autre état, puis à nouveau à INP, Adobe Workfront capture uniquement l’horodatage de la première modification à INP.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Forfait Adobe Workfront*</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Modifier l’accès à Créer des rapports, des tableaux de bord et des calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorisations d’objets</strong> </p> </td> 
   <td> <p>Gérer les autorisations sur l’objet auquel le formulaire est joint</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.<br>Pour plus d’informations sur les autorisations des tableaux de bord, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref"> Partage de rapports, de tableaux de bord et de calendriers </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Condition requise

Pour ajouter un champ calculé qui affiche l’historique de modification d’un champ à un formulaire personnalisé, vous devez d’abord créer le formulaire personnalisé.

## Affichage d’un horodatage d’état dans un formulaire personnalisé

1. Accédez à un formulaire personnalisé dans lequel vous souhaitez ajouter le champ.
1. Cliquez sur **Calculé** pour ajouter un champ personnalisé calculé au formulaire.
1. Saisissez un **Libellé** pour le champ personnalisé, par exemple *Champ personnalisé Horodatage d’état*.
1. Cliquez sur **Terminé**, puis sur **Enregistrer+Fermer**.
1. rouvrez le formulaire personnalisé, puis sélectionnez le nouveau **champ personnalisé Horodatage d’état** sur le formulaire.
1. Dans la zone **Calcul**, copiez et collez le calcul suivant pour votre champ personnalisé :

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Ce calcul est identique pour tous les objets et pour tous les états. Dans ce calcul, vous devez toujours utiliser la clé à trois lettres, et non le nom d’état de l’objet.
   >
   >Pour plus d’informations sur les clés pour les états, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Cliquez sur **Enregistrer+Fermer**.

   Vous pouvez désormais créer des rapports sur le champ personnalisé Horodatage d’état ou l’utiliser dans d’autres calculs, dans des rapports ou dans des champs personnalisés.
