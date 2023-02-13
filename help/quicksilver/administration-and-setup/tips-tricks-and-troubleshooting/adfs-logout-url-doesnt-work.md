---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: L’URL de déconnexion ADFS ne fonctionne pas
description: La procédure décrite sur cette page s’applique uniquement aux organisations qui ne sont pas encore intégrées à Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# L’URL de déconnexion ADFS ne fonctionne pas

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui ne sont pas encore intégrées au [!UICONTROL Adobe Admin Console].
>
>Si votre entreprise a été intégrée à la variable [!UICONTROL Adobe Admin Console], voir [Différences d’administration basées sur les plateformes ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problème

Lorsque vous utilisez l’URL de déconnexion ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), vous recevez une page de message avec l’erreur : &quot;Un problème s&#39;est produit lors de l&#39;accès au site. Essayez de revenir sur le site.&quot;

Si le problème persiste, contactez l&#39;administrateur de ce site et indiquez le numéro de référence suivant pour identifier le problème : **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

1. Dans votre serveur de gestion ADFS, accédez à **[!UICONTROL Relations de confiance]** > **[!UICONTROL Confiance des parties]** > `<your party trust>` propriétés.

1. Sous , **[!UICONTROL Points de fin]** , cliquez sur **[!UICONTROL Ajouter]**.

1. **[!UICONTROL Type de point d’entrée]** = Déconnexion SAML, liaison = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Vous pouvez définir une URL de réponse si vous souhaitez qu’elle revienne vers une autre page. Nous vous recommandons toutefois le site ADFS, car il vous avertit que vous êtes déconnecté, mais que vous devez toujours fermer votre navigateur.
