---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Désactivation ou réactivation d’une entreprise
description: Vous pouvez désactiver une société que vous n’utilisez plus tout en conservant toutes ses données historiques associées. Si vous désactivez une entreprise déjà utilisée quelque part dans le système, elle continue à fonctionner comme elle l’a toujours fait. Il n’est ni supprimé ni bloqué.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Désactivation ou réactivation d’une entreprise

Vous pouvez désactiver une société que vous n’utilisez plus tout en conservant toutes ses données historiques associées. Si vous désactivez une entreprise déjà utilisée quelque part dans le système, elle continue à fonctionner comme elle l’a toujours fait. Il n’est ni supprimé ni bloqué.

## Exigences d’accès

Pour gérer les entreprises dans , vous devez disposer des éléments suivants : [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan*</p> </td> 
   <td>[!UICONTROL Team] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>L’une des options suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès [!UICONTROL Administrateur système] qui permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
     <li> <p>Accès administratif pour la gestion des entreprises, ce qui vous permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </li> 
    </ul> <p><b>NOTE</b>:  
     <ul> 
      <li> <p>Vous pouvez également gérer les entreprises associées à n’importe quel groupe auquel vous êtes affecté en tant qu’administrateur de groupe.</p> </li> 
      <li> <p>Pour ajouter et supprimer des utilisateurs du [!DNL Workfront] système, vous devez disposer de l’une des fonctionnalités suivantes :</p> 
       <ul> 
        <li> <p>Niveau d’accès [!UICONTROL Administrateur système]. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
        <li> <p>Dans votre niveau d’accès, [!UICONTROL Modifier] doit être sélectionné pour le paramètre [!UICONTROL Utilisateurs] . En outre, pour le paramètre [!UICONTROL Utilisateurs] , sous [!UICONTROL Ajuster vos paramètres] <img src="assets/gear-icon-in-access-levels.png"> , l’option [!UICONTROL Créer] et au moins l’une des deux options [!UICONTROL User Admin] doivent être activées. </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>Si vous utilisez l’option [!UICONTROL User Admin (Group Users)], vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
       </ul> <p>Pour plus d’informations sur le paramètre Utilisateurs dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Désactivation ou réactivation d’une entreprise

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe] Workfront, puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Entreprises]** ![](assets/companies-icon-left-panel.png).

1. Sélectionnez une ou plusieurs sociétés à désactiver ou à réactiver.
1. Cliquez sur **[!UICONTROL Modifier]**.
1. Pour une seule entreprise, désactivez la variable **[!UICONTROL Est Principal]** pour la désactiver ou activer l’option pour l’activer.

   Ou

   Pour plusieurs entreprises, sélectionnez **[!UICONTROL Non]** de la **[!UICONTROL Est Principal]** pour les désactiver, ou **[!UICONTROL Oui]** pour les activer.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
