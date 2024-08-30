---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Nom d’utilisateur ou d’utilisatrice déjà utilisé
description: Si vous recevez une erreur indiquant que le nom d’utilisateur ou d’utilisatrice est déjà utilisé, lisez ces conseils.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 98%

---

# Nom d’utilisateur déjà utilisé

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Administrateur ou administratrice système</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Questions

Lors de la création d’un utilisateur ou d’une utilisatrice, une erreur [!UICONTROL Oups] s’affiche, indiquant que le nom d’utilisateur ou d’utilisatrice est déjà utilisé. Le système ne comporte aucune autre occurrence de cet e-mail. Pourquoi ce message s’affiche-t-il ?

## Solution

Cela peut se produire si le nom d’utilisateur ou d’utilisatrice ou l’adresse e-mail n’est pas unique dans l’instance [!DNL Adobe Workfront] active. Les utilisateurs et utilisatrices peuvent avoir le même nom d’utilisateur ou d’utilisatrice ou la même adresse e-mail dans des instances distinctes. Par exemple, l’utilisateur ou l’utilisatrice A peut avoir les adresses e-mail suivantes associées à un compte [!DNL Workfront] : utilisateurouutilisatricea@entreprise1.com et utilisateurouutilisatricea@entreprise2.com.

>[!NOTE]
>
>La personne principale chargée de l’administratrion de [!DNL Workfront] ne peut pas avoir le même nom d’utilisateur ou d’utilisatrice ou la même adresse e-mail s’il s’agit d’instances Workfront distinctes sur le même cluster.
>
>Si les instances se trouvent sur des clusters différents, la personne principale chargée de l’administration peut avoir le même nom d’utilisateur ou d’utilisatrice ou la même adresse e-mail. Vous pouvez afficher le cluster sur lequel se trouve votre instance via [!UICONTROL Configuration] > [!UICONTROL Système] > [!UICONTROL Infos client].

### Vérifiez si votre nom d’utilisateur ou d’utilisatrice est unique dans votre instance.

Veillez à ce que le nom d’utilisateur ou d’utilisatrice et l’adresse e-mail soient uniques dans l’instance [!DNL Workfront] actuelle :

{{step-1-to-users}}

1. Dans la liste des personnes, consultez la colonne **[!UICONTROL E-mail]** pour vous assurer qu’il n’y a pas d’adresses e-mails en double.
1. Ajoutez une colonne pour le nom d’utilisateur ou d’utilisatrice à la vue.

   1. Dans le menu déroulant **[!UICONTROL Vue]**, cliquez sur **[!UICONTROL Personnaliser la vue]**.
   1. Cliquez sur **[!UICONTROL Ajouter une colonne]**.
   1. Dans le champ de recherche, saisissez le *[!UICONTROL nom d’utilisateur ou d’utilisatrice]*.
   1. Sélectionnez **[!UICONTROL Utilisateur ou utilisatrice]** > **[!UICONTROL Nom d’utilisateur ou d’utilisatrice]**.
   1. Enregistrez la vue.\
      Vous obtenez ainsi une vue des noms d’utilisateur ou d’utilisatrice dans laquelle vous pouvez rechercher des doublons.

1. Dans la liste des personnes, consultez la colonne **[!UICONTROL Nom d’utilisateur ou d’utilisatrice]** pour vous assurer qu’il n’y a pas de doublons.
