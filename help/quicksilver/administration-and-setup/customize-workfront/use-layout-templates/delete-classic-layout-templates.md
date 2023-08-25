---
title: Suppression de modèles de mise en page classiques
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Les modèles de mise en page de l’expérience Workfront classique ne sont plus disponibles dans l’interface de Workfront, mais peuvent tout de même affecter les données Workfront. Cela peut entraîner des incohérences dans les champs affectés par les modèles de mise en page (tels que Partagés avec) sur les rapports ou les tableaux de bord.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c68b63230b07ea8c8475b710e256b5e0f049b1eb
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Accorder un accès administratif à un modèle de mise en page

Les modèles de mise en page de l’expérience Workfront classique ne sont plus disponibles dans l’interface de Workfront, mais peuvent tout de même affecter les données Workfront. Cela peut entraîner des incohérences dans les champs affectés par les modèles de mise en page (tels que Partagés avec) sur les rapports ou les tableaux de bord.

Vous pouvez résoudre ces incohérences en supprimant les modèles de mise en page Classic. Comme elles ne sont pas disponibles dans l’interface de Workfront, utilisez l’API Workfront pour les supprimer.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur système.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Suppression des modèles de mise en page Classic à l’aide d’un appel API

Vous pouvez saisir des appels d’API dans la barre d’URL de votre navigateur et appuyer sur Entrée. La réponse de l’API s’affiche dans votre navigateur.

>[!NOTE]
>
>Les modèles de mise en page globale et système ne peuvent pas être supprimés.

1. Connectez-vous à Workfront.
1. Recherchez le modèle de mise en page que vous souhaitez supprimer à l’aide de l’appel API suivant :
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. Notez l’identifiant du modèle de mise en page que vous souhaitez supprimer.
1. Recherchez votre ID de session à l’aide de l’appel API suivant :
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >Ne partagez jamais votre ID de session avec personne.

1. Insérez l’identifiant du modèle de mise en page et l’identifiant de session dans l’appel API suivant :
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Collez l’appel API de l’étape 4 dans la barre d’URL de votre navigateur et appuyez sur Entrée.

   Le modèle de mise en page est ainsi supprimé.



