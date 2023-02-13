---
product-area: projects
navigation-topic: manage-issues
title: Copier les problèmes
description: Vous pouvez copier un problème ou une requête et les enregistrer sur le même projet ou sur un autre. Vous pouvez également copier un problème d’une tâche vers un autre projet.
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 1%

---

# Copier les problèmes

Vous pouvez copier un problème ou une requête et les enregistrer sur le même projet ou sur un autre. Vous pouvez également copier un problème d’une tâche vers un autre projet.

Vous pouvez copier des problèmes à partir des objets suivants :

* D’un projet au même projet (dupliquez-le sur le même projet)
* D’une tâche à la même tâche (dupliquer si sur la même tâche)
* D’un projet à un autre
* d’une tâche à un projet ;

>[!TIP]
>
>&quot;Problèmes&quot; et &quot;requêtes&quot; sont interchangeables dans Workfront. Vous pouvez enregistrer les problèmes sur les projets et les tâches pour indiquer les travaux imprévus qui doivent être résolus. Vous pouvez également envoyer des requêtes qui sont enregistrées en tant que problèmes sur un projet désigné comme file d’attente de requêtes.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> <p>Passez en revue la licence ou une licence supérieure pour copier un problème dans la section Problèmes d’un projet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Affichage ou accès supérieur à Projets et tâches</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux problèmes de votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations liées au problème</p> <p>Attribuez des autorisations à l’élément sur lequel vous copiez le problème avec la possibilité d’ajouter des problèmes.</p> <p> Pour plus d’informations sur l’octroi d’autorisations aux problèmes, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partage d’un problème </a></p> <p>Pour plus d’informations sur la demande d’autorisations supplémentaires, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Considérations pour les problèmes liés aux documents ou aux files d’attente de demandes

Tenez compte des points suivants lors de la copie de problèmes qui contiennent des documents ou qui sont associés à une file d’attente de demandes :

* **Lorsqu’un problème est associé à une file d’attente de demandes :** Lorsque vous copiez un problème dans un autre objet et que le problème est associé à une file d’attente de requêtes, le problème copié n’est plus associé à la file d’attente d’origine du premier problème.
* **Lorsqu’un document est joint au problème :** Lorsque vous copiez un problème dans un autre objet et qu’un document y est associé, le document et ses versions passent également au nouveau problème. Les bons à tirer ou les validations associées au document ne sont pas déplacés.
* **Lorsqu’un problème est lié à un document ou à un dossier :** Lorsque vous copiez un problème dont les documents ou dossiers sont liés à un service tiers comme Google Drive, les liens vers les documents sont transférés vers le problème copié. 

## Copie des problèmes dans une liste

Vous pouvez copier un ou plusieurs problèmes à partir d’une liste de problèmes ou d’un rapport de problèmes.

1. Accédez au projet contenant le ou les problèmes que vous souhaitez copier.

   Ou

   Accédez à un rapport de problèmes.

1. Si vous avez choisi d’accéder à un projet, cliquez sur **Problèmes** dans le panneau de gauche.
1. Sélectionnez le ou les problèmes que vous souhaitez copier, puis cliquez sur le bouton **Plus de menu** en haut de la liste des problèmes, puis cliquez sur **Copier vers**.

   ![](assets/copy-issue-in-list-nwe-350x169.png)

1. Passez à la copie du problème, comme décrit dans la section . [Copier un seul problème](#copy-a-single-issue) commençant par l’étape 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:&nbsp;ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## Copier un seul problème {#copy-a-single-issue}

Vous pouvez copier un problème lors de son affichage.

1. Accédez à un problème que vous souhaitez copier, puis cliquez sur le bouton **Plus** menu ![](assets/more-icon.png) à droite du nom du problème, puis **Copier** à .

   ![](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   Le **Copier le problème** s’affiche.

   ![](assets/copy-issue-box-nwe-350x285.png)

1. Dans le **Sélectionner le projet de destination** , indiquez le nom du projet dans lequel vous souhaitez copier les problèmes. Le nom du projet actif s’affiche par défaut.

   >[!TIP]
   >
   >Seuls 100 projets s’affichent dans la liste.

1. (Conditionnel) Cliquez sur **accès aux demandes** si vous n’avez pas accès aux problèmes de copie du projet.
1. (Conditionnel) Continuez à copier le problème vers le projet de destination sélectionné sans demander l’accès si vous avez accès à l’une des tâches du projet de destination pour ajouter des problèmes.

   ![](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Des messages similaires s’affichent si le projet sélectionné est en attente d’approbation, terminé ou mort, lorsque l’administrateur de Workfront empêche l’ajout de problèmes à ces projets. Pour plus d’informations, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facultatif) Dans le **Options** désélectionnez les éléments répertoriés dans le tableau ci-dessous pour les supprimer du nouveau problème. Toutes les options sont sélectionnées par défaut.

   >[!NOTE]
   Cela a un impact uniquement sur les problèmes copiés et non sur les problèmes d’origine.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Affectations</td> 
      <td>Supprime les utilisateurs, les rôles de tâche ou les équipes affectés au problème.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progression</td> 
      <td>Supprime le pourcentage de réussite, le cas échéant, du problème. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td><span style="line-height: 1.5;">supprime tous les éléments de l’onglet documents, y compris les versions de documents, les documents liés et les dossiers.</span> <br>Par défaut, les BAT et les validations de document ne peuvent pas être copiés vers un autre problème.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autorisations</td> 
      <td>Supprime les entités avec lesquelles le problème est partagé. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mises à jour</td> 
      <td>Supprime les commentaires de la section Mises à jour du problème.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Données personnalisées</td> 
      <td>Supprime les informations du formulaire personnalisé sur le problème, ainsi que les informations sur les formulaires personnalisés associés aux documents joints au problème, si ceux-ci sont également copiés avec le problème. Les formulaires personnalisés restent attachés aux problèmes et documents, mais les informations sur les formulaires ne seront pas transférées vers le nouveau numéro. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Dans le **Sélectionner une tâche** , sélectionnez la tâche dans laquelle vous souhaitez déplacer le problème.
1. Cliquez sur **Problème de copie** ou **Copie de problèmes** si vous avez sélectionné plusieurs problèmes dans une liste.

   Les problèmes copiés sont ajoutés au projet spécifié.

 
