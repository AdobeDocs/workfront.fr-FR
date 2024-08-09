---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configuration de votre Liste autorisée de messagerie
description: Si votre entreprise utilise le plan WorkfrontEnterprise, vous pouvez créer une liste autorisée de messagerie Workfront pour contrôler quels domaines de messagerie sont autorisés à accepter les courriers électroniques de Workfront et quels domaines de messagerie peuvent se trouver dans l’adresse que les utilisateurs spécifient dans leur profil utilisateur. Cela s’avère utile si la stratégie de sécurité de votre entreprise empêche les utilisateurs d’envoyer des données stockées dans Workfront à des adresses électroniques externes. Vous pouvez inclure uniquement les domaines internes de votre société dans la liste autorisée pour vous assurer que cette stratégie est respectée.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 17%

---

# Configuration de votre liste autorisée de messagerie

Si votre entreprise utilise le forfait Workfront Enterprise, vous pouvez créer une liste autorisée de messagerie Workfront à contrôler :

* Les domaines de messagerie autorisés à accepter les courriers électroniques de Workfront.
* Les domaines de messagerie pouvant se trouver dans l’adresse électronique que les utilisateurs spécifient dans leur profil utilisateur.

Cela s’avère utile si la stratégie de sécurité de votre entreprise empêche les utilisateurs d’envoyer des données stockées dans Workfront à des adresses électroniques externes. Vous pouvez inclure uniquement les domaines internes de votre société dans la liste autorisée pour vous assurer que cette stratégie est respectée.

>[!IMPORTANT]
>
>Votre équipe informatique doit s’assurer que les courriers électroniques entrants provenant de `notifications@my.workfront.com` ne sont pas bloqués dans le système de votre entreprise.
>
>Tous les courriers électroniques provenant de Workfront sont envoyés à partir de cette adresse afin d’augmenter le succès de la diffusion des emails et d’éliminer les usurpations des emails. Cela inclut les alertes automatisées et la communication utilisateur-utilisateur.
>
>Par exemple, la ligne De dans un email Workfront que vous recevez d’un utilisateur nommé Joan Harris ressemblerait à ceci :
>`Joan Harris <notifications@my.workfront.com>`

Pour plus d’informations sur la configuration du pare-feu de votre entreprise pour ouvrir la communication entre votre environnement et les serveurs Adobe Workfront, voir [Configuration de la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices</a>.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Autres listes autorisées

Si votre entreprise dispose du plan d’entreprise, vous pouvez configurer une liste autorisée IP Adobe Workfront qui limite l’accès à Workfront à 45 adresses IP ou plages d’adresses que vous spécifiez. Cela fournit une couche supplémentaire de sécurité pour l’application Workfront. Pour plus d’informations, voir [Limiter l’accès à Adobe Workfront en fonction de l’adresse IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

En outre, si votre pare-feu ou votre serveur de messagerie est configuré pour autoriser l’accès à certains fournisseurs uniquement, vous devez ajouter certaines adresses IP à sa liste autorisée. Cela permet d’établir une communication entre votre environnement et les serveurs Adobe Workfront. Pour plus d’informations à ce sujet, voir [Configuration de la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configuration de votre liste autorisée de messagerie

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Informations sur le client**.
1. Dans la section **Liste autorisée email**, sélectionnez **Activer la Liste autorisée de domaine**, puis cliquez sur **Ajouter un domaine**.
1. Dans la zone qui s’affiche, saisissez un domaine que vous souhaitez autoriser, par exemple `ourcompany.com`, puis cliquez sur **Ajouter un domaine**.
1. Répétez l’étape précédente pour ajouter les autres domaines que vous souhaitez autoriser.
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.
