---
navigation-topic: notifications
title: Activation de la diffusion des emails à partir de l’environnement Preview Sandbox
description: Si vous souhaitez recevoir des notifications par e-mail de l’environnement de prévisualisation des environnements Sandbox, vous devez activer cette fonctionnalité dans vos paramètres utilisateur pendant que vous êtes connecté à l’aperçu.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Activation de la diffusion des emails à partir de l’environnement Preview Sandbox

[!UICONTROL Adobe Workfront] désactive toutes les communications par courrier électronique à partir des environnements Preview et Custom Refresh Sandbox. Pour plus d’informations sur l’environnement de prévisualisation Sandbox, voir [Environnement Adobe Workfront Preview Sandbox](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Pour plus d’informations sur l’environnement Sandbox d’actualisation personnalisée, voir [Environnement Sandbox d’actualisation personnalisée d’Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Si vous souhaitez recevoir les notifications suivantes de l’environnement Preview Sandbox, vous devez activer cette fonctionnalité dans vos paramètres utilisateur lorsque vous êtes connecté à Preview :

* Notifications par e-mail déclenchées par des notifications d’événement
* Notifications de rappel
* Notifications automatiques des rappels tardifs ou anticipés
* Invitations par email

Vous pouvez le faire pour vous-même ou pour tout utilisateur ayant accès aux modifications. Pour plus d’informations sur l’accès nécessaire à la modification des utilisateurs, voir [Accorder l’accès aux utilisateurs](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>La remise des rapports et les notifications push sur l’application mobile sont toujours désactivées pour l’environnement de prévisualisation Sandbox. Ni vous ni le [!DNL Workfront] Lorsque vous accédez à l’environnement Preview Sandbox, l’administrateur peut activer la remise de rapports ou les notifications push pour l’application mobile.
>
>Pour plus d’informations sur les diffusions de rapports, voir [Présentation de la diffusion des rapports](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

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
   <td> <p>[!UICONTROL Request] ou version ultérieure pour modifier votre propre paramètre</p> <p>[!UICONTROL Planifier] pour modifier le paramètre pour d’autres utilisateurs</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Vous devez disposer de l’une des options suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès [!UICONTROL Administrateur système].</p> <p> Pour plus d’informations sur ce niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
     <li> <p>Dans votre niveau d’accès, [!UICONTROL Modifier] doit être sélectionné pour le paramètre [!UICONTROL Utilisateurs] . Et, pour le paramètre [!UICONTROL Utilisateurs] , sous [!UICONTROL Ajuster vos paramètres] <img src="assets/gear-icon-in-access-levels.png"> , l’option [!UICONTROL Créer] et au moins l’une des deux options [!UICONTROL User Admin] doivent être activées. </p> <p>Si vous utilisez l’option [!UICONTROL User Admin (Group Users)], vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Pour plus d’informations sur le paramètre [!UICONTROL Utilisateurs] dans un niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
    </ul> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Activation de la diffusion des emails à partir de l’environnement Preview Sandbox

1. Connectez-vous à l’environnement Preview Sandbox.
1. Cliquez sur l’image de votre profil dans le coin supérieur droit de la [!DNL Adobe Workfront]. Cliquez ensuite sur le bouton **[!UICONTROL Plus]** et sélectionnez **[!UICONTROL Modifier]**.

   Ou

   Recherchez un utilisateur dans [!DNL Workfront] et cliquez sur leur nom. Cliquez ensuite sur le bouton **[!UICONTROL Plus]** et sélectionnez **[!UICONTROL Modifier]**.

   Ou

   Pour plusieurs utilisateurs : Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **[!UICONTROL Utilisateurs]** ![](assets/users-icon-in-main-menu.png).  Sélectionnez ensuite plusieurs utilisateurs, puis cliquez sur **[!UICONTROL Modifier]**.

1. Cliquez sur **[!UICONTROL Préférences]**.
1. Sélectionner **[!UICONTROL Réception d’emails à partir de cet environnement de test]**.

   >[!NOTE]
   >
   >Cette option n’est pas disponible si vous vous trouvez dans un environnement de production.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
