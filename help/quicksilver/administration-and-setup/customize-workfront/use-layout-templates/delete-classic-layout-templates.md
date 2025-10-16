---
title: Supprimer des modèles de mise en page classiques
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Les modèles de mise en page de l’expérience Workfront classique ne sont plus disponibles dans l’interface Workfront, mais peuvent tout de même affecter les données Workfront. Cela peut entraîner des incohérences dans les champs affectés par les modèles de mise en page (tels que Partagé avec) sur les rapports ou les tableaux de bord.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 97%

---

# Supprimer les modèles de mise en page classiques

Les modèles de mise en page de l’expérience Workfront classique ne sont plus disponibles dans l’interface Workfront, mais peuvent tout de même affecter les données Workfront. Cela peut entraîner des incohérences dans les champs affectés par les modèles de mise en page (tels que Partagé avec) sur les rapports ou les tableaux de bord.

Vous pouvez résoudre ces incohérences en supprimant les modèles de mise en page classiques. Comme ceux-ci ne sont pas disponibles dans l’interface Workfront, vous devez utiliser l’API Workfront pour les supprimer.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.</p>
        <p>Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Supprimer les modèles de mise en page classiques à l’aide d’un appel API

Vous pouvez saisir des appels API dans la barre d’URL de votre navigateur et appuyer sur la touche Entrée. La réponse de l’API s’affiche dans votre navigateur.

>[!NOTE]
>
>Les modèles de mise en page globaux et de système ne peuvent pas être supprimés.

1. Connectez-vous à Workfront.
1. Recherchez le modèle de mise en page à supprimer à l’aide de l’appel API suivant :
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. Notez l’ID du modèle de mise en page à supprimer.
1. Recherchez votre ID de session à l’aide de l’appel API suivant :
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >Ne partagez jamais votre ID de session avec qui que ce soit.

1. Insérez l’ID du modèle de mise en page et l’ID de session dans l’appel API suivant :
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Collez l’appel API de l’étape 4 dans la barre d’URL de votre navigateur et appuyez sur Entrée.

   Le modèle de mise en page est ainsi supprimé.
