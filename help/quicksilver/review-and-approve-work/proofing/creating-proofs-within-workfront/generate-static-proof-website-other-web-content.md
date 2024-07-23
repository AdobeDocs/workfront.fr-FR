---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve statique pour un site web ou un autre contenu web
description: Vous pouvez générer un nouveau BAT statique ou une nouvelle version d’un BAT statique existant pour le contenu web. Le contenu web peut inclure des éléments tels que des publicités avec diffusion vidéo en continu, des animations d’HTML ou des bannières interactives, mais il sera découpé en plusieurs captures d’écran pour permettre la vérification statique.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 15%

---

# Créer une épreuve statique pour un site web ou un autre contenu web

Vous pouvez générer un nouveau BAT statique ou une nouvelle version d’un BAT statique existant pour le contenu web. Le contenu web peut inclure des éléments tels que des publicités avec diffusion vidéo en continu, des animations d’HTML ou des bannières interactives, mais il sera découpé en plusieurs captures d’écran pour permettre la vérification statique.

Tenez compte des points suivants lors de la création de BAT statiques pour un site web ou un autre contenu web :

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : sélectionnez ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

+++

## Créer une épreuve statique pour un site web ou un autre contenu web

Pour créer un BAT statique, le site web doit être accessible publiquement (et non derrière un pare-feu), ou la liste autorisée de votre entreprise doit inclure le domaine Workfront. Workfront ne peut pas capturer un site web protégé par mot de passe comme BAT statique.

>[!TIP]
>
>Nous vous recommandons de procéder à la vérification interactive plutôt que de procéder à la vérification statique des pages internes nécessitant des pages protégées par une autorisation et un mot de passe. Pour plus d’informations, voir [Présentation des BAT de contenu interactif](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Accédez au projet, à la tâche ou au problème où vous souhaitez créer un BAT de site web ou une nouvelle version d’un BAT existant.
1. Cliquez sur **Documents** dans le panneau de gauche .
1. (Conditionnel) Si vous créez un BAT, cliquez sur **Ajouter nouveau**, puis sur **BAT** dans le menu qui s’affiche.
1. (Conditionnel) Si vous créez une version d’un BAT existant :

   1. Placez le pointeur de la souris sur le BAT de l’URL pour lequel vous souhaitez créer une version, puis sélectionnez-le en cliquant sur l’arrière-plan bleu clair qui l’entoure.

      ![Select_BAT_by_selection_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Cliquez sur **Ajouter** > **Version** > **Bon à tirer**.

1. Saisissez l’URL du site Web à tester dans la zone **Ajouter des fichiers**, puis appuyez sur **Entrée**.

   >[!NOTE]
   >
   > L’URL doit comporter moins de 1 000 caractères.

1. Cliquez sur l’URL que vous avez ajoutée.

   Les options de configuration du BAT du site web s’affichent.

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Facultatif) Si vous souhaitez remplacer le nom du BAT de l’URL du site Web par un autre nom, saisissez un **Nom du BAT.**
1. Assurez-vous que la **capture d’écran** est sélectionnée et utilisez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Résolution de capture d’écran</strong> </td> 
      <td> <p>Ajustez la résolution de votre contenu lorsque les réviseurs visualisent le BAT, ce qui leur permet de voir comment il apparaît sur des appareils de tailles différentes, tels que les téléphones, tablettes et moniteurs.</p> <p>Si vous sélectionnez plusieurs résolutions, un BAT distinct est créé pour chaque résolution sélectionnée.</p> <p>Remarque : Lorsqu’un réviseur commente le BAT, le commentaire inclut la résolution qui s’affiche lorsque le commentaire a été fait, de sorte que les autres réviseurs sachent quelle résolution est associée au commentaire. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Rechercher des sous-pages</strong> </td> 
      <td> <p>Capturez les sous-pages du site web ainsi que ses principales pages. Vous pouvez cliquer sur Sélectionner tout pour inclure toutes les pages ou sur certaines pages à inclure uniquement. Les boutons plus et moins vous permettent de développer et de fermer les zones de sous-page du site web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas modifier le paramètre Capturer la capture d’écran pour les versions ultérieures du BAT que vous créez.

1. Cliquez sur **Terminé**.

   Si vous avez sélectionné plusieurs résolutions de capture d’écran à l’étape 8, la liste comprend un ensemble de captures d’écran pour chaque résolution. Vous pouvez générer ces captures d’écran sous la forme de BAT distincts ou les combiner en un seul BAT (voir  dans .). Nous vous recommandons de les combiner, en particulier si vous créez un BAT statique pour le site web.

   >[!NOTE]
   >
   >Si vous ajoutez une nouvelle version à un BAT d’URL existant, toutes les options configurées sur le BAT d’origine ou la version précédente sont conservées dans cette version.

1. Cliquez sur **Créer un BAT** pour créer un BAT simple sans processus de révision.\
   ou\
   Poursuivez en configurant un BAT avancé :

   * [Créer une épreuve avancée avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
