---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve pour le contenu interactif dans un fichier ZIP
description: Vous pouvez générer une épreuve pour un contenu interactif qui n’est pas un site web et qui est stocké dans un fichier ZIP. Parmi les exemples de ce type de contenu web, on peut citer les publicités avec vidéo ou audio en continu, les animations HTML, les bannières interactives.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 100%

---

# Créer une épreuve pour le contenu interactif dans un fichier ZIP

Vous pouvez générer une épreuve pour un contenu interactif qui n’est pas un site web et qui est stocké dans un fichier ZIP. Parmi les exemples de ce type de contenu web, on peut citer les publicités avec vidéo ou audio en continu, les animations HTML, les bannières interactives.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Plan actuel : Pro ou version supérieure</p> <p>ou</p> <p>Plan hérité : Premium</p> <p>Pour plus d’informations sur l’accès à la relecture avec les différents plans, voir la section <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Plan hérité : n’importe lequel (la relecture doit être activée pour l’utilisateur ou l’utilisatrice)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre administrateur ou administratrice Workfront ou Workfront Proof.

+++

## Créer une épreuve pour le contenu interactif dans un fichier ZIP

Lorsque vous ajoutez du contenu interactif dans un fichier ZIP à une épreuve, Adobe Workfront crée une épreuve à partir des documents zippés. Le temps de chargement varie en fonction de la taille du fichier. La création de fichiers plus volumineux prend plus de temps. Vous pouvez quitter la page et Workfront continue à créer votre fichier.La taille maximale du chargement de fichier est de 4 Go. 

1. Préparez votre contenu en créant un fichier ZIP groupé.

   Le fichier ZIP doit répondre aux exigences suivantes :

   * Toutes les ressources, telles que CSS, JavaScript, vidéos, sons et images, doivent être incluses dans le fichier de lot.
   * Assurez-vous que le fichier principal (tel qu’index.html, index.htm) se trouve dans le dossier racine et qu’il s’agit du seul fichier .html/.htm qui y est stocké.

     Si le fichier principal n’est pas placé dans le dossier racine, Workfront recherche le fichier principal dans le dossier.

   * La taille maximale du lot est de 500 Mo.
   * Dans le cas des fichiers ZIP créés dans iOS, l’outil identifie automatiquement le bon dossier dans lequel le contenu est placé.

1. Accédez au projet, à la tâche ou au problème pour lequel vous souhaitez télécharger le fichier ZIP.
1. Cliquez sur **Documents** dans le panneau de gauche.
1. Cliquez sur **Ajouter nouveau**, puis sur **Épreuve** dans le menu qui apparaît.
1. Dans la section **Ajouter des fichiers**, glissez-déposez ou recherchez le fichier ZIP dont vous avez besoin.
1. Cliquez sur **Créer une épreuve** pour créer une épreuve simple sans procédure de révision.\
   ou\
   Poursuivez en configurant une épreuve avancée :

   * [Créer une épreuve avancée avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
