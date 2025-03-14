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
source-git-commit: d4ebdcc942f119dc229e2a3216dbe82b3d701cba
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 92%

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
      <td> <p>Permet aux utilisateurs et utilisatrices d’accéder aux applications mobiles (Workfront View pour les applications iPad et téléphones portables) et à l’application Workfront Outlook.</p> <p>Cette option est activée par défaut. </p> <p>Pour plus d’informations sur Workfront View, consultez la section <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utiliser Adobe Workfront View</a>. Pour plus d’informations sur les applications mobiles, consultez la section <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Utiliser l’application mobile Adobe Workfront : index des articles</a>.</p> <p>Pour plus d’informations sur le plug-in Outlook, consultez la section <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Configurer Adobe Workfront pour Outlook</a>.</p> </td> 
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
     <tr> 
      <td role="rowheader">Demander aux utilisateurs et aux utilisatrices externes de s’inscrire avec un mot de passe</td> 
      <td> <p>Exige que les utilisateurs et utilisatrices externes s’inscrivent avant de pouvoir afficher des éléments dans Workfront. Cette option est désactivée par défaut. Lorsque vous activez cette option, les personnes sans compte Workfront qui sont incluses dans certaines mises à jour via leurs adresses e-mail sont invitées à créer un compte avant de pouvoir afficher l’élément dans lequel elles sont incluses. Cela leur crée un compte d’utilisateur ou d’utilisatrice externe.</p> <p>Cette option est désactivée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Déconnecte automatiquement les utilisateurs après</td> 
      <td> Vous permet de spécifier le moment où une personne est déconnectée de Workfront après une période d’inactivité. Par défaut, les utilisateurs et utilisatrices sont déconnectés après 8 heures d’inactivité. <p>Cette option affecte également les clientes et clients Workfront qui utilisent une solution d’authentification unique.</p> <p>Ce paramètre n’est pas disponible pour les organisations qui ont été migrées vers Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Déconnecter automatiquement les utilisateurs mobiles après </td> 
      <td>Vous permet de spécifier le moment où une personne est déconnectée de l’application Workfront après une période d’inactivité. Par défaut, les utilisateurs et utilisatrices sont déconnectés après 7 jours d’inactivité. <p>Cette option affecte également les clientes et clients Workfront qui utilisent une solution d’authentification unique.</p> <p>Ce paramètre n’est pas disponible pour les organisations qui ont été migrées vers Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL Aide</td> 
      <td>Vous permet de définir un site d’aide personnalisé interne vers lequel l’icône d’aide du menu principal redirigera. Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configurer une URL d’aide personnalisée</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Les utilisateurs et utilisatrices du système voient par défaut la nouvelle expérience d’accueil. </td> 
      <td>Vous permet de spécifier si les utilisateurs et les utilisatrices voient la nouvelle expérience d’accueil par défaut. Lorsque cette option est activée, les utilisateurs et les utilisatrices voient la nouvelle expérience d’accueil par défaut, mais peuvent toujours individuellement choisir d’activer ou de désactiver cette dernière. Lorsque cette option est désactivée, les utilisateurs et les utilisatrices ne voient pas la bannière qui leur permet de basculer vers la nouvelle page d’accueil. Toutefois, ils peuvent toujours accéder à la nouvelle page d’accueil en saisissant manuellement <code>/home/workspaces</code> à la fin de l’URL de leur instance. Ce paramètre est activé par défaut.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Activer la liste de travail Priorités </td> 
      <td>Permet de choisir d’activer ou de désactiver l’expérience de la liste de travail Priorités pour vos utilisateurs. Les utilisateurs verront toujours les icônes Priorités dans Workfront, mais ils n’auront pas accès à la fonctionnalité. Pour plus d'informations sur les priorités, voir <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Prise en main des priorités</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Environnements de test</td> 
      <td>Vous permet d’accéder à vos environnements de test Workfront. Pour plus d’informations, consultez <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">L’environnement de sandbox de prévisualisation Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

   Les modifications que vous avez enregistrées ici affectent l’expérience de l’ensemble des utilisateurs et utilisatrices de Workfront et de toute personne qui interagit avec le système en tant qu’utilisateur ou utilisatrice externe.
