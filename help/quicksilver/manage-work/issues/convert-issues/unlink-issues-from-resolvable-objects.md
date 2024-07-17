---
product-area: projects
navigation-topic: convert-issues
title: Dissocier les problèmes de leurs objets de résolution
description: Lorsque vous créez un projet ou une tâche en convertissant un problème au projet ou à la tâche, vous avez la possibilité de conserver le problème d’origine. Votre administrateur Adobe Workfront doit activer cette préférence pour que vous disposiez de cette option lors de la conversion du problème. Pour plus d’informations sur la conversion de problèmes en projets et tâches, voir Présentation de la conversion de problèmes dans Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 22%

---

# Dissocier les problèmes de leurs objets de résolution

Lorsque vous créez un projet ou une tâche en convertissant un problème au projet ou à la tâche, vous avez la possibilité de conserver le problème d’origine. Votre administrateur Adobe Workfront doit activer cette préférence pour que vous disposiez de cette option lors de la conversion du problème.\
Pour plus d’informations sur la conversion de problèmes en projets et tâches, voir [Présentation de la conversion de problèmes dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Lorsque vous décidez de conserver le problème qui a été converti dans le projet ou la tâche, la résolution du problème est liée au projet ou à la tâche. Le problème devient l’objet résolvable du projet ou de la tâche. Le projet ou la tâche sont les objets de résolution du problème.

Vous pouvez également lier manuellement un problème à un autre problème. Le deuxième problème devient l’objet de résolution du premier numéro, dans ce cas.\
Pour plus d’informations sur la résolution d’objets, voir [Présentation de la résolution et de la résolution d’objets résolvables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>Le statut du problème ne peut pas être modifié, car il change automatiquement avec celui de l’objet de résolution.

Vous pouvez dissocier la résolution d’un problème de celle d’un projet, d’une tâche ou d’un problème en supprimant le projet, la tâche ou le problème du problème.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Affichage de l’accès aux tâches et aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations sur le problème</p> <p>Affichage des autorisations sur la tâche ou le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Dissocier un problème d’un projet, d’une tâche ou d’un problème

1. Accédez au problème lié à un projet, une tâche ou un problème.
1. Cliquez sur la section **Détails du problème** .
1. Accédez à la zone **Overview** de la section **Issue Details** .
1. Dans le champ **Résolu par** , supprimez le type d’objet résolvable .\
   Un problème peut être résolu par un projet, une tâche ou un problème.

   Cela supprime l’objet de résolution du problème.

1. Cliquez sur **Enregistrer** **Modifications**.\
   Le problème n’est plus lié à un projet, à une tâche ou à un problème, et vous pouvez désormais le résoudre indépendamment.
