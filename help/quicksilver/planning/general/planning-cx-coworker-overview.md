---
title: Présentation d’Adobe Workfront Planning CX Coworker
description: Vous pouvez utiliser CX Coworker dans Workfront Planning pour effectuer des actions similaires aux enregistrements et autres objets de Planning que vous effectueriez normalement dans l'interface. Les commandes de l’utilisateur et l’exécution par l’IA de ces commandes fonctionnent ensemble pour s’assurer que les modifications apportées par l’IA sont reflétées avec précision dans votre environnement.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '1119'
ht-degree: 7%
---

# Présentation d’Adobe Workfront Planning CX Coworker

<!--replaced information from the AI Assistant for Planning article with CX Coworker-->

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Le CX Coworker est une interface conversationnelle qui vous permet de décrire un objectif en langage clair, puis de planifier, d’exécuter et de valider le travail sur l’ensemble de votre planification Workfront et d’autres systèmes Adobe connectés avant de le ramener pour approbation.

Le CX Coworker préserve tout ce que fait AI Assistant aujourd’hui tout en ajoutant des fonctionnalités de bout en bout plus puissantes dans une nouvelle expérience plein écran et dans le rail de droite de Workfront.

Il fonctionne dans le cadre des contrôles d’accès au niveau des produits de votre entreprise. Les utilisateurs ne peuvent donc effectuer que les actions qu’ils sont déjà autorisés à effectuer dans Workfront, avec un accès en lecture seule par défaut et un accès en écriture contrôlé par les administrateurs Workfront.

>[!IMPORTANT]
>
>CX Coworker n’est actuellement pas disponible pour les organisations des secteurs de la santé, de la finance ou de certains autres secteurs qui disposent de données sensibles. AI Assistant est disponible pour ces organisations.
>
>Pour plus d’informations, voir [&#x200B; Présentation de l’assistant AI &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Packages Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront ou workflow avec un package Planning</p>
Ou
<p>Tout package Planning lorsqu’il est acheté en tant que produit autonome</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td>  
   <p>Votre administrateur doit effectuer les opérations suivantes pour autoriser l’accès au CX Coworker dans Planning :</p>
   <ul>
   <li><p>Ajoutez des types de licence Workflow et Planning à votre niveau d'accès lorsque vous disposez à la fois d'un package Workflow et Planning</p></li>
   <li><p>Désélectionnez Désactiver le panneau CX Coworker dans le paramètre Workfront de votre niveau d’accès. Elle est sélectionnée par défaut.</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Paramètres système</p></td> 
   <td>   <p>Votre administrateur Workfront doit sélectionner les outils MCP Lecture seule et Écriture seule dans les Préférences système de la Configuration. Les outils MCP en lecture seule sont sélectionnés par défaut.</p> 
    </td> 
  </tr> 
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives au CX Coworker

* Le CX Coworker doit être activé pour votre organisation avant d’être disponible pour les utilisateurs de votre société.

  Pour plus d’informations, consultez la présentation de [&#128279;](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

* Une fois que Workfront a activé l’agent pour votre instance Workfront, il est disponible pour l’administrateur Workfront principal qui peut l’activer pour votre organisation. Pour plus d’informations, voir [&#x200B; Configuration des préférences système &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* L’administrateur Workfront doit également activer le CX Coworker pour vous, dans votre niveau d’accès. Pour plus d’informations, voir [Créer et modifier des niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Le CX Coworker fonctionne avec des informations et des objets qui se trouvent dans Workfront ou Workfront Planning et auxquels vous avez l’autorisation d’accéder. Dans le rail de droite Planification, le panneau Collègue fonctionne dans le contexte de l’espace de travail, du type d’enregistrement ou de la page d’enregistrement que vous avez ouvert.

* Les actions effectuées par CX Coworker dans la zone Planning s’inscrivent dans le cadre de vos autorisations Workfront Planning et de votre niveau d’accès Workfront. Pour plus d’informations, voir les articles suivants :

  * [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Vue d’ensemble du type de licence lors de l’utilisation de la planification Adobe Workfront](/help/quicksilver/planning/access/license-type-overview.md)

* Les modifications apportées par CX Coworker pour le compte de l’utilisateur sont suivies dans le panneau Historique de l’enregistrement.

* Les actions effectuées par le CX Coworker sont permanentes et peuvent être irréversibles. Par exemple, la suppression d’un champ est irréversible. Passez en revue toutes les actions proposées par le CX Coworker avant de les accepter.

* Lors de la création, de la mise à jour ou de la suppression d’un objet par le biais du CX Coworker, le CX Coworker affiche les actions prévues et demande une confirmation. Vous pouvez ensuite confirmer ou annuler les actions.

## Fonctionnalité actuellement disponible pour le CX Coworker

Actuellement, le CX Coworker est disponible dans la zone Planning de Workfront et utilise un ensemble de compétences pour accéder aux informations des objets Planning et les manipuler. Pour plus d’informations, voir [Compétences &#x200B;](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md).

Vous pouvez utiliser le CX Coworker pour effectuer les actions suivantes :

* Rechercher des enregistrements. Vous pouvez effectuer une recherche en fonction des informations contenues dans n’importe quel champ d’enregistrement.
* Créer des enregistrements. Un identifiant avec un lien vers le nouvel enregistrement s’affiche une fois l’enregistrement créé. Vous pouvez spécifier les champs que vous souhaitez mettre à jour pendant le processus de création, tels que les dates ou la description.
* Créez des enregistrements basés sur un document que vous téléchargez. Workfront prend en charge les formats de document suivants pour CX Coworker :

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT et la plupart des formats d’image
* Mettre à jour les champs des enregistrements affichés à l’écran
* Supprimer, dupliquer ou restaurer des enregistrements
* Lier des enregistrements à d&#39;autres enregistrements
* Afficher l&#39;historique des modifications d&#39;un enregistrement


## Localisation du CX Coworker dans Workfront Planning

Le CX Coworker se trouve dans les zones suivantes de Workfront Planning :

* La barre de navigation principale, dans le coin supérieur droit de l’écran.
* Dans la zone des détails d’un enregistrement lorsque vous l’ouvrez dans un nouvel onglet.

## Accès au CX Coworker dans la zone Planning


1. Connectez-vous à Workfront, puis cliquez sur l’icône **Menu principal** ![Menu principal Lignes](assets/lines-main-menu.png) dans le coin supérieur gauche, puis cliquez sur **Planning**.

   La zone Planification s’ouvre.

   Recherchez l’icône **AI** ![AI](assets/ai-icon.png) dans le coin supérieur droit de la page ou passez aux étapes ci-dessous.

1. Cliquez sur une carte **espace de travail**.

1. Cliquez sur une carte **type d’enregistrement**.

1. Cliquez sur un **enregistrement** pour ouvrir la page **Détails** de l’enregistrement, puis cliquez sur l’ouverture dans .

1. Cliquez sur l’icône **&#x200B;**&#x200B;dans le coin supérieur droit de l’écran.

1. Dans l’espace prévu à cet effet, commencez à saisir des commandes pour le CX Coworker, puis cliquez sur Entrée lorsque vous avez terminé.

   Panneau ![CX Coworker avec une zone de commande vide](assets/cx-coworker-right-rail.png)

   Par exemple, vous pouvez saisir l’une des valeurs suivantes :

   * Créez un nouvel enregistrement de campagne appelé Vente d’été 2026.
   * Mettez à jour le champ Budget dans l’enregistrement Campagne d’été sur 75 000 $
   * Supprimez l’enregistrement de la campagne nommé Ancienne promotion
   * Restaurer la campagne que j’ai supprimée accidentellement

   >[!TIP]
   >
   >Assurez-vous que votre administrateur Workfront a activé les outils MCP en écriture seule dans vos préférences système avant de demander au CX Coworker d’effectuer des actions de modification sur les objets.

   Un indicateur visuel s’affiche pendant le traitement des commandes par CX Coworker, définissant les attentes en matière de temps de réponse.

   Après avoir reçu une réponse réussie, suivez les liens fournis ou notez les modifications sur la gauche.


1. (Facultatif) Cliquez sur l’icône **Développer le plein écran** ![Icône Développer le plein écran](assets/expand-full-screen-icon.png) pour ouvrir la boîte de dialogue Collègue dans un onglet de navigateur complet.


