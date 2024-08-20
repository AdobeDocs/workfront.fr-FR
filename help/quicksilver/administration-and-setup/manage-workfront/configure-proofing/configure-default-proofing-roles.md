---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuration des rôles de vérification par défaut
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer les rôles de vérification par défaut pour les utilisateurs et les utilisateurs invités ayant accès aux BAT créés dans Workfront. Toute personne qui ajoute des utilisateurs à un BAT peut ajuster ces rôles pour eux.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 34%

---

# Configurer des rôles de relecture par défaut

En tant qu’administrateur Adobe Workfront, vous pouvez configurer les rôles de vérification par défaut pour les utilisateurs et les utilisateurs invités ayant accès aux BAT créés dans Workfront. Toute personne qui ajoute des utilisateurs à un BAT peut ajuster ces rôles pour eux.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur Workfront. Pour plus d’informations sur les administrateurs de Workfront, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès d’administration complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Configurer des rôles de relecture par défaut

{{step-1-to-setup}}

<!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Cliquez sur **Révision et approbation** près du bas de la liste qui s’affiche à gauche.
1. Dans la section **Rôles pour les destinataires désignés d’un BAT de document** , sélectionnez le rôle par défaut pour les utilisateurs et les utilisateurs invités qui sont ajoutés au workflow d’un BAT.

   Voir [Droits associés aux rôles de vérification](#rights-associated-with-proofing-roles) ci-dessous pour obtenir la liste de chaque rôle de vérification et des droits qui lui sont associés.

   >[!NOTE]
   >
   >* Ce paramètre s’applique uniquement aux utilisateurs créés dans le système Workfront une fois le rôle défini, et non aux utilisateurs existants.
   >* La personne qui ajoute des utilisateurs au BAT peut ajuster ce rôle, comme décrit dans [Ajouter des utilisateurs à un BAT](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) dans [Partager un BAT dans Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

1. Dans la section **Rôles pour les non-destinataires qui ouvrent un BAT de document** , sélectionnez le rôle par défaut pour les utilisateurs et les utilisateurs invités qui peuvent accéder à un BAT, mais ne sont pas ajoutés au workflow du BAT.

   Cette situation se produit lorsque les utilisateurs et les invités ont accès à un document pour lequel un BAT a été créé : même s&#39;ils n&#39;ont pas été ajoutés au workflow du BAT, ils peuvent ouvrir le BAT.

   **Exemples :** Voici des exemples d’utilisation de ce paramètre :

   * Vous sélectionnez **Lecture seule** pour limiter toutes les activités de BAT, comme l&#39;ajout de commentaires et la prise de décisions à ceux qui ont été invités à le faire.
   * Vous sélectionnez **Réviseur** car vous souhaitez que tout membre de l’équipe puisse ajouter des annotations et des commentaires sur un BAT.

1. Cliquer sur **Enregistrer**.

## Droits associés aux rôles de vérification {#rights-associated-with-proofing-roles}

Le tableau suivant présente chaque rôle et les droits qui lui sont associés :

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Consulter une épreuve</strong> </p> </th> 
   <th> <p><strong>Ajouter des annotations</strong> </p> </th> 
   <th> <p><strong>Ajouter des commentaires</strong> </p> </th> 
   <th> <p><strong>Modifier ses propres commentaires en l’absence de réponse</strong> </p> </th> 
   <th> <p><strong>Prendre une décision</strong> </p> </th> 
   <th> <p><strong>Supprimer les commentaires d’autres personnes</strong> </p> </th> 
   <th>Résoudre les commentaires</th> 
   <th>Appliquer des actions aux commentaires</th> 
   <th> <p><strong>Modifier l’épreuve</strong> </p> </th> 
   <th>Partager l’épreuve avec d’autres personnes</th> 
   <th>Créer une version</th> 
   <th> <p><strong>Afficher les demandes d’approbation dans la zone d’accueil</strong> </p> </th> 
   <th>Ajouter de nouvelles personnes réviseuses</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>En lecture seule</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Réviseur</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Approbateur</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Personne réviseuse et approbatrice</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Auteur et autrice</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Modérateur</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Les utilisateurs et utilisatrices des nouveaux plans Workfront peuvent accorder des rôles d’auteur et d’autrice ou de modérateur et de modératrice à n’importe quelle personne dans le système. Les utilisateurs et utilisatrices disposant de plans hérités peuvent accorder des rôles d’auteur et d’autrice ou de modérateur et de modératrice à toute personne disposant d’une licence d’épreuve dans le système.
