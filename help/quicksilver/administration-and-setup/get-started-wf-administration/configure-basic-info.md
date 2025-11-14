---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configuration des informations de base pour votre système
description: Dans le cadre de la configuration de votre système Adobe Workfront, vous pouvez gérer les détails sur votre organisation dans la section Informations de base de votre page Infos client.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: 01a80f6140650ca12aaee14115f79449dcfa2a18
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 92%

---

# Configurer des informations de base pour votre système

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Dans le cadre de la configuration de votre système Adobe Workfront, vous pouvez gérer les détails sur votre organisation dans la section Informations de base de votre page Infos client.

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

## Accéder à la page Infos client

Le client ou la cliente représente l’instance Workfront de votre organisation. En tant que client ou cliente Workfront, les options disponibles dans cette zone vous sont propres.

Pour accéder à la page Infos client :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Infos client**.

   Selon le package Workfront que vous avez acheté, certaines sections peuvent être manquantes dans la page Informations sur le client. Contactez votre représentant de compte si vous avez besoin de connaître le package Workfront utilisé par votre organisation.

   Les sections disponibles dans la zone Infos client sont les suivantes :

   * **Informations de base**

     Pour plus d’informations sur la configuration des informations de base dans Workfront, voir [Configurer les informations de base](#configure-basic-info).

   * **Paramètres de la clé API**

     Pour plus d’informations sur les paramètres de la clé API, voir [Gérer les clés API](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **Liste autorisée d’adresses IP**

     Pour plus d’informations sur l’ajout des adresses IP à votre liste autorisée pour l’emplacement où vos utilisateurs et utilisatrices peuvent accéder à Workfront, voir [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * placer sur la liste autorisée **E-mail**

     Pour plus d’informations sur l’ajout d’e-mails à votre placer sur la liste autorisée place sur la liste autorisée, voir [Configurer votre e-mail](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

   <!--
   * **License**

     For information about licenses, see [Manage available licenses in your system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).-->

## Configurer les informations de base {#configure-basic-info}

Dans la zone Informations de base de votre page Infos client, certains détails sur votre client ou votre cliente sont configurés par Workfront et s’affichent en lecture seule. Vous pouvez en configurer d’autres. Toutes les options que vous pouvez modifier dans cette zone ont un effet global sur l’ensemble des personnes utilisant Workfront.

Pour configurer votre section Informations de base dans votre zone Infos client :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Infos client**.

1. Dans la section **Informations de base** en haut de la page **Infos client**, recherchez les informations suivantes sur votre instance avec Workfront :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td>Le nom de votre organisation, qui correspond également au nom de votre société. Il est ajouté par Workfront et ne peut pas être modifié.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuration du cluster </td> 
      <td>Le numéro de cluster de votre instance.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Adresse e-mail de l'administrateur</td> 
      <td> <p>L’adresse e-mail de votre administrateur ou administratrice Workfront. Vous pouvez modifier ce champ pour qu’il corresponde à l’adresse e-mail de l’une de vos personnes administratrices de Workfront. La personne associée à cette adresse e-mail est considérée comme la principale personne administratrice Workfront de votre système Workfront. Toute communication à l’échelle du site provenant de Workfront est dirigée vers cette adresse e-mail. Il est donc important de la mettre à jour.</p> <p><b>NOTE</b> : vous ne pouvez pas désactiver, supprimer ou modifier le niveau d’accès de la personne associée à l’adresse e-mail de la personne administratrice.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domaine</td> 
      <td> <p>Le domaine est défini par Workfront lors de la création de votre compte.</p> <p>Le domaine identifie votre sous-domaine unique de l’URL que vous utilisez pour accéder à Workfront.<p>Par exemple, si le domaine « monentreprise » a été attribué à votre organisation, l’URL que vous utilisez pour accéder à Workfront est <i>https://monentreprise.my.workfront.com.</i>.</p><p>Vous ne pouvez pas modifier le domaine vous-même. Si vous souhaitez modifier votre domaine, vous pouvez contacter le service clientèle de Workfront. Pour plus d’informations sur le contact avec le service clientèle de Workfront, voir <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contacter le service clientèle</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuseau horaire</td> 
      <td> <p>Il s’agit du fuseau horaire par défaut de votre instance Workfront. Vous pouvez modifier ce champ pour qu’il corresponde au fuseau horaire de votre emplacement Workfront principal. Le fuseau horaire que vous sélectionnez détermine ce qui suit : </p> 
       <ul> 
        <li>La date et l’heure qui s’affichent dans les e-mails sortants.</li> 
        <li>Le fuseau horaire par défaut pour les nouveaux utilisateurs et utilisatrices lors de leur création.</li> 
       </ul> <p>Les utilisateurs et utilisatrices peuvent modifier le fuseau horaire de leur instance Workfront dans leur profil. Lorsque les utilisateurs et les utilisatrices modifient leur fuseau horaire, la date et l’heure de leurs e-mails envoyés à partir de Workfront correspondent à leurs préférences de profil. Pour plus d’informations sur la modification des préférences de profil des utilisateurs et utilisatrices, voir <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurer mes paramètres</a>. Ce fuseau horaire est sélectionné comme fuseau horaire par défaut lorsque vous créez un nouveau planning. Pour plus d’informations sur la création de plannings, voir <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Créer un planning</a>.</p> <p>Pour plus d’informations sur l’utilisation des plannings pour aider les utilisateurs et les utilisatrices à collaborer avec des fuseaux horaires différents dans Workfront, voir <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Travailler avec des fuseaux horaires différents</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Paramètres régionaux d’e-mail par défaut</td> 
      <td>Contrôle les formats de langue, de date et de nombres utilisés dans les e-mails sortants. Les paramètres régionaux sélectionnés ici sont utilisés par défaut lors de la création de nouveaux utilisateurs et de nouvelles utilisatrices. Les utilisateurs et les utilisatrices peuvent modifier leurs paramètres régionaux dans leur profil d’utilisateur ou d’utilisatrice. Lorsque les utilisateurs et les utilisatrices modifient leurs paramètres régionaux, les formats de langue, de date et de nombres dans leurs e-mails envoyés à partir de Workfront correspondent à leurs préférences de profil. Pour plus d’informations sur la modification de vos préférences de profil, voir <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurer mes paramètres</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pourcentage de stockage</td> 
      <td> <p>Il s’agit de la quantité d’espace de stockage de documents disponible dans votre instance Workfront.<br>Le quota contient les documents que vous chargez directement dans Workfront.<br>Il n’inclut pas les éléments suivants :</p> 
       <ul> 
        <li>Les documents que vous liez à Workfront à partir de tout autre fournisseur de services tiers (SharePoint, Google Drive, WebDam, Box, Dropbox, ou tout autre fournisseur de gestion des ressources numériques).</li> 
        <li>Vos données Workfront (projets, tâches, problèmes, utilisateurs et utilisatrices, etc.).</li> 
       </ul> </td> 
     </tr>
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.
