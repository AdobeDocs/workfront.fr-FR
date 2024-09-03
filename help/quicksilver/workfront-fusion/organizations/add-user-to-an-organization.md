---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Ajouter un utilisateur ou une utilisatrice à une organisation dans Adobe Workfront Fusion
description: Vous pouvez ajouter des utilisateurs et des utilisatrices aux organisations dans Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 1b4a6d2b2ad57ddf1afd5dadf8b1fed358f95b61
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 55%

---

# Ajout d’un utilisateur à une organisation ou une équipe dans Adobe Workfront Fusion

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées à l’[!DNL Adobe Admin Console]. Si votre entreprise a été intégrée à l’[!DNL Adobe Admin Console], vous devez effectuer cette action via l’[!DNL Adobe Admin Console].
>
>Pour obtenir des instructions sur l’ajout d’un utilisateur une fois que votre organisation a été déplacée vers [!DNL  Adobe Admin Console] et l’Adobe d’expérience unifiée, voir [Ajout d’utilisateurs à [!DNL Adobe Workfront Fusion] par l’intermédiaire de [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md).
>
>Pour suivre la procédure correspondant à votre situation et à son intégration ou non à Adobe Admin Console, consultez la section [Différences en matière d’administration en fonction de la plateforme (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigence de produit hérité : votre organisation doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> 
     <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront Fusion] de votre organisation.</p>
     <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront Fusion] de votre équipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ajout des utilisateurs et des utilisatrices à une organisation


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

Pour ajouter des utilisateurs et des utilisatrices à l’organisation, vous devez être un administrateur ou une administratrice de l’organisation à laquelle vous souhaitez ajouter des personnes. Pour plus d’informations sur les rôles, voir [Rôles d’organisation dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

Pour ajouter une personne à l’organisation :

1. Accédez à **[!UICONTROL Organisations]** dans le menu et sélectionnez l’organisation à laquelle vous souhaitez ajouter une personne.
1. Ouvrez l’onglet **[!UICONTROL Utilisateurs et utilisatrices]** dans votre tableau de bord.
1. Cliquez sur **[!UICONTROL Inviter un nouvel utilisateur]** et envoyez l’invitation en cliquant sur **[!UICONTROL Envoyer]**.

   >[!NOTE]
   >
   >   
   >Si vous ne voyez pas le bouton [!UICONTROL Inviter une nouvelle personne], cela signifie que votre organisation a été intégrée à [!DNL Adobe Business Platform.].
   >
   >  Pour plus d’informations sur l’ajout d’une personne à une organisation intégrée à [!DNL Adobe Business Platform], consultez la section [Ajouter des utilisateurs et des utilisatrices à [!DNL Adobe Workfront Fusion] via [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md).

1. Remplissez le formulaire.

   <table style="table-layout:auto">
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Email address]</td>
      <td>
        Entrez l’adresse électronique de l’utilisateur.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>Saisissez le nom complet de l’utilisateur.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Role] </td>
      <td>Sélectionnez le rôle de l’utilisateur. Pour plus d'informations sur les rôles, voir <a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">Rôles de l'organisation et de l'équipe.</a></p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Équipes</td>
      <td>Sélectionnez toutes les équipes dont vous souhaitez que l’utilisateur soit membre.</td>
    </tr>
    <tr>
      <td role="rowheader">Note</td>
      <td>Saisissez une note pour l’utilisateur. Cette note s’affiche dans le courrier électronique d’invitation de l’utilisateur.</td>
    </tr>
  </tbody>
</table>

La personne reçoit un e-mail lui permettant d’accepter l’invitation.

## Ajout d’un utilisateur à une équipe

Vos utilisateurs sont affectés à des équipes lorsque vous les créez. Si un utilisateur existant doit être ajouté à une équipe, vous pouvez le faire sur la page Utilisateurs de l’équipe.

L’ajout d’un utilisateur à une équipe est géré à partir de la page de cette équipe.

1. Allez dans l’équipe à laquelle vous souhaitez ajouter l’utilisateur en sélectionnant **Organisations** dans le panneau de gauche, en cliquant sur l’onglet **Équipes** de la page de l’organisation et en sélectionnant l’équipe.

   Ou

   Si vous êtes sur la page d’une autre équipe, cliquez sur la liste déroulante de l’équipe en haut de la page.

1. Sur la page de l’équipe (avec le nom de l’équipe en haut de la page), sélectionnez l’onglet **Utilisateurs** .
1. Localisez l’utilisateur sur la page. Les utilisateurs de votre entreprise apparaissent sur cette page même s’ils ne font pas partie de l’équipe.
1. Cliquez sur **Aucun** à droite du nom de l’utilisateur, puis sélectionnez le rôle que vous souhaitez qu’il ait dans l’équipe.

L’utilisateur est ajouté à l’équipe.