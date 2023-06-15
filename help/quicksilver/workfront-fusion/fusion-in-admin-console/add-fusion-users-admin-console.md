---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Ajout d’utilisateurs à Adobe Workfront Fusion via Adobe Admin Console
description: Vous pouvez ajouter un utilisateur à Adobe Admin Console et l’affecter à Adobe Workfront Fusion ou affecter un utilisateur existant de Adobe Admin Console à Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 1%

---

# Ajout d’utilisateurs à [!DNL Adobe Workfront Fusion] via la [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>Les procédures décrites sur cette page s’appliquent uniquement aux organisations qui ont été intégrées au [!DNL Adobe Admin Console].
>
>Si votre entreprise n’a pas encore été intégrée à la variable [!DNL Adobe Admin Console], voir [Ajout d’un utilisateur à une organisation dans [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à la variable [!DNL Adobe Admin Console], voir [Différences d’administration basées sur les plateformes ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

Vous pouvez ajouter un utilisateur à la variable [!DNL Adobe Admin Console] et les affecter à [!DNL Adobe Workfront Fusion]ou affecter un utilisateur existant dans le [!DNL Adobe Admin Console] to [!DNL Workfront Fusion].

Pour une vidéo décrivant [!DNL Workfront Fusion] dans le [!DNL Adobe Admin Console], y compris comment ajouter des utilisateurs, voir [[!DNL Fusion] sur Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL Fusion Workfront pour l’automatisation et l’intégration du travail] </p> <p>[!UICONTROL Workfront Fusion for Work Automation] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] droits d’administrateur</td> 
   <td>Vous devez être un [!UICONTROL Administrateur de la configuration du produit] de [!DNL Adobe] produits pour votre organisation.</td> 
  </tr>
  </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

&#42;&#42;Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Conditions préalables

Avant d’utiliser la variable [!DNL Admin Console] pour [!DNL Workfront], vous devriez recevoir un courrier électronique vous invitant à accéder à la console.

1. Si vous découvrez [!DNL Adobe] et vous avez reçu un e-mail vous indiquant que vous disposez désormais des droits de gestion [!DNL Adobe] logiciel et services pour votre organisation, cliquez sur le bouton dans le courrier électronique pour créer un [!DNL Adobe] et ouvrez le [!DNL Admin Console].

   Ou

   Si vous disposez déjà d’un compte d’Adobe, accédez au [[!DNL Adobe Admin Console] page](https://adminconsole.adobe.com/).


## Ajoutez un nouvel utilisateur au [!DNL Adobe Admin Console] et [!DNL Workfront Fusion]

1. Dans la [[!DNL Adobe Admin Console] page](https://adminconsole.adobe.com/), sélectionnez la variable **[!UICONTROL Produits]** dans la barre de navigation supérieure, puis sélectionnez l’option **[!DNL Workfront Fusion]** mosaïque produit.

   ![Fusion en Admin Console](assets/fusion-product-admin-console.png)

1. Dans la liste qui s’affiche, sélectionnez l’organisation à laquelle vous souhaitez ajouter un utilisateur.

   ![Instance de fusion dans Admin Console](assets/fusion-instances-admin-console.png)

1. Dans la liste qui s’affiche, avec la fonction **[!UICONTROL Profils de produit]** sélectionné, cliquez sur le nom de la [!DNL Workfront Fusion] [!UICONTROL Profil de produits] lien.

   ![Profil de produit Workfront Fusion](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > N’apportez aucune modification à la variable [!UICONTROL Profil de produits] elle-même.

1. Avec le **[!UICONTROL Utilisateurs]** sélectionné au-dessus de la liste, cliquez sur **[!UICONTROL Ajouter un utilisateur]**.

1. Dans le **[!UICONTROL Ajout d’utilisateurs à ce profil de produit]** , saisissez l’adresse électronique ou le nom d’un utilisateur à ajouter, puis sélectionnez-le dans la liste qui s’affiche.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   L’utilisateur est créé dans [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Facultatif) Passez à la [Modifier le niveau d’accès d’un utilisateur dans [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Modification du niveau d’accès d’un utilisateur dans Workfront Fusion

### Remplacer le rôle d’un utilisateur par Administrateur

Attribuer un rôle d’administrateur à un utilisateur doit être effectué dans la variable [!DNL Adobe Admin Console].

1. Sur le [!DNL Workfront Fusion] [!UICONTROL Profil de produits] dans laquelle vous avez ajouté l’utilisateur, sélectionnez la variable **[!UICONTROL Administrateurs]** .

1. Cliquez sur **[!UICONTROL Ajouter un administrateur]**.

1. Dans le **[!UICONTROL Ajout d’administrateurs de profil de produit]** , saisissez l’adresse électronique ou le nom d’un utilisateur à ajouter, puis sélectionnez-le dans la liste qui s’affiche.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Cet utilisateur est désormais administrateur dans [!DNL Workfront Fusion].

### Remplacer le rôle d’un utilisateur par [!UICONTROL membre], [!UICONTROL Comptable]ou [!UICONTROL Développeur d’applications].

[!UICONTROL membre], [!UICONTROL Comptable], et [!UICONTROL Développeur d’applications] les rôles sont gérés dans [!DNL Workfront Fusion].

Pour obtenir des instructions, voir [Affichage ou modification des rôles utilisateur](../organizations/manage-fusion-users.md#view-or-edit-user-roles) dans l’article [Gérer [!DNL Adobe Workfront Fusion] utilisateurs de votre entreprise](../organizations/manage-fusion-users.md)

## Attribuer un utilisateur existant dans le [!DNL Adobe Admin Console] to [!DNL Workfront Fusion]

1. Commencez à modifier l’utilisateur comme décrit dans la section &quot;Modifier les détails de l’utilisateur&quot; de l’article. [Gérer les utilisateurs individuellement](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) dans le [!DNL Adobe Admin Console] documentation.

1. Ajouter **[!DNL Adobe Workfront Fusion]** aux produits affectés à l’utilisateur.
