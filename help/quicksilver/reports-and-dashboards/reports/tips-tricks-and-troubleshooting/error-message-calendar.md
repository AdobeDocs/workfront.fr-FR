---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Message d’erreur sur le calendrier : "Ce calendrier dispose des droits d’affichage d’un utilisateur désactivé.""'
description: Découvrez le message d’erreur "Ce calendrier a les droits d’affichage d’un utilisateur désactivé".
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 6%

---

# Message d’erreur sur le calendrier : &quot;Ce calendrier dispose des droits d’affichage d’un utilisateur désactivé.&quot;

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Planifier, travailler</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un calendrier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Problème

Vous recevez l’erreur suivante lors de l’accès à un calendrier partagé avec vous : 

*Ce calendrier dispose des droits d&#39;affichage d&#39;un utilisateur désactivé. Demandez à un administrateur de corriger les privilèges de calendrier.*

## Cause

L’utilisateur qui a créé ce calendrier (son propriétaire d’origine) est un utilisateur qui a été désactivé. 

## Solution

Vous pouvez résoudre ce problème de la manière suivante :

1. Copiez le calendrier d&#39;origine. Lorsque vous copiez un calendrier, vous en devenez le propriétaire. Le calendrier copié doit afficher toutes les informations du calendrier original.\
   Pour plus d’informations sur la copie d’un calendrier, voir [Copier un rapport de calendrier](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Partagez le calendrier copié avec les mêmes utilisateurs que le calendrier original. Tous les utilisateurs doivent voir les mêmes informations dans le nouveau calendrier.
1. (Facultatif et conditionnel) Si vous êtes autorisé à gérer le calendrier d’origine, supprimez tous les autres utilisateurs avec lesquels le calendrier est partagé dans la zone Partage du calendrier. Cela évite la confusion des utilisateurs qui tentent d’afficher un mauvais calendrier.
