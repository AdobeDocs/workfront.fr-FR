---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configuration des préférences système
description: En tant qu’administrateur d’Adobe Workfront, vous pouvez configurer les préférences de votre système Workfront, y compris les préférences de sécurité.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 11%

---

# Configurer les préférences système

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

{{important-admin-console-onboard}}

En tant qu’administrateur Adobe Workfront, vous pouvez configurer les préférences de votre système Workfront, notamment :

* Accès à Workfront à partir d’applications mobiles et d’autres applications intégrées
* Règles d’incorporation de Workfront dans un iFrame

Les modifications que vous apportez dans les préférences du système ont un impact sur tous les utilisateurs de votre système et sur leur expérience dans Workfront.

Nous vous recommandons de configurer vos préférences système lors de l’implémentation de Workfront et de ne les revoir qu’occasionnellement.

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
   <td><p>Nouvelle : standard</p>
   <p>ou</p>
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuration des préférences du système

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Préférences**.

1. Sélectionnez l’un des champs suivants pour définir les paramètres de votre entreprise :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Activer le processus de version rapide</p> </td> 
      <td>Permet d’activer les versions Workfront mensuelles pour votre organisation plutôt que les versions trimestrielles.</p><p>Pour plus d’informations sur le processus de publication rapide, voir <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Activation ou désactivation de versions rapides pour votre organisation</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Autorisation de l’incorporation de Workfront dans un iFrame</p> </td> 
      <td>Vous permet d’incorporer Workfront dans un iFrame.<p>Cette option est désactivée par défaut.</p><p><b>IMPORTANT</b> : l’affichage d’une application web dans un iFrame rend l’application sujette à une vulnérabilité de sécurité de détournement de clic.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser l'authentification SAML 2.0 dans les modules complémentaires Office 365</td> 
      <td> <p>Vous permet d’incorporer Workfront dans un iFrame uniquement pour les modules complémentaires Office 365 lorsque Workfront est intégré à une solution de connexion unique SAML 2.0. </p> <p>Cette option est activée par défaut.</p> <p><b>REMARQUE</b> : si vous activez l’option ci-dessus, <strong>Autoriser l’incorporation de Workfront dans un iframe</strong>, l’option <strong>Autoriser l’authentification SAML 2.0 dans les modules complémentaires Office 365</strong> est activée et grisée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activer l’utilisation des informations de session lors de la création d’URL de page externes</td> 
      <td> <p>Permet aux utilisateurs d’utiliser les informations d’ID de session d’un site lors de l’ajout d’une page externe à un tableau de bord.</p> <p>Cette option n’est pas sécurisée et désactivée par défaut. Il est recommandé d’utiliser OAuth à la place pour les intégrations.</p> <p>Pour plus d’informations sur l’ajout de pages externes à un tableau de bord, voir <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incorporation d’une page web externe dans un tableau de bord</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permet aux utilisateurs d’utiliser les applications mobiles Workfront et le module complémentaire Workfront Outlook</td> 
      <td> <p>Permet aux utilisateurs d’accéder aux applications mobiles (vue Workfront pour les applications iPad et de téléphone mobile) et à l’application Workfront Outlook.</p> <p>Cette option est activée par défaut. </p> <p>Pour plus d’informations sur la vue Workfront, voir <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utilisation de la vue Adobe Workfront</a>. Pour plus d'informations sur les applications mobiles, voir <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Utilisation de l'application mobile Adobe Workfront : article index</a>.</p> <p>Pour plus d’informations sur le module externe Outlook, voir <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Configuration d’Adobe Workfront pour Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collaboration avec les personnes sans compte Workfront à l’aide d’adresses électroniques</p> </td> 
      <td>Permet aux utilisateurs de Workfront de partager certains éléments avec des personnes sans compte Workfront en incluant leur adresse électronique au lieu de leur nom. Les utilisateurs peuvent partager les éléments suivants avec des utilisateurs externes à l’aide de leur adresse électronique :
       <ul>
        <li>Document<br></li>
        <li>Demande de document<br></li>
        <li>Validation du document</li>
        <li>Calendrier</li>
       </ul><p>Cette option est activée par défaut.</p> <p><b>Important</b> : Le niveau d’accès des utilisateurs externes n’est pas disponible dans votre instance Workfront si cette option est désactivée. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Niveaux d’accès intégrés</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger que les utilisateurs externes s’enregistrent avec un mot de passe</td> 
      <td> <p>Nécessite que les utilisateurs externes s’enregistrent avant de pouvoir afficher les éléments dans Workfront. Par défaut, cette option est désactivée. Lorsque vous activez cette option, les personnes sans compte Workfront qui sont incluses dans certaines mises à jour par leur adresse électronique sont invitées à créer un compte avant de pouvoir afficher l’élément sur lequel elles sont incluses. Cela crée un compte d’utilisateur externe pour ces utilisateurs.</p> <p>Cette option est désactivée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Déconnecte automatiquement les utilisateurs après</td> 
      <td> Permet d’indiquer quand un utilisateur est déconnecté de Workfront, après une période d’inactivité. Par défaut, les utilisateurs sont déconnectés après 8 heures d’inactivité. <p>Cette option affecte également les clients Workfront qui utilisent une solution de connexion unique.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Déconnecter automatiquement les utilisateurs mobiles après </td> 
      <td>Permet d’indiquer quand un utilisateur est déconnecté de l’application Workfront, après une période d’inactivité. Par défaut, les utilisateurs sont déconnectés après 7 jours d’inactivité. <p>Cette option affecte également les clients Workfront qui utilisent une solution de connexion unique.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL Aide</td> 
      <td>Permet de définir un site d’aide personnalisé interne auquel accéder l’icône d’aide du menu principal. Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configuration d’une URL d’aide personnalisée</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Les utilisateurs du système verront par défaut l’expérience Nouvelle page d’accueil. </td> 
      <td>Permet d’indiquer si les utilisateurs verront l’expérience Nouvelle page d’accueil par défaut. Lorsqu’ils sont activés, les utilisateurs voient l’expérience Nouvelle page d’accueil par défaut, mais peuvent toujours choisir d’activer ou de désactiver cette dernière individuellement. Lorsque cette option est désactivée, les utilisateurs ne voient pas la bannière qui leur permet de passer à la nouvelle page d’accueil. Toutefois, ils peuvent toujours accéder à leur page d’accueil en saisissant manuellement <code>/home/workspaces</code> à la fin de l’URL de leur instance. Ce paramètre est activé par défaut.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Environnements de test</td> 
      <td>Vous permet d’accéder à vos environnements de test Workfront. Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">L’environnement Sandbox d’aperçu Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

   Les modifications que vous avez enregistrées ici affectent l’expérience de tous les utilisateurs de Workfront et de toute personne qui interagit avec le système en tant qu’utilisateur externe.
