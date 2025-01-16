---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Ajouter des utilisateurs et des utilisatrices à Adobe Workfront Fusion via Adobe Admin Console
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 83%

---

# Ajouter des utilisateurs et des utilisatrices à [!DNL Adobe Workfront Fusion] via [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Ajouter des utilisateurs et utilisatrices à Adobe Workfront Fusion via Adobe Admin Console](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/add-fusion-users-admin-console.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

>[!IMPORTANT]
>
>Les procédures décrites sur cette page s’appliquent uniquement aux organisations qui ont été intégrées à [!DNL Adobe Admin Console].
>
>Si votre organisation n’a pas encore été intégrée à [!DNL Adobe Admin Console], voir [Ajouter un utilisateur ou une utilisatrice à une organisation dans  [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Pour obtenir une liste de procédures qui varient selon que votre organisation a été intégrée ou non à [!DNL Adobe Admin Console], voir [Différences d’administration en fonction de la plateforme ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

Vous pouvez ajouter un utilisateur ou une utilisatrice à [!DNL Adobe Admin Console] et l’affecter à [!DNL Adobe Workfront Fusion] ou affecter un utilisateur ou une utilisatrice existant dans [!DNL Adobe Admin Console] à [!DNL Workfront Fusion].

Pour regarder une vidéo décrivant [!DNL Workfront Fusion] dans [!DNL Adobe Admin Console], y compris l’ajout d’utilisateurs ou d’utilisatrices, voir [[!DNL Fusion]  sur Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigence du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] droits d’administration</td> 
   <td>Vous devez être un ou une [!UICONTROL Product Configuration Administrator] de produits [!DNL Adobe] pour votre entreprise.</td> 
  </tr>
  </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

&#42;&#42;Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Conditions préalables

Avant d’utiliser [!DNL Admin Console] pour [!DNL Workfront], vous devriez recevoir un e-mail vous invitant à accéder à la console.

1. Si vous commencez sur [!DNL Adobe] et que vous avez reçu un e-mail vous indiquant que vous disposez désormais de droits d’administration du logiciel et des services [!DNL Adobe] pour votre entreprise, cliquez sur le bouton dans l’e-mail pour créer un compte [!DNL Adobe] et ouvrir [!DNL Admin Console].

   Ou

   Si vous disposez déjà d’un compte Adobe, accédez à la page [[!DNL Adobe Admin Console] ](https://adminconsole.adobe.com/).


## Ajouter un nouvel utilisateur ou une nouvelle utilisatrice à [!DNL Adobe Admin Console] et [!DNL Workfront Fusion]

1. Dans la page [[!DNL Adobe Admin Console] ](https://adminconsole.adobe.com/), sélectionnez l’onglet **[!UICONTROL Produits]** dans la barre de navigation supérieure, puis sélectionnez la mosaïque du produit **[!DNL Workfront Fusion]**.

   ![Fusion dans Admin Console](assets/fusion-product-admin-console.png)

1. Dans la liste qui s’affiche, sélectionnez l’entreprise à laquelle vous souhaitez ajouter un utilisateur ou une utilisatrice.

   ![Instance Fusion dans Admin Console](assets/fusion-instances-admin-console.png)

1. Dans la liste qui s’affiche, avec l’onglet **[!UICONTROL Profils de produit]** sélectionné, cliquez sur le nom du lien [!UICONTROL Profil de produit] [!DNL Workfront Fusion].

   ![Profil de produit Workfront Fusion](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > N’apportez aucune modification au [!UICONTROL Profil de produit] en lui-même.

1. Avec l’onglet **[!UICONTROL Utilisateurs et utilisatrices]** sélectionné au-dessus de la liste, cliquez sur **[!UICONTROL Ajouter un utilisateur ou une utilisatrice]**.

1. Dans la zone **[!UICONTROL Ajouter des utilisateurs et des utilisatrices à ce profil de produit]**, saisissez l’adresse e-mail ou le nom d’un utilisateur ou d’une utilisatrice que vous souhaitez ajouter, puis sélectionnez-le dans la liste qui s’affiche.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   La personne est créée dans [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Facultatif) Passez à la section [Modifier le niveau d’accès d’un utilisateur ou d’une utilisatrice dans  [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion).

## Modifier le niveau d’accès d’un utilisateur ou d’une utilisatrice dans Workfront Fusion

### Modifier le rôle d’un utilisateur ou d’une utilisatrice sur Administrateur ou administratrice

L’attribution d’un rôle d’administrateur ou d’administratrice à une personne doit être effectuée dans l’[!DNL Adobe Admin Console].

1. Sur la page [!DNL Workfront Fusion] [!UICONTROL Profil de produit] dans laquelle vous avez ajouté la personne, sélectionnez l’onglet **[!UICONTROL Administrateurs et administratrices]**.

1. Cliquez sur **[!UICONTROL Ajouter un administrateur ou une administratrice]**.

1. Dans la zone **[!UICONTROL Ajouter des administrateurs et administratrices de profil de produit]**, saisissez l’adresse e-mail ou le nom d’une personne à ajouter, puis sélectionnez l’élément dans la liste qui s’affiche.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Cette personne est désormais un administrateur ou une adminstratrice dans [!DNL Workfront Fusion].

### Remplacez le rôle d’une personne par [!UICONTROL Personne membre], [!UICONTROL Personne chargée de la comptabilité] ou [!UICONTROL Personne chargée du développement d’applications].

Les rôles de [!UICONTROL Personne membre], [!UICONTROL Personne chargée de la comptabilité], et [!UICONTROL Personne chargée du développement d’applications] sont gérés dans [!DNL Workfront Fusion].

Pour obtenir des instructions, voir [Afficher ou modifier des rôles d’utilisateur ou d’utilisatrice](../organizations/manage-fusion-users.md#view-or-edit-user-roles) dans l’article [Gérer les utilisateurs et utilisatrices  [!DNL Adobe Workfront Fusion]  de votre entreprise](../organizations/manage-fusion-users.md).

## Attribuer une personne existante dans l’[!DNL Adobe Admin Console] à [!DNL Workfront Fusion]

Vous pouvez ajouter un utilisateur existant à une équipe dans Fusion. Cela est géré dans Fusion.

Pour plus d’informations, consultez la section [Ajouter un utilisateur à une équipe](/help/quicksilver/workfront-fusion/organizations/add-user-to-an-organization.md#add-a-user-to-a-team) dans l’article Ajout d’un utilisateur à une organisation ou à une équipe dans Adobe Workfront Fusion.
