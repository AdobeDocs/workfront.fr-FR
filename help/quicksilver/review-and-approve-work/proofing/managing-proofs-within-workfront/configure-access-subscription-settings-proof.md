---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Configurer les paramètres d’accès et d’abonnement d’une épreuve
description: Vous pouvez configurer certains paramètres d’accès et d’abonnement pour des épreuves individuelles, par exemple s’il est nécessaire d’obliger les personnes à se connecter et s’il est possible d’autoriser les personnes à s’abonner à l’épreuve. Vous pouvez configurer les paramètres d’accès et d’abonnement pour une épreuve pendant que vous la créez ou vous pouvez les configurer pour une épreuve qui existe déjà dans Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 100%

---

# Configurer les paramètres d’accès et d’abonnement d’une épreuve

Vous pouvez configurer certains paramètres d’accès et d’abonnement pour des épreuves individuelles, par exemple s’il est nécessaire d’obliger les personnes à se connecter et s’il est possible d’autoriser les personnes à s’abonner à l’épreuve. Vous pouvez configurer les paramètres d’accès et d’abonnement pour une épreuve pendant que vous la créez ou vous pouvez les configurer pour une épreuve qui existe déjà dans Workfront.

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

## Configurer les paramètres d’accès et d’abonnement lors de la création d’une épreuve

Pour configurer les paramètres d’accès et d’abonnement pour une épreuve pendant sa création :

1. Accédez au projet, à la tâche ou au problème pour lequel vous souhaitez créer une épreuve, puis cliquez sur la section **Documents**.
1. Cliquez sur **Ajouter nouveau** dans la zone supérieure droite.
1. Faites défiler l’écran jusqu’à **Paramètres de l’épreuve** dans le coin inférieur droit de la page **Nouvelle épreuve**.

1. Configurez les paramètres suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Autoriser le partage de l’épreuve via une URL publique ou un code intégré</strong> </td> 
      <td>Lorsque cette option est sélectionnée, l’épreuve peut être partagée via une URL publique ou un code intégré.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Autoriser l’abonnement à l’épreuve via une URL publique ou un code intégré</strong> </td> 
      <td>Lorsque cette option est sélectionnée, les personnes qui n’ont pas été explicitement ajoutées à l’épreuve peuvent s’y abonner. La personne qui s’abonne à l’épreuve se voit attribuer le rôle et l’adresse e-mail que vous définissez dans les paramètres suivants :
       <ul>
        <li><p><strong>Rôle de personne abonnée :</strong> le rôle d’épreuve par défaut attribué à tous les réviseurs et réviseuses qui s’abonnent à l’épreuve.</p><p>Important : si <strong>Autoriser le partage avec</strong> est défini sur toute autre valeur que <strong>Tous</strong> dans les paramètres de Workfront Proof, l’abonnement ne fonctionne que pour les personnes de l’organisation. Pour plus d’informations, voir <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurer des paramètres d’épreuve dans Workfront Proof</a>.</p></li>
        <li><strong>Paramètres des alertes par e-mail pour les personnes abonnées :</strong> l’alerte par défaut qui est affectée à tous les réviseurs et réviseuses qui s’abonnent à l’épreuve.</li>
       </ul><p>
        <ul>
         <li><strong>Un accès à l’épreuve via un lien e-mail requis pour :</strong> Indiquez si la personne abonnée reçoit un e-mail avec un lien vers l’épreuve. Vous pouvez sélectionner <strong>Aucun e-mail</strong> (aucun lien d’e-mail n’est nécessaire pour accéder à l’épreuve), <strong>E-mail de notification de l’épreuve uniquement</strong> (la personne abonnée reçoit un lien vers l’épreuve par e-mail sans vérification), ou <strong>E-mails de validation et de notification de l’épreuve</strong> (la personne abonnée reçoit un lien vers l’épreuve par e-mail et doit cliquer sur le lien pour accéder à une épreuve ; l’objectif de cette option est de s’assurer que la personne a saisi une adresse e-mail correcte à laquelle elle a accès).</li>
        </ul><p>Note : si un workflow automatisé est joint aux épreuves, tous les abonnements génèrent des e-mails de confirmation pour les personnes propriétaires des épreuves, afin qu’elles puissent décider à quelle étape la personne doit être ajoutée.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continuez à créer votre épreuve.

## Configurer les paramètres d’accès et d’abonnement pour une épreuve existante

Pour configurer les paramètres d’accès et d’abonnement pour une épreuve qui existe déjà dans Workfront :

1. Dans la zone Documents, sélectionnez le document contenant l’épreuve pour laquelle vous souhaitez configurer les paramètres, puis cliquez sur **Détails du document**.
1. Dans le panneau de gauche, cliquez sur **Paramètres de la visionneuse de relecture**.
1. Configurez les paramètres suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Autoriser le partage de l’épreuve via une URL publique ou un code intégré</strong><strong></strong> </td> 
      <td>Lorsque cette option est sélectionnée, l’épreuve peut être partagée via une URL publique ou un code intégré.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Autoriser l’abonnement à l’épreuve via une URL publique ou un code intégré</strong> </td> 
      <td>Lorsque cette option est sélectionnée, les personnes qui n’ont pas été explicitement ajoutées à l’épreuve peuvent s’y abonner. La personne qui s’abonne à l’épreuve se voit attribuer le rôle et l’adresse e-mail que vous définissez dans les paramètres suivants :
       <ul>
        <li><p><strong>Rôle de personne abonnée :</strong> le rôle d’épreuve par défaut attribué à tous les réviseurs et réviseuses qui s’abonnent à l’épreuve.</p><p>Important : si <strong>Autoriser le partage avec</strong> est défini sur toute autre valeur que <strong>Tous</strong> dans les paramètres de Workfront Proof, l’abonnement ne fonctionne que pour les personnes de l’organisation. Pour plus d’informations, voir <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurer des paramètres d’épreuve dans Workfront Proof</a>.</p></li>
        <li><strong>Paramètres des alertes par e-mail pour les personnes abonnées :</strong> l’alerte par défaut qui est affectée à tous les réviseurs et réviseuses qui s’abonnent à l’épreuve.</li>
       </ul><p>
        <ul>
         <li><strong>Un accès à l’épreuve via un lien e-mail requis pour :</strong> Indiquez si la personne abonnée reçoit un e-mail avec un lien vers l’épreuve. Vous pouvez sélectionner <strong>Aucun e-mail</strong> (aucun lien d’e-mail n’est nécessaire pour accéder à l’épreuve), <strong>E-mail de notification de l’épreuve uniquement</strong> (la personne abonnée reçoit un lien vers l’épreuve par e-mail sans vérification), ou <strong>E-mails de validation et de notification de l’épreuve</strong> (la personne abonnée reçoit un lien vers l’épreuve par e-mail et doit cliquer sur le lien pour accéder à une épreuve ; l’objectif de cette option est de s’assurer que la personne a saisi une adresse e-mail correcte à laquelle elle a accès).</li>
        </ul><p>Note : si un workflow automatisé est joint aux épreuves, tous les abonnements génèrent des e-mails de confirmation pour les personnes propriétaires des épreuves, afin qu’elles puissent décider à quelle étape la personne doit être ajoutée.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.
