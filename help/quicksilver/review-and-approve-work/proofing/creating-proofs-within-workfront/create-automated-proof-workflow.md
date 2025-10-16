---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve avancée avec un workflow automatisé
description: Un workflow automatisé facilite la gestion du processus de révision si votre processus est complexe ou si vous envoyez régulièrement du contenu aux mêmes personnes pour révision. L’épreuve passe d’une étape à l’autre et Adobe Workfront avertit tour à tour les utilisateurs et utilisatrices lorsqu’ils doivent effectuer la révision. Pour plus d’informations sur les workflows automatisés, voir Vue d’ensemble des workflows automatisés.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1783'
ht-degree: 99%

---

# Créer une épreuve avancée avec un workflow automatisé

<!-- Audited: 2/2024 -->

Un workflow automatisé facilite la gestion du processus de révision si votre processus est complexe ou si vous envoyez régulièrement du contenu aux mêmes personnes pour révision. L’épreuve passe d’une étape à l’autre et Adobe Workfront avertit tour à tour les utilisateurs et utilisatrices lorsqu’ils doivent effectuer la révision. Pour plus d’informations sur les workflows automatisés, voir [Vue d’ensemble des workflows automatisés](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> Standard</p>
   <p>Travail ou plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux documents</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une épreuve avancée avec un workflow automatisé

1. Accédez à l’élément (projet, tâche ou problème) pour lequel vous souhaitez obtenir l’épreuve, puis cliquez sur l’onglet **Documents**.
1. Cliquez sur **Ajouter** > Épreuve, chargez le contenu, puis parcourez les sections répertoriées ci-dessous.

   ou

   Pointez sur un document existant, puis cliquez sur **Créer une épreuve** > **Épreuve avancée** et parcourez les sections répertoriées ci-dessous.

## Configurer les étapes de l’épreuve

1. Dans la section Type de workflow, choisissez **Automatisé**.
1. (Facultatif) Si vous souhaitez utiliser un modèle de workflow automatisé créé et partagé avec vous par l’équipe d’administration Workfront, cliquez sur **Ajouter un modèle**, sélectionnez le modèle dans la zone qui s’affiche, puis cliquez sur **Ajouter un modèle**.

   >[!NOTE]
   >
   >Tenez compte des points suivants lorsque vous utilisez un modèle de workflow automatisé :
   >   
   >* Les paramètres d’un modèle de workflow automatisé déterminent ce que vous pouvez faire avec le workflow automatisé pour une épreuve. Par exemple, si le bouton Ajouter une étape est désactivé dans le modèle, il n’est pas visible lorsque vous travaillez avec les paramètres de workflow automatisé de l’épreuve.
   >* Lorsqu’une personne est ajoutée à une étape dans un modèle de workflow automatisé, mais qu’elle est déjà présente en tant que réviseur ou réviseuse sur l’épreuve, l’application du modèle supprime le réviseur ou la réviseuse de l’étape. Si vous n’ajoutez pas d’autre réviseur ou réviseuse à l’étape, un message vous invite à le faire.
   >* Votre capacité à modifier un modèle de workflow automatisé dépend des paramètres de modèle configurés par l’équipe d’administration Workfront, comme décrit dans . Si la possibilité de modifier le modèle est désactivée, seule la personne propriétaire du modèle peut le modifier.

1. Configurez la première étape du workflow automatisé :

   1. (Facultatif) Pour donner un nom à la première étape, cliquez sur **Étape 1**, puis saisissez le nom.
   1. Dans la section **Personne destinataires** de l’étape, ajoutez les réviseurs et réviseuses.

      >[!NOTE]
      >
      >Tenez compte des points suivants lorsque vous ajoutez des réviseurs et réviseuses à une étape :
      >   
      >* Vous pouvez ajouter des utilisateurs et utilisatrices externes à une étape avec une adresse e-mail.
      >* Après avoir ajouté un utilisateur ou une utilisatrice à une étape, vous pouvez configurer ses paramètres sur l’épreuve.
      >* Vous pouvez faire glisser les utilisateurs et utilisatrices directement vers une autre étape, ou les faire glisser vers une étape du diagramme **Étapes**. Pour sélectionner plusieurs utilisateurs et utilisatrices, appuyez sur Maj+Ctrl (sous Windows) ou Maj+Commande (sous Mac).
      >* Vous ne pouvez ajouter un utilisateur ou une utilisatrice qu’une seule fois à une épreuve, ce qui signifie que vous ne pouvez pas ajouter la même personne à plusieurs étapes de l’épreuve.
      >* Les réviseurs et réviseuses qui ne sont pas ajoutés à une étape privée ne peuvent pas voir cette étape sur l’épreuve ou les commentaires faits à cette étape.
      >* Par défaut, l’ajout d’un utilisateur ou d’une utilisatrice à une étape lui donne accès pour afficher l’épreuve à partir du moment où l’épreuve est créée. Votre équipe d’administration Workfront peut empêcher les utilisateurs et utilisatrices d’accéder à l’épreuve jusqu’à ce que le workflow entre dans l’étape où sont ajoutés les utilisateurs et utilisatrices.

   1. Cliquez sur **Paramètres de l’étape**.
   1. Cliquez sur une option **Activer l’étape** pour indiquer le mode d’activation de l’étape.

      Pour la première étape, vous ne pouvez sélectionner que **Lors de la création de l’épreuve**, **À une date et une heure spécifiques**, ou **Manuellement**.

   1. (Le cas échéant) Si vous avez sélectionné **À une date et une heure spécifiques** à l’étape précédente, sélectionnez la date et l’heure d’activation de l’étape dans la zone **Activer le** qui s’affiche.

   1. Utilisez l’une des options suivantes pour continuer à configurer l’étape.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Définir une date d’échéance pour l’étape</td>
         <td><p>Pour définir une date d’échéance pour l’étape, cliquez sur une option dans la liste déroulante <strong>Options de date d’échéance</strong>. Ensuite, sous <strong>Date d’échéance</strong>, effectuez l’une des opérations suivantes :</p>
          <ul>
           <li>Si vous choisissez <strong>Définir la date spécifique</strong> : sélectionnez la date et l’heure d’échéance de votre choix.</li>
           <li>Si vous choisissez <strong>Calculer à partir de la date d’activation de l’étape</strong> : sélectionnez le nombre de jours ouvrés à ajouter à la date d’activation de l’étape pour déterminer l’échéance.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Verrouiller l’étape</td>
         <td>Spécifiez quand l’étape peut être verrouillée. </td>
        </tr>
        <tr>
         <td role="rowheader">Transférer les droits de décision principaux vers</td>
         <td><p>Sélectionnez la personne décisionnaire principale sur l’étape (disponible uniquement après avoir ajouté au moins une personne à l’étape qui dispose du rôle d’épreuve approbateur ou approbatrice ou d’un rôle de niveau supérieur). Si vous sélectionnez une personne décisionnaire principale, l’option <strong>Une seule décision requise</strong> est désactivée sur cette étape.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Exiger une seule décision pour cette étape</td>
         <td>Met fin à l’ensemble du processus de révision lorsque l’une des personnes décisionnaires prend une décision.<p>Cette option n’est pas disponible si vous avez désigné un utilisateur ou une utilisatrice dans le menu déroulant <strong>Personne décisionnaire principale</strong>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Rendre cette étape privée</td>
         <td>Permet uniquement aux personnes suivantes d’afficher les commentaires et les décisions relatifs à cette étape : superviseurs et superviseuses, administrateurs et administratrices Workfront et administrateurs et administratrices Workfront Proof.</td>
        </tr>
       </tbody>
      </table>

1. Pour ajouter et configurer une autre étape, procédez comme suit :

   1. Cliquez sur **Nouvelle étape**.
   1. (Facultatif) Pour créer un nom pour la première étape, cliquez sur **Étape 2** (ou **Étape 3**, **Étape 4**, etc.), puis saisissez le nom.

   1. Cliquez sur **Activer l’étape**, puis sélectionnez une option pour spécifier si l’étape est activée automatiquement ou manuellement.

      En plus des options **Lors de la création de l’épreuve**, **À une date et une heure spécifiques**, ou **Manuellement**, vous pouvez sélectionner une option qui dépend de ce qui s’est passé à l’étape précédente :

      ![Activer les options d’étape](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Si vous avez sélectionné une option Activer l’étape qui dépend de ce qui s’est passé à l’étape précédente, utilisez les options qui s’affichent pour configurer le paramètre d’activation.

      Par exemple, si vous avez sélectionné **Lorsque le statut de l’étape précédente change**, sélectionnez l’**étape précédente**, puis sélectionnez le statut dans la zone **Statut modifié à**.

1. Répétez l’étape précédente si nécessaire pour ajouter d’autres étapes.

   Lorsque vous ajoutez des étapes au processus automatisé, un diagramme s’affiche à l’écran pour les représenter :

   ![diagramme Étapes](assets/stages-diagram-350x213.png)

1. Passez à [Configurer les paramètres d’e-mail pour l’épreuve](#configure-email-settings-for-the-proof) ci-dessous.

## Configurer les paramètres d’e-mail de l’épreuve {#configure-email-settings-for-the-proof}

1. Dans la section **Notification par e-mail**, choisissez d’envoyer des notifications par e-mail et un message personnalisé aux utilisateurs et utilisatrices que vous avez sélectionnés dans [Créer une épreuve avancée avec un workflow automatisé](#workflow) plus tôt dans cet article :

   <table>
      <tbody>
      <tr>
      <td>Informer les personnes destinataires de l’épreuve</td>
      <td>Sélectionnez cette option pour envoyer une notification par e-mail aux utilisateurs et utilisatrices. Lorsque <strong>Partage de base</strong> est sélectionné dans la section <strong>Workflow</strong>, une notification par e-mail est envoyée lors de la création de l’épreuve. Lorsque <strong>Workflow automatisé</strong> est sélectionné dans la section <strong>Workflow</strong>, une notification par e-mail est envoyée lorsque l’épreuve entre dans l’étape du workflow automatisé auquel la personne est associée.</td>
      </tr>
      <tr>
      <td>Ajouter un message personnalisé</td>
      <td>Sélectionnez cette option pour inclure un message personnalisé dans la notification. Vous pouvez spécifier un objet et un corps de message. Le corps du message peut inclure une mise en forme en texte enrichi (gras, puces et liens hypertexte).</td>
      </tr>
      </tbody>
      </table>


1. Passez à [Configurer les paramètres de l’épreuve](#configure-proof-settings) ci-dessous.

## Configurer les paramètres de l’épreuve {#configure-proof-settings}

1. Dans la section **Paramètres de l’épreuve**, sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Connexion requise : l’épreuve ne peut être partagée qu’avec d’autres utilisateurs et utilisatrices.</td> 
      <td>Lorsque cette option est désactivée (par défaut), toute personne disposant de l’URL peut afficher l’épreuve. <br>Lorsque cette option est sélectionnée, ce qui suit s’applique :
       <ul>
        <li>L’épreuve n’est accessible qu’aux utilisateurs et utilisatrices pouvant afficher l’épreuve.</li>
        <li>Les utilisateurs et utilisatrices ne peuvent pas se connecter à l’épreuve à moins qu’ils n’aient été ajoutés à l’épreuve.</li>
        <li>Les abonnements ne peuvent pas être activés.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Une seule décision requise pour cette épreuve</td> 
      <td>Lorsque cette option est sélectionnée, la révision est terminée une fois que l’une des personnes décisionnaires a pris sa décision.<br>Cette option est désactivée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger que les décisions soient signées de manière électronique</td> 
      <td>Les utilisateurs et utilisatrices doivent indiquer leur nom d’utilisateur ou d’utilisatrice et leur mot de passe au moment où ils prennent une décision sur une épreuve.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’épreuve lorsque toutes les décisions requises sont prises.</td> 
      <td>Lorsque ce paramètre est activé, l’état de l’épreuve est verrouillé une fois toutes les décisions prises. L’état passe automatiquement de déverrouillé à verrouillé lorsque la dernière personne chargée de l’approbation prend sa décision.<br>Cette option est désactivée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Télécharger le fichier original</td> 
      <td>Lorsque cette option est sélectionnée, les réviseurs et réviseuses peuvent télécharger le fichier original à partir duquel l’épreuve a été créée.<br>Si cette option est désélectionnée, l’icône Télécharger n’est plus visible.<br>Cette option est activée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partager l’épreuve via une URL publique ou un code intégré</td> 
      <td>Lorsque cette option est sélectionnée, l’épreuve peut être partagée via une URL publique ou un code intégré.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">S’abonner à l’épreuve via une URL publique ou un code intégré</td> 
      <td>Lorsque cette option est sélectionnée, les personnes qui n’ont pas été explicitement ajoutées à l’épreuve peuvent s’y abonner. La personne qui s’abonne à l’épreuve se voit attribuer le rôle et l’adresse e-mail que vous définissez dans les paramètres suivants :
       <ul>
        <li><strong>Rôle de personne abonnée :</strong> rôle d’épreuve par défaut attribué à tous les réviseurs et toutes les réviseuses qui s’abonnent à l’épreuve.</li>
        <li><strong>Paramètres des alertes par e-mail pour les personnes abonnées :</strong> alerte par e-mail par défaut attribuée à tous les réviseurs et toutes les réviseuses qui s’abonnent à l’épreuve.</li>
       </ul><p>
        <ul>
         <li><strong>Accès à l’épreuve via un lien par e-mail requis pour :</strong> indiquez si la personne abonnée reçoit un e-mail avec un lien vers l’épreuve. Vous pouvez sélectionner <strong>Aucun e-mail</strong> (aucun lien d’e-mail n’est nécessaire pour accéder à l’épreuve), <strong>E-mail de notification d’épreuve uniquement</strong> (la personne abonnée reçoit un lien vers l’épreuve par e-mail sans vérification), ou <strong>E-mails de validation et de notification d’épreuve</strong> (la personne abonnée reçoit un lien vers l’épreuve par e-mail et doit cliquer sur le lien pour y accéder ; l’objectif de cette option est de s’assurer que la personne a saisi une adresse e-mail correcte à laquelle elle a accès).</li>
        </ul><p><strong>Note :</strong> si le workflow automatisé est joint aux épreuves, tous les abonnements génèrent des e-mails de confirmation pour les personnes propriétaires de l’épreuve, afin qu’elles puissent décider à quelle étape la personne doit être ajoutée.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Créer une épreuve**.

   Workfront commence à générer une épreuve des documents ou des sites web sélectionnés. Selon la taille et le type du fichier, le délai de chargement d’un document peut varier. Faites preuve de patience, car la génération de fichiers volumineux prend plus de temps. Vous pouvez quitter la page. Workfront continue à générer votre fichier. La taille maximale du chargement de fichier est de 4 Go.

1. Une fois l’épreuve générée, cliquez sur **Ouvrir l’épreuve** pour lancer la visionneuse de relecture.

   ![Ouvrir l&#39;épreuve](assets/open-proof-350x132.png)

   Les utilisateurs et utilisatrices qui n’ont pas la vérification activée sur leur compte peuvent toujours consulter le document et envoyer des commentaires à l’épreuve[.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
