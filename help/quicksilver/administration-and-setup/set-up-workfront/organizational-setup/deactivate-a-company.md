---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Désactiver ou réactiver une entreprise
description: Vous pouvez désactiver une entreprise que vous n’utilisez plus tout en conservant toutes les données historiques qui lui sont associées. Si vous désactivez une entreprise déjà utilisée quelque part dans le système, elle continue à fonctionner comme avant. Elle n’est ni supprimée ni bloquée.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: 30b61b32add4c6d062b5b524773d309008c9563d
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 63%

---

# Désactiver ou réactiver une entreprise

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

Vous pouvez désactiver une entreprise que vous n’utilisez plus tout en conservant toutes les données historiques qui lui sont associées. Si vous désactivez une entreprise déjà utilisée quelque part dans le système, elle continue à fonctionner comme avant. Elle n’est ni supprimée ni bloquée.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] paquet</p> </td> 
   <td><p>Tous</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
  <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Le niveau d'accès [!UICONTROL System Administrator], qui permet de modifier n'importe quelle société du système.</p> </li> 
     <li> <p>Accès administratif pour gérer les sociétés, ce qui vous permet de modifier n’importe quelle société du système.</p> </li> 
    </ul> <p><b>NOTE</b> :  
     <ul> 
      <li> <p>Vous pouvez également gérer les entreprises associées à un groupe pour lequel vous faites partie de l’équipe d’administration.</p> </li> 
      <li> <p>Pour ajouter et supprimer des utilisateurs du système [!DNL Workfront], vous devez disposer de l’un des éléments suivants :</p> 
       <ul> 
        <li> <p>Niveau d’accès [!UICONTROL System Administrator]. </p> </li> 
        <li> <p><b>[!UICONTROL Users]</b> paramètre de votre niveau d'accès configuré pour <b> l'accès à[!UICONTROL Edit]</b>, avec <b>[!UICONTROL Create]</b> et au moins l'une des deux options <b>[!UICONTROL User Admin]</b> activées sous <b>[!UICONTROL Affiner vos paramètres]</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p> <img src="assets/access-req-users.png"> </p> <p>De ces deux options, si <b>[!UICONTROL User Admin (Group Users)]</b> est activé, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Désactiver ou réactiver une entreprise

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Entreprises]** ![Icône Entreprises](assets/companies-icon-left-panel.png).

1. Sélectionnez une ou plusieurs entreprises à désactiver ou réactiver.
1. Cliquez sur **[!UICONTROL Modifier]**.<!--MAKE THIS A SEPARATE NUMBERED LINE<span class="preview">In the Preview environment, disable the **[!UICONTROL Is Active]** option to deactivate it, or enable the option to activate it.</span>-->
1. <!--In the Production environment, -->Pour une seule entreprise, désactivez l’option **[!UICONTROL Est active]** pour la désactiver ou activez l’option pour l’activer.

   Ou

   Pour plusieurs entreprises, sélectionnez **[!UICONTROL Non]** dans le menu déroulant **[!UICONTROL Est active]** pour les désactiver, ou **[!UICONTROL Oui]** pour les activer.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
