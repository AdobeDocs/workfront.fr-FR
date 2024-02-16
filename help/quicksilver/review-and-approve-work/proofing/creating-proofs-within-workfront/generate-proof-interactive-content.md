---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Création d’un BAT pour le contenu interactif dans un fichier ZIP
description: Vous pouvez générer un BAT pour le contenu interactif hors site web stocké dans un fichier ZIP. Parmi les exemples de ce type de contenu web, citons les publicités avec diffusion vidéo ou audio en continu, les animations par HTML, les bannières interactives.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# Création d’un BAT pour le contenu interactif dans un fichier ZIP

Vous pouvez générer un BAT pour le contenu interactif hors site web stocké dans un fichier ZIP. Parmi les exemples de ce type de contenu web, citons les publicités avec diffusion vidéo ou audio en continu, les animations par HTML, les bannières interactives.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Création d’un BAT pour le contenu interactif dans un fichier ZIP

Une fois que vous avez ajouté du contenu interactif dans un fichier ZIP à un BAT, Adobe Workfront crée un bon à tirer des documents compressés. Selon la taille du fichier, le temps de chargement peut varier. La création de fichiers plus volumineux prend plus de temps. Vous pouvez quitter la page et Workfront continue à créer votre fichier. La taille maximale du téléchargement de fichier est de 4 Go. 

1. Préparez votre contenu en créant un fichier compressé ZIP.

   Le fichier ZIP doit répondre aux exigences suivantes :

   * Toutes les ressources, telles que CSS, JavaScript, vidéos, sons et images, doivent être incluses dans le fichier de bundle.
   * Assurez-vous que le fichier principal (index.html, index.htm, par exemple) se trouve dans le dossier racine et qu’il s’agit du seul fichier .html/.htm qui y est stocké.

     Si le fichier principal n’est pas placé dans le dossier racine, Workfront recherche le dossier pour trouver le fichier principal.

   * La taille maximale du lot est de 500 Mo.
   * Dans le cas de fichiers ZIP créés dans iOS, l’outil identifie automatiquement le dossier approprié où le contenu est placé.

1. Accédez au projet, à la tâche ou à l’emplacement où vous souhaitez charger le fichier ZIP.
1. Cliquez sur **Documents** dans le panneau de gauche .
1. Cliquez sur **Ajouter**, puis cliquez sur **Bon à tirer** dans le menu qui s’affiche.
1. Dans le **Ajouter des fichiers** , effectuez un glisser-déposer ou recherchez le fichier ZIP dont vous avez besoin.
1. Cliquez sur **Créer un BAT** pour créer un BAT simple sans processus de révision.\
   ou\
   Poursuivez en configurant un BAT avancé :

   * [Créer un BAT avancé avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer un BAT avancé avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
