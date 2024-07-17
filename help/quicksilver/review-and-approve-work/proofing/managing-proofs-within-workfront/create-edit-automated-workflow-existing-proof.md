---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Créer ou modifier un workflow automatisé pour une épreuve existante
description: Les processus automatisés facilitent la gestion du processus de révision si votre processus est complexe ou si vous envoyez régulièrement du contenu à des fins de révision à des groupes de personnes identiques. Lorsque vous créez un BAT avec un workflow automatisé, le BAT passe de l’étape à l’étape jusqu’à l’approbation finale. Les participants sont avertis lorsque c’est à leur tour de réviser le document.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 8%

---

# Créer ou modifier un workflow automatisé pour une épreuve existante

Les processus automatisés facilitent la gestion du processus de révision si votre processus est complexe ou si vous envoyez régulièrement du contenu à des fins de révision à des groupes de personnes identiques. Lorsque vous créez un BAT avec un workflow automatisé, le BAT passe de l’étape à l’étape jusqu’à l’approbation finale. Les participants sont avertis lorsque c’est à leur tour de réviser le document.

Pour plus d’informations sur la création d’un workflow automatisé pour un nouveau BAT, voir [Création d’un BAT avancé avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

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

## Créez ou modifiez un workflow automatisé pour un BAT existant :

1. Passez la souris sur le document dans la zone Documents, puis cliquez sur Processus de vérification.

   Ou

   Si vous vérifiez le BAT dans la visionneuse de vérification, cliquez sur **Workflow** ![](assets/workflow-icon-proofing-viewer.png) dans le panneau de gauche, puis cliquez sur l’icône Modifier ![](assets/edit-icon-proofing-viewer.png) pour ouvrir les paramètres de workflow automatisé du BAT.

1. (Conditionnel) Si le BAT utilise actuellement un processus de base (sans étapes), cliquez sur **Convertir en processus automatisé** dans l’écran qui s’affiche.

   >[!NOTE]
   >
   >Vous ne pouvez pas modifier la première étape lorsque vous passez d’un workflow de base à un workflow automatisé, mais vous pouvez ajouter et configurer de nouvelles étapes.

1. Conditionnel) Pour utiliser un modèle de workflow automatisé créé et partagé avec vous par l’administrateur Adobe Workfront, cliquez sur **Ajouter un modèle**, sélectionnez le modèle dans la zone qui s’affiche, puis cliquez sur **Ajouter un modèle**.

   Pour plus d’informations, voir [À propos de l’utilisation des modèles de workflow automatisés](#about-using-automated-workflow-templates) dans cet article.

1. Ajoutez une étape au workflow automatisé :

   1. Cliquez sur **Nouvelle étape** près du coin supérieur droit.
   1. Dans la zone qui s’affiche, saisissez un **nom** pour l’étape.
   1. (Facultatif) Définissez une échéance pour la scène.
   1. Dans la section **Activer l’étape** , choisissez comment activer l’étape :


      <table>
      <tbody>
      <tr>
      <td><strong>Lors de la création du BAT</strong></td>
      <td>L'étape devient active automatiquement car le BAT a déjà été créé.</td>
      </tr>
      <tr>
      <td><strong>Lorsque l'étape précédente est arrivée à échéance</strong></td>
      <td>Cliquez sur l’étape précédente dans la liste déroulante <strong>Etape parente</strong> .</td>
      </tr>
      <tr>
      <td><strong>À une date et une heure spécifiques</strong></td>
      <td>Cliquez sur la zone <strong>On</strong> pour sélectionner la date, puis cliquez sur la zone située à droite pour sélectionner l’heure.</td>
      </tr>
      <tr>
      <td><strong>Toutes les décisions sont approuvées ou approuvées avec des modifications sur l’étape parent</strong></td>
      <td>Cliquez sur la scène parente dans la liste déroulante <strong>Etape parente</strong> .</td>
      </tr>
      <tr>
      <td><strong>Toutes les décisions sont approuvées sur l’étape parent</strong></td>
      <td>Cliquez sur la scène parente dans la liste déroulante <strong>Etape parente</strong> .</td>
      </tr>
      <tr>
      <td><strong>Toutes les décisions sont prises</strong></td>
      <td>Cliquez sur la scène parente dans la liste déroulante <strong>Etape parente</strong> .</td>
      </tr>
      </tbody>
      </table>


   1. Saisissez le nom du contact ou l&#39;adresse email, puis configurez les paramètres pour les réviseurs de l&#39;étape.

      Pour plus d’informations sur l’ajout de réviseurs, voir [À propos de l’ajout de réviseurs à une étape](#about-adding-reviewers-to-a-stage) dans cet article.

   1. Utilisez l’une des options suivantes pour configurer davantage l’étape :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong> Options de date limite</strong> </td>
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
         <td role="rowheader">Décisionnaire principal</td>
         <td><p>Sélectionnez le décideur de Principal sur l’étape (disponible uniquement après avoir ajouté au moins une personne à l’étape qui dispose du rôle Bon à tirer d’approbateur ou d’un rôle d’approbateur supérieur). Si vous sélectionnez un décideur de Principal, l’option <strong>Une seule décision requise</strong> est désactivée à cette étape.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Une seule décision requise</td>
         <td>Met fin à l’ensemble du processus de révision lorsque l’un des décideurs prend une décision.<p>Cette option n’est pas disponible si vous avez désigné un utilisateur dans le menu déroulant <strong>Décideur de Principal</strong> .</p></td>
        </tr>
        <tr>
         <td role="rowheader">Etape privée</td>
         <td>Permet uniquement aux personnes suivantes d’afficher les commentaires et les décisions pris à cette étape : superviseurs, administrateurs Adobe Workfront et administrateurs Workfront Proof</td>
        </tr>
        <tr>
         <td role="rowheader">Notifier les personnes par e-mail</td>
         <td>Alerte les réviseurs avec une notification par email lorsqu'ils se chargent de l'exécution du BAT.</td>
        </tr>
       </tbody>
      </table>

   1. Cliquez sur **Ajouter une étape**.

1. Répétez l’étape précédente si nécessaire pour ajouter d’autres étapes.

   Lorsque vous ajoutez des étapes au processus automatisé, un diagramme s’affiche à l’écran pour les représenter :

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Lorsque vous avez terminé d’ajouter des scènes, cliquez sur **Terminé**.

## À propos de l’utilisation des modèles de processus automatisés {#about-using-automated-workflow-templates}

Tenez compte des points suivants lorsque vous utilisez un modèle de workflow automatisé :

1. Les paramètres d’un modèle de workflow automatisé déterminent ce que vous pouvez faire avec le workflow automatisé pour un BAT. Par exemple, si le bouton Ajouter une scène est désactivé dans le modèle, il n’est pas visible car vous travaillez avec les paramètres de workflow automatisé du BAT.
1. Lorsqu’une personne est ajoutée à un niveau dans un modèle de workflow automatisé, mais également déjà présente en tant que validant sur le BAT, l’application du modèle supprime le validant de l’étape. Si vous n’ajoutez pas d’autre réviseur à l’étape, un message vous invite à en ajouter un.
1. Votre capacité à modifier un modèle de workflow automatisé dépend des paramètres de modèle configurés par l’administrateur de Workfront, comme décrit dans la section . Si la possibilité de modifier le modèle est désactivée, seul le propriétaire du modèle peut le modifier.

## A propos de l’ajout de réviseurs à une étape {#about-adding-reviewers-to-a-stage}

Tenez compte des points suivants lors de l’ajout de réviseurs à une étape :

* Une fois que vous avez ajouté un utilisateur à une étape, vous pouvez configurer les paramètres de cet utilisateur sur le BAT, tels que le rôle du BAT et les autorisations supplémentaires qu’il doit posséder, ainsi que le type d’alertes par e-mail qu’il recevra lorsque des personnes auront commenté et pris des décisions sur le BAT.
* Vous pouvez faire glisser un ou plusieurs utilisateurs d’une étape vers une autre. Vous pouvez faire glisser les utilisateurs directement vers une autre étape ou faire glisser les utilisateurs vers une étape sur le diagramme **Étapes**. Pour sélectionner plusieurs utilisateurs, appuyez sur Maj+Ctrl (sous Windows) ou Maj+Commande (sous Mac).
* Vous ne pouvez ajouter un validant qu&#39;une seule fois à un BAT, ce qui signifie que vous ne pouvez pas ajouter la même personne à plusieurs étapes du BAT.
* Les réviseurs qui ne sont pas ajoutés à une scène privée ne peuvent pas voir cette scène sur le BAT ou les commentaires faits à cette étape.
* Par défaut, l’ajout d’un utilisateur à un environnement intermédiaire lui donne accès pour afficher le BAT à partir du moment où le BAT est créé.

  Votre administrateur Workfront peut empêcher les utilisateurs d’accéder au BAT jusqu’à ce que le workflow entre dans l’étape où l’utilisateur a été ajouté. Pour plus d’informations, voir  dans .
