---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve statique pour un site web ou tout autre contenu web
description: Vous pouvez générer une nouvelle épreuve statique ou une nouvelle version d’une épreuve statique existante pour le contenu web. Le contenu web peut inclure des éléments tels que des publicités avec vidéo en streaming, des animations HTML ou des bannières interactives, mais il sera découpé en plusieurs captures d’écran pour permettre la relecture statique.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 0a7cdf217d3c8227c569831b16f09c0b1d9c7111
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 100%

---

# Créer une épreuve statique pour un site web ou tout autre contenu web

Vous pouvez générer une nouvelle épreuve statique ou une nouvelle version d’une épreuve statique existante pour le contenu web. Le contenu web peut inclure des éléments tels que des publicités avec vidéo en streaming, des animations HTML ou des bannières interactives, mais il sera découpé en plusieurs captures d’écran pour permettre la relecture statique.

Tenez compte des points suivants lors de la création d’épreuves statiques pour un site web ou tout autre contenu web :

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Plan actuel : Pro ou version supérieure</p> <p>ou</p> <p>Formule héritée : Select ou Premium</p> <p>Pour plus d’informations sur la relecture de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
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

## Créer une épreuve statique pour un site web ou tout autre contenu web

Pour créer une épreuve statique, le site web doit être accessible publiquement (et non derrière un pare-feu), ou la liste autorisée de votre entreprise doit inclure le domaine Workfront. Workfront ne peut pas capturer un site web protégé par mot de passe comme épreuve statique.

>[!TIP]
>
>Nous vous recommandons la relecture interactive plutôt que la relecture statique pour les pages internes qui nécessitent une autorisation et les pages protégées par mot de passe. Pour plus d’informations, voir [Vue d’ensemble des épreuves de contenu interactif](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Accédez au projet, à la tâche ou au problème où vous souhaitez créer une épreuve de site web ou une nouvelle version d’une épreuve existante.
1. Cliquez sur **Documents** dans le panneau de gauche.
1. (Le cas échéant) Si vous créez une épreuve, cliquez sur **Ajouter**, puis sur **Épreuve** dans le menu qui s’affiche.
1. (Le cas échéant) Si vous créez une version d’une épreuve existante, procédez comme suit :

   1. Placez le pointeur de la souris sur l’épreuve de l’URL dont vous souhaitez créer une nouvelle version, puis sélectionnez-la en cliquant sur l’arrière-plan bleu clair qui l’entoure.

      ![Select_BAT_by_selection_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Cliquez sur **Ajouter** > **Version** > **Épreuve**.

1. Saisissez l’URL du site web que vous souhaitez réviser dans la zone **Ajouter des fichiers**, puis appuyez sur **Entrée**.

   >[!NOTE]
   >
   > L’URL doit comporter moins de 2 000 caractères.

1. Cliquez sur l’URL que vous avez ajoutée.

   Les options de configuration de l’épreuve du site web s’affichent.

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Facultatif) Si vous souhaitez remplacer le nom de l’épreuve de l’URL du site web par un autre, saisissez le **Nom de l’épreuve**.
1. Assurez-vous que l’option **Capturer une copie d’écran** est sélectionnée et utilisez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Résolution de la copie d’écran</strong> </td> 
      <td> <p>Ajustez la résolution de votre contenu lorsque les réviseurs et réviseuses visualisent l’épreuve, ce qui leur permet de voir comment elle apparaît sur des appareils de tailles différentes, tels que les téléphones, des tablettes et des moniteurs.</p> <p>Si vous sélectionnez plusieurs résolutions, une épreuve distincte est créée pour chaque résolution sélectionnée.</p> <p>Note : lorsqu’un réviseur ou une réviseuse commente l’épreuve, le commentaire inclut la résolution qui s’affiche lorsque le commentaire a été fait, de sorte que les autres réviseurs et réviseuses sachent quelle résolution est associée au commentaire. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Rechercher des sous-pages</strong> </td> 
      <td> <p>Capturez les sous-pages du site web ainsi que ses pages principales. Vous pouvez cliquer sur Sélectionner tout pour inclure toutes les pages ou cliquer uniquement sur certaines pages à inclure. Les boutons Plus et Moins vous permettent de développer et de fermer les zones de sous-page du site web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas modifier le paramètre Capturer la copie d’écran pour les versions ultérieures de l’épreuve que vous créez.

1. Cliquez sur **Terminé**.

   Si vous avez sélectionné plusieurs résolutions de copie d’écran à l’étape 8, la liste comprend un ensemble de copies d’écran pour chaque résolution. Vous pouvez générer ces copies d’écran sous la forme d’épreuves distinctes ou les combiner en une seule épreuve (voir dans ). Nous vous recommandons de les combiner, en particulier si vous créez une épreuve statique pour le site web.

   >[!NOTE]
   >
   >Si vous ajoutez une nouvelle version à une épreuve d’URL existante, toutes les options configurées sur l’épreuve d’origine ou la version précédente sont conservées dans cette version.

1. Cliquez sur **Créer une épreuve** pour créer une épreuve simple sans processus de révision.\
   ou\
   Poursuivez en configurant une épreuve avancée :

   * [Créer une épreuve avancée avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
