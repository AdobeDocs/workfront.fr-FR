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
TQID: https://experienceleague.adobe.com/a8hcTFpx3LmuGpQM8Wk8BpLDCFUVJWLAcP-YV5ogK0U
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 403
ht-degree: 89%

---

# Configurer votre liste autorisée d’e-mails

Si votre entreprise utilise le plan d’entreprise Workfront, vous pouvez créer un e-mail Workfront afin de contrôler :

* Les domaines d’e-mails autorisés à accepter les e-mails de Workfront.
* Les domaines d’e-mails pouvant se trouver dans l’adresse e-mail que les utilisateurs et les utilisatrices spécifient dans leur profil.

Cela s’avère utile si la politique de sécurité de votre entreprise empêche les utilisateurs et les utilisatrices d’envoyer des données stockées dans Workfront à des adresses e-mail externes. Vous pouvez inclure uniquement les domaines internes de votre société dans la liste autorisée pour vous assurer que cette politique est respectée.

>[!IMPORTANT]
>
>Votre équipe informatique doit s’assurer que les e-mails entrants provenant de `notifications@my.workfront.com` ne sont pas bloqués dans le système de votre entreprise.
>
>Tous les e-mails provenant de Workfront sont envoyés à partir de cette adresse afin d’augmenter le succès de la diffusion des e-mails et d’éliminer les usurpations des e-mails. Cela inclut les alertes automatisées et la communication entre utilisateurs et utilisatrices.
>
>Par exemple, la ligne De d’un e-mail Workfront que vous recevez d’un utilisateur nommé Joan Harris ressemble à ceci :
>`Joan Harris <notifications@my.workfront.com>`

Pour plus d’informations sur la configuration du pare-feu de votre entreprise pour ouvrir la communication entre votre environnement et les serveurs Adobe Workfront, consultez [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur ou une administratrice Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Autres listes autorisées

Si votre pare-feu ou serveur de messagerie est configuré pour accorder l’accès uniquement à certains fournisseurs, vous devez ajouter certaines adresses IP à sa liste autorisée. Cela permet d’établir une communication entre votre environnement et les serveurs Adobe Workfront. Pour plus d’informations à ce sujet, consultez [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurer votre liste autorisée d’e-mails

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Infos client**.
1. Dans la section **Liste autorisée d’e-mails**, sélectionnez **Activer la liste autorisée de domaines**, puis cliquez sur **Ajouter un domaine**.
1. Dans la zone qui s’affiche, saisissez un domaine que vous souhaitez autoriser, par exemple `ourcompany.com`, puis cliquez sur **Ajouter un domaine**.
1. Répétez l’étape précédente pour ajouter les autres domaines que vous souhaitez autoriser.
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.
