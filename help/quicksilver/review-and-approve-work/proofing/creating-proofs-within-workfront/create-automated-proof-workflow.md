---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve avancée avec un workflow automatisé
description: Un processus automatisé facilite la gestion du processus de révision si votre processus est complexe ou si vous envoyez régulièrement du contenu à des personnes identiques pour révision. Le BAT passe d’une étape à l’autre et Adobe Workfront avertit chaque utilisateur lorsqu’il est à son tour de le vérifier. Pour plus d’informations sur les workflows automatisés, voir Présentation des workflows automatisés.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 4%

---

# Créer une épreuve avancée avec un workflow automatisé

<!-- Audited: 2/2024 -->

Un processus automatisé facilite la gestion du processus de révision si votre processus est complexe ou si vous envoyez régulièrement du contenu à des personnes identiques pour révision. Le BAT passe d’une étape à l’autre et Adobe Workfront avertit chaque utilisateur lorsqu’il est à son tour de le vérifier. Pour plus d’informations sur les workflows automatisés, voir [Présentation des workflows automatisés](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>Nouveau : Tous</p><p>Formule actuelle : Pro ou supérieure</p><p>Formule héritée : sélection ou supérieure</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouvelle : standard</p><p>Plan actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès en modification aux documents</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une épreuve avancée avec un workflow automatisé

1. Accédez au projet, à la tâche ou à l’emplacement où vous souhaitez obtenir le BAT, puis cliquez sur l’onglet **Documents** .
1. Cliquez sur **Ajouter un nouvel** > Bon à tirer, téléchargez le contenu, puis parcourez les sections répertoriées ci-dessous.

   ou

   Passez la souris sur un document existant, puis cliquez sur **Créer un bon à tirer** > **BAT avancé** et parcourez les sections répertoriées ci-dessous.

## Configuration des étapes du BAT

1. Dans la section Type de workflow , sélectionnez **Automated**.
1. (Facultatif) Si vous souhaitez utiliser un modèle de workflow automatisé créé et partagé avec vous par votre administrateur Workfront, cliquez sur **Ajouter un modèle**, sélectionnez le modèle dans la zone qui s’affiche, puis cliquez sur **Ajouter un modèle**.

   >[!NOTE]
   >
   >Tenez compte des points suivants lorsque vous utilisez un modèle de workflow automatisé :
   >   
   >* Les paramètres d’un modèle de workflow automatisé déterminent ce que vous pouvez faire avec le workflow automatisé pour un BAT. Par exemple, si le bouton Ajouter une scène est désactivé dans le modèle, il n’est pas visible car vous travaillez avec les paramètres de workflow automatisé du BAT.
   >* Lorsqu’une personne est ajoutée à un niveau dans un modèle de workflow automatisé, mais également déjà présente en tant que validant sur le BAT, l’application du modèle supprime le validant de l’étape. Si vous n’ajoutez pas d’autre réviseur à l’étape, un message vous invite à en ajouter un.
   >* Votre capacité à modifier un modèle de workflow automatisé dépend des paramètres de modèle configurés par l’administrateur de Workfront, comme décrit dans la section . Si la possibilité de modifier le modèle est désactivée, seul le propriétaire du modèle peut le modifier.

1. Configurez la première étape du processus automatisé :

   1. (Facultatif) Si vous souhaitez créer un nom pour la première étape, cliquez sur **Stage 1**, puis saisissez le nom.
   1. Dans la section **Destinataires** de l’étape, ajoutez les réviseurs à l’étape.

      >[!NOTE]
      >
      >Tenez compte des points suivants lors de l’ajout de réviseurs à une étape :
      >   
      >* Vous pouvez ajouter des utilisateurs externes à une étape avec une adresse électronique.
      >* Après avoir ajouté un utilisateur à une étape, vous pouvez configurer les paramètres de cet utilisateur sur le BAT.
      >* Vous pouvez faire glisser les utilisateurs directement vers une autre étape ou faire glisser les utilisateurs vers une étape sur le diagramme **Étapes**. Pour sélectionner plusieurs utilisateurs, appuyez sur Maj+Ctrl (sous Windows) ou Maj+Commande (sous Mac).
      >* Vous ne pouvez ajouter un validant qu&#39;une seule fois à un BAT, ce qui signifie que vous ne pouvez pas ajouter la même personne à plusieurs étapes du BAT.
      >* Les réviseurs qui ne sont pas ajoutés à une scène privée ne peuvent pas voir cette scène sur le BAT ou les commentaires faits à cette étape.
      >* Par défaut, l’ajout d’un utilisateur à un environnement intermédiaire lui donne accès pour afficher le BAT à partir du moment où le BAT est créé. Votre administrateur Workfront peut empêcher les utilisateurs d’accéder au BAT jusqu’à ce que le workflow entre dans l’étape où l’utilisateur a été ajouté.

   1. Cliquez sur **Paramètres d’évaluation**.
   1. Cliquez sur une option **Activer l’étape** pour indiquer comment activer l’étape.

      Pour la première étape, vous pouvez sélectionner uniquement **Lors de la création du BAT**, **À une date et une heure spécifiques** ou **Manuellement**.

   1. (Conditionnel) Si vous avez sélectionné **À une date et une heure spécifiques** à l’étape précédente, sélectionnez la date et l’heure d’activation de la scène dans la zone **Activer sur** qui s’affiche.

   1. Utilisez l’une des options ci-dessous pour configurer davantage l’étape.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Définir la date limite d’évaluation</td>
         <td><p>Pour définir une échéance pour l’étape, cliquez sur une option dans la liste déroulante <strong>Options de date</strong>. Ensuite, sous <strong>Deadline</strong>, effectuez l’une des opérations suivantes :</p>
          <ul>
           <li>Si vous choisissez <strong>Définir la date spécifique</strong> : sélectionnez la date d'échéance et l'heure de votre choix.</li>
           <li>Si vous choisissez <strong>Calculer à partir de la date d’activation de l’étape</strong> : sélectionnez le nombre de jours ouvrés à ajouter à la date d’activation de l’étape pour déterminer l’échéance.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Verrouiller l’étape</td>
         <td>Spécifiez quand la scène peut être verrouillée. </td>
        </tr>
        <tr>
         <td role="rowheader">Transférer les droits de décision principaux vers</td>
         <td><p>Sélectionnez le décideur de Principal sur l’étape (disponible uniquement après avoir ajouté au moins une personne à l’étape qui dispose du rôle Bon à tirer d’approbateur ou d’un rôle d’approbateur supérieur). Si vous sélectionnez un décideur de Principal, l’option <strong>Une seule décision requise</strong> est désactivée à cette étape.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Exiger une seule décision pour cette étape</td>
         <td>Met fin à l’ensemble du processus de révision lorsque l’un des décideurs prend une décision.<p>Cette option n’est pas disponible si vous avez désigné un utilisateur dans le menu déroulant <strong>Décideur de Principal</strong> .</p></td>
        </tr>
        <tr>
         <td role="rowheader">Rendre cette étape privée</td>
         <td>Permet uniquement aux personnes suivantes d’afficher les commentaires et les décisions pris à cette étape : superviseurs, administrateurs Workfront et administrateurs Workfront Proof</td>
        </tr>
       </tbody>
      </table>

1. Pour ajouter et configurer une autre étape :

   1. Cliquez sur **Nouvelle étape**.
   1. (Facultatif) Si vous souhaitez créer un nom pour la première étape, cliquez sur **Stage 2** (ou **Stage 3**, **Stage 4**, etc.), puis saisissez le nom.

   1. Cliquez sur **Activer l’étape**, puis sélectionnez une option pour indiquer si l’étape est activée automatiquement ou manuellement.

      Outre les options **Lors de la création du BAT**, **À une date et une heure spécifiques** ou **Manuellement**, vous pouvez sélectionner une option qui dépend de ce qui s’est produit à l’étape précédente :

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Si vous avez sélectionné une option Activer l’étape qui dépend de ce qui s’est passé à l’étape précédente, utilisez les options qui s’affichent pour configurer le paramètre d’activation.

      Par exemple, si vous avez sélectionné **Lorsque l’état de l’étape précédente change**, sélectionnez l’état **Étape précédente**, puis sélectionnez l’état dans la zone **État modifié en**.

1. Répétez l’étape précédente si nécessaire pour ajouter d’autres étapes.

   Lorsque vous ajoutez des étapes au processus automatisé, un diagramme s’affiche à l’écran pour les représenter :

   ![](assets/stages-diagram-350x213.png)

1. Poursuivez avec [Configurez les paramètres de courrier électronique pour le BAT](#configure-email-settings-for-the-proof) ci-dessous.

## Configuration des paramètres de courrier électronique pour le BAT {#configure-email-settings-for-the-proof}

1. Dans la section **Notification par e-mail** , choisissez d&#39;envoyer des notifications par e-mail et un message personnalisé aux utilisateurs que vous avez sélectionnés dans [Créer un BAT avancé avec un workflow automatisé](#workflow) plus tôt dans cet article :

   <table>
      <tbody>
      <tr>
      <td>Informer les destinataires de ce BAT</td>
      <td>Sélectionnez cette option pour envoyer une notification électronique aux utilisateurs. Lorsque l'option <strong>Partage de base</strong> est sélectionnée dans la section <strong>Workflow</strong>, une notification par e-mail est envoyée lors de la création du BAT. Lorsque <strong>Workflow automatisé</strong> est sélectionné dans la section <strong>Workflow</strong>, une notification par e-mail est envoyée lorsque le BAT entre dans l’étape du workflow automatisé auquel l’utilisateur est associé.</td>
      </tr>
      <tr>
      <td>Ajout d’un message personnalisé</td>
      <td>Sélectionnez cette option pour inclure un message personnalisé dans la notification. Vous pouvez spécifier un objet et un corps de message. Le corps du message peut inclure une mise en forme en texte enrichi (gras, puces et liens hypertexte).</td>
      </tr>
      </tbody>
      </table>


1. Passez à [Configuration des paramètres du BAT](#configure-proof-settings) ci-dessous.

## Configuration des paramètres du BAT {#configure-proof-settings}

1. Dans la section **Paramètres de BAT**, sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Connexion requise : le BAT ne peut être partagé qu’avec d’autres utilisateurs.</td> 
      <td>Lorsque cette option est désactivée (par défaut), toute personne disposant de l’URL peut afficher le BAT. <br>Lorsque cette option est sélectionnée :
       <ul>
        <li>Seuls les utilisateurs de Workfront Proof peuvent afficher le BAT.</li>
        <li>Les utilisateurs ne peuvent pas se connecter au BAT à moins qu’ils n’aient été ajoutés au BAT.</li>
        <li>Les abonnements ne peuvent pas être activés.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Une seule décision requise pour ce BAT</td> 
      <td>Lorsque cette option est sélectionnée, la révision est terminée une fois que l’un des décideurs a pris sa décision.<br>Cette option est désactivée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger que les décisions soient signées de manière électronique</td> 
      <td>Les utilisateurs doivent indiquer leur nom d’utilisateur et leur mot de passe au moment où ils prennent une décision sur un BAT.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller le BAT lorsque toutes les décisions requises sont prises</td> 
      <td>Lorsque ce paramètre est activé, l’état du BAT est verrouillé une fois toutes les décisions prises. L’état est automatiquement modifié du déverrouillé au verrouillé lorsque l’approbateur final prend sa décision.<br>Cette option est désactivée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Télécharger le fichier d’origine</td> 
      <td>Lorsque cette option est sélectionnée, les réviseurs peuvent télécharger le fichier d'origine à partir duquel le BAT a été créé.<br>Lorsque cette option est désélectionnée, l’icône Télécharger n’est plus visible.<br>Cette option est activée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partage du BAT via une URL publique ou un code intégré</td> 
      <td>Lorsque cette option est sélectionnée, le BAT peut être partagé via une URL publique ou un code intégré.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abonnez-vous au BAT via une URL publique ou un code intégré</td> 
      <td>Lorsque cette option est sélectionnée, les personnes qui n’ont pas été explicitement ajoutées au BAT peuvent s’abonner au BAT. La personne qui s'abonne au BAT se voit attribuer le rôle et l'email que vous définissez dans les paramètres suivants :
       <ul>
        <li><strong>Rôle d’abonné : </strong> rôle de BAT par défaut attribué à tous les réviseurs qui souscrivent au BAT.</li>
        <li><strong>Paramètres des alertes par email pour les abonnés :</strong> L’alerte par défaut qui est attribuée à tous les réviseurs qui souscrivent au BAT.</li>
       </ul><p>
        <ul>
         <li><strong>L'accès au BAT par le biais d'un lien d'email est requis pour :</strong> Configurez si l'abonné reçoit un email avec un lien vers le BAT. Vous pouvez sélectionner <strong>Aucun email</strong> (aucun lien d'email n'est nécessaire pour accéder au BAT), <strong>Email de notification de BAT uniquement</strong> (l'abonné reçoit un lien vers le BAT par email sans vérification) ou <strong>Email de validation et de notification de BAT</strong> (l'abonné reçoit un lien vers le BAT par email et doit cliquer sur le lien pour accéder à un BAT, l'option permettant de s'assurer que la personne que l'adresse email indiquée dans un email adresse à laquelle ils ont accès).</li>
        </ul><p><strong>Remarque : </strong> Si le workflow automatisé joint tous les abonnements, les propriétaires de BAT reçoivent des emails de confirmation, afin qu’ils puissent décider à quelle étape la personne doit être ajoutée.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Créer un bon à tirer**.

   Workfront commence à générer un bon à tirer des documents ou des sites Web sélectionnés. Selon la taille et le type du fichier, le délai de téléchargement d’un document peut varier. Soyez patient car la génération de fichiers plus volumineux prend plus de temps. Vous pouvez quitter la page et Workfront continue à générer votre fichier. La taille maximale du téléchargement de fichier est de 4 Go.

1. Une fois le BAT généré, cliquez sur **Ouvrir le BAT** pour lancer la visionneuse de BAT.

   ![](assets/open-proof-350x132.png)

   Les utilisateurs pour lesquels la vérification n’est pas activée sur leur compte peuvent toujours afficher le document et envoyer des commentaires au BAT [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
