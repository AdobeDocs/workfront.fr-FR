---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurer Votre Place sur la liste autorisée E-Mail
description: Si votre entreprise utilise la formule Entreprise de Workfront, vous pouvez créer une liste autorisée d’e-mails Workfront pour contrôler les domaines d’e-mails autorisés à recevoir des e-mails de Workfront, mais aussi définir les domaines d’e-mails utilisables dans l’adresse e-mail spécifiée dans le profil de l’utilisateur ou de l’utilisatrice. Cela s’avère utile si la politique de sécurité de votre entreprise empêche les utilisateurs et les utilisatrices d’envoyer des données stockées dans Workfront à des adresses e-mail externes. Vous pouvez inclure uniquement les domaines internes de votre société dans la liste autorisée pour vous assurer que cette politique est respectée.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: 937965ad495453e185504d53f9d9c88c3cd7e201
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 95%

---

# Configurer votre liste autorisée d’e-mails

Si votre entreprise utilise le plan d’entreprise Workfront, vous pouvez créer un e-mail Workfront placer sur la liste autorisée afin de contrôler :

* Les domaines d’e-mails autorisés à accepter les e-mails de Workfront.
* Les domaines d’e-mails pouvant se trouver dans l’adresse e-mail que les utilisateurs et les utilisatrices spécifient dans leur profil.

Cela s’avère utile si la politique de sécurité de votre entreprise empêche les utilisateurs et les utilisatrices d’envoyer des données stockées dans Workfront à des adresses e-mail externes. Vous pouvez inclure uniquement les domaines internes de votre société dans la liste autorisée pour vous assurer que cette politique est respectée.

>[!IMPORTANT]
>
>Votre équipe informatique doit s’assurer que les e-mails entrants provenant de `notifications@my.workfront.com` ne sont pas bloqués dans le système de votre entreprise.
>
>Tous les e-mails provenant de Workfront sont envoyés à partir de cette adresse afin d’augmenter le succès de la diffusion des e-mails et d’éliminer les usurpations des e-mails. Cela inclut les alertes automatisées et la communication entre utilisateurs et utilisatrices.
>
>Par exemple, la ligne De dans un e-mail Workfront que vous recevez d’une utilisatrice nommée Joan Harris ressemblerait à ceci :
>`Joan Harris <notifications@my.workfront.com>`

Pour plus d’informations sur la configuration du pare-feu de votre entreprise pour ouvrir la communication entre votre environnement et les serveurs Adobe Workfront, consultez [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices</a>.</p> <p><b>NOTE</b> : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront si des restrictions supplémentaires sont définies pour votre niveau d’accès. Pour plus d’informations sur la façon dont l’administrateur ou l’administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Autres listes autorisées

Si votre entreprise dispose de la formule Entreprise, vous pouvez configurer une liste autorisée d’adresses IP d’Adobe Workfront qui limite l’accès à Workfront à 75 adresses IP ou plages d’adresses IP que vous spécifiez. Cela fournit une couche supplémentaire de sécurité pour l’application Workfront. Pour plus d’informations, consultez [Limiter l’accès à Adobe Workfront en fonction de l’adresse IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Aussi, si votre pare-feu ou serveur de messagerie est configuré pour autoriser l’accès à certains fournisseurs uniquement, vous devez ajouter certaines adresses IP à sa liste autorisée. Cela permet d’établir une communication entre votre environnement et les serveurs Adobe Workfront. Pour plus d’informations à ce sujet, consultez [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurer votre liste autorisée d’e-mails

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Infos client**.
1. Dans la section **Liste autorisée d’e-mails**, sélectionnez **Activer la liste autorisée de domaines**, puis cliquez sur **Ajouter un domaine**.
1. Dans la zone qui s’affiche, saisissez un domaine que vous souhaitez autoriser, par exemple `ourcompany.com`, puis cliquez sur **Ajouter un domaine**.
1. Répétez l’étape précédente pour ajouter les autres domaines que vous souhaitez autoriser.
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.
