---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuration des rôles de vérification par défaut
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer les rôles de relecture par défaut pour les utilisateurs et utilisatrices et les personnes invitées ayant accès aux épreuves créées dans Workfront. Toute personne qui ajoute des utilisateurs et utilisatrices à une épreuve peut ajuster ces rôles pour eux.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 99%

---

# Configurer des rôles de relecture par défaut

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer les rôles de relecture par défaut pour les utilisateurs et utilisatrices et les personnes invitées ayant accès aux épreuves créées dans Workfront. Toute personne qui ajoute des utilisateurs et utilisatrices à une épreuve peut ajuster ces rôles pour eux.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront. Pour plus d’informations sur les administrateurs et administratrices Workfront, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder un accès administratif complet à un utilisateur ou une utilisatrice</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

+++

## Configurer des rôles de relecture par défaut

{{step-1-to-setup}}

<!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Cliquez sur **Révision et approbation** près du bas de la liste qui s’affiche à gauche.
1. Dans la section **Rôles pour les personnes destinataires désignées d’une épreuve de document**, sélectionnez le rôle par défaut pour les utilisateurs et utilisatrices et les personnes invitées qui sont ajoutés au workflow d’une épreuve.

   Consultez la section [Droits associés aux rôles de relecture](#rights-associated-with-proofing-roles) ci-dessous pour une liste de chaque rôle de relecture et des droits qui lui sont associés.

   >[!NOTE]
   >
   >* Ce paramètre s’applique uniquement aux utilisateurs et utilisatrices créés dans le système Workfront une fois le rôle défini, et non à celles et ceux existants.
   >* La personne qui ajoute des utilisateurs et utilisatrices à l’épreuve peut ajuster ce rôle, comme décrit dans la section [Ajouter des utilisateurs et utilisatrices à une épreuve](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) dans [Partager une épreuve dans Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

1. Dans la section **Rôles pour les personnes non-destinataires ouvrant une épreuve de document**, sélectionnez le rôle par défaut pour les utilisateurs et utilisatrices et les personnes invitées pouvant accéder à une épreuve mais qui ne sont pas ajoutés au workflow de l’épreuve.

   Cela se produit lorsque les utilisateurs et utilisatrices et les personnes invitées ont accès à un document pour lequel une épreuve a été créée : ils peuvent ouvrir une épreuve, même s’ils n’ont pas été ajoutés à son workflow.

   **Exemples :** voici quelques exemples d’utilisation de ce paramètre :

   * Vous sélectionnez **Lecture seule** pour limiter toute activité d’une épreuve, comme l’ajout de commentaires et la prise de décisions, aux personnes qui ont été invitées à le faire.
   * Vous sélectionnez **Rôle de révision**, car vous souhaitez que toute personne membre de l’équipe puisse ajouter des annotations et des commentaires à une épreuve.

1. Cliquer sur **Enregistrer**.

## Droits associés aux rôles de relecture {#rights-associated-with-proofing-roles}

Le tableau suivant présente chaque rôle et les droits qui lui sont associés :

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
   <th> <p><strong>Afficher une épreuve</strong> </p> </th> 
   <th> <p><strong>Ajouter des balises</strong> </p> </th> 
   <th> <p><strong>Ajouter des commentaires</strong> </p> </th> 
   <th> <p><strong>Modifier ses propres commentaires en l’absence de réponse</strong> </p> </th> 
   <th> <p><strong>Prendre une décision</strong> </p> </th> 
   <th> <p><strong>Supprimer des commentaires d’autres personnes</strong> </p> </th> 
   <th>Résoudre les commentaires</th> 
   <th>Appliquer des actions aux commentaires</th> 
   <th> <p><strong>Modifier l’épreuve</strong> </p> </th> 
   <th>Partager l’épreuve</th> 
   <th>Créer une nouvelle version</th> 
   <th> <p><strong>Afficher les demandes d’approbation dans la zone d’accueil</strong> </p> </th> 
   <th>Ajouter de nouveaux réviseurs et réviseuses</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Lecture seule</strong> </p> </td> 
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
   <td> <p><strong>Réviseur et réviseuse, approbateur et approbatrice</strong> </p> </td> 
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
>Les personnes disposant des nouveaux plans Workfront peuvent accorder des rôles de création ou de modération à n’importe quelle personne du système. Les personnes utilisant les plans hérités peuvent accorder des rôles de création ou de modération aux utilisateurs et utilisatrices disposant d’une licence de relecture dans le système.
