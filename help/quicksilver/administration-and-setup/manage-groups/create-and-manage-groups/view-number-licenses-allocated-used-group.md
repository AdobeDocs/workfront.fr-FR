---
title: Afficher le nombre de licences attribuées et utilisées dans un groupe
description: En tant qu’administrateur d’Adobe Workfront, vous pouvez consulter le nombre des différents types de licences actuellement utilisés dans votre groupe et dans ses sous-groupes. Cela s’avère utile lorsque vous devez évaluer la redistribution des licences.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Afficher le nombre de licences attribuées et utilisées dans un groupe

En tant qu’administrateur d’Adobe Workfront, vous pouvez consulter le nombre des différents types de licences actuellement utilisés dans votre groupe et dans ses sous-groupes. Cela s’avère utile lorsque vous devez évaluer la redistribution des licences.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

>[!IMPORTANT]
>
>La licence d’un utilisateur n’est comptabilisée dans un groupe particulier que si le groupe est le groupe d’accueil de l’utilisateur.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Formule Workfront</a>*</td> 
   <td> <p>Equipe ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Licence Adobe Workfront</a>*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur de groupe du groupe ou un administrateur Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Afficher le nombre de licences utilisées dans un groupe

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe.
1. Sur la page qui s’affiche, dans la zone d’en-tête située dans le coin supérieur droit, affichez la variable **Licences en cours d’utilisation** pour afficher le nombre de **Plan** et **Travail** licences en cours d’utilisation.

   Si vous affichez un groupe de niveau supérieur et que l’administrateur Workfront a défini un nombre maximal de chaque type de licence pour le groupe, ces nombres s’affichent également. Par exemple, dans le groupe ci-dessous, 10 utilisateurs au maximum peuvent disposer d’une licence Plan et 15 d’une licence Work :

   ![](assets/licenses-used-allocated.png)

   Pour plus d’informations sur la façon dont un administrateur Workfront définit un nombre maximal de licences allouées pour un groupe, reportez-vous à la section . [Définition du nombre maximal de licences pour un groupe d’accueil](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) dans l’article [Gestion des licences disponibles dans votre système](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Si le groupe que vous observez est un sous-groupe, vous ne pouvez afficher que le nombre de licences utilisées, et non le nombre maximal de licences attribuées au groupe. Cela est dû au fait que les administrateurs de Workfront ne définissent pas de nombre maximal de licences pour un sous-groupe.
   >
   >![](assets/subgroup-used-licenses-only.png)

1. Pour connaître les nombres distincts de chaque type de licence actuellement utilisée dans le groupe (y compris Review and Request), cliquez sur la zone de texte directement sous **Licences en cours d’utilisation :**

   ![](assets/click-text-to-see-more.png)

   La boîte qui s’affiche fournit les mêmes informations pour les quatre types de licence Workfront : Planifier, travailler, réviser et demander. En bas de l’écran, vous pouvez voir le nombre total de licences utilisées par les membres de ce groupe ou par l’un de ses sous-groupes :

   ![](assets/more-license-info.png)

   Pour les licences de révision et de demande, la colonne Max. affiche toujours Illimité.
