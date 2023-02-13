---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Limitation de l’accès à Adobe Workfront par adresse IP
description: Vous pouvez configurer une liste autorisée IP Adobe Workfront qui limite l’accès à Workfront à 45 adresses IP ou plages d’adresses IP que vous spécifiez. Cela fournit une couche supplémentaire de sécurité pour l’application Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 1%

---

# Limitation de l’accès à Adobe Workfront par adresse IP

Vous pouvez configurer une liste autorisée IP Adobe Workfront qui limite l’accès à Workfront à 45 adresses IP ou plages d’adresses IP que vous spécifiez. Cela fournit une couche supplémentaire de sécurité pour l’application Workfront.

Ces adresses IP ou plages d’adresses doivent être fournies par votre administrateur réseau.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Entreprise</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Autres listes autorisées

Si votre pare-feu ou serveur de messagerie est configuré pour autoriser l’accès à certains fournisseurs uniquement, vous devez ajouter certaines adresses IP à sa liste autorisée. Cela permet d’établir une communication entre votre environnement et les serveurs Adobe Workfront. Pour plus d’informations à ce sujet, voir [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

En outre, si votre entreprise utilise le forfait Enterprise, vous pouvez configurer la liste autorisée de messagerie de Workfront pour contrôler quels domaines de messagerie sont autorisés à accepter les courriers électroniques de Workfront et quels domaines de messagerie peuvent se trouver dans l’adresse électronique que les utilisateurs spécifient dans leur profil utilisateur Workfront. Pour plus d’informations, voir [Configuration de votre liste autorisée de messagerie](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Ajout d’adresses IP à la liste autorisée

Une fois que vous avez ajouté des adresses IP à la liste autorisée Workfront, seules ces adresses IP peuvent être utilisées pour accéder à Workfront. Les utilisateurs qui tentent d’accéder à Workfront à partir d’une autre adresse IP reçoivent un message d’erreur indiquant que leur adresse IP est bloquée.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Informations sur le client.**

1. Dans le **LISTE AUTORISÉE IP** , sélectionnez **Activez la liste autorisée IP.**

   Cette option est désactivée par défaut.

1. Indiquez l’adresse IP que vous utilisez actuellement pour accéder au système Workfront.

   Ou

   Indiquez une plage d’adresses IP qui inclut celle que vous utilisez actuellement pour accéder au système Workfront.

   L’adresse IP que vous utilisez pour accéder à Workfront doit être ajoutée à la liste autorisée avant l’activation de la liste autorisée.

1. Cliquez sur **Ajouter une plage d’adresses IP,** indiquez ensuite l’adresse IP ou la plage d’adresses IP auxquelles vous souhaitez pouvoir accéder à Workfront.
1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres adresses IP ou plages d’adresses.

   Vous pouvez ajouter jusqu’à 45 adresses ou plages.

1. Cliquer sur **Enregistrer.**
