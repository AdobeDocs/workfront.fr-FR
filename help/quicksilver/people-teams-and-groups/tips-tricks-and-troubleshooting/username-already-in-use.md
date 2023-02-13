---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Nom d’utilisateur déjà utilisé
description: Lisez ces conseils lorsque vous obtenez une erreur indiquant que le nom d’utilisateur est déjà utilisé.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Nom d’utilisateur déjà utilisé

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license</strong></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Questions

Lors de la création d’un utilisateur, une [!UICONTROL Oups] s’affiche et indique que le nom d’utilisateur a déjà été utilisé. Il n’existe aucune autre occurrence de cet email dans le système. Pourquoi est-ce affiché ?

## Solution

Cela peut se produire, car le nom d’utilisateur ou l’adresse électronique n’est pas unique dans la variable active. [!DNL Adobe Workfront] instance. Les utilisateurs peuvent avoir le même nom d’utilisateur ou la même adresse électronique dans des instances distinctes. Par exemple, l’utilisateur A peut avoir les adresses électroniques suivantes associées à une [!DNL Workfront] compte : usera@company1.com et usera@company2.com.

>[!NOTE]
>
>La Principale [!DNL Workfront] L’administrateur ne peut pas avoir le même nom d’utilisateur ou la même adresse électronique s’il se trouve dans des instances Workfront distinctes sur le même cluster.
>
>Si les instances se trouvent sur des grappes différentes, l’administrateur Principal peut avoir le même nom d’utilisateur ou la même adresse électronique. Vous pouvez afficher la grappe sur laquelle se trouve votre instance. [!UICONTROL Configuration] > [!UICONTROL Système] > [!UICONTROL Informations sur le client].

### Vérifiez si votre nom d’utilisateur est unique dans votre instance.

Assurez-vous que le nom d’utilisateur et l’adresse électronique sont uniques dans la variable actuelle [!DNL Workfront] instance :

1. Comme la variable [!DNL Workfront] administrator, cliquez sur **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Utilisateurs]**.
1. Dans la liste des personnes, regardez dans la **[!UICONTROL Email]** pour vous assurer qu’il n’y a pas de doublon d’emails.
1. Ajoutez une colonne pour le nom d’utilisateur à la vue.

   1. Dans le **[!UICONTROL Affichage]** menu déroulant, cliquez sur **[!UICONTROL Vue Personnaliser]**.
   1. Cliquez sur **[!UICONTROL Ajouter une colonne]**.
   1. Dans le champ de recherche, saisissez *[!UICONTROL username]*.
   1. Sélectionner **[!UICONTROL Utilisateur]** > **[!UICONTROL Nom d’utilisateur]**.
   1. Enregistrez la vue.\
      Vous obtenez ainsi une vue affichant les noms d’utilisateur dans laquelle vous pouvez rechercher le doublon.

1. Dans la liste des personnes, regardez dans la **[!UICONTROL Nom d’utilisateur]** pour vous assurer qu’il n’y a pas de noms d’utilisateur en double.
