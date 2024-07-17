---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve interactive pour un site web ou un autre contenu web
description: Vous pouvez générer un nouveau BAT interactif ou une nouvelle version d’un BAT interactif existant pour le contenu web. Il peut s’agir d’un site web ou d’autres types de contenu interactif, tels que des publicités avec diffusion vidéo ou audio en continu, des animations d’HTML et des bannières interactives.
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 35d76d3cb06c9e9b449844f304f1443e24a221d4
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 22%

---

# Créer une épreuve interactive pour un site web ou un autre contenu web

Vous pouvez générer un nouveau BAT interactif ou une nouvelle version d’un BAT interactif existant pour le contenu web. Il peut s’agir d’un site web ou d’autres types de contenu interactif, tels que des publicités avec diffusion vidéo ou audio en continu, des animations d’HTML et des bannières interactives.

Dans un BAT interactif, les réviseurs peuvent naviguer et interagir comme ils le feraient habituellement avec le site web ou tout autre contenu web.

>[!IMPORTANT]
>
>Assurez-vous que le site web ou le contenu interactif est accessible aux personnes qui vont le consulter. Ils ne peuvent y accéder que s&#39;ils peuvent également y accéder sur Internet.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
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

## Créer une épreuve interactive pour un site web ou un autre contenu web

1. Accédez au projet, à la tâche ou au problème où vous souhaitez créer un BAT de site web ou une nouvelle version d’un BAT existant.
1. Cliquez sur **Documents** dans le panneau de gauche.
1. (Conditionnel) Si vous créez un BAT, cliquez sur **Ajouter nouveau**, puis sur **BAT** dans le menu qui s’affiche.

1. (Conditionnel) Sur la page **New BAT** s’affiche, si vous créez une version d’un BAT existant :

   1. Pointez sur le BAT de l’URL pour lequel vous souhaitez créer une version, puis sélectionnez-le en cliquant sur l’arrière-plan bleu clair qui l’entoure.

      ![Select_BAT_by_selection_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)


   1. Dans la liste déroulante **Ajouter un nouveau**, cliquez sur **Version** > **Bon à tirer**.

1. Dans la section **Ajouter des fichiers** , saisissez l’URL du site Web à tester, puis appuyez sur **Entrée**.  Vous pouvez répéter ce processus pour ajouter plusieurs sites Web à vérifier.

   ![BAT_website.png](assets/proof-website-350x65.png)


   >[!NOTE]
   >
   > L’URL doit comporter moins de 1 000 caractères.

1. Cliquez sur l’URL que vous avez ajoutée.

   ![](assets/click-url-350x137.png)

1. (Facultatif) Si vous souhaitez remplacer le nom du BAT de l’URL du site Web par un autre nom, saisissez un **Nom du BAT**.
1. Sélectionnez **Interactive**, puis cliquez sur **Done**.

   >[!NOTE]
   >
   >Si vous ajoutez une nouvelle version à un BAT d’URL existant, toutes les options configurées sur le BAT d’origine ou la version précédente sont conservées dans cette version.

1. Cliquez sur **Créer un BAT** pour créer un BAT simple sans processus de révision.\
   ou\
   Poursuivez en configurant un BAT avancé :

   * [Créer une épreuve avancée avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
