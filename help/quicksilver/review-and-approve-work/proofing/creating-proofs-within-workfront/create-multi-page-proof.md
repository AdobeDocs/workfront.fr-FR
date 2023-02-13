---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Création d’un BAT multi-page
description: Vous pouvez combiner plusieurs fichiers en un seul BAT multi-page. Les réviseurs peuvent utiliser les outils de navigation de la visionneuse de vérification pour parcourir les pages dans un BAT multipage.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# Création d’un BAT multi-page

Vous pouvez combiner plusieurs fichiers en un seul BAT multi-page. Les réviseurs peuvent utiliser les outils de navigation de la visionneuse de vérification pour parcourir les pages dans un BAT multipage.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou version ultérieure</p> <p>ou</p> <p>Plan hérité : Sélectionner ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Travail ou plan</p> <p>Plan hérité : N’importe quel (la vérification doit être activée pour l’utilisateur)</p> </td> 
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

&#42;Pour savoir quel profil d’autorisation de plan, de licence ou de BAT vous avez, contactez votre administrateur de BAT Workfront ou Workfront.

## Création d’un BAT multi-page

Lorsque cette option est activée, les fichiers statiques et les sites web sont disponibles dans un seul bon à tirer. Lorsque cette option est désactivée, tous les documents et sites web sont générés en tant que BAT individuels. Vous pouvez télécharger jusqu’à 100 fichiers à la fois.

Pour créer un BAT multi-page :

1. Accédez au projet, à la tâche ou au problème pour lequel vous souhaitez obtenir le BAT, puis cliquez sur le bouton **Documents** .
1. Cliquez sur **Ajouter** > **Bon à tirer** .
1. Faites glisser et déposez les fichiers ou recherchez-les et sélectionnez-les dans l’explorateur de fichiers. Vous pouvez charger jusqu’à 50 fichiers à la fois. Pour plus d’informations sur les limites de fichiers, voir [Considérations](#considerations) dans cet article.

   >[!NOTE]
   >
   >Les fichiers interactifs, y compris les vidéos et les sites web interactifs, ne peuvent pas être combinés en un seul BAT.

1. Sous **BAT unique**, activez l’option , **Combiner tous les fichiers compatibles en un seul BAT**.
1. Dans le **Nom du BAT** , indiquez un nouveau nom pour le BAT combiné.
1. (Facultatif) Dans la liste des fichiers que vous avez chargés, réorganisez les fichiers en les faisant glisser. L’ordre des fichiers est l’ordre des pages du BAT combiné.
1. (Facultatif) Pour supprimer un seul fichier de la page Nouveau BAT, passez la souris sur le fichier et cliquez sur le bouton **Corbeille** qui s’affiche à droite.

   Ou

   Pour supprimer tous les fichiers chargés en une seule fois, cliquez sur **Tout supprimer** dans le coin supérieur droit de la liste.

1. Une fois tous vos fichiers téléchargés, vous devez décider si vous souhaitez configurer un BAT de base ou un BAT automatisé :

   * Avec un BAT de base, vous pouvez ajouter autant de validants que vous le souhaitez à un BAT, mais ils ne sont pas organisés par étapes. Tous les opérateurs validants que vous ajoutez peuvent accéder au BAT immédiatement après sa création. Pour configurer un BAT de base, voir [Créer un BAT avancé avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Avec un BAT automatisé, le BAT passe d’une étape à l’autre et Adobe Workfront avertit chaque utilisateur lorsqu’il lui appartient de le vérifier. pour configurer un BAT automatisé, voir [Créer un BAT avancé avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Considérations {#considerations}

Tenez compte des points suivants lorsque vous combinez des fichiers dans un seul BAT :

* Vous pouvez charger jusqu’à 500 fichiers distincts.
* Vous pouvez combiner des fichiers statiques de différents types (par exemple, PDF, JPG, DOC, PPT, EXC), jusqu’à 2 000 pages au total.
* Vous pouvez combiner des captures Web statiques.
* Vous pouvez combiner des fichiers de GIF ; cependant, les GIFs animés sont traités comme des fichiers statiques.
* Vous ne pouvez pas combiner des fichiers AV et des captures Web interactives.
* La miniature du BAT est extraite de la première page du BAT (voir [Gestion des détails du BAT dans le BAT Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Vous pouvez vérifier les noms des fichiers qui ont été combinés pour créer le BAT sur la page Détails du BAT. Pour plus d’informations, voir [Gestion des détails du BAT dans le BAT Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Si l&#39;option de téléchargement des fichiers originaux est activée sur le BAT, vous pouvez télécharger tous les fichiers qui ont été combinés afin de créer le BAT en tant que fichier .zip. Pour plus d’informations, voir  [Téléchargement des fichiers stockés dans le bon à tirer Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
