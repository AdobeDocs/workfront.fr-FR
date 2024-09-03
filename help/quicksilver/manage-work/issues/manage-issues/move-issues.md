---
product-area: projects
navigation-topic: manage-issues
title: Déplacer les problèmes
description: Vous pouvez déplacer des problèmes entre des projets et des tâches.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 100%

---

# Déplacer les problèmes

Vous pouvez déplacer des problèmes entre les objets suivants :

* D’un projet à un autre.
* D’une tâche à une autre dans le même projet ou dans un autre projet.
* D’une tâche au projet ou à un autre projet.
* D’un projet à une tâche dans le même projet ou à une tâche dans un autre projet.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> <p>Licence de révision ou une licence supérieure pour déplacer les problèmes dans la section Problèmes d’un projet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Affichage ou accès supérieur aux Projets et aux Tâches</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux problèmes liés à votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a>. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations liées aux problèmes</p> <p>Autorisations Contribuer à l’élément vers lequel vous déplacez le problème avec la possibilité d’ajouter des problèmes.</p> <p> Pour plus d’informations sur l’octroi d’autorisations aux problèmes, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partager un problème</a></p> <p>Pour plus d’informations sur la demande d’autorisations supplémentaires, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Remarques relatives au déplacement de problèmes

Tenez compte des points suivants lors du déplacement de problèmes qui contiennent des documents ou qui sont associés à une file d’attente des demandes :

* **Lorsqu’un problème est associé à une file d’attente des demandes :** lorsque vous déplacez un problème vers un autre objet et qu’il est associé à une file d’attente des demandes, le problème déplacé n’est plus associé à la file d’attente d’origine de laquelle provenait le premier problème.
* **Lorsqu’un document est joint au problème :** lorsque vous déplacez un problème vers un autre objet et qu’un document lui est joint, le document, ses versions et ses épreuves sont également déplacés vers le nouveau problème. Les approbations associées au document ne sont pas déplacées.
* **Lorsqu’un problème est lié à un document ou à un dossier :** lorsque vous déplacez un problème dont les documents ou dossiers sont liés à un service tiers tel que Google Drive, les liens vers les documents sont déplacés avec le problème.

## Déplacer les problèmes dans une liste

Vous pouvez déplacer un ou plusieurs problèmes à partir d’une liste de problèmes ou d’un rapport de problèmes.

1. Accédez au projet contenant le ou les problèmes que vous souhaitez déplacer.

   Ou

   Accédez à un rapport de problèmes.

1. Si vous avez choisi d’accéder à un projet, cliquez sur **Problèmes** dans le panneau de gauche.
1. Sélectionnez le ou les problèmes que vous souhaitez déplacer, cliquez sur le **menu Plus** en haut de la liste des problèmes, puis sur **Déplacer vers**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Poursuivez le déplacement du problème, comme décrit dans la section [Déplacer un seul problème](#move-a-single-issue) en commençant à l’étape 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## Déplacer un seul problème {#move-a-single-issue}

Vous pouvez déplacer un problème lorsqu’il est affiché.

### Déplacer un seul problème dans l’environnement de prévisualisation

1. Accédez à un problème que vous souhaitez copier, cliquez sur le menu **Plus** ![](assets/more-icon.png) à droite du nom du problème, puis sélectionnez **Déplacer vers**.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   La zone **Déplacer le problème** s’affiche.

   ![](assets/move-issue-box-nwe-350x280.png)

1. Dans la section **Sélectionner le projet de destination**, indiquez le nom du projet dans lequel vous souhaitez déplacer les problèmes. Le nom du projet actuel s’affiche par défaut.

   >[!TIP]
   >
   >Seuls 100 projets s’affichent dans la liste.

1. (Le cas échéant) Cliquez sur **Demander l’accès** si vous n’avez pas accès au déplacement des problèmes vers le projet.
1. (Le cas échéant) Continuez à déplacer le problème sur le projet de destination sélectionné sans demander l’accès si vous disposez de l’accès à l’une de ses tâches.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Des messages similaires s’affichent si le projet sélectionné est en attente d’approbation, terminé ou immobilisé, lorsque l’administration de Workfront empêche l’ajout de problèmes à ces projets. Pour plus d’informations, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facultatif) Dans la section **Options**, désélectionnez les éléments voulus répertoriés dans le tableau ci-dessous pour les supprimer du problème déplacé. Toutes les options sont sélectionnées par défaut.

   >[!IMPORTANT]
   >
   >La désélection d’éléments dans la liste des options entraîne une perte de données. Les informations du problème existant seront supprimées et ne pourront pas être récupérées.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sélectionner tout</td> 
      <td>Désélectionnez cette option pour supprimer toutes les informations du problème lorsque vous le déplacez vers son nouvel emplacement. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Affectations</td> 
      <td>Supprime les personnes, les fonctions ou les équipes affectées au problème.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progression</td> 
      <td>Supprime le pourcentage terminé, le cas échéant, du problème. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Documents</p></td> 
      <td> <p>Supprime tous les éléments de l’onglet Documents, y compris les versions de documents, les documents liés et les dossiers.

   <b>NOTE</b>

   Si vous choisissez de ne pas déplacer les documents avec le problème, ceux-ci seront supprimés et placés dans la corbeille pendant 30 jours. Un administrateur ou une administratrice peut les restaurer et ils réapparaîtront sur le problème déplacé.

   Si le problème est supprimé après son déplacement, les documents restaurés sont placés dans la zone Documents de la page de l’utilisateur ou de l’utilisatrice de l’administrateur ou l’administratrice qui les restaure.
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Autorisations</td> 
      <td>Supprime les entités avec lesquelles le problème est partagé. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mises à jour</td> 
      <td>Supprime les commentaires de la section Mises à jour du problème.</td> 
     </tr> 
    </tbody> 
   </table>


1. (Facultatif) Dans la section **Sélectionner une tâche**, sélectionnez la tâche dans laquelle vous souhaitez déplacer le problème.
1. Cliquez sur **Déplacer le problème** ou **Déplacer les problèmes**, si vous avez sélectionné plusieurs problèmes dans une liste.

   Les problèmes déplacés sont ajoutés au projet spécifié.




