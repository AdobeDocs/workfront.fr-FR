---
content-type: release-notes
navigation-topic: 2019-4-release-activity
title: Autres améliorations de la version 2019.4
description: Cette page décrit les différentes améliorations apportées à la version 2019.4. Il sera disponible dans l’environnement de production la semaine du 11 novembre 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed7488f1-2076-4160-97f3-a3da25cccd0f
source-git-commit: e1bf5fbc7dc25bf8ce472b21b9a0906530f82cf0
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Autres améliorations de la version 2019.4

Cette page décrit les différentes améliorations apportées à la version 2019.4. Il sera disponible dans l’environnement de production la semaine du 11 novembre 2019.

Pour obtenir la liste de toutes les modifications apportées à la version 2019.4, voir [Présentation de la version 2019.4](../../../../product-announcements/product-releases/quarterly-release-archive/2019.4-release-activity/2019-4-release-activity-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td> <strong>Démarrage d’un workflow de vérification automatique à partir d’un document CC d’Adobe</strong> <p>Sans quitter Adobe CC, vous pouvez lancer un processus de vérification automatique pour un document Adobe CC que vous avez créé. Pour plus d’informations, voir la section <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md#generate" class="MCXref xref" xrefformat="{para}">Générer un BAT à partir d’Illustrator ou d’InDesign</a> dans l’article <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md" class="MCXref xref" xrefformat="{para}">Utilisation de l’extension Workfront pour Illustrator et InDesign</a>.</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td><strong>Workfront G Suite add-on</strong> <p>Now you can manage Workfront objects directly from Gmail, Google Calendar, and Google Drive.</p> <p>When you open a Workfront notification email, instantly view all information about the associated object and take actions, such as reviewing content or updating a status, without leaving your Inbox.</p> <p>When you open a non-Workfront email:</p> 
     <ul> 
      <li>Convert it into a task or issue.</li> 
      <li>Associate it with a project.</li> 
      <li>Assign it as a work item.</li> 
      <li>Add it to a work item as an update.</li> 
      <li>Upload its attachments to Workfront.</li> 
     </ul> <p>Manage Workfront objects without leaving G Suite:</p> 
     <ul> 
      <li>Post updates and replies to comments.</li> 
      <li>View and manage documents associated with a task or issue.</li> 
     </ul> <p>Access and work with object details:</p> 
     <ul> 
      <li>Read the description</li> 
      <li>View the parent object</li> 
      <li>Change the status</li> 
      <li>Access custom data</li> 
      <li>Mark it as complete.</li> 
     </ul> <p>And access your Workfront Home content, including tasks, issues, approvals, and access requests, without leaving G Suite.</p> <p>For more information, see <a href="../../../../workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront for G Suite</a>.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td> <strong>Empêcher les doublons d’adresses email</strong> <p>Vous ne pouvez plus utiliser la même adresse électronique lors de la création de plusieurs utilisateurs dans Workfront, même si ces adresses électroniques varient selon la casse. Par exemple, vous ne pouvez pas créer un utilisateur avec l’adresse électronique JohnDoe@example.com et un autre avec l’adresse électronique johndoe@example.com. </p> <p>Avant cette modification, la création d’utilisateurs avec des adresses électroniques correspondantes qui différaient uniquement par cas était prise en charge. </p> <p>Remarque : Les utilisateurs existants avec des adresses électroniques correspondantes qui ne diffèrent que par casse devront être mis à jour à une date ultérieure. Si des utilisateurs d’une instance Workfront ont des adresses électroniques correspondantes qui ne diffèrent que par la casse, Workfront vous contactera avec des informations supplémentaires et une chronologie du moment où celles-ci doivent être mises à jour.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Types d’objet supplémentaires disponibles pour les champs de saisie anticipée dans un formulaire personnalisé</strong> 
     <p>Désormais, lorsque vous créez un champ personnalisé Type, vous pouvez associer les types d’objet suivants au champ : Utilisateur, Société, Groupe, Rôle de tâche, Portfolio, Programme, Projet et Modèle.</p> 
     <p>Auparavant, vous pouviez uniquement associer le type d’objet Utilisateur à un champ personnalisé Type.</p> 
     <p>Pour plus d’informations, voir la section <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create" class="MCXref xref" xrefformat="{para}">Création ou modification d’un formulaire personnalisé</a> dans l’article <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Création ou modification d’un formulaire personnalisé</a>.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> <strong>Nom de fichier de la dernière version d’un document affiché</strong> <p>Désormais, lorsque vous téléchargez une version de document avec un nom de fichier différent de celui de la version existante, le nouveau nom de fichier s’affiche dans Workfront.</p> <p>Auparavant, lorsque vous ajoutiez une nouvelle version avec un nom de fichier différent, le nom de fichier de la version précédente continuait à s’afficher dans Workfront.</p> <p>Pour plus d’informations, voir <a href="../../../../documents/managing-documents/upload-new-document-version.md" class="MCXref xref" xrefformat="{para}">Télécharger une nouvelle version d’un document</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <strong>Ajout d’un filtre à un champ Type dans un formulaire personnalisé</strong> <p>Désormais, lorsque vous ajoutez un champ Type à un formulaire personnalisé, vous pouvez ajouter un filtre pour limiter les objets disponibles lorsque quelqu’un utilise le champ. Par exemple, vous pouvez limiter le champ de sorte que l’utilisateur ne puisse sélectionner que les membres des équipes marketing et ventes de votre organisation.</p> <p>Pour plus d’informations, voir la section Créer et ajouter un nouveau champ dans l’article Création d’un Forms personnalisé .</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Modifier le type d’affichage d’un champ dans un formulaire personnalisé</strong> 
     <p>Vous pouvez désormais modifier le type d’affichage d’un champ dans un formulaire personnalisé.</p> 
     <p>Par exemple, si vous avez créé un champ Cases à cocher, vous pouvez le changer en Champ déroulant ou Champ Boutons radio. Ces trois types d’affichage de champ sont interchangeables.</p> 
     <p>Si vous avez créé un champ de texte d’une seule ligne, vous pouvez également le remplacer par un champ de texte de paragraphe. Ces deux types d’affichage de champ sont interchangeables.</p> 
     <p>Auparavant, pour modifier le type d’affichage d’un champ personnalisé, vous deviez créer un nouveau champ et supprimer l’ancien champ. Il fallait pour cela transférer des données, ce qui prenait souvent du temps.</p> 
     <p>Pour plus d’informations, voir <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create" class="MCXref xref" xrefformat="{para}">Création ou modification d’un formulaire personnalisé</a> dans l’article <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Création ou modification d’un formulaire personnalisé</a></p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Créer des calendriers et des rapports de temps d’expiration</strong> 
     <p>Vous pouvez désormais voir le temps de pause de l’utilisateur pour une meilleure planification et une meilleure exécution. Vous pouvez également ajouter de nouveaux rapports et calendriers de désactivation à vos tableaux de bord pour une vue en temps réel de la disponibilité des utilisateurs.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
