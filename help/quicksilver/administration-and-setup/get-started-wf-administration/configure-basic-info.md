---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configuration des informations de base pour votre système
description: Dans le cadre de la configuration de votre système Adobe Workfront, vous pouvez gérer les détails sur votre organisation dans la section Informations de base de votre page Informations sur le client .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 2%

---

# Configuration des informations de base pour votre système

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Dans le cadre de la configuration de votre système Adobe Workfront, vous pouvez gérer les détails sur votre organisation dans la section Informations de base de votre page Informations sur le client .

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Accès aux informations sur le client

Le client représente l’instance Workfront de votre entreprise. En tant que client de Workfront, les options disponibles dans cette zone vous sont propres.

Pour accéder à la page Informations sur le client :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Système** > **Informations sur le client**.

   Selon le plan Workfront que vous avez acheté, il se peut que certaines sections ne figurent pas dans la page Informations sur le client . Contactez votre gestionnaire de compte si vous devez déterminer le plan Workfront utilisé par votre entreprise.

   Les sections disponibles dans la zone Informations sur le client sont les suivantes :

   * **Informations de base**

      Pour plus d’informations sur la configuration des informations de base dans Workfront, voir [Configuration des informations de base](#configure-basic-info).

   * **Paramètres de la clé API**

      Pour plus d’informations sur les paramètres de clé API, voir [Gestion des clés d’API](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **Liste autorisée d’adresses IP**

      Pour plus d’informations sur l’ajout des adresses IP à votre liste autorisée pour l’emplacement où vos utilisateurs peuvent accéder à Workfront, voir [Configuration de la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **Licence**

      Pour plus d’informations sur les licences, voir [Gestion des licences disponibles dans votre système](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## Configuration des informations de base {#configure-basic-info}

Dans la zone Informations de base de votre page Informations sur le client, certains détails sur votre client sont configurés par Workfront et s’affichent en lecture seule. Vous pouvez configurer d’autres détails. Toutes les options que vous pouvez modifier dans cette zone ont un effet global sur tous les utilisateurs de Workfront.

Pour configurer votre section Informations de base dans votre zone Informations sur le client :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Système** > **Informations sur le client**.

1. Dans le **Informations de base** en haut de la page **Informations sur le client** recherchez les informations suivantes sur votre instance avec Workfront :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td>Nom de votre organisation, qui correspond également au nom de votre société. Il est ajouté par Workfront et ne peut pas être modifié.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuration du cluster </td> 
      <td>Numéro de grappe de votre instance.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Adresse e-mail de l'administrateur</td> 
      <td> <p>Adresse électronique de votre administrateur Workfront. Vous pouvez modifier ce champ pour qu’il corresponde à l’adresse électronique de l’un de vos administrateurs Workfront. L’utilisateur associé à cette adresse électronique est considéré comme le principal administrateur Workfront de votre système Workfront. Toute communication à l’échelle du site provenant de Workfront est dirigée vers cette adresse électronique. Il est donc important de la mettre à jour.</p> <p><b>REMARQUE</b>: Vous ne pouvez pas désactiver, supprimer ou modifier le niveau d’accès de l’utilisateur associé à l’adresse électronique d’administrateur.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domaine</td> 
      <td> <p>Le domaine est défini par Workfront lors de la création de votre compte.</p> <p>Le domaine identifie votre sous-domaine unique de l’URL que vous utilisez pour accéder à Workfront.<p>Par exemple, si le domaine "mycompany" a été attribué à votre organisation, l’URL que vous utilisez pour accéder à Workfront est <i>https://mycompany.my.workfront.com.</i></p><p>Vous ne pouvez pas modifier le domaine vous-même. Si vous souhaitez modifier votre domaine, vous pouvez contacter le service clientèle de Workfront. Pour plus d’informations sur les contacts avec le service clientèle de Workfront, voir <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contacter le service clientèle</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuseau horaire</td> 
      <td> <p>Il s’agit du fuseau horaire par défaut de votre instance Workfront. Vous pouvez modifier ce champ pour qu’il corresponde au fuseau horaire de votre Principal emplacement Workfront. Le fuseau horaire sélectionné détermine ce qui suit : </p> 
       <ul> 
        <li>Date et heure affichées dans les emails sortants</li> 
        <li>Fuseau horaire par défaut pour les nouveaux utilisateurs lorsqu’ils sont créés</li> 
       </ul> <p>Les utilisateurs peuvent modifier le fuseau horaire de leur instance Workfront sous leur profil. Lorsque les utilisateurs modifient leur fuseau horaire, la date et l’heure de leurs emails en provenance de Workfront correspondent à leurs préférences de profil. Pour plus d’informations sur la modification des préférences de profil utilisateur, voir <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurer mes paramètres</a>. Il est sélectionné comme fuseau horaire par défaut lors de la création d’un nouveau planning. Pour plus d’informations sur la création de plannings, voir <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Création d’un planning</a>.</p> <p>Pour plus d’informations sur l’utilisation des plannings pour aider les utilisateurs à collaborer dans Workfront dans les fuseaux horaires, voir <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Utilisation des fuseaux horaires</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Paramètre local</td> 
      <td>Contrôle le format de la langue, de la date et du numéro utilisé dans les emails sortants. Le paramètre régional sélectionné ici est le paramètre régional par défaut lors de la création de nouveaux utilisateurs. Les utilisateurs peuvent modifier leurs paramètres régionaux dans leur profil utilisateur. Lorsque les utilisateurs modifient leurs paramètres régionaux, le format de langue, de date et de numéro dans leurs emails depuis Workfront correspond à leurs préférences de profil. Pour plus d’informations sur la modification des préférences de profil, voir <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurer mes paramètres</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Pourcentage de stockage</td> 
      <td> <p>Il s’agit de la quantité d’espace de stockage de documents disponible dans votre instance Workfront.<br>Le quota contient les documents que vous téléchargez directement dans Workfront.<br>Elle ne comprend pas :</p> 
       <ul> 
        <li>Documents que vous liez à Workfront à partir de tout autre fournisseur de services tiers (SharePoint, Google Drive, Webdam, Box, Dropbox, tout autre fournisseur Document Asset Management).</li> 
        <li>Vos données Workfront (projets, tâches, problèmes, utilisateurs, etc.).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Version du produit</td> 
      <td>Il s’agit du type d’instance Workfront qui vous est affectée. La version du produit de la plupart des clients Workfront est la suivante : <strong>Entreprise</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.
