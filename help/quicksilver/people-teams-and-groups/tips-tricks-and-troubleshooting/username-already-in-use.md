---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Nom d’utilisateur ou d’utilisatrice déjà en cours d’utilisation
description: Lisez ces conseils lorsque vous obtenez une erreur indiquant que le nom d’utilisateur est déjà utilisé.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 11%

---

# Nom d’utilisateur ou d’utilisatrice déjà en cours d’utilisation

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence</strong></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Questions

Lors de la création d’un utilisateur, une erreur [!UICONTROL Whoops] s’affiche pour indiquer que le nom d’utilisateur est déjà utilisé. Il n’existe aucune autre occurrence de cet email dans le système. Pourquoi est-ce affiché ?

## Solution

Cela peut se produire, car le nom d’utilisateur ou l’adresse électronique n’est pas unique dans l’instance [!DNL Adobe Workfront] actuelle. Les utilisateurs peuvent avoir le même nom d’utilisateur ou la même adresse électronique dans des instances distinctes. Par exemple, l’utilisateur A peut avoir les adresses électroniques suivantes associées à un compte [!DNL Workfront] : usera@company1.com et usera@company2.com.

>[!NOTE]
>
>L&#39;administrateur principal [!DNL Workfront] ne peut pas avoir le même nom d&#39;utilisateur ou la même adresse électronique s&#39;il se trouve dans des instances Workfront distinctes sur le même cluster.
>
>Si les instances se trouvent sur des grappes différentes, l’administrateur principal peut avoir le même nom d’utilisateur ou la même adresse électronique. Vous pouvez afficher la grappe sur laquelle se trouve votre instance sous [!UICONTROL Configuration] > [!UICONTROL Système] > [!UICONTROL Informations sur le client].

### Vérifiez si votre nom d’utilisateur est unique dans votre instance.

Assurez-vous que le nom d’utilisateur et l’adresse électronique sont uniques dans l’instance [!DNL Workfront] actuelle :

1. En tant qu&#39;administrateur [!DNL Workfront], cliquez sur l&#39;icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Utilisateurs]**.
1. Dans la liste des personnes, recherchez dans la colonne **[!UICONTROL Email]** pour vous assurer qu’il n’y a pas de doublons d’emails.
1. Ajoutez une colonne pour le nom d’utilisateur à la vue.

   1. Dans le menu déroulant **[!UICONTROL Affichage]**, cliquez sur **[!UICONTROL Personnaliser la vue]**.
   1. Cliquez sur **[!UICONTROL Ajouter une colonne]**.
   1. Dans le champ de recherche, saisissez *[!UICONTROL nom d’utilisateur]*.
   1. Sélectionnez **[!UICONTROL User]** > **[!UICONTROL Username]**.
   1. Enregistrez la vue.\
      Vous obtenez ainsi une vue affichant les noms d’utilisateur dans laquelle vous pouvez rechercher le doublon.

1. Dans la liste des personnes, recherchez dans la colonne **[!UICONTROL Nom d’utilisateur]** pour vous assurer qu’il n’y a pas de noms d’utilisateur en double.
