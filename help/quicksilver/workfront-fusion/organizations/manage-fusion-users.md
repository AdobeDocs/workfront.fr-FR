---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Gérer [!DNL Adobe Workfront Fusion] utilisateurs de votre entreprise
description: Gérer [!DNL Adobe Workfront Fusion] utilisateurs de votre entreprise
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Gérer [!DNL Adobe Workfront Fusion] utilisateurs de votre entreprise

[!DNL Adobe Workfront Fusion] les administrateurs peuvent gérer les rôles utilisateur dans [!DNL Workfront Fusion].

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

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
   <td> <p>Workfront Fusion pour l’automatisation et l’intégration du travail,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
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

## Affichage ou modification des rôles utilisateur {#view}

[!DNL Adobe Workfront Fusion] Les administrateurs peuvent afficher et mettre à jour les rôles utilisateur.

1. Lors de la connexion en tant que [!DNL Workfront Fusion] administrator, sélectionnez **[!UICONTROL Utilisateurs]** dans le volet de navigation de gauche.
1. Cliquez sur **[!UICONTROL Détails]** dans la ligne de l’utilisateur que vous souhaitez afficher.
1. (Facultatif) Pour mettre à jour le rôle de l’utilisateur, cliquez sur la liste déroulante du **[!DNL Role]** dans la ligne de l’organisation dans laquelle vous souhaitez modifier le rôle de l’utilisateur, puis sélectionnez le nouveau rôle.

## Affichage ou modification des détails de l’utilisateur {#view2}

[!DNL Adobe Workfront Fusion] Les administrateurs peuvent afficher et mettre à jour les détails des utilisateurs.

1. Lors de la connexion en tant que [!DNL Workfront Fusion] administrator, sélectionnez **[!UICONTROL Utilisateurs]** dans le volet de navigation de gauche.
1. Cliquez sur **[!UICONTROL Détails]** dans la ligne de l’utilisateur que vous souhaitez afficher.
1. (Facultatif) Pour mettre à jour les détails de l’utilisateur, cliquez sur **[!UICONTROL Options]** dans le coin supérieur droit de l’écran, puis sélectionnez **[!UICONTROL Modifier les détails]**.

## Suppression d’un utilisateur {#delete}

[!DNL Adobe Workfront Fusion] Les administrateurs peuvent supprimer des utilisateurs.

1. Lors de la connexion en tant que [!DNL Workfront Fusion] administrator, sélectionnez [!UICONTROL Utilisateurs] dans le volet de navigation de gauche.
1. Cliquez sur **[!UICONTROL Détails]** dans la ligne de l’utilisateur que vous souhaitez afficher.
1. (Facultatif) Pour mettre à jour les détails de l’utilisateur, cliquez sur **[!UICONTROL Options]** dans le coin supérieur droit de l’écran, puis sélectionnez **[!UICONTROL Supprimer]**.

### Considérations relatives à la suppression d’un utilisateur dans Workfront Fusion

* Lorsqu’un utilisateur est supprimé, ses connexions, clés et webhooks sont supprimées. Tous les scénarios appartenant à l’utilisateur sont transférés au propriétaire de l’organisation. Les connexions dans ces scénarios doivent être mises à jour, car les connexions appartenant à l’utilisateur ne sont plus valides.
* Si l’utilisateur supprimé possède des applications ou des modèles publics, les applications ou les modèles publics sont transférés au propriétaire de l’organisation. S’il n’existe pas de propriétaire d’organisation, les applications ou les modèles publics sont transférés à un autre utilisateur.
