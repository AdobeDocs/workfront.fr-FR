---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Gérer les utilisateurs  [!DNL Adobe Workfront Fusion] de votre entreprise
description: Gérer les utilisateurs  [!DNL Adobe Workfront Fusion] de votre entreprise
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 32%

---

# Gérer les utilisateurs [!DNL Adobe Workfront Fusion] de votre entreprise

Les administrateurs [!DNL Adobe Workfront Fusion] peuvent gérer les rôles utilisateur dans [!DNL Workfront Fusion].

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
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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
     <p>Vous devez être un administrateur ou une administratrice de [!DNL Workfront Fusion] pour votre organisation.</p>
     <p>Vous devez être un administrateur ou une administratrice de [!DNL Workfront Fusion] pour votre équipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Affichage ou modification des rôles utilisateur {#view}

Les administrateurs [!DNL Adobe Workfront Fusion] peuvent afficher et mettre à jour les rôles utilisateur.

1. Lors de la connexion en tant qu’administrateur [!DNL Workfront Fusion], sélectionnez **[!UICONTROL Utilisateurs]** dans le volet de navigation de gauche.
1. Cliquez sur **[!UICONTROL Details]** dans la ligne de l’utilisateur que vous souhaitez afficher.
1. (Facultatif) Pour mettre à jour le rôle de l’utilisateur, cliquez sur la liste déroulante dans la colonne **[!DNL Role]** de la ligne de l’organisation dans laquelle vous souhaitez modifier le rôle de l’utilisateur, puis sélectionnez le nouveau rôle.

## Affichage ou modification des détails de l’utilisateur {#view2}

Les administrateurs [!DNL Adobe Workfront Fusion] peuvent afficher et mettre à jour les détails des utilisateurs.

1. Lors de la connexion en tant qu’administrateur [!DNL Workfront Fusion], sélectionnez **[!UICONTROL Utilisateurs]** dans le volet de navigation de gauche.
1. Cliquez sur **[!UICONTROL Details]** dans la ligne de l’utilisateur que vous souhaitez afficher.
1. (Facultatif) Pour mettre à jour les détails de l’utilisateur, cliquez sur **[!UICONTROL Options]** dans le coin supérieur droit de l’écran, puis sélectionnez **[!UICONTROL Modifier les détails]**.

## Suppression d’un utilisateur {#delete}

Les administrateurs [!DNL Adobe Workfront Fusion] peuvent supprimer des utilisateurs.

1. Lors de la connexion en tant qu’administrateur [!DNL Workfront Fusion], sélectionnez [!UICONTROL Utilisateurs] dans le volet de navigation de gauche.
1. Cliquez sur **[!UICONTROL Details]** dans la ligne de l’utilisateur que vous souhaitez afficher.
1. (Facultatif) Pour mettre à jour les détails de l’utilisateur, cliquez sur **[!UICONTROL Options]** dans le coin supérieur droit de l’écran, puis sélectionnez **[!UICONTROL Supprimer]**.

### Considérations relatives à la suppression d’un utilisateur dans Workfront Fusion

* Lorsqu’un utilisateur est supprimé, ses connexions, clés et webhooks sont supprimées. Tous les scénarios appartenant à l’utilisateur sont transférés au propriétaire de l’organisation. Les connexions dans ces scénarios doivent être mises à jour, car les connexions appartenant à l’utilisateur ne sont plus valides.
* Si l’utilisateur supprimé possède des applications ou des modèles publics, les applications ou les modèles publics sont transférés au propriétaire de l’organisation. S’il n’existe pas de propriétaire d’organisation, les applications ou les modèles publics sont transférés à un autre utilisateur.
