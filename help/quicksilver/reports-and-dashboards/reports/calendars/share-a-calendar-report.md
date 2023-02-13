---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Partage d’un rapport de calendrier
description: Vous pouvez partager un calendrier avec d’autres utilisateurs et le rendre public, ce qui permet à une personne sans [!DNL Adobe Workfront] licence pour l’afficher.
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Partage d’un rapport de calendrier

Vous pouvez partager un calendrier avec d’autres utilisateurs et le rendre public, ce qui permet à une personne sans [!DNL Adobe Workfront] licence pour l’afficher.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Review] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>[!UICONTROL Vue] ou accès supérieur à [!UICONTROL aux rapports], aux [!UICONTROL Tableaux de bord] et aux [!UICONTROL Calendriers]</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations d’[!UICONTROL Affichage] ou supérieures au rapport Calendrier, avec accès au partage</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Partage d’un calendrier avec [!DNL Workfront] utilisateurs {#share-a-calendar-with-workfront-users}

Le partage d’un calendrier est similaire au partage d’autres objets. Pour plus d’informations sur le partage d’objets dans [!DNL Adobe Workfront], voir [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Les calendriers qui ont été partagés avec vous s’affichent avec un astérisque (&#42;) en regard du nom du calendrier.

Pour partager un calendrier dans [!DNL Workfront]:

1. Accédez au calendrier que vous souhaitez partager.
1. Cliquez sur **[!UICONTROL Actions du calendrier]**, puis cliquez sur **[!UICONTROL Partage]**.

1. Dans le **[!UICONTROL Accorder à l’accès au calendrier]** , commencez à saisir le nom de l’utilisateur, de l’équipe, du rôle, du groupe ou de la société que vous souhaitez partager le calendrier, puis cliquez sur le nom qui s’affiche dans la liste déroulante.\
   Pour en savoir plus sur la définition des autorisations, voir [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Facultatif) Répétez l’étape 3 pour chaque utilisateur, équipe, rôle ou groupe auquel vous souhaitez accorder l’accès au calendrier.
1. Spécifiez les autorisations pour chaque utilisateur, équipe, rôle, groupe ou société que vous avez ajouté à l’étape 3 en cliquant sur le menu déroulant, puis sélectionnez le niveau d’autorisation à accorder :

   * **[!UICONTROL Affichage]:** Les utilisateurs peuvent consulter et partager le calendrier.

      ![Partage du calendrier avec l’accès Affichage](assets/calendar-share-view-permissions-350x249.png)

   * **[!UICONTROL Gérer]:** Les utilisateurs disposent d’un accès complet au calendrier, moins les droits d’administration, qui sont accordés au niveau de l’accès, ainsi que toutes les autorisations d’affichage.

      ![Partage du calendrier avec Gérer l’accès](assets/calendar-share-manage-permissions-350x241.png)

      >[!NOTE]
      >
      >Le [!DNL Workfront] L’administrateur et le créateur du calendrier peuvent supprimer des autorisations de ces entités.

1. (Facultatif) Selon le rôle d’un utilisateur, vous pouvez cliquer sur **[!UICONTROL Options avancées]**, puis cliquez sur **[!UICONTROL Partager]**&#x200B; pour permettre à l’utilisateur de partager le calendrier avec d’autres utilisateurs.

   Pour plus d’informations sur les niveaux d’autorisation, voir [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Facultatif) Pour mettre le calendrier à la disposition de tous les utilisateurs [!DNL Workfront] utilisateurs, cliquez sur l’icône d’engrenage, puis, dans le menu déroulant, cliquez sur **[!UICONTROL rendre visible à l’échelle du système ;]** pour mettre l’objet à la disposition de tous [!DNL Workfront] utilisateurs.\
   Tous les utilisateurs peuvent voir l’objet en fonction des autorisations que vous avez définies.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Partage d’un calendrier avec un lien public

Vous pouvez rendre un calendrier public et partager un lien avec des personnes qui n’ont pas de [!DNL Workfront] licence.

1. Accédez au calendrier que vous souhaitez partager.
1. Cliquez sur **[!UICONTROL Actions du calendrier]**, puis cliquez sur **[!UICONTROL Partage]**.

1. Cliquez sur l’icône d’engrenage, puis sur **[!UICONTROL Rendre ceci public aux utilisateurs externes]**.
1. Cliquez sur **[!UICONTROL Copier le lien]**.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Partage d’un calendrier avec un lien privé

Vous pouvez partager un lien de calendrier privé avec [!DNL Workfront] utilisateurs. Les utilisateurs doivent se connecter pour afficher le calendrier lorsqu’ils utilisent le lien.

1. Accédez au calendrier que vous souhaitez partager.
1. Cliquez sur **[!UICONTROL Actions du calendrier]**, puis cliquez sur **[!UICONTROL Obtenir un lien partagé]**.

1. Cliquez sur **[!UICONTROL Copier le lien]**.

   >[!NOTE]
   >
   >[!DNL Workfront] les utilisateurs doivent avoir accès au calendrier pour pouvoir y accéder à partir du lien. Pour accorder l’accès, voir [Partage d’un calendrier avec [!DNL Workfront] utilisateurs](#share-a-calendar-with-workfront-users).\
   >Si les utilisateurs n’y ont pas accès, ils peuvent le demander après avoir collé le lien dans leur navigateur.
