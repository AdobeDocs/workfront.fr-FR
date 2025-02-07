---
title: Configurer une URL d’aide personnalisée
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: Si vous créez un site d’aide interne personnalisé contenant des informations sur la manière dont votre entreprise utilise Workfront, vous pouvez configurer l’icône d’aide du menu principal de manière à renvoyer vers ce site.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d2b63508-1943-4f9e-888e-8f1bfb54c33e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 50%

---

# Configurer une URL d’aide personnalisée

Si vous créez un site d’aide interne personnalisé contenant des informations sur la manière dont votre entreprise utilise Workfront, vous pouvez configurer l’icône d’aide du menu principal de manière à renvoyer vers ce site.

![Bouton Aide personnalisé](assets/custom-help-button.png)

Cela n’affecte pas les liens d’aide contextuelle dans Workfront, qui redirigent les utilisateurs vers le site d’aide de Workfront.

Pour plus d’informations sur la manière dont les utilisateurs accèdent à la fois à une URL d’aide personnalisée que vous configurez dans Workfront et au site d’aide standard de Workfront, voir [Accès à l’aide d’Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/access-workfront-help.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer une URL d’aide personnalisée

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Préférences**.
1. Dans la section **Préférences générales**, dans le champ **URL d’aide personnalisée**, saisissez l’URL où se trouve votre site d’aide personnalisée.

   Si l’emplacement de votre aide personnalisée nécessite des informations de connexion, ces dernières sont requises pour les personnes accédant au site à partir de Workfront. Si vous n’utilisez pas l’authentification unique (SSO), il se peut que les informations d’identification de votre site d’aide personnalisée doivent être gérées séparément des informations d’identification de Workfront.

1. Cliquer sur **Enregistrer**.

   Une fois que vous avez enregistré une URL d’aide personnalisée, vous pouvez revenir au site d’aide par défaut de Workfront en supprimant l’URL personnalisée et en cliquant sur **Enregistrer**.
