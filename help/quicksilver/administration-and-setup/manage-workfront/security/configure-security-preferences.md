---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurer les préférences système
description: En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez configurer les préférences de votre système Workfront, y compris les préférences de sécurité.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: f5044d457ebf203269e8007075e98ba4c136660f
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 75%

---

# Configurer les préférences système

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{important-admin-console-onboard}}

En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez configurer les préférences de votre système Workfront, notamment :

* L’accès à Workfront à partir d’applications mobiles et d’autres applications intégrées
* Règles d’incorporation de Workfront dans un iframe

Les modifications apportées aux préférences système ont un impact sur toutes les personnes présentes dans le système et sur leur expérience dans Workfront.

Nous vous recommandons de configurer vos préférences système lors de l’implémentation de Workfront et de ne les revoir qu’occasionnellement.

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
   <td><p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
      <td role="rowheader">Autoriser les personnes à utiliser les applications mobiles Workfront et le module complémentaire Workfront Outlook</td> 
      <td> <p>Permet aux utilisateurs et utilisatrices d’accéder aux applications mobiles (Workfront View pour les applications iPad et téléphones portables) et à l’application Workfront Outlook.</p> <p>Cette option est activée par défaut. </p> <p>Pour plus d’informations sur Workfront View, consultez la section <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utiliser Adobe Workfront View</a>. Pour plus d’informations sur les applications mobiles, consultez la section <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Utiliser l’application mobile Adobe Workfront : index des articles</a>.</p> </td> 
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
     <!--<tr> 
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
     </tr> -->
     <tr> 
      <td role="rowheader">URL Aide</td> 
      <td>Vous permet de définir un site d’aide personnalisé interne vers lequel l’icône d’aide du menu principal redirigera. Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configurer une URL d’aide personnalisée</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Activer la liste de travail Priorités </td> 
      <td>Permet de choisir d’activer ou de désactiver l’expérience de la liste de travail Priorités pour vos utilisateurs. Les utilisateurs verront toujours les icônes Priorités dans Workfront, mais ils n’auront pas accès à la fonctionnalité. Pour plus d'informations sur les priorités, voir <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Prise en main des priorités</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Activer AI</span> </td> 
      <td><span class="preview">Permet de choisir d’activer l’IA, y compris l’assistant IA. <p><b>Remarque </b> : votre entreprise doit répondre à des exigences spécifiques pour activer l’IA. Pour plus d’informations sur l’IA, y compris ses exigences, consultez <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md"> Présentation de l’assistant IA</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Saisie automatique de formulaire </span></td> 
      <td><span class="preview">Permet de choisir d’activer la possibilité de remplir automatiquement les formulaires de demande en fonction des données de demande précédentes. Pour plus d’informations sur la saisie automatique des formulaires, voir <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">Saisie automatique d’une demande à partir de données précédentes</a>.</span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Participer aux programmes Beta de l’IA </span></td> 
      <td><span class="preview">Permet de choisir d’activer les fonctionnalités d’IA actuellement dans Beta. Si vous activez cette option, vous pouvez sélectionner les fonctionnalités d’IA Beta à activer. Pour plus d’informations sur chaque fonctionnalité AI Beta, cliquez sur l’icône d’information en regard de cette fonctionnalité.</span></td> 
     </tr>
     <tr> 
      <td role="rowheader">Environnements de test</td> 
      <td>Vous permet d’accéder à vos environnements de test Workfront. Pour plus d’informations, consultez <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">L’environnement de sandbox de prévisualisation Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

   Les modifications que vous avez enregistrées ici affectent l’expérience de l’ensemble des utilisateurs et utilisatrices de Workfront et de toute personne qui interagit avec le système en tant qu’utilisateur ou utilisatrice externe.
