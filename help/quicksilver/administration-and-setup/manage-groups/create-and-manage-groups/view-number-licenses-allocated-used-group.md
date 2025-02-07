---
title: Afficher le nombre de licences attribuées et utilisées dans un groupe
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez afficher le décompte des différents types de licences actuellement utilisées dans votre groupe et ses sous-groupes. Cette fonction est utile lorsque vous devez déterminer s’il convient de redistribuer les licences.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 91%

---

# Afficher le nombre de licences attribuées et utilisées dans un groupe

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez afficher le décompte des différents types de licences actuellement utilisées dans votre groupe et ses sous-groupes. Cette fonction est utile lorsque vous devez déterminer s’il convient de redistribuer les licences.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

>[!IMPORTANT]
>
>La licence d’un utilisateur ou d’une utilisatrice n’est comptabilisée dans un groupe particulier que si ce groupe est le groupe interne de cette personne.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher le nombre de licences utilisées dans un groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

1. Cliquez sur le nom du groupe.
1. Sur la page qui s’affiche, dans la zone d’en-tête située en haut à droite, consultez la zone **Licences utilisées** pour connaître le nombre de licences **Plan** et **Travail** actuellement utilisées.

   Si vous visualisez un groupe de premier niveau et que l’administrateur ou l’administratrice Workfront a défini un nombre maximum de chaque type de licence pour le groupe, ces nombres sont également affichés. Par exemple, dans le groupe ci-dessous, au maximum 10 utilisateurs et utilisatrices peuvent disposer d’une licence Plan et au maximum 15 utilisateurs et utilisatrices peuvent disposer d’une licence Travail :

   ![Licences attribuées](assets/licenses-used-allocated.png)

   Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront définit un nombre maximum de licences attribuées à un groupe, voir la section [Définir le nombre maximum de licences pour un groupe interne](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) dans l’article [Gérer les licences disponibles dans votre système](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Si le groupe que vous examinez est un sous-groupe, vous ne pouvez visualiser que le nombre de licences utilisées, et non le nombre maximum de licences attribuées au groupe. En effet, les administrateurs et administratrices Workfront ne définissent pas de nombre maximum de licences pour un sous-groupe.
   >
   >![Licences utilisées dans le sous-groupe](assets/subgroup-used-licenses-only.png)
   >

1. Pour obtenir un décompte séparé de chaque type de licence actuellement utilisé dans le groupe (y compris Révision et Demande), cliquez sur la zone de texte située juste sous **Licences utilisées :**

   ![Cliquez pour en savoir plus](assets/click-text-to-see-more.png)

   La zone qui s’affiche fournit les mêmes informations pour les quatre types de licence Workfront : Plan, Travail, Révision et Demande. En bas de la zone, vous pouvez voir le nombre total de licences utilisées par les personnes membres de ce groupe ou de l’un de ses sous-groupes :

   ![Informations de licence supplémentaires](assets/more-license-info.png)

   Pour les licences Révision et Demande, la colonne Max affiche toujours Illimité.
