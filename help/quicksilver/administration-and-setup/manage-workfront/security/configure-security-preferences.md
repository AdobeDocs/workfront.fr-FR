---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configure System Preferences
description: En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez configurer les préférences de votre système Workfront, y compris les préférences de sécurité.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 77b78c5905736092c972e08283fdabf321bfa580
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 72%

---

# Configurer les préférences système

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

{{important-admin-console-onboard}}

En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez configurer les préférences de votre système Workfront, notamment :

* L’accès à Workfront à partir d’applications mobiles et d’autres applications intégrées
* Règles d’incorporation de Workfront dans un iframe

Les modifications apportées aux préférences système ont un impact sur toutes les personnes présentes dans le système et sur leur expérience dans Workfront.

Nous vous recommandons de configurer vos préférences système lors de l’implémentation de Workfront et de ne les revoir qu’occasionnellement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
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

## Configurer les préférences système

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Préférences**.

1. Sélectionnez l’un des champs suivants pour définir les paramètres de votre entreprise :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Activer le processus de version rapide</p> </td> 
      <td>Permet d’activer les versions Workfront mensuelles pour votre organisation au lieu des versions trimestrielles.</p><p>Pour plus d’informations sur le processus de versions rapides, consultez la section <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Activer ou désactiver les versions rapides pour votre organisation</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Autoriser l’incorporation de Workfront dans un iframe</p> </td> 
      <td>Vous permet d’incorporer Workfront dans un iframe.<p>Cette option est désactivée par défaut.</p><p><b>IMPORTANT</b> : l’affichage d’une application web dans un iframe rend l’application vulnérable aux attaques par détournement de clic.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser l'authentification SAML 2.0 dans les modules complémentaires Office 365</td> 
      <td> <p>Vous permet d’incorporer Workfront dans un iframe uniquement pour les modules complémentaires Office 365 lorsque Workfront est intégré à une solution d’authentification unique SAML 2.0. </p> <p>Cette option est activée par défaut.</p> <p><b>NOTE</b> : si vous activez l’option ci-dessus, <strong>Autoriser l’incorporation de Workfront dans un iframe</strong>, l’option <strong>Autoriser l’authentification SAML 2.0 dans les modules complémentaires Office 365</strong> est activée et grisée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activer l’utilisation des informations de session lors de la création d’URL de page externe.</td> 
      <td> <p>Permet aux utilisateurs et utilisatrices d’utiliser les informations d’ID de session d’un site lors de l’ajout d’une page externe à un tableau de bord.</p> <p>Cette option n’est pas sécurisée et est désactivée par défaut. Il est recommandé d’utiliser OAuth à la place pour les intégrations.</p> <p>Pour plus d’informations sur l’ajout de pages externes à un tableau de bord, consultez la section <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incorporer une page web externe dans un tableau de bord</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Let people use Workfront's mobile applications</td> 
      <td> <p>Allows users to access the mobile apps (Workfront View for iPad and mobile phone apps)</p> <p>Cette option est activée par défaut. </p> <p>Pour plus d’informations sur Workfront View, consultez la section <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utiliser Adobe Workfront View</a>. Pour plus d’informations sur les applications mobiles, consultez la section <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Utiliser l’application mobile Adobe Workfront : index des articles</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collaborer avec des personnes sans les comptes Workfront en utilisant leur adresse e-mail</p> </td> 
      <td>Permet aux utilisateurs et utilisatrices de Workfront de partager certains éléments avec des personnes sans compte Workfront en incluant leur adresse e-mail au lieu de leur nom. Les utilisateurs et utilisatrices peuvent partager les éléments suivants avec des utilisateurs et utilisatrices externes à l’aide de leur adresse e-mail :
       <ul>
        <li>Document<br></li>
        <li>Demande de document<br></li>
        <li>Approbation de document</li>
        <li>Calendrier</li>
       </ul><p>Cette option est activée par défaut.</p> <p><b>Important</b> : le niveau d’accès Utilisateur ou utilisatrice externe n’est pas disponible dans votre instance Workfront si cette option est désactivée. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Niveaux d’accès intégrés</a>.</p> </td> 
     </tr> 
     <!--
     <tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>
     -->
     <tr> 
      <td role="rowheader">URL Aide</td> 
      <td>Vous permet de définir un site d’aide personnalisé interne vers lequel l’icône d’aide du menu principal redirigera. Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configurer une URL d’aide personnalisée</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Activer la liste de travail Priorités </td> 
      <td>Lets you choose to enable or disable the Priorities worklist experience for your users. Users will still see the Priorities icons in Workfront, but they will not have access to the functionality. For more information about Priorities, see <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Get started with Priorities</a>.</td> 
     </tr>
      <tr> 
      <td role="rowheader">Enable Adobe Enterprise Storage </td> 
      <td>Lets you choose to enable or disable Adobe Enterprise Storage for your entire organization or for specific groups. For more information about Adobe Enterprise Storage, see <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md">Enable Adobe enterprise storage for your organization</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Activer l’IA </td> 
      <td>Lets you choose to enable AI, including AI Assistant. <p><b>Note</b>: Your organization must meet specific requirements to enable AI. For more information about AI, including the requirements, see <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">AI Assistant overview</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Form Auto-complete </td> 
      <td>Lets you choose to enable the ability to auto-complete request forms based on previous request data. For more information about Form Auto-Complete, see <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">Auto-fill a request from previous data</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Participer aux programmes bêta de l’IA </td> 
      <td>&gt;Lets you choose to enable AI features that are currently in Beta. If you enable this option, you can then select which AI Beta features to enable. For more information about each AI Beta feature, click the information icon next to that feature.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Environnements de test</td> 
      <td>Vous permet d’accéder à vos environnements de test Workfront. Pour plus d’informations, consultez <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">L’environnement de sandbox de prévisualisation Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

   Les modifications que vous avez enregistrées ici affectent l’expérience de l’ensemble des utilisateurs et utilisatrices de Workfront et de toute personne qui interagit avec le système en tant qu’utilisateur ou utilisatrice externe.
