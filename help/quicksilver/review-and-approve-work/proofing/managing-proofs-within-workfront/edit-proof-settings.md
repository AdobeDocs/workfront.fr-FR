---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Modifier les paramètres des épreuves
description: Vous pouvez modifier les paramètres de l’épreuve que vous avez créée à tout moment.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: a036a99c13d80a2ba2305ebcdc799ad6e5b62b39
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 100%

---

# Modifier les paramètres des épreuves

Vous pouvez modifier les paramètres de l’épreuve que vous avez créée à tout moment.

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
   <td role="rowheader">Rôle de l’épreuve</td> 
   <td>Auteur ou autrice, ou modérateur ou modératrice</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre administrateur ou administratrice Workfront ou Workfront Proof.

+++

## Modifier les paramètres des épreuves

Certains paramètres peuvent être verrouillés si l’équipe d’administration Workfront les a désactivés au niveau du compte.

1. Accédez au projet, à la tâche ou au problème pour qui vous souhaitez créer une épreuve, puis cliquez sur l’onglet **Documents**.
1. Survolez l’épreuve avec la souris, puis cliquez sur **Détails du document**.
1. Dans le panneau de gauche, cliquez sur **Paramètres de la visionneuse de relecture**.
1. Ajustez les paramètres suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Authentification requise. Impossible de partager cette épreuve avec des utilisateurs invités</td> 
      <td> <p>Si vous avez besoin de niveaux de sécurité supérieurs pour votre processus de révision et d’approbation, vous pouvez utiliser l’option Connexion requise pour l’épreuve. Cela signifie que seules les personnes utilisant Workfront peuvent être ajoutées à l’épreuve. Elles doivent également saisir leur adresse e-mail et leur mot de passe avant de pouvoir y accéder.</p> <p>Note : <em style="font-style: normal;">si l’option Connexion requise est activée, les abonnements ne peuvent pas être activés.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger que les décisions soient signées de manière électronique</td> 
      <td> <p>Vous pouvez exiger une signature électronique de toute personne chargée de la révision prenant une décision sur l’épreuve. Lorsqu’un réviseur ou une réviseuse prend une décision, un message apparaît, lui demandant de saisir son adresse électronique et son mot de passe et de confirmer sa décision.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’épreuve lorsque toutes les décisions requises sont prises.</td> 
      <td> <p>Vous pouvez définir l’état d’une épreuve sur verrouillée lorsque la personne approbatrice finale prend sa décision. Cela s’avère utile si vous souhaitez vous assurer que vos réviseurs et réviseuses ne puissent pas revenir sur l’épreuve et ajouter des commentaires supplémentaires ou modifier leurs décisions.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser le téléchargement du fichier original</td> 
      <td> <p>Vous pouvez autoriser les approbateurs et approbatrices d’une épreuve à télécharger le fichier d’origine à partir duquel une épreuve a été créée. Cette option est activée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">autoriser le partage de l'épreuve via une URL publique ou un code intégré</td> 
      <td>Vous pouvez permettre aux utilisateurs et utilisatrices de partager l’épreuve avec une URL publique ou un code intégré. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser l'abonnement à l'épreuve via une URL publique ou un code intégré</td> 
      <td> <p>L’activation de l’inscription à l’épreuve permet aux personnes qui n’y ont pas été explicitement ajoutées de s’y inscrire (c’est-à-dire de s’ajouter à l’épreuve). Elles recevront alors le rôle et l’alerte e-mail que vous leur avez attribués dans les paramètres d’abonnement.</p> <p>Si l’inscription a été activée sur une épreuve, les champs ci-dessous deviennent actifs :</p> 
       <ul> 
        <li><strong>Validation d’abonnement requise</strong> : la personne abonnée doit cliquer sur un lien dans un e-mail pour accéder à une épreuve.<br> En sélectionnant cette option, la personne qui s’abonne ne disposera pas d’un accès immédiat à l’épreuve, mais recevra un lien vers l’épreuve par e-mail. La validation d’abonnement a pour but de s’assurer que la personne a saisi une adresse e-mail correcte à laquelle elle a accès.</li> 
        <li><strong>Rôle par défaut pour les nouvelles personnes abonnées</strong> : il s’agit du rôle de l’épreuve par défaut qui sera attribué à tous les approbateurs et à toutes les approbatrices qui s’abonnent à l’épreuve.</li> 
        <li><strong>Alerte e-mail par défaut pour les nouvelles personnes abonnées</strong> : il s’agit de l’alerte e-mail par défaut qui sera affectée à tous les approbateurs et toutes les approbatrices qui s’abonnent à l’épreuve.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

 
