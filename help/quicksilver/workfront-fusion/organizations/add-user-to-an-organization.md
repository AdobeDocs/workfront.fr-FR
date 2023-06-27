---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Ajout d’un utilisateur à une organisation dans Adobe Workfront Fusion
description: Vous pouvez ajouter des utilisateurs aux organisations dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---

# Ajout d’un utilisateur à une organisation dans Adobe Workfront Fusion

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées au [!DNL Adobe Admin Console]. Si votre entreprise a été intégrée à la variable [!DNL Adobe Admin Console], vous devez effectuer cette action via le [!DNL Adobe Admin Console].
>
>Pour plus d’informations sur l’ajout d’un utilisateur dans la variable[!DNL  Adobe Admin Console], reportez-vous à la section &quot;Modifier les détails de l’utilisateur&quot; de l’article [Gérer les utilisateurs individuellement](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) ou contactez votre [!UICONTROL Adobe Admin Console] Administrateur.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Admin Console, reportez-vous à la section [Différences d’administration basées sur les plateformes (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

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
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail, [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
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

<p>La procédure d’ajout d’un utilisateur à votre organisation Fusion varie selon que votre organisation a été intégrée à Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Ajout d’un utilisateur à une organisation intégrée à Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Ajout d’un utilisateur à une organisation qui n’a pas été intégrée à Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Ajout d’un utilisateur à une organisation intégrée à Adobe Business Platform</strong></p>
<p>Si votre entreprise a été intégrée à Adobe Business Platform, vous devez effectuer cette action via Adobe Admin Console.</p>
<p>Pour plus d’informations sur l’ajout d’un utilisateur dans Adobe Admin Console :</p>
<ul>
<li> <p>Voir <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Création d’utilisateurs dans Workfront avec Adobe Admin Console</a></p> </li>
<li> <p>Voir la section "Ajouter des utilisateurs" de l’article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gérer les utilisateurs individuellement</a></p> </li>
<li> <p>Contactez votre administrateur Adobe Admin Console.</p> </li>
</ul>
<p>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Business Platform, voir <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Ajout d’un utilisateur à une organisation qui n’a pas été intégrée à Adobe Business Console</strong></p>

Pour ajouter des utilisateurs à l’organisation, vous devez être un administrateur de l’organisation à laquelle vous souhaitez ajouter des utilisateurs. Pour plus d’informations sur les rôles, voir [Rôles d’organisation dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Pour ajouter un utilisateur à l’organisation :

1. Accédez à **[!UICONTROL Organisations]** dans le menu et sélectionnez l’organisation à laquelle vous souhaitez ajouter un utilisateur.
1. Ouvrez le **[!UICONTROL Utilisateurs]** dans votre tableau de bord.
1. Cliquez sur **[!UICONTROL Invitation d’un nouvel utilisateur]**, remplissez le formulaire (Email, Message, Rôle) et envoyez l’invitation en cliquant sur **[!UICONTROL Envoyer]**.

>[!NOTE]
>
>   
><p>Si le bouton [!UICONTROL Inviter un nouvel utilisateur] n’apparaît pas, votre organisation a été intégrée à la variable [!DNL Adobe Business Platform.] </p>
>
>   <p>Pour plus d’informations sur l’ajout d’un utilisateur à une organisation intégrée au [!DNL Adobe Business Platform], voir <a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Ajout d’un utilisateur à une organisation qui a été intégrée au [!DNL Adobe Business Platform]</a></p>

L’utilisateur reçoit un courrier électronique d’invitation par lequel il peut accepter l’invitation en cliquant sur une [!UICONTROL Acceptation du rôle] bouton .
