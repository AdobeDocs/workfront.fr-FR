---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Restreindre l’accès à Adobe Workfront par adresse IP
description: Vous pouvez configurer une liste autorisée d’adresses IP d’Adobe Workfront qui limite l’accès à Workfront à 75 adresses IP ou plages d’adresses IP que vous spécifiez. Cela fournit une couche supplémentaire de sécurité pour l’application Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 22ae8b489c63ba6eea1472cf415f95e375a94773
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 97%

---

# Limiter l’accès à Adobe Workfront en fonction de l’adresse IP

<!--
>[!IMPORTANT]
>
>This functionality is not currently available to organizations that have been onboarded to the Adobe Admin Console. It will be available in the Adobe Admin Console in a future release. -->

Vous pouvez configurer une liste autorisée d’adresses IP d’Adobe Workfront qui limite l’accès à Workfront à 75 adresses IP ou plages d’adresses IP que vous spécifiez. Cela fournit une couche supplémentaire de sécurité pour l’application Workfront.

Ces adresses IP ou plages d’adresses doivent être fournies par votre administrateur ou administratrice réseau.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Autres listes autorisées

Si votre pare-feu ou serveur de messagerie est configuré pour accorder l’accès uniquement à certains fournisseurs, vous devez ajouter certaines adresses IP à sa liste autorisée. Cela permet d’établir une communication entre votre environnement et les serveurs Adobe Workfront. Pour plus d’informations à ce sujet, consultez [Configurer la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

En outre, si votre entreprise utilise la formule Entreprise, vous pouvez configurer la liste autorisée de messagerie de Workfront pour contrôler quels domaines de messagerie sont autorisés à accepter les e-mails de Workfront et quels domaines de messagerie peuvent se trouver dans l’adresse e-mail que les utilisateurs et utilisatrices spécifient dans leur profil utilisateur Workfront. Pour plus d’informations, voir [Configurer votre liste autorisée de messagerie](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Ajout d’adresses IP à la liste autorisée

Une fois que vous avez ajouté des adresses IP à la liste autorisée Workfront, seules ces adresses IP peuvent être utilisées pour accéder à Workfront. Les personnes qui tentent d’accéder à Workfront depuis une autre adresse IP reçoivent un message d’erreur indiquant que leur adresse IP est bloquée.

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Infos client**.

1. Dans la section **Liste autorisée d’adresses IP**, sélectionnez **Activer la liste autorisée d’adresses IP.**

   Cette option est désactivée par défaut.

1. Indiquez l’adresse IP que vous utilisez actuellement pour accéder au système Workfront.

   Ou

   Indiquez une plage d’adresses IP qui inclut celle que vous utilisez actuellement pour accéder au système Workfront.

   L’adresse IP que vous utilisez pour accéder à Workfront doit être ajoutée à la liste autorisée avant l’activation de la liste autorisée.

1. Cliquez sur **Ajouter une plage d’adresses IP,** indiquez ensuite l’adresse IP ou la plage d’adresses IP que vous souhaitez voir accéder à Workfront.
1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres adresses IP ou plages d’adresses.

   Vous pouvez ajouter jusqu’à 75 adresses ou plages.

1. Cliquer sur **Enregistrer**.
