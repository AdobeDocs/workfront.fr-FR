---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve pour le contenu interactif dans un fichier ZIP
description: Vous pouvez générer une épreuve pour un contenu interactif qui n’est pas un site web et qui est stocké dans un fichier ZIP. Parmi les exemples de ce type de contenu web, on peut citer les publicités avec vidéo ou audio en continu, les animations HTML, les bannières interactives.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
TQID: https://experienceleague.adobe.com/wJNC4pCRhTpOfoiB1X6-6vKrYvWA2EaR-x2HfhwcDaY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 93%

---

# Créer une épreuve pour le contenu interactif dans un fichier ZIP

Vous pouvez générer une épreuve pour un contenu interactif qui n’est pas un site web et qui est stocké dans un fichier ZIP. Parmi les exemples de ce type de contenu web, on peut citer les publicités avec vidéo ou audio en continu, les animations HTML, les bannières interactives.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Standard</p>
   <p>Travail ou plan</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux documents</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une épreuve pour le contenu interactif dans un fichier ZIP

Une fois que vous avez ajouté du contenu interactif dans un fichier ZIP à une épreuve, Adobe Workfront crée une épreuve des documents compressés. Selon la taille du fichier, le temps de chargement peut varier. La création de fichiers plus volumineux prend plus de temps. Vous pouvez quitter la page et Workfront continue à créer votre fichier. La taille maximale de chargement de fichier est de 4 Go. 

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
