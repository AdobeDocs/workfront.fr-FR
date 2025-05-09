---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Gérer les invitations par e-mail pour les nouveaux utilisateurs
description: En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez ajouter des utilisateurs et des utilisatrices à Workfront et les informer qu’ils ont été ajoutés en leur envoyant des invitations par e-mail.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: dccbd5a036e1b148bc8f3e41fac3a67babe6dc9a
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 96%

---

# Gérer les invitations par e-mail aux nouveaux utilisateurs et utilisatrices

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>La procédure décrite sur cette page ne s’applique qu’aux entreprise qui n’ont pas encore été intégrées à l’Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, vous devez effectuer cette action via Adobe Admin Console.
>
>Pour suivre la procédure correspondant à votre situation et à son intégration ou non à Adobe Admin Console, consultez la section [Différences en matière d’administration en fonction de la plateforme (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez ajouter des utilisateurs et des utilisatrices à Workfront et les informer qu’ils ont été ajoutés en leur envoyant des invitations par e-mail.

L’invitation par e-mail permet aux nouveaux utilisateurs et utilisatrices de suivre un lien où ils pourront choisir un mot de passe pour leur compte Workfront. Ils peuvent alors terminer la configuration de leur compte.

Pour garantir la sécurité des nouveaux comptes, nous vous recommandons d’utiliser des invitations par e-mail pour vos nouveaux utilisateurs et utilisatrices, afin qu’ils puissent choisir leur propre mot de passe. Vous pouvez également sélectionner un mot de passe pour un nouvel utilisateur ou une nouvelle utilisatrice lors de la création de son compte. Pour plus d’informations sur l’ajout de nouveaux utilisateurs et utilisatrices à Workfront, voir [Ajouter des utilisateurs et des utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Vous pouvez configurer les e-mails des nouveaux utilisateurs et utilisatrices pour les personnes suivantes :

* Toute nouvelle personne ajoutée à Workfront
* Utilisateurs et utilisatrices ajoutés à Workfront avec une licence Demande

Tous les nouveaux utilisateurs et utilisatrices voient le même e-mail lorsqu’une invitation par e-mail est envoyée.

Pour plus d’informations sur la réception d’invitations par e-mail, voir [Recevoir des invitations par e-mail et créer un mot de passe pour Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Administrateur ou administratrice système</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Renvoyer des invitations par e-mail aux utilisateurs non enregistrés existants

Les invitations par e-mail sont générées dans les scénarios suivants :

* Lorsque vous créez un utilisateur ou une utilisatrice et que vous sélectionnez l’option **Envoyer un e-mail d’invitation à cette personne** sur le formulaire **Nouvel utilisateur ou nouvelle utilisatrice**. Pour plus d’informations sur la création d’utilisateurs et utilisatrices, voir [Ajouter des utilisateurs et des utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Lorsque vous importez plusieurs nouveaux utilisateurs et utilisatrices et que vous sélectionnez l’option **Envoyer des e-mails d’invitation à ces personnes**. Pour plus d’informations sur l’import de plusieurs nouveaux utilisateurs et utilisatrices, voir [Importer des utilisateurs et des utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Une fois les utilisateurs et utilisatrices créés, vous pouvez générer manuellement les invitations destinées aux utilisateurs et utilisatrices qui n’ont pas encore enregistré leur compte auprès de Workfront et qui n’ont pas encore défini de mot de passe Workfront.\
  Les utilisateurs et utilisatrices pour lesquels un compte a été créé mais n’ont pas encore enregistré leur compte sont marqués du statut **Non enregistré** dans Workfront.

  >[!NOTE]
  >
  >Si vous désélectionnez la case **Envoyer un e-mail d’invitation à cette personne** lorsque vous créez l’utilisateur ou l’utilisatrice, l’invitation par e-mail ne peut pas être générée manuellement. L’envoi manuel des invitations par e-mail n’est possible que pour les utilisateurs et utilisatrices qui ont reçu l’invitation par e-mail initiale lors de la création de leur compte. Pour plus d’informations sur la création de nouveaux utilisateurs et utilisatrices, voir [Ajouter des utilisateurs et des utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Pour renvoyer manuellement des invitations par e-mail à des utilisateurs non enregistrés existants :

{{step-1-to-users}}

1. Sélectionnez l’utilisateur ou l’utilisatrice dont le nom est suivi de l’étiquette **Non enregistré**.

   ![Non enregistré](assets/unreg-user-qs-350x221.png)

1. Cliquez sur l’icône Plus ![icône Plus](assets/more-icon.png), puis sur **Rappeler à l’utilisateur de s’enregistrer**.

   Une invitation par e-mail est envoyée à la nouvelle personne avec un nouveau lien qu’elle peut utiliser pour créer son mot de passe Workfront.

   >[!NOTE]
   >
   >Si votre entreprise a été intégrée à Admin Console et que vous ajoutez un utilisateur ou une utilisatrice via Workfront, vous n’avez pas la possibilité d’envoyer une invitation par e-mail à de nouveaux utilisateurs et utilisatrices.
   >
   >Les nouveaux utilisateurs et utilisatrices d’Adobe sont ajoutés à Admin Console et Admin Console leur envoie un e-mail pour les inviter à terminer le processus d’enregistrement. Tous les utilisateurs et utilisatrices doivent terminer le processus d’enregistrement pour accéder à n’importe quel système d’Adobe.
   >
   >Pour les utilisateurs et utilisatrices d’Adobe existants, l’utilisateur ou l’utilisatrice peut recevoir ou non un e-mail sur la disponibilité de Workfront. Il s’agit d’une préférence contrôlée par l’administrateur ou l’administratrice d’Adobe pour le produit.

## Configurer des invitations par e-mail {#configure-email-invitations}

En tant qu’administrateur ou administratrice Workfront, vous pouvez configurer le message que vous incluez avec les invitations par e-mail pour les nouveaux utilisateurs et utilisatrices.

{{step-1-to-setup}}

1. Dans la liste de gauche, cliquez sur **E-mail** > **Invitations**.

1. Dans la section **Options générales**, effectuez l’une des modifications suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Désactiver les liens d’invitation après ... jours</strong> </td> 
      <td> <p>Sélectionnez la durée au bout de laquelle les invitations par e-mail ne contiennent plus de lien valide vers Workfront. Le nombre de jours par défaut est 45.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Inclure un message et/ou une condition de service</strong> </td> 
      <td> <p>Sélectionnez cette option si vous souhaitez modifier l’invitation par e-mail pour tous les nouveaux utilisateurs et utilisatrices ajoutés à Workfront. Cela n’inclut pas les utilisateurs et utilisatrices disposant d’une licence Demande.</p> 
       <ul> 
        <li><strong>Message</strong> : si vous choisissez de modifier l’invitation par e-mail pour tous les nouveaux utilisateurs et utilisatrices, indiquez le texte que vous souhaitez inclure dans vos invitations par e-mail en tant que corps de l’e-mail.</li> 
        <li><strong>Conditions générales</strong> : si vous choisissez de modifier l’invitation par e-mail pour tous les nouveaux utilisateurs et utilisatrices, indiquez le texte que vous souhaitez inclure dans vos invitations par e-mail en tant que conditions générales.<br></li> 
        <li><strong>Inclure un message et/ou une condition de service pour les utilisateurs et utilisatrices de bureau d’aide</strong> : sélectionnez cette option si vous souhaitez modifier l’invitation par e-mail pour tous les nouveaux utilisateurs et utilisatrices ajoutés à Workfront qui disposent d’une licence Demande.</li> 
        <li><strong>Message</strong> : si vous choisissez de modifier l’invitation par e-mail pour tous les nouveaux utilisateurs et utilisatrices disposant d’une licence Demande, spécifiez le texte que vous souhaitez inclure dans vos invitations par e-mail en tant que corps de l’e-mail.</li> 
        <li><strong>Conditions générales</strong> : si vous choisissez de modifier l’invitation par e-mail pour tous les nouveaux utilisateurs et utilisatrices disposant d’une licence Demande, spécifiez le texte que vous souhaitez inclure dans vos invitations par e-mail comme conditions générales.<br></li> 
        <li> <p>Dans la section <strong>Prévisualisation Invitation</strong>, vous pouvez voir une prévisualisation de votre invitation par e-mail. Si vous avez choisi d’inclure un message personnalisé dans votre invitation par e-mail, le message personnalisé s’affiche dans cette zone.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.
