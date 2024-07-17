---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Désactiver ou réactiver une entreprise
description: Vous pouvez désactiver une société que vous n’utilisez plus tout en conservant toutes ses données historiques associées. Si vous désactivez une entreprise déjà utilisée quelque part dans le système, elle continue à fonctionner comme elle l’a toujours fait. Il n’est ni supprimé ni bloqué.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 53%

---

# Désactiver ou réactiver une entreprise

Vous pouvez désactiver une société que vous n’utilisez plus tout en conservant toutes ses données historiques associées. Si vous désactivez une entreprise déjà utilisée quelque part dans le système, elle continue à fonctionner comme elle l’a toujours fait. Il n’est ni supprimé ni bloqué.

## Conditions d’accès

Pour gérer les entreprises dans [!DNL Workfront], vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] forfait*</p> </td> 
   <td>[!UICONTROL Team] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licence*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Utilisez l’une des configurations suivantes :</p> 
    <ul> 
     <li> <p>Le niveau d’accès [!UICONTROL System Administrator], qui vous permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices</a>. </p> </li> 
     <li> <p>L’accès administratif à la gestion des entreprises, qui vous permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones</a>.</p> </li> 
    </ul> <p><b>REMARQUE</b> :  
     <ul> 
      <li> <p>Vous pouvez également gérer les entreprises associées à un groupe pour lequel vous faites partie de l’équipe d’administration.</p> </li> 
      <li> <p>Pour pouvoir ajouter ou supprimer des personnes du système [!DNL Workfront], vous devez disposer de l’un des éléments suivants :</p> 
       <ul> 
        <li> <p>Niveau d’accès [!UICONTROL System Administrator]. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à une personne un accès administratif complet</a>. </p> </li> 
        <li> <p>Dans votre niveau d’accès, [!UICONTROL Edit] doit être sélectionné pour le paramètre [!UICONTROL Users]. En outre, pour le paramètre [!UICONTROL Utilisateurs] , sous [!UICONTROL Ajuster vos paramètres] <img src="assets/gear-icon-in-access-levels.png"> , l’option [!UICONTROL Créer] et au moins l’une des deux options [!UICONTROL Administration des utilisateurs] doivent être activées. </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>Si vous utilisez l’option [!UICONTROL User Admin (Group Users)], vous devez faire partie de l’équipe d’administration du groupe dont la personne est membre.</p> </li> 
       </ul> <p>Pour plus d’informations sur le paramètre Utilisateurs et utilisatrices dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux personnes</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur [!DNL Workfront].

## Désactiver ou réactiver une entreprise

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe] Workfront, puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Entreprises]** ![](assets/companies-icon-left-panel.png).

1. Sélectionnez une ou plusieurs sociétés à désactiver ou à réactiver.
1. Cliquez sur **[!UICONTROL Modifier]**.
1. Pour une seule entreprise, désactivez l’option **[!UICONTROL Est active]** pour la désactiver ou activez l’option pour l’activer.

   Ou

   Pour plusieurs sociétés, sélectionnez **[!UICONTROL Non]** dans le menu déroulant **[!UICONTROL Est actif]** pour les désactiver ou **[!UICONTROL Oui]** pour les activer.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
