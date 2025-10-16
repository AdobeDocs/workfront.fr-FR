---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Créer ou modifier un workflow automatisé pour une épreuve existante
description: Les workflows automatisés facilitent la gestion du processus de révision si votre processus est complexe ou si vous envoyez régulièrement du contenu pour révision aux mêmes groupes de personnes. Lorsque vous créez une épreuve avec un workflow automatisé, l’épreuve passe d’une étape à l’autre jusqu’à l’approbation finale. Les personnes participantes sont averties lorsque c’est à leur tour de réviser le document.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 96%

---

# Créer ou modifier un workflow automatisé pour une épreuve existante

Les workflows automatisés facilitent la gestion du processus de révision si votre processus est complexe ou si vous envoyez régulièrement du contenu pour révision aux mêmes groupes de personnes.Lorsque vous créez une épreuve avec un workflow automatisé, l’épreuve passe d’une étape à l’autre jusqu’à l’approbation finale. Les personnes participantes sont averties lorsque c’est à leur tour de réviser le document.

Pour plus d’informations sur la création d’un workflow automatisé pour une nouvelle épreuve, voir [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Travail ou plan</p>
   </td> 
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

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créez ou modifiez un workflow automatisé pour une épreuve existante :

1. Passez la souris sur le document dans la zone Documents, puis cliquez sur Workflow de relecture.

   Ou

   Si vous consultez le BAT dans la visionneuse de BAT, cliquez sur **Workflow** ![icône de workflow](assets/workflow-icon-proofing-viewer.png) dans le panneau de gauche, puis cliquez sur l’icône Modifier ![icône Modifier](assets/edit-icon-proofing-viewer.png) pour ouvrir les paramètres de Workflow automatisé pour le BAT.

1. (Le cas échéant) Si l’épreuve utilise actuellement un workflow de base (sans étapes), cliquez sur **Convertir en workflow automatisé** dans l’écran qui s’affiche.

   >[!NOTE]
   >
   >Vous ne pouvez pas modifier la première étape lorsque vous passez d’un workflow de base à un workflow automatisé, mais vous pouvez ajouter et configurer de nouvelles étapes.

1. (Le cas échéant) Pour utiliser un modèle de workflow automatisé que l’équipe d’administration Adobe Workfront a créé et partagé avec vous, cliquez sur **Ajouter un modèle**, sélectionnez le modèle dans la zone qui s’affiche, puis cliquez sur **Ajouter un modèle**.

   Pour plus d’informations, voir [À propos de l’utilisation des modèles de workflow automatisé](#about-using-automated-workflow-templates) dans cet article.

1. Ajoutez une étape au workflow automatisé :

   1. Cliquez sur **Nouvelle étape** près du coin supérieur droit.
   1. Dans la zone qui s’affiche, saisissez un **Nom** pour l’étape.
   1. (Facultatif) Définissez une échéance pour l’étape.
   1. Dans la section **Activer l’étape**, choisissez le mode d’activation de l’étape :


      <table>
      <tbody>
      <tr>
      <td><strong>Lors de la création des épreuves</strong></td>
      <td>L’étape devient active automatiquement, car l’épreuve a déjà été créée.</td>
      </tr>
      <tr>
      <td><strong>Lorsque l'étape précédente est arrivée à échéance</strong></td>
      <td>Cliquez sur l’étape précédente dans la liste déroulante <strong>Étape parent</strong>.</td>
      </tr>
      <tr>
      <td><strong>À une date et une heure spécifiques</strong></td>
      <td>Cliquez sur la case <strong>Activé</strong> pour sélectionner la date, puis sur la case à droite pour sélectionner l’heure.</td>
      </tr>
      <tr>
      <td><strong>Toutes les décisions sont approuvées ou approuvées avec des modifications sur l’étape parent.</strong></td>
      <td>Cliquez sur l’étape parent dans la liste déroulante <strong>Étape parent</strong>.</td>
      </tr>
      <tr>
      <td><strong>Toutes les décisions sont approuvées sur l’étape parent.</strong></td>
      <td>Cliquez sur l’étape parent dans la liste déroulante <strong>Étape parent</strong>.</td>
      </tr>
      <tr>
      <td><strong>Toutes les décisions sont prises.</strong></td>
      <td>Cliquez sur l’étape parent dans la liste déroulante des <strong>Étapes parent</strong>.</td>
      </tr>
      </tbody>
      </table>


   1. Saisissez le nom du contact ou l’adresse e-mail, puis configurez les paramètres pour les réviseurs et réviseuses de l’étape.

      Pour plus d’informations sur l’ajout de réviseurs et réviseuses, voir [À propos de l’ajout de réviseurs et réviseuses à une étape](#about-adding-reviewers-to-a-stage) dans cet article.

   1. Utilisez l’une des options suivantes pour configurer davantage l’étape :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Options de date d’échéance</strong> </td>
         <td><p>Pour définir une échéance pour l’étape, cliquez sur une option dans la liste déroulante des <strong>Options de date d’échéance</strong>. Ensuite, sous <strong>Date d’échéance</strong>, effectuez l’une des opérations suivantes :</p>
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
         <td role="rowheader">Décisionnaire principal</td>
         <td><p>Sélectionnez la personne décisionnaire principale sur l’étape (disponible uniquement après avoir ajouté au moins une personne à l’étape qui dispose d’un rôle de relecture d’approbation ou supérieur). Si vous sélectionnez une personne décisionnaire principale, l’option <strong>Une seule décision requise</strong> est désactivée sur cette étape.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Une seule décision requise</td>
         <td>Met fin à l’ensemble du processus de révision lorsque l’une des personnes décisionnaires prend une décision.<p>Cette option n’est pas disponible si vous avez désigné un utilisateur ou une utilisatrice dans le menu déroulant des <strong>Personnes décisionnaires principales</strong>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Étape privée</td>
         <td>Permet uniquement aux personnes suivantes d’afficher les commentaires et les décisions prises à cette étape : superviseurs ou superviseuses, administrateurs ou administratrices Adobe Workfront et administrateurs ou administratrices Workfront Proof.</td>
        </tr>
        <tr>
         <td role="rowheader">Notifier les personnes par e-mail</td>
         <td>Alerte les réviseurs et réviseuses avec une notification par e-mail lorsqu’il vient leur tour de travailler sur une épreuve.</td>
        </tr>
       </tbody>
      </table>

   1. Cliquez sur **Ajouter une étape**.

1. Répétez l’étape précédente si nécessaire pour ajouter d’autres étapes.

   Lorsque vous ajoutez des étapes au processus automatisé, un diagramme s’affiche à l’écran pour les représenter :

   ![Diagramme de workflow](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Lorsque vous avez terminé d’ajouter des étapes, cliquez sur **Terminé**.

## À propos de l’utilisation des modèles de workflow automatisés {#about-using-automated-workflow-templates}

Tenez compte des points suivants lorsque vous utilisez un modèle de workflow automatisé :

1. Les paramètres d’un modèle de workflow automatisé déterminent ce que vous pouvez faire avec le workflow automatisé pour une épreuve. Par exemple, si le bouton Ajouter une étape est désactivé dans le modèle, il n’est pas visible lorsque vous travaillez avec les paramètres de workflow automatisé de l’épreuve.
1. Lorsqu’une personne est ajoutée à une étape dans un modèle de workflow automatisé, mais qu’elle est déjà présente en tant que réviseur ou réviseuse sur l’épreuve, l’application du modèle supprime le réviseur ou la réviseuse de l’étape. Si vous n’ajoutez pas d’autre réviseur ou réviseuse à l’étape, un message vous invite à le faire.
1. Votre capacité à modifier un modèle de workflow automatisé dépend des paramètres de modèle configurés par l’équipe d’administration Workfront, comme décrit dans . Si la possibilité de modifier le modèle est désactivée, seul la personne propriétaire du modèle peut le modifier.

## À propos de l’ajout de réviseurs et réviseuses à une étape {#about-adding-reviewers-to-a-stage}

Tenez compte des points suivants lors de l’ajout de réviseurs et réviseuses à une étape :

* Une fois que vous avez ajouté une personne à une étape, vous pouvez configurer les paramètres de cette personne sur l’épreuve, tels que le rôle de l’épreuve et les autorisations supplémentaires qu’elle doit posséder, ainsi que le type d’alertes par e-mail qu’elle recevra lorsque des personnes auront commenté et pris des décisions sur l’épreuve.
* Vous pouvez faire glisser une ou plusieurs personnes d’une étape vers une autre. Vous pouvez faire glisser les personnes directement vers une autre étape, ou vous pouvez les faire glisser vers une étape sur le diagramme des **Étapes**. Pour sélectionner plusieurs utilisateurs et utilisatrices, appuyez sur Maj+Ctrl (sous Windows) ou Maj+Commande (sous Mac).
* Vous ne pouvez ajouter un réviseur ou une réviseuse qu’une seule fois à une épreuve, ce qui signifie que vous ne pouvez pas ajouter la même personne à plusieurs étapes de l’épreuve.
* Les réviseurs et réviseuses qui ne sont pas ajoutés à une étape privée ne peuvent pas voir cette étape sur l’épreuve ou les commentaires faits à cette étape.
* Par défaut, l’ajout d’une personne à une étape lui donne accès pour afficher l’épreuve à partir du moment où l’épreuve est créée.

  Votre équipe d’administration Workfront peut empêcher les utilisateurs et utilisatrices d’accéder à l’épreuve jusqu’à ce que le workflow entre dans l’étape où sont ajoutés les utilisateurs et utilisatrices. Pour plus d’informations, voir .
