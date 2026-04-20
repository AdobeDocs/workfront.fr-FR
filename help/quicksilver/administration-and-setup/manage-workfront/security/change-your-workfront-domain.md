---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Modification De Votre Domaine Adobe Workfront
description: En tant qu’administrateur ou administratrice Adobe Workfront et contact de support Workfront autorisé, vous pouvez demander de l’aide à l’équipe de support Workfront pour modifier le domaine Workfront de votre entreprise.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 97%

---

# Modifier votre domaine Adobe Workfront

>[!IMPORTANT]
>
>La procédure décrite sur cette page ne s’applique qu’aux entreprise qui n’ont pas encore été intégrées à l’Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, il n’est pas possible de modifier votre domaine Workfront.
>
>Pour suivre la procédure correspondant à votre situation et à son intégration ou non à Adobe Admin Console, consultez la section [Différences en matière d’administration en fonction de la plateforme (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

En tant qu’administrateur ou administratrice Adobe Workfront et contact de support Workfront autorisé, vous pouvez demander de l’aide à l’équipe de support Workfront pour modifier le domaine Workfront de votre entreprise.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Demander une modification de domaine

1. Commencez à créer un ticket de support sur Experience League.
1. Dans la boîte **Description**, incluez le nouveau domaine que vous souhaitez, ainsi que la période pendant laquelle vous souhaitez que le nouveau domaine soit mis en ligne.
1. Terminez de remplir les cases du cas de support, puis cliquez sur **Envoyer**.

Vous pouvez également appeler le support Workfront pour obtenir de l’aide sur le changement de domaine.

<!--

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.


-->
