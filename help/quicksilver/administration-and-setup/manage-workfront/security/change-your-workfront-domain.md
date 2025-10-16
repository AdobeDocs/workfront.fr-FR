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
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '378'
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
   <td role="rowheader">Package Adobe Workfront</td> 
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

## Mettre à jour le nouveau domaine si vous êtes client ou cliente SSO

Si votre entreprise utilise l’authentification unique, les étapes suivantes sont requises une fois que votre domaine Workfront a été modifié.

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre organisation repose sur Adobe IMS. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

{{step-1-to-setup}}

1. Dans la barre latérale gauche, cliquez sur **Système** > **Informations sur la clientèle** et assurez-vous que votre domaine est mis à jour sur la page Informations sur la clientèle.

1. Dans la barre latérale gauche, cliquez sur **Système** > **Authentification unique (SSO)**.

1. Cliquez sur **Télécharger les métadonnées SAML 2.0**.
1. Une fois le fichier téléchargé, ouvrez-le et assurez-vous des éléments suivants :

   1. **entityID** pointe vers le nouveau domaine.
   1. Tous les emplacements dans **`<md:AssertionConsumerService>`** pointent vers le nouveau domaine.

1. Indiquez le fichier de métadonnées téléchargé à votre fournisseur d’identité afin qu’il puisse être mis à jour de son côté.
1. Assurez-vous que le domaine est mis à jour pour toutes les intégrations Workfront utilisées par votre organisation.
