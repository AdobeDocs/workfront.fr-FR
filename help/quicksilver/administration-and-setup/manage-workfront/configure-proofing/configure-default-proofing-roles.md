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
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Configuration des rôles de vérification par défaut

En tant qu’administrateur Adobe Workfront, vous pouvez configurer les rôles de vérification par défaut pour les utilisateurs et les utilisateurs invités ayant accès aux BAT créés dans Workfront. Toute personne qui ajoute des utilisateurs à un BAT peut ajuster ces rôles pour eux.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un administrateur Workfront. Pour plus d’informations sur les administrateurs Workfront, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Configuration des rôles de vérification par défaut

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Cliquez sur **Révision et approbation** près du bas de la liste qui s’affiche à gauche.
1. Dans le **Rôles pour les destinataires désignés d’un BAT de document** , sélectionnez le rôle par défaut pour les utilisateurs et les utilisateurs invités qui sont ajoutés au workflow d’un BAT.

   Voir [Droits associés aux rôles de vérification](#rights-associated-with-proofing-roles) ci-dessous pour une liste de chaque rôle de vérification et des droits qui lui sont associés.

   >[!NOTE]
   >
   >* Ce paramètre s’applique uniquement aux utilisateurs créés dans le système Workfront après la définition du rôle. pour les utilisateurs existants.
   >* La personne qui ajoute des utilisateurs au BAT peut ajuster ce rôle, comme décrit dans la section [Ajout d’utilisateurs à un BAT](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Partage d’un BAT dans Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).


1. Dans le **Rôles pour les non-destinataires qui ouvrent un BAT de document** , sélectionnez le rôle par défaut pour les utilisateurs et les utilisateurs invités qui peuvent accéder à un BAT, mais ne sont pas ajoutés au workflow du BAT.

   Cette situation se produit lorsque les utilisateurs et les invités ont accès à un document pour lequel un BAT a été créé : même s&#39;ils n&#39;ont pas été ajoutés au workflow du BAT, ils peuvent ouvrir le BAT.

   **Exemples :** Voici quelques exemples d’utilisation de ce paramètre :

   * Vous pouvez sélectionner **Lecture seule** limiter toutes les activités de BAT, comme l&#39;ajout de commentaires et la prise de décisions à ceux qui ont été invités à le faire ;
   * Vous pouvez sélectionner **Réviseur** car vous souhaitez que tout membre de l’équipe puisse ajouter des annotations et des commentaires sur un BAT.

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
   <th> <p><strong>Afficher un bon à tirer</strong> </p> </th> 
   <th> <p><strong>Ajouter des balises</strong> </p> </th> 
   <th> <p><strong>Ajouter des commentaires</strong> </p> </th> 
   <th> <p><strong>Modifier ses propres commentaires en l’absence de réponse</strong> </p> </th> 
   <th> <p><strong>Prendre une décision</strong> </p> </th> 
   <th> <p><strong>Supprimer les commentaires d’autres utilisateurs</strong> </p> </th> 
   <th>Résoudre les commentaires</th> 
   <th>Application d’actions aux commentaires</th> 
   <th> <p><strong>Modifier le BAT</strong> </p> </th> 
   <th>Partager le BAT avec d’autres personnes</th> 
   <th>Créer une version</th> 
   <th> <p><strong>Affichage des demandes d’approbation dans la zone d’accueil</strong> </p> </th> 
   <th>Ajouter de nouveaux opérateurs validants</th> 
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
   <td> <p><strong>Réviseur et approbateur</strong> </p> </td> 
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
   <td> <p><strong>Auteur</strong> </p> </td> 
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
>Les utilisateurs des nouveaux plans Workfront peuvent accorder des rôles d’auteur ou de modérateur à n’importe quel utilisateur du système. Les utilisateurs sur les plans hérités peuvent accorder des rôles d’auteur ou de modérateur à tout utilisateur disposant d’une licence de BAT dans le système.
