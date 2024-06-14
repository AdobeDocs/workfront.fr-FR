---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Création et gestion de modèles de processus automatisés
description: En tant qu’administrateur Adobe Workfront, si le processus d’examen du contenu de votre entreprise est souvent répété ou si le contenu est souvent examiné par les mêmes personnes, vous pouvez créer des modèles de workflow automatisé qui contiennent les réviseurs avec les rôles de BAT et les paramètres de notification que vous spécifiez. Un modèle de workflow automatisé peut être simple avec un ou deux réviseurs ou complexe avec de nombreuses étapes et dépendances.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 2%

---

# Création et gestion de modèles de processus automatisés

<!-- Audited: 2/2024 -->

En tant qu’administrateur Adobe Workfront, si le processus d’examen du contenu de votre entreprise est souvent répété ou si le contenu est souvent examiné par les mêmes personnes, vous pouvez créer des modèles de workflow automatisé qui contiennent les réviseurs avec les rôles de BAT et les paramètres de notification que vous spécifiez. Un modèle de workflow automatisé peut être simple avec un ou deux réviseurs ou complexe avec de nombreuses étapes et dépendances.

Les modèles de workflow automatisés facilitent la création d’un BAT avec un workflow automatisé. Lorsqu’un utilisateur crée un BAT, il choisit simplement le modèle dont il a besoin.

Vous pouvez facilement modifier n’importe quel modèle de workflow automatisé, ajouter ou supprimer des réviseurs et des étapes, à tout moment. Et les créateurs de BAT qui utilisent le modèle peuvent ajouter ou supprimer des réviseurs pour le BAT.

Tenez compte des points suivants lorsque vous utilisez un modèle de workflow automatisé :

1. Les paramètres d’un modèle de workflow automatisé déterminent ce que vous pouvez faire avec le workflow automatisé pour un BAT. Par exemple, si le bouton Ajouter une scène est désactivé dans le modèle, il n’est pas visible car vous travaillez avec les paramètres de workflow automatisé du BAT.
1. Lorsqu’une personne est ajoutée à un niveau dans un modèle de workflow automatisé, mais également déjà présente en tant que validant sur le BAT, l’application du modèle supprime le validant de l’étape. Si vous n’ajoutez pas d’autre réviseur à l’étape, un message vous invite à en ajouter un.
1. Votre capacité à modifier un modèle de workflow automatisé dépend des paramètres de modèle configurés par l’administrateur de Workfront, comme décrit dans la section . Si la possibilité de modifier le modèle est désactivée, seul le propriétaire du modèle peut le modifier.

Pour plus d’informations sur les processus automatisés, voir [Présentation des processus automatisés](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>Nouveau : Quelconque</p><p>Actuel : Pro ou supérieur</p><p>Hérité : Premium ou Sélectionner</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard</p><p>Actuel : travail ou plan</p> <p>Hérité : Toutes (la vérification doit être activée pour l’utilisateur)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>L’administrateur doit être sélectionné dans votre profil d’autorisation de BAT. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création d’un modèle de processus automatisé

{{step1-to-proofing}}

1. Cliquez sur **Workflows** dans le panneau de gauche.
1. Sur le **Workflow** , cliquez sur **Nouveau** > **Nouveau modèle**.

1. Dans le **Détails** , renseignez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du modèle</td> 
      <td>(Obligatoire) Saisissez le nom du modèle. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propriétaire du modèle</td> 
      <td>Vous pouvez sélectionner l’administrateur Workfront ou l’administrateur Workfront Proof qui gérera le modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groupe de modèles</td> 
      <td> <p> Si les processus automatisés de votre entreprise sont organisés en groupes, vous pouvez sélectionner le nom du groupe. Voir <a href="#create-automated-workflow-template-groups" class="MCXref xref">Création de groupes de modèles de processus automatisé</a> plus loin dans cet article.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Fuseau horaire du modèle </td> 
      <td> <p>Le fuseau horaire par défaut du modèle est celui dans lequel vous travaillez. Si le fuseau horaire des créateurs et réviseurs du BAT qui utiliseront le modèle est différent, vous pouvez le modifier ici afin de vous assurer que les échéances de l’évaluation sont définies aux bons moments pour ces utilisateurs. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser</td> 
      <td> <p>Vous pouvez sélectionner les activités d’évaluation que vous souhaitez mettre à la disposition de la personne pour créer des BAT à l’aide du modèle.</p> 
      <p><b>Avertissement</b>: si vous ne sélectionnez pas les options Ajouter une scène et Ajouter des personnes aux scènes, ni le propriétaire du modèle ni le propriétaire d'un BAT utilisant ce modèle ne pourront ajouter une scène ou partager le BAT. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Dans le **Phases** , configurez chaque étape du modèle de workflow automatisé.

   Vous pouvez ajouter plusieurs scènes et les créer entre elles.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>Le nom de l’étape s’affiche dans le diagramme Processus automatisé au haut de la section Processus, sur la page Détails du bon à tirer et dans les notifications électroniques envoyées aux réviseurs.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activer l’étape</td> 
      <td> <p>Indiquez si l’étape est activée automatiquement ou manuellement. Pour la première étape, vous pouvez sélectionner <strong>Lors de la création du BAT</strong>, <strong>À une date et une heure spécifiques</strong>, ou <strong>Manuellement</strong>.</p> <p>Les autres options deviennent disponibles lorsque vous ajoutez une seconde étape, car elles vous obligent à sélectionner une étape parent. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date limite calculée à partir de</td> 
      <td> <p>Indiquez le mode de calcul du délai :</p> 
       <ul> 
        <li> <p><strong>Création de BAT</strong>: dans la liste déroulante sous <strong>Date limite (+ jours ouvrables)</strong>, sélectionnez le nombre de jours ouvrables à ajouter à la date de création du BAT pour définir automatiquement une date limite sur le BAT.</p> </li> 
        <li><strong>Lorsque l’étape démarre</strong>: dans la liste déroulante sous <strong>Date limite (+ jours ouvrables)</strong>, sélectionnez le nombre de jours ouvrés à ajouter à la date d’activation de l’évaluation pour définir automatiquement une échéance sur le BAT.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’étape</td> 
      <td>Indiquez si vous souhaitez autoriser le verrouillage de l’étape pour les commentaires. Les options sont de verrouiller une étape manuellement ou automatiquement, au démarrage de l’étape suivante ou lorsque toutes les décisions sont prises sur l’étape parent.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décisionnaire principal</td> 
      <td> <p>Les décideurs disponibles s’affichent dans la liste uniquement après avoir ajouté les réviseurs à l’étape.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Une seule décision requise</td> 
      <td>Le processus d'examen de l'étape sera achevé dès que l'un des décideurs aura présenté sa décision. Pour plus d’informations, voir <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configuration des paramètres de BAT dans Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etape privée</td> 
      <td>Masque les commentaires et les décisions de aux personnes qui ne sont pas ajoutées à l’étape ou qui ne sont pas administrateurs Workfront. Pour plus d’informations, voir <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Présentation des processus automatisés</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ne pas autoriser la suppression de cette étape</td> 
      <td> <p>Rend l’étape obligatoire.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Si les bons à tirer qui utiliseront ce modèle sont toujours envoyés à la même personne dans l’étape, ajoutez-les ici afin que les utilisateurs n’aient pas à les ajouter chaque fois qu’ils créent un bon à tirer.

   Choisir le **Rôle** sur les BAT qui utiliseront ce modèle et le **Alertes par email** vous souhaitez que l’utilisateur reçoive lorsqu’il travaille sur des bons à tirer qui utilisent ce modèle.

   Pour plus d’informations sur les rôles sur un BAT, voir [Configuration des rôles de vérification par défaut](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Pour plus d’informations sur les alertes par email de BAT, voir la section [Configuration des paramètres par défaut d’un BAT pour un utilisateur](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) dans l’article  [Configuration des paramètres de notification électronique dans Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Chaque utilisateur ne peut être ajouté qu’à une seule étape. Vous pouvez ajouter autant d’utilisateurs que vous le souhaitez à une étape.

   >[!TIP]
   >
   >Vous pouvez faire glisser et déposer les noms des réviseurs entre les étapes du diagramme des étapes. Les étapes disponibles sont mises en surbrillance en bleu.

1. Répétez les deux étapes précédentes pour toute autre étape que vous souhaitez ajouter au modèle.

   En haut de la page **Workflow** , vous pouvez voir un diagramme du processus automatisé que vous configurez. Au fur et à mesure que vous continuez à ajouter des scènes, elles apparaissent sur le diagramme avec des lignes indiquant les dépendances entre elles. Vous pouvez cliquer sur une étape du diagramme pour afficher les paramètres de cette étape.

   Si vous n’avez pas besoin de voir le diagramme, vous pouvez cliquer sur **Masquer le diagramme**.

1. Dans le **Partager le modèle avec** , cliquez sur une option (si le modèle n’est pas déjà partagé avec l’ensemble de l’organisation) pour spécifier qui pourra l’utiliser.

   Par défaut, les nouveaux modèles de workflow automatisé sont partagés avec tous les membres de votre entreprise.

1. Cliquez sur **Créer**.

## Modification d’un modèle de processus automatisé

En tant qu’administrateur Workfront Proof, vous pouvez modifier un modèle de workflow automatisé. Vos modifications sont enregistrées automatiquement au fur et à mesure que vous les apportez.

{{step1-to-proofing}}

1. Cliquez sur **Workflows** dans le panneau de gauche.
1. Dans le **Modèles de workflow** qui s’affiche, cliquez sur le modèle à modifier.
1. Dans le **Détails** , renseignez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du modèle</td> 
      <td>(Obligatoire) Saisissez le nom du modèle. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propriétaire du modèle</td> 
      <td>Vous pouvez sélectionner l’administrateur Workfront ou l’administrateur Workfront Proof qui gérera le modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groupe de modèles</td> 
      <td> <p> Si les processus automatisés de votre entreprise sont organisés en groupes, vous pouvez sélectionner le nom du groupe. Voir <a href="#create-automated-workflow-template-groups" class="MCXref xref">Création de groupes de modèles de processus automatisé</a> plus loin dans cet article.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuseau horaire du modèle </td> 
      <td> <p>Le fuseau horaire par défaut du modèle est celui dans lequel vous travaillez. Si le fuseau horaire des créateurs et réviseurs du BAT qui utiliseront le modèle est différent, vous pouvez le modifier ici afin de vous assurer que les échéances de l’évaluation sont définies aux bons moments pour ces utilisateurs. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser</td> 
      <td> <p>Sélectionnez les activités d'évaluation que vous souhaitez mettre à la disposition de ceux qui créent des BAT à l'aide du modèle. </p> <p><b>Avertissement</b>: si vous ne sélectionnez pas les options Ajouter une scène et Ajouter des personnes aux scènes, ni le propriétaire du modèle ni le propriétaire d'un BAT utilisant ce modèle ne pourront ajouter une scène ou partager le BAT.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Dans le **Workflow** , modifiez le nom d’une étape et développez ses paramètres. ![](assets/arrow-button.png) pour apporter les modifications nécessaires :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Date limite calculée à partir de</td> 
      <td> <p>Indiquez le mode de calcul du délai :</p> 
       <ul> 
        <li> <p><strong>Date limite calculée à partir de la création du BAT</strong>: dans la variable <strong>Définition de la date limite d’évaluation</strong> dans la liste déroulante, sélectionnez le nombre de jours ouvrés à ajouter à la date de création du BAT pour définir automatiquement une date limite sur le BAT.</p> </li> 
        <li><strong>Date limite calculée à partir de l’activation de l’étape</strong>: dans la variable <strong>Définition de la date limite d’évaluation</strong> dans la liste déroulante, sélectionnez le nombre de jours ouvrés à ajouter à la date d’activation de l’évaluation afin de définir automatiquement une échéance sur le BAT.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activer l’étape</td> 
      <td> <p>Indiquez si l’étape est activée automatiquement ou manuellement. Pour la première étape, vous pouvez sélectionner <strong>Lors de la création du BAT</strong>, <strong>À une date et une heure spécifiques</strong>, ou <strong>Manuellement</strong>.</p> <p>Les autres options deviennent disponibles lorsque vous ajoutez une seconde étape, car elles vous obligent à sélectionner une étape parent. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’étape</td> 
      <td>Indiquez si vous souhaitez autoriser le verrouillage de l’étape pour les commentaires. Les options sont de verrouiller une étape manuellement ou automatiquement, au démarrage de l’étape suivante ou lorsque toutes les décisions sont prises sur l’étape parent.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décision</td> 
      <td>Termine l’étape la première fois qu’un des décideurs envoie sa décision. Pour plus d’informations, voir <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configuration des paramètres de BAT dans Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privacy</td> 
      <td>Masque dans le compte les commentaires et les décisions de pour les personnes qui ne sont pas ajoutées à l’étape ou qui ne sont pas des superviseurs et au-dessus. Pour plus d’informations, voir <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Présentation des processus automatisés</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suppression d’étapes</td> 
      <td>Rend l’étape obligatoire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Plus <img src="assets/more-icon.png"></td> 
      <td>Ajoutez des réviseurs à l’étape ou supprimez l’étape.<p>Si chacun de vos bons à tirer est envoyé à la même personne au cours d’une étape spécifique, vous pouvez spécifier son nom ici afin de ne pas avoir à les ajouter chaque fois que vous créez un bon à tirer. Saisissez et sélectionnez le nom d’un utilisateur que vous souhaitez ajouter à l’étape, puis ajoutez-lui la valeur <strong>Rôle</strong> sur le BAT et <strong>Alertes par email</strong> paramètres que vous souhaitez pour l’utilisateur. Pour plus d’informations sur la vérification des rôles, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configuration des rôles de vérification par défaut</a>. Pour plus d’informations sur les alertes par email de BAT, voir la section <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configuration des paramètres par défaut d’un BAT pour un utilisateur</a> dans l’article <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configuration des paramètres de notification électronique dans Workfront Proof</a>.</p><p>Vous pouvez ajouter autant d’utilisateurs que vous le souhaitez à une étape.</p><p>Conseil : Vous pouvez faire glisser et déposer les noms des réviseurs entre les étapes du diagramme des étapes. Les étapes disponibles sont mises en surbrillance en bleu.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Répétez l’étape pour toutes les autres étapes à ajouter au modèle.

   En haut de la page **Workflow** , vous pouvez voir un diagramme du processus automatisé que vous configurez. Au fur et à mesure que vous continuez à ajouter des scènes, elles apparaissent sur le diagramme avec des lignes indiquant les dépendances entre elles. Vous pouvez cliquer sur une étape du diagramme pour afficher les paramètres de cette étape.

   Si vous n’avez pas besoin de voir le diagramme, vous pouvez cliquer sur **Masquer le diagramme**.

1. Dans le **Partagé avec** si vous souhaitez supprimer un utilisateur, cliquez sur Plus ![](assets/more-icon.png) à droite, puis cliquez sur **Supprimer**.

## Création de groupes de modèles de processus automatisé {#create-automated-workflow-template-groups}

En tant qu’administrateur Workfront, vous pouvez afficher et gérer tous les modèles de processus automatisés dans le compte de votre entreprise. Il peut s’avérer utile d’organiser les modèles en groupes.

Pour créer un groupe de modèles de processus automatisé :

{{step1-to-proofing}}

1. Cliquez sur **Workflows** dans le panneau de gauche.
1. Sur le **Workflow** , cliquez sur **Nouveau** > **Nouveau groupe de modèles**.
1. Saisissez un nom explicite pour le nouveau groupe de modèles, puis appuyez sur **Entrée**.

Vous pouvez déplacer les modèles entre les groupes en les faisant glisser et en les déposant.

## Gestion des modèles de workflow automatisés

{{step1-to-proofing}}

1. Dans le panneau de gauche de Workfront Proof, cliquez sur **Workflows**.
1. Sur le **Workflows** qui s’affiche, effectuez l’une des opérations suivantes :

   * Ajouter un nouveau modèle
   * Ajouter un nouveau groupe de modèles
   * Supprimer un ou plusieurs groupes de modèles
   * Accès aux détails d’un modèle
   * Faire glisser un modèle vers un autre groupe de modèles
