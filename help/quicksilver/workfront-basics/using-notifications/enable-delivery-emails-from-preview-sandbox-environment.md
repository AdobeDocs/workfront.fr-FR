---
navigation-topic: notifications
title: Activer l’envoi d’e-mails à partir de l’environnement de prévisualisation des sandbox
description: Si vous souhaitez recevoir des notifications par e-mail de l’environnement de prévisualisation des environnements Sandbox, vous devez activer cette fonctionnalité dans vos paramètres utilisateur pendant que vous êtes connecté à l’aperçu.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 23%

---

# Activer l’envoi d’e-mails à partir de l’environnement de prévisualisation des sandbox

[!UICONTROL Adobe Workfront] désactive toutes les communications par courrier électronique à partir des environnements Preview et Custom Refresh Sandbox. Pour plus d’informations sur l’environnement Preview Sandbox, voir [L’environnement Sandbox d’aperçu Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Pour plus d’informations sur l’environnement Sandbox d’actualisation personnalisée, voir [L’environnement Sandbox d’actualisation personnalisée d’Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Si vous souhaitez recevoir les notifications suivantes de l’environnement Preview Sandbox, vous devez activer cette fonctionnalité dans vos paramètres utilisateur lorsque vous êtes connecté à Preview :

* Notifications par e-mail déclenchées par des notifications d’événement
* Notifications de rappel
* Notifications automatiques des rappels tardifs ou anticipés
* Invitations par email

Vous pouvez le faire pour vous-même ou pour tout utilisateur ayant accès aux modifications. Pour plus d’informations sur l’accès nécessaire à la modification des utilisateurs, voir [Octroi de l’accès aux utilisateurs](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>La remise des rapports et les notifications push sur l’application mobile sont toujours désactivées pour l’environnement de prévisualisation Sandbox. Ni vous, ni l’administrateur [!DNL Workfront] ne pouvez activer la remise de rapports ou les notifications push pour l’application mobile lorsque vous accédez à l’environnement Preview Sandbox.
>
>Pour plus d’informations sur les diffusions de rapports, voir [Présentation de la diffusion de rapports](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Request] ou version ultérieure pour modifier votre propre paramètre</p> <p>[!UICONTROL Planifier] pour modifier le paramètre pour d’autres utilisateurs</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès [!UICONTROL Administrateur système].</p> <p> Pour plus d’informations sur ce niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi à un utilisateur d’un accès administratif complet</a>. </p> </li> 
     <li> <p>Dans votre niveau d’accès, [!UICONTROL Edit] doit être sélectionné pour le paramètre [!UICONTROL Users]. Et, pour le paramètre [!UICONTROL Utilisateurs] , sous [!UICONTROL Ajuster vos paramètres] <img src="assets/gear-icon-in-access-levels.png"> , l’option [!UICONTROL Créer] et au moins l’une des deux options [!UICONTROL Administrateur des utilisateurs] doivent être activées. </p> <p>Si vous utilisez l’option [!UICONTROL User Admin (Group Users)], vous devez faire partie de l’équipe d’administration du groupe dont la personne est membre.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Pour plus d’informations sur le paramètre [!UICONTROL Utilisateurs] dans un niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Octroi de l’accès aux utilisateurs</a>.</p> </li> 
    </ul> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Activation de la diffusion des emails à partir de l’environnement Preview Sandbox

1. Connectez-vous à l’environnement Preview Sandbox.
1. Cliquez sur l’image de votre profil dans le coin supérieur droit de [!DNL Adobe Workfront]. Cliquez ensuite sur le menu **[!UICONTROL Plus]** et sélectionnez **[!UICONTROL Modifier]**.

   Ou

   Recherchez un utilisateur dans [!DNL Workfront] et cliquez sur son nom. Cliquez ensuite sur le menu **[!UICONTROL Plus]** et sélectionnez **[!UICONTROL Modifier]**.

   Ou

   Pour plusieurs utilisateurs : cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **[!UICONTROL Utilisateurs]** ![](assets/users-icon-in-main-menu.png).  Sélectionnez ensuite plusieurs utilisateurs et cliquez sur **[!UICONTROL Modifier]**.

1. Cliquez sur **[!UICONTROL Preferences]**.
1. Sélectionnez **[!UICONTROL Recevoir les emails de cet environnement de test]**.

   >[!NOTE]
   >
   >Cette option n’est pas disponible si vous vous trouvez dans un environnement de production.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
