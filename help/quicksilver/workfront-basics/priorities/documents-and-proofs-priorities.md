---
navigation-topic: get-started-with-workfront
title: Charger des documents et créer des épreuves dans les priorités
description: Documents
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: 63aa5e45-e51d-4049-a5d9-18dfaaa79647
source-git-commit: b886284eb44c2154987019655ff07cdeb0e1ae22
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 29%

---

# Charger des documents et créer des épreuves dans les priorités

Vous pouvez charger des documents et créer des épreuves dans Priorités.

Priorités affiche les éléments de travail qui vous sont affectés. Vous ne pouvez pas voir les éléments de travail affectés à votre équipe.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> 
   <p>Nouveau : Tous </p>
   <p>Actuel : Pro ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
      <p><strong>Charger les documents</strong></p>
   <p>Nouveau : contributeur</p>
   <p>Actuel : demande</p>
      <p><strong>Créer des épreuves</strong></p>
        <p>Nouveau : Standard</p>
     <p>Actuelle : Travail ou Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Charger un document vers un élément de travail

Vous pouvez charger un document vers un élément de travail à partir de la liste de travail ou de la page Détails de l’élément de travail.

### Panneau Résumé de la liste de travail


{{step1-to-priorities}}

1. Dans la liste des tâches, passez la souris sur le nom de la tâche, puis cliquez sur l’icône **Résumé** ![icône Ouvrir le résumé](assets/summary-icon.png).
1. Vérifiez que vous êtes sur l’onglet **Tâche** ou **Événements** dans le panneau de résumé.
1. Cliquez sur l’icône **Télécharger le fichier** ![Télécharger le fichier](assets/upload-file-icon.png).
1. Glissez-déposez votre fichier ou collez-le à partir du presse-papiers en utilisant les touches Cmd/Ctrl + V
ou
Cliquez sur **Ajouter des fichiers** pour parcourir les fichiers ou importer des fichiers d’un fournisseur Document Cloud.
   ![Ajouter des fichiers](assets/add-files.png)
1. (Facultatif) Ajoutez un commentaire.
1. (Facultatif) Ajoutez d’autres fichiers.

   >[!NOTE]
   >
   >Les fichiers supplémentaires sont chargés en tant que documents distincts.
1. Cliquez sur **Charger**.

### Détails de l’élément de travail

{{step1-to-priorities}}

1. Dans la liste des tâches, cliquez sur le nom de l’élément de travail.
1. Cliquez sur l’onglet **Documents** en haut de l’écran.
1. Cliquez sur **Charger le document** dans le coin supérieur droit, puis sélectionnez **Document**.
1. Glissez-déposez votre fichier ou collez-le à partir du presse-papiers en utilisant les touches Cmd/Ctrl + V
ou
Cliquez sur **Ajouter des fichiers** pour parcourir les fichiers ou importer des fichiers d’un fournisseur Document Cloud.
   ![Ajouter des fichiers](assets/add-files.png)
1. (Facultatif) Ajoutez un commentaire.
1. (Facultatif) Ajoutez d’autres fichiers.

   >[!NOTE]
   >
   >Les fichiers supplémentaires sont chargés en tant que documents distincts.
1. Cliquez sur **Charger**.


## Création d’une épreuve simple ou avancée

Vous pouvez créer un BAT à partir d’un document de la liste de travail ou de la page Détails de l’élément de travail.

### Panneau Résumé de la liste de travail


{{step1-to-priorities}}

1. Dans la liste des tâches, passez la souris sur le nom de la tâche, puis cliquez sur l’icône **Résumé** ![icône Ouvrir le résumé](assets/summary-icon.png).
1. Vérifiez que vous êtes sur l’onglet **Tâche** ou **Événements** dans le panneau de résumé.
1. Cliquez sur l’icône **Documents** ![icône Documents](assets/show-document-icon.png) dans le rail latéral droit.
1. Cliquez sur l’icône **Télécharger le fichier** ![Télécharger le fichier](assets/upload-file-icon.png), puis sélectionnez le fichier.

   >[!NOTE]
   >
   >Vous devez charger le document avant de pouvoir créer l’épreuve.


1. Une fois le fichier chargé, sélectionnez-le dans la section **Documents**.
1. Cliquez sur **Créer une épreuve** dans le coin supérieur droit de la zone des détails du fichier.
1. Choisissez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><b>Épreuve simple</b></td> 
      <td>Cette option crée une épreuve sans workflow associé et applique les paramètres d’épreuve par défaut. Vous pouvez mettre à jour les paramètres par défaut de l’épreuve ou ajouter un workflow après avoir créé l’épreuve. Pour plus d’informations sur les paramètres d’épreuve, consultez <a href="/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Modification des paramètres d’épreuve</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Épreuve avancée</b></td> 
      <td> <p>Cette option vous permet de configurer un workflow de base ou avancé et de modifier les paramètres de l’épreuve que vous créez. Pour plus d’informations, consultez les ressources suivantes : </p> 
       <ul> 
        <li><p><a href="/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Créer une épreuve avancée avec un workflow de base</a> </p> </li> 
        <li> <p><a href="/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Créer une épreuve avancée avec un workflow automatisé</a></p></li> 
       </ul>
        </td> 
     </tr> 
    </tbody> 
   </table>

### Détails de l’élément de travail

{{step1-to-priorities}}

1. Dans la liste des tâches, cliquez sur le nom de l’élément de travail.
1. Cliquez sur l’onglet **Documents** en haut de l’écran.
1. Cliquez sur **Charger le document** dans le coin supérieur droit, puis sélectionnez **Épreuve**.
1. Créez un BAT, comme décrit dans la section
   [Créer une épreuve avancée avec un workflow de base](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   [Créer une épreuve avancée avec un workflow automatisé](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

<!--

## Open a proof



## Edit a document

Edit name

Add description

manage

Add new version, open proof, edit, download, move, share, remove
-->

## Filtrer et trier

Vous pouvez organiser votre document à l’aide de filtres et d’options de tri.

### Filtre

Vous pouvez filtrer les documents par

* Ajout par
* Type de fichier

### Trier

Vous pouvez trier les documents par

* Date d’ajout
* Type de fichier
