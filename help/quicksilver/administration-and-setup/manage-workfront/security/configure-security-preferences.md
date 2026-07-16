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
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/46D3BBajFk39FP-dMDk0SuSSGM5nYPKas11Bs159R9Y
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: b0dd2c2c448c829b2ce1559ddc87880c9a47a68f
workflow-type: tm+mt
source-wordcount: 1218
ht-degree: 48%

---

# Configurer les préférences système

{{preview-fast-release-general}}

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
      <td role="rowheader">Autoriser les personnes à utiliser les applications mobiles Workfront</td> 
      <td> <p>Permet aux utilisateurs d’accéder aux applications mobiles (vue Workfront pour iPad et applications de téléphone mobile)</p> <p>Cette option est activée par défaut. </p> <p>Pour plus d’informations sur Workfront View, consultez la section <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utiliser Adobe Workfront View</a>. Pour plus d’informations sur les applications mobiles, consultez la section <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Utiliser l’application mobile Adobe Workfront : index des articles</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collaborer avec des personnes sans les comptes Workfront en utilisant leur adresse e-mail</p> </td> 
      <td>Permet aux utilisateurs et utilisatrices de Workfront de partager certains éléments avec des personnes sans compte Workfront en incluant leur adresse e-mail au lieu de leur nom. Les utilisateurs et utilisatrices peuvent partager les éléments suivants avec des utilisateurs et utilisatrices externes à l’aide de leur adresse e-mail :
       <ul>
        <li>Document<br></li>
        <li>Demande de document<br></li>
        <li>Approbation de document</li>
        <li>Calendrier</li>
       </ul><p>Cette option est activée par défaut.</p> <p><b>IMPORTANT </b> : le niveau d'accès Utilisateur externe n'est pas disponible dans votre instance Workfront si cette option est désactivée. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Niveaux d’accès intégrés</a>.</p> </td> 
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
      <td role="rowheader">Désactiver la mise à niveau automatique dans les niveaux d’accès</td> 
      <td>Vous pouvez désactiver le processus de mise à niveau automatique pour les niveaux d’accès Contributeur. Lorsque ce paramètre est coché, les utilisateurs disposant d’une licence de contributeur qui ont dépassé leur limite de décision d’approbation doivent être mis à niveau manuellement par l’administrateur vers une nouvelle licence.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Activer la liste de travail Priorités </td> 
      <td>Permet de choisir d’activer ou de désactiver l’expérience de la liste de travail Priorités pour vos utilisateurs. Les utilisateurs verront toujours les icônes Priorités dans Workfront, mais ils n’auront pas accès à la fonctionnalité. Pour plus d'informations sur les priorités, voir <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Prise en main des priorités</a>.</td> 
     </tr>
     <tr>
      <td>Toujours appliquer les champs obligatoires en mode de modification en masse</td>
      <td><p>Permet de choisir de forcer les utilisateurs à saisir des informations dans les champs requis lors de la modification en bloc d’objets.</p> <p>Lorsque cette option est sélectionnée, les champs obligatoires doivent avoir des valeurs avant d’être enregistrés en mode de modification en bloc. Si une valeur est manquante dans le champ obligatoire pour au moins un objet sélectionné en bloc, l’enregistrement n’est pas autorisé.</p> <p>Lorsque cette option n’est pas sélectionnée, les champs obligatoires ne sont appliqués que lorsqu’un utilisateur modifie le champ. Si un champ n’est pas modifié, il est traité comme facultatif et non validé.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Préférences de stockage </td> 
      <td>Dans cette section, vous pouvez activer les préférences cloud d’Adobe. Permet de choisir d’activer ou de désactiver l’espace de stockage dans le cloud Adobe pour l’ensemble de l’organisation ou pour des groupes spécifiques. 
      <p>Mettez à jour les informations suivantes :</p>
      <ul><li><b>Par défaut</b> : sélectionnez le stockage Workfront hérité ou l’espace de stockage cloud Adobe.</li>
      <li><b>Autoriser les utilisateurs à sélectionner un fournisseur de stockage</b> : permet aux utilisateurs de choisir entre les deux types de stockage lors de la création d’objets Workfront.</li>
      <li><b>S’applique à</b> : indiquez si les paramètres par défaut s’appliquent à l’ensemble de l’organisation ou à des groupes spécifiques</li>
      <li><b>Sélectionner les portfolios à convertir en stockage dans le cloud Adobe</b> : sélectionnez les portfolios que vous souhaitez convertir automatiquement du stockage hérité de Workfront vers le stockage dans le cloud Adobe. Les portefeuilles sont convertis lorsque vous enregistrez les préférences système.</li></ul>     
    Pour plus d’informations sur l’espace de stockage dans le cloud d’Adobe, voir <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md">Activer l’espace de stockage dans le cloud Adobe pour votre organisation</a>.</td></tr>
    <tr> 
      <td role="rowheader">Sélectionner les portefeuilles à convertir vers l’espace de stockage Adobe </td> 
      <td>Permet de convertir des portfolios de stockage Workfront hérités existants en stockage dans le cloud Adobe. Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md">Conversion de portefeuilles hérités en espace de stockage Adobe</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Activer l’IA </td> 
      <td>En activant les paramètres de la zone des préférences de l’IA, vous pouvez activer l’IA, y compris l’assistant IA. <p><b>REMARQUE </b> : votre entreprise doit répondre à des exigences spécifiques pour activer l’IA. Pour plus d’informations sur l’IA, y compris ses exigences, consultez <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md"> Présentation de l’assistant IA</a>.</p></td> 
     </tr>
    <tr> 
      <td role="rowheader">Remplissage de formulaire par IA </td> 
      <td>Autoriser les personnes à utiliser Remplir le formulaire avec l’IA pour remplir automatiquement un formulaire de demande. Pour plus d’informations, consultez <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md">Utilisation du remplissage de formulaire optimisé par l’IA pour remplir une demande à l’aide d’invites ou de documents</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Saisie automatique intelligente dans les formulaires de demande </td> 
      <td>Permet de choisir d’activer la possibilité de remplir automatiquement les formulaires de demande en fonction des données de demande précédentes. Pour plus d’informations sur la saisie automatique des formulaires, voir <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">Saisie automatique d’une demande à partir de données précédentes</a>.</td> 
     </tr>
    <tr> 
      <td role="rowheader">Concepteur de planification</td> 
      <td>Cette option est disponible uniquement pour les clients qui ont acheté un package Workfront Planning. L'activation de ce paramètre permet aux utilisateurs de créer et de modifier des espaces de travail à l'aide de Planning Designer. Pour plus d’informations, voir <a href="/help/quicksilver/planning/general/planning-ai-designer.md">Prise en main d’Adobe Workfront Planning Designer</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Participer aux programmes bêta de l’IA </td> 
      <td>Permet de choisir d’activer les fonctionnalités d’IA actuellement dans Beta. Si vous activez cette option, vous pouvez sélectionner les fonctionnalités d’IA Beta à activer. Pour plus d’informations sur chaque fonctionnalité AI Beta, cliquez sur l’icône d’information en regard de cette fonctionnalité.</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Outils MCP en lecture seule</span></td> 
      <td><span class="preview">Permet au serveur Workfront MCP d’effectuer des actions de lecture sur les données Workfront, par exemple, rechercher ou répertorier des projets, des tâches ou d’autres éléments. Cette option est activée par défaut.<p>Pour plus d’informations sur le serveur MCP Workfront, consultez <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Configuration du serveur MCP Adobe Workfront</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Créer des outils MCP</span></td> 
      <td><span class="preview">Permet au serveur Workfront MCP d’effectuer des actions de création, de mise à jour et de suppression sur les données Workfront. Cette option est désactivée par défaut.<p>Pour plus d’informations sur le serveur MCP Workfront, consultez <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Configuration du serveur MCP Adobe Workfront</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader">Environnements de test</td> 
      <td>Vous permet d’accéder à vos environnements de test Workfront. Pour plus d’informations, consultez <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">L’environnement de sandbox de prévisualisation Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

   Les modifications que vous avez enregistrées ici affectent l’expérience de l’ensemble des utilisateurs et utilisatrices de Workfront et de toute personne qui interagit avec le système en tant qu’utilisateur ou utilisatrice externe.
