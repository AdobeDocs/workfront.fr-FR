---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: L’URL de déconnexion ADFS ne fonctionne pas
description: La procédure décrite sur cette page s’applique uniquement aux organisations qui ne sont pas encore intégrées à Adobe Admin Console.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 97%

---

# L’URL de déconnexion ADFS ne fonctionne pas

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui ne sont pas encore intégrées à [!UICONTROL Adobe Admin Console].
>
>Si votre entreprise est intégrée à [!UICONTROL Adobe Admin Console], consultez l’article [Différences d’administration selon les plateformes ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problème

Lors de l’utilisation de l’URL de déconnexion ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), vous recevez une page de message d’erreur : « Un problème s’est produit lors de l’accès au site. Essayez de revenir sur le site. »

Si le problème persiste, contactez l’administration de ce site et indiquez le numéro de référence suivant pour identifier le problème : **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

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
   <td role="rowheader">Licence Adobe [!DNL Workfront]</td> 
   <td> 
   <p>Nouveau : Standard</p>
   Ou
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>  
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez l’article [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

1. Dans votre serveur de gestion ADFS, accédez aux propriétés **[!UICONTROL Relations de confiance]** > **[!UICONTROL Partie de confiance]** > `<your party trust>`.

1. Sous l’onglet **[!UICONTROL Points d’entrée]**, cliquez sur **[!UICONTROL Ajouter]**.

1. **[!UICONTROL Type de point d’entrée]** = Déconnexion SAML, liaison = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Vous pouvez définir une URL de réponse si vous souhaitez qu’elle revienne vers une autre page. Nous vous recommandons toutefois le site ADFS, car il vous avertit de votre déconnexion, mais vous devez également fermer votre navigateur.
