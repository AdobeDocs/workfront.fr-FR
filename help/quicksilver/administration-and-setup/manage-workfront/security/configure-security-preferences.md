---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configuration des préférences de sécurité système
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer les préférences de sécurité de votre système Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: efe1fee1504e39b22b2a40f5e319f53c698acea5
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 5%

---

# Configuration des préférences système

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

En tant qu’administrateur Adobe Workfront, vous pouvez configurer les préférences de votre système Workfront :

* Accès à Workfront à partir d’applications mobiles et d’autres applications intégrées
* Règles d’incorporation de Workfront dans un iFrame

Les modifications que vous apportez dans les préférences du système ont un impact sur tous les utilisateurs de votre système et sur leur expérience dans Workfront.

Nous vous recommandons de configurer vos préférences système lors de l’implémentation de Workfront et de ne les revoir qu’occasionnellement.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
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
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuration des préférences du système

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Système** > **Préférences**.

1. Sélectionnez l’un des champs suivants pour définir les paramètres de votre entreprise :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Activation du processus de révision rapide</p> </td> 
      <td>Permet d’activer les versions Workfront mensuelles pour votre organisation plutôt que les versions trimestrielles.</p><p>Pour plus d’informations sur le processus de publication rapide, voir <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Activation ou désactivation de versions rapides pour votre entreprise</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Autoriser l’incorporation de <strong>Workfront</strong> dans un iframe</p> </td> 
      <td>Vous permet d’incorporer Workfront dans un iFrame.<p>Cette option est désactivée par défaut.</p><p><b>IMPORTANT</b>: l’affichage d’une application web dans un iframe rend l’application vulnérable à une vulnérabilité de sécurité de détournement de clic.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser l'authentification SAML 2.0 dans les modules complémentaires Office 365</td> 
      <td> <p>Vous permet d’incorporer Workfront dans un iFrame uniquement pour les modules complémentaires Office 365 lorsque Workfront est intégré à une solution de connexion unique SAML 2.0. </p> <p>Cette option est activée par défaut.</p> <p><b>REMARQUE</b>: si vous activez l’option ci-dessus, <strong>Autorisation de l’incorporation de Workfront dans un iFrame</strong>, l’option <strong>Autorisation de l’authentification SAML 2.0 dans les modules complémentaires Office 365</strong> est activé et grisé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Active l'utilisation des informations de session lors de la création d'URL de page externe</td> 
      <td> <p>Permet aux utilisateurs d’utiliser les informations d’ID de session d’un site lors de l’ajout d’une page externe à un tableau de bord.</p> <p>Pour plus d’informations sur l’ajout de pages externes à un tableau de bord, voir <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incorporation d’une page web externe dans un tableau de bord</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permet aux utilisateurs d’utiliser Workfront pour les applications mobiles et la variable <strong>Workfront</strong> Module complémentaire Outlook</td> 
      <td> <p>Permet aux utilisateurs d’accéder aux applications mobiles (vue Workfront pour les applications iPad et de téléphone mobile) et à l’application Workfront Outlook.</p> <p>Cette option est activée par défaut. </p> <p>Pour plus d’informations sur la vue Workfront, voir <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Utilisation de la vue Adobe Workfront</a>. Pour plus d’informations sur les applications mobiles, voir <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Utilisation de l’application mobile Adobe Workfront</a>.</p> <p>Pour plus d’informations sur le module externe Outlook, voir <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Configuration d’Adobe Workfront pour Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collaboration avec les personnes sans compte Workfront à l’aide d’adresses électroniques</p> </td> 
      <td>Permet aux utilisateurs de Workfront de partager certains éléments avec des personnes sans compte Workfront en incluant leur adresse électronique au lieu de leur nom. Les utilisateurs peuvent partager les éléments suivants avec des utilisateurs externes à l’aide de leur adresse électronique :
       <ul>
        <li>Document<br></li>
        <li>Demande de document<br></li>
        <li>Validation du document</li>
        <li>Calendrier</li>
       </ul><p>Cette option est activée par défaut.</p> <p><b>Important</b>: le niveau d’accès Utilisateur externe n’est pas disponible dans votre instance Workfront si cette option est désactivée. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Niveaux d’accès intégrés dans Workfront</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Demander aux utilisateurs externes de s'inscrire avec un mot de passe</td> 
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
      <td role="rowheader">Les utilisateurs du système verront par défaut l’expérience Nouvelle page d’accueil. </td> 
      <td>Permet d’indiquer si les utilisateurs verront l’expérience Nouvelle page d’accueil par défaut. Lorsqu’ils sont activés, les utilisateurs voient l’expérience Nouvelle page d’accueil par défaut, mais peuvent toujours choisir d’activer ou de désactiver cette dernière individuellement. <b>Lorsque cette option est désactivée, les utilisateurs n’ont pas la possibilité d’utiliser la nouvelle page d’accueil.</b> Ce paramètre est activé par défaut.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

   Les modifications que vous avez enregistrées ici affectent l’expérience de tous les utilisateurs de Workfront et de toute personne qui interagit avec eux en tant qu’utilisateur externe.
