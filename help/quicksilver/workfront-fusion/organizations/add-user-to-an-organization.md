---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Ajouter un utilisateur ou une utilisatrice à une organisation dans Adobe Workfront Fusion
description: Vous pouvez ajouter des personnes aux organisations dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 447ab70566d5f9de3bc368933c9efdb94d2b9e7e
workflow-type: ht
source-wordcount: '395'
ht-degree: 100%

---

# Ajouter un utilisateur ou une utilisatrice à une organisation dans Adobe Workfront Fusion

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées à [!DNL Adobe Admin Console]. Si votre entreprise a été intégrée à [!DNL Adobe Admin Console], vous devez effectuer cette action via [!DNL Adobe Admin Console].
>
>Pour plus d’informations sur l’ajout d’une personne à [!DNL  Adobe Admin Console], consultez la section « Modifier les détails des utilisateurs et des utilisatrices » de l’article [Gérer les utilisateurs et utilisatrices individuellement](https://helpx.adobe.com/fr/enterprise/using/manage-users-individually.html) ou contactez votre administrateur ou administratrice [!UICONTROL Adobe Admin Console].
>
>Pour obtenir une liste des différentes procédures selon que votre organisation a été intégrée à Adobe Admin Console, consultez l’article [Différences d’administration en fonction de la plateforme (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> 
     <p>Vous devez être un administrateur ou une administratrice de [!DNL Workfront Fusion] pour votre entreprise.</p>
     <p>Vous devez être un administrateur ou une administratrice de [!DNL Workfront Fusion] pour votre équipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ajouter des personnes à une organisation


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

Pour ajouter des personnes à l’organisation, vous devez être un administrateur ou une administratrice de l’organisation à laquelle vous souhaitez ajouter des personnes. Pour plus d’informations sur les rôles, consultez la section [Rôles d’organisation dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Pour ajouter une personne à l’organisation, procédez comme suit :

1. Accédez à **[!UICONTROL Organisations]** dans le menu et sélectionnez l’organisation à laquelle vous souhaitez ajouter une personne.
1. Ouvrez l’onglet **[!UICONTROL Utilisateurs et utilisatrices]** dans votre tableau de bord.
1. Cliquez sur **[!UICONTROL Inviter une nouvelle personne]**, remplissez le formulaire (E-mail, Message, Rôle) et envoyez l’invitation en cliquant sur **[!UICONTROL Envoyer]**.

>[!NOTE]
>
>   
>Si vous ne voyez pas le bouton [!UICONTROL Inviter une nouvelle personne], cela signifie que votre organisation a été intégrée à [!DNL Adobe Business Platform.].
>
>  Pour plus d’informations sur l’ajout d’une personne à une organisation intégrée à [!DNL Adobe Business Platform], consultez la section [Ajouter des utilisateurs et des utilisatrices à [!DNL Adobe Workfront Fusion] via [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md).

La personne reçoit un e-mail lui permettant d’accepter l’invitation.
