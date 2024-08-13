---
title: Suppression de modèles de mise en page classiques
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Les modèles de disposition de l’expérience Workfront classique ne sont plus disponibles dans l’interface Workfront, mais peuvent tout de même affecter les données Workfront. Cela peut entraîner des incohérences dans les champs affectés par les modèles de disposition (tels que Partagé avec) sur les rapports ou les tableaux de bord.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 68%

---

# Accorder un accès administratif à un modèle de mise en page

Les modèles de disposition de l’expérience Workfront classique ne sont plus disponibles dans l’interface Workfront, mais peuvent tout de même affecter les données Workfront. Cela peut entraîner des incohérences dans les champs affectés par les modèles de disposition (tels que Partagé avec) sur les rapports ou les tableaux de bord.

Vous pouvez résoudre ces incohérences en supprimant les modèles de mise en page Classic. Comme elles ne sont pas disponibles dans l’interface de Workfront, utilisez l’API Workfront pour les supprimer.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur système.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Supprimer les modèles de disposition classiques à l’aide d’un appel API

Vous pouvez saisir des appels d’API dans la barre d’URL de votre navigateur et appuyer sur Entrée. La réponse de l’API s’affiche dans votre navigateur.

>[!NOTE]
>
>Les modèles de disposition globaux et de système ne peuvent pas être supprimés.

1. Connectez-vous à Workfront.
1. Recherchez le modèle de disposition à supprimer à l’aide de l’appel API suivant :
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. Notez l’ID du modèle de disposition à supprimer.
1. Recherchez votre ID de session à l’aide de l’appel API suivant :
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >Ne partagez jamais votre ID de session avec qui que ce soit.

1. Insérez l’ID du modèle de disposition et l’ID de session dans l’appel API suivant :
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Collez l’appel API de l’étape 4 dans la barre d’URL de votre navigateur et appuyez sur Entrée.

   Le modèle de disposition est ainsi supprimé.
