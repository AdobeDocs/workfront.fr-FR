---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Taguer des utilisateurs ou des utilisatrices pour partager une épreuve
description: Lorsque vous commentez une épreuve dans la visionneuse de relecture, vous pouvez taguer d’autres personnes pour attirer leur attention sur votre commentaire par e-mail et les ajouter au workflow de l’épreuve.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: fe269b088c82e7045ffbb5155d54432e0b413cbe
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 98%

---

# Taguer des utilisateurs ou des utilisatrices pour partager une épreuve

Lorsque vous commentez une épreuve dans la visionneuse de relecture, vous pouvez taguer d’autres personnes pour attirer leur attention sur votre commentaire par e-mail et les ajouter au workflow de l’épreuve.

Lorsque vous taguez des utilisateurs et utilisatrices dans des commentaires sur une épreuve, les personnes que vous pouvez baliser peuvent varier en fonction de divers facteurs, tels que les autorisations d’utilisation individuelles et votre appartenance à l’organisation :

* Si vous êtes la personne ayant créé ou détenant l’élément ou si vous disposez d’autorisations spécifiques, vous pouvez taguer les personnes en dehors du workflow d’épreuve et partager l’épreuve avec elles.
* Si votre nom a été ajouté à l’épreuve en tant qu’utilisateur ou utilisatrice externe et que vous êtes membre d’un autre environnement avec un compte d’épreuve différent, vous ne pouvez taguer que les personnes de votre environnement d’origine. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Conditions d’accès {#access-requirements}

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Tous</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Rôle de l’épreuve</td> 
   <td>Auteur ou autrice, ou modérateur ou modératrice</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve</td> 
   <td>Personne chargée de la supervision ou administrateur ou administratrice</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux documents</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Taguer des utilisateurs ou des utilisatrices pour partager une épreuve

Les personnes disposant du profil d’autorisation pour l’épreuve ou le rôle d’épreuve décrit dans la section [Conditions d’accès](#access-requirements) ci-dessus peuvent taguer des personnes pour partager une épreuve par défaut. Vous pouvez également taguer des personnes pour partager une épreuve, quel que soit le profil d’autorisation pour l’épreuve ou le rôle d’épreuve si vous êtes la personne propriétaire ou ayant créé l’épreuve. Vous pouvez permettre aux utilisateurs et utilisatrices disposant de profils d’autorisation pour l’épreuve ou de rôles d’épreuve inférieurs de taguer des personnes pour partager une épreuve lors de la création d’une épreuve. Pour plus d’informations, voir la section [Configurer le workflow et ajouter des réviseurs et réviseuses](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) dans l’article [Créer une épreuve avancée avec un workflow de base](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).

>[!NOTE]
>
>Vous ne pouvez taguer un collaborateur ou une collaboratrice externe à l’aide de son adresse e-mail que si l’une des conditions suivantes est vraie :>
>* Un utilisateur ou une utilisatrice du compte Workfront de votre entreprise a précédemment ajouté l’adresse e-mail du collaborateur ou de la collaboratrice à une épreuve.
>* Le collaborateur ou la collaboratrice a déjà utilisé l’adresse e-mail pour s’abonner à une épreuve dans le compte Workfront de votre entreprise.
>

Pour taguer quelqu’un et partager une épreuve dans un commentaire :

1. Lorsque vous commentez une épreuve, saisissez un signe @ suivi du nom ou de l’adresse e-mail de la personne. Lorsque vous commencez à saisir, les noms disponibles apparaissent dans une liste déroulante.
1. Sélectionnez le nom de la personne lorsque vous le voyez dans la liste déroulante.

   >[!TIP]
   >
   >Si vous souhaitez fermer la liste déroulante sans sélectionner personne, vous pouvez appuyer sur la touche **Échap** ou cliquer n’importe où en dehors de la liste.

1. Répétez les étapes 1 et 2 pour toutes les autres personnes que vous souhaitez taguer dans le commentaire.
1. Terminez le commentaire, puis cliquez sur **Publier**.
1. (Le cas échéant) Si vous avez tagué une personne qui n’a pas encore été ajoutée à l’épreuve, indiquez un **Rôle d’épreuve** et un paramètre **Alertes par e-mail** pour chaque personne répertoriée dans la zone qui s’affiche, puis cliquez sur **Ajouter des personnes et publier un commentaire**.

   ![Ajouter des personnes à l&#39;épreuve](assets/add-people-to-proof-350x220.png)

   Pour plus d’informations sur les rôles d’épreuve, voir . Pour plus d’informations sur les alertes par e-mail d’épreuve, consultez la section de l’article [Configurer les paramètres de notification par e-mail dans Workfront Proof](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Si l’épreuve comporte un workflow automatisé, les personnes que vous taguez sont ajoutées à l’étape dans laquelle vous vous trouvez. Pour plus d’informations, voir [Vue d’ensemble du workflow automatisé](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Toute personne que vous taguez reçoit un e-mail de notification à propos de votre commentaire sur l’épreuve, quels que soient les paramètres d’alerte par e-mail de l’épreuve qu’elle utilise :

   * Si la personne reçoit un e-mail de résumé quotidien ou horaire, Workfront envoie la notification séparément et inclut des informations sur votre commentaire d’épreuve dans l’e-mail de résumé.
   * Si la personne reçoit des alertes pour toute l’activité ou pour les réponses à ses commentaires, la notification remplace les notifications concernant ces commentaires et réponses.

Pour plus d’informations sur d’autres façons d’ajouter des personnes à une épreuve, voir [Partager une épreuve dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
