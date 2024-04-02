---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Ajout d’un utilisateur à une organisation dans Adobe Workfront Fusion
description: Vous pouvez ajouter des utilisateurs aux organisations dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 447ab70566d5f9de3bc368933c9efdb94d2b9e7e
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Ajout d’un utilisateur à une organisation dans Adobe Workfront Fusion

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées au [!DNL Adobe Admin Console]. Si votre entreprise a été intégrée à la variable [!DNL Adobe Admin Console], vous devez effectuer cette action via le [!DNL Adobe Admin Console].
>
>Pour plus d’informations sur l’ajout d’un utilisateur dans la variable[!DNL  Adobe Admin Console], reportez-vous à la section &quot;Modifier les détails de l’utilisateur&quot; de l’article [Gérer les utilisateurs individuellement](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) ou contactez votre [!UICONTROL Adobe Admin Console] Administrateur.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Admin Console, voir [Différences d’administration basées sur les plateformes (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelles : non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail, [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de l’[!UICONTROL Select] ou de l’[!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> 
     <p>Vous devez être un [!DNL Workfront Fusion] administrateur de votre entreprise.</p>
     <p>Vous devez être un [!DNL Workfront Fusion] administrateur de votre équipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ajout d’utilisateurs à une organisation


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->

Pour ajouter des utilisateurs à l’organisation, vous devez être un administrateur de l’organisation à laquelle vous souhaitez ajouter des utilisateurs. Pour plus d’informations sur les rôles, voir [Rôles d’organisation dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Pour ajouter un utilisateur à l’organisation :

1. Accédez à **[!UICONTROL Organisations]** dans le menu et sélectionnez l’organisation à laquelle vous souhaitez ajouter un utilisateur.
1. Ouvrez le **[!UICONTROL Utilisateurs]** dans votre tableau de bord.
1. Cliquez sur **[!UICONTROL Invitation d’un nouvel utilisateur]**, remplissez le formulaire (Email, Message, Rôle) et envoyez l’invitation en cliquant sur **[!UICONTROL Envoyer]**.

>[!NOTE]
>
>   
>Si vous ne voyez pas le [!UICONTROL Invitation d’un nouvel utilisateur] , votre organisation a été intégrée à la fonction [!DNL Adobe Business Platform.]
>
>  Pour plus d’informations sur l’ajout d’un utilisateur à une organisation intégrée au [!DNL Adobe Business Platform], voir [Ajout d’utilisateurs à [!DNL Adobe Workfront Fusion] par le biais du [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

L’utilisateur reçoit un courrier électronique lui permettant d’accepter l’invitation.
