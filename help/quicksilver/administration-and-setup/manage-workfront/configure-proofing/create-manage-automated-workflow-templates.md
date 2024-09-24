---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Création et gestion de modèles de workflow automatisés
description: En tant qu’administrateur ou administratrice Adobe Workfront, si le processus de révision du contenu de votre entreprise est souvent effectué ou si le contenu est souvent révisé par les mêmes personnes, vous pouvez créer des modèles de workflow automatisé qui contiennent lesdites personnes réviseuses avec les rôles d’approbation et les paramètres de notification que vous spécifiez. Un modèle de workflow automatisé peut être simple avec une ou deux personnes réviseuses, ou bien complexe avec de nombreuses étapes et dépendances.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: 7a2cfddf4683b5b49121bbe3987498297b963ffa
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 98%

---

# Créer et gérer des modèles de workflows automatisés

<!-- Audited: 2/2024 -->

En tant qu’administrateur ou administratrice Adobe Workfront, si le processus de révision du contenu de votre entreprise est souvent effectué ou si le contenu est souvent révisé par les mêmes personnes, vous pouvez créer des modèles de workflow automatisé qui contiennent lesdites personnes réviseuses avec les rôles d’approbation et les paramètres de notification que vous spécifiez. Un modèle de workflow automatisé peut être simple avec une ou deux personnes réviseuses, ou bien complexe avec de nombreuses étapes et dépendances.

Les modèles de workflow automatisé facilitent la création d’une épreuve avec un workflow automatisé. Lorsqu’une personne crée une épreuve, elle choisit simplement le modèle dont elle a besoin.

Il est possible de facilement modifier n’importe quel modèle de workflow automatisé, d’ajouter ou de supprimer à tout moment des personnes réviseuses et des étapes. De même, les créateurs et créatrices d’épreuves qui utilisent le modèle peuvent ajouter des personnes réviseuses à l’épreuve ou en supprimer.

Tenez compte des points suivants lorsque vous utilisez un modèle de workflow automatisé :

1. Les paramètres d’un modèle de workflow automatisé déterminent ce que vous pouvez faire avec le workflow automatisé pour une épreuve. Par exemple, si le bouton Ajouter une étape est désactivé dans le modèle, il n’est pas visible lorsque vous travaillez avec les paramètres de workflow automatisé de l’épreuve.
1. Lorsqu’une personne est ajoutée à une étape dans un modèle de workflow automatisé, mais également déjà présente en tant que validant sur le BAT, l’application du modèle supprime le validant de l’étape. Si vous n’ajoutez pas d’autre réviseur ou réviseuse à l’étape, un message vous invite à le faire.
1. Votre capacité à modifier un modèle de workflow automatisé dépend des paramètres de modèle configurés par l’équipe d’administration Workfront, comme décrit dans . Si la possibilité de modifier le modèle est désactivée, seule la personne propriétaire du modèle peut le modifier.

Pour plus d’informations sur les workflows automatisés, consultez la section [Vue d’ensemble des workflows automatisés](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Nouveau : Tous</p><p>Actuel : Pro ou supérieur</p><p>Héritée : Premium ou Select</p> <p>Pour plus d’informations sur l’accès à la relecture avec les différentes formules, consultez la section <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard</p><p>Actuelle : Travail ou Plan</p> <p>Héritée : toutes (la relecture doit être activée pour l’utilisateur ou l’utilisatrice)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>L’option d’administration doit être sélectionnée dans votre profil d’autorisation d’épreuve. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un modèle de workflow automatisé

{{step1-to-proofing}}

1. Cliquez sur **Workflows** dans le panneau de gauche.
1. Dans l’onglet **Workflow**, cliquez sur **Nouveau** > **Nouveau modèle**.

1. Dans la section **Détails**, saisissez les informations suivantes :

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
      <td>Vous pouvez sélectionner l’administrateur ou l’administratrice Workfront ou Workfront Proof qui gérera le modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groupe de modèles</td> 
      <td> <p> Si les workflows automatisés de votre entreprise sont organisés en groupes, vous pouvez sélectionner le nom du groupe. Pour plus d’informations, consultez la section <a href="#create-automated-workflow-template-groups" class="MCXref xref">Créer des groupes de modèles de workflows automatisés</a> plus loin dans cet article.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Fuseau horaire du modèle </td> 
      <td> <p>Le fuseau horaire par défaut du modèle est celui dans lequel vous travaillez. Si le fuseau horaire des personnes chargées de la création et de la révision des épreuves est différent, vous pouvez le modifier ici afin de vous assurer que les échéances des étapes sont correctement définies pour ces utilisateurs et ces utilisatrices. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser</td> 
      <td> <p>Vous pouvez sélectionner les activités d’étapes que vous souhaitez mettre à la disposition de la personne pour créer des épreuves à l’aide du modèle.</p> 
      <p><b>AVERTISSEMENT</b> : si vous ne sélectionnez pas les options Ajouter une étape et Ajouter des personnes aux étapes, ni la personne propriétaire du modèle ni la personne propriétaire d’une épreuve utilisant ce modèle ne pourront ajouter une étape ou partager l’épreuve. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Dans la section **Étapes**, configurez chaque étape du modèle de workflow automatisé.

   Vous pouvez ajouter plusieurs étapes et créer entre elles.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>Le nom de l’étape s’affiche dans le diagramme Workflow automatisé au haut de la section Workflow, sur la page Détails de l’épreuve et dans les notifications envoyées par e-mail aux réviseurs et réviseuses.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activer l’étape</td> 
      <td> <p>Indiquez si l’étape est activée automatiquement ou manuellement. Pour la première étape, vous pouvez sélectionner <strong>Lors de la création de l’épreuve</strong>, <strong>À une date et une heure spécifiques</strong> ou <strong>Manuellement</strong>.</p> <p>Les autres options deviennent disponibles lorsque vous ajoutez une seconde étape, car elles vous obligent à sélectionner une étape parent. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date d’échéance calculée à partir de</td> 
      <td> <p>Indiquez le mode de calcul de la date d’échéance :</p> 
       <ul> 
        <li> <p><strong>Création de l’épreuve</strong> : dans la liste déroulante sous <strong>Date d’échéance (+ jours ouvrables)</strong>, sélectionnez le nombre de jours ouvrables à ajouter à la date de création de l’épreuve pour définir automatiquement une date d’échéance sur l’épreuve.</p> </li> 
        <li><strong>Lorsque l’étape démarre</strong> : dans la liste déroulante sous <strong>Date d’échéance (+ jours ouvrables)</strong>, sélectionnez le nombre de jours ouvrables à ajouter à la date d’activation de l’étape pour définir automatiquement une date d’échéance sur l’épreuve.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’étape</td> 
      <td>Indiquez si vous souhaitez autoriser le verrouillage de l’étape pour les commentaires. Les options sont de verrouiller une étape manuellement ou automatiquement, au démarrage de l’étape suivante ou lorsque toutes les décisions sont prises sur l’étape parent.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décisionnaire principal</td> 
      <td> <p>Les personnes responsables de la prise de décision disponibles s’affichent dans la liste uniquement après avoir ajouté les réviseurs et réviseuses à l’étape.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Une seule décision requise</td> 
      <td>Le processus de révision de l’étape sera achevé dès que l’une des personnes responsables de la prise de décision aura présenté sa décision. Pour plus d’informations, voir <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurer des paramètres d’épreuve dans Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Étape privée</td> 
      <td>Masque les commentaires et les décisions aux personnes qui ne sont pas ajoutées à l’étape ou qui ne sont pas administrateurs ou administratrices Workfront. Pour plus d’informations, voir<a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Vue d’ensemble du workflow automatisé</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ne pas autoriser la suppression de cette étape</td> 
      <td> <p>Rend l’étape obligatoire.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Si les épreuves qui utiliseront ce modèle sont toujours envoyées aux mêmes personnes dans l’étape, ajoutez-les ici afin que les personnes n’aient pas à les ajouter chaque fois qu’elles créent une épreuve.

   Choisissez le **Rôle** de chaque personne sur les épreuves qui utiliseront ce modèle et les **Alertes par e-mail** que vous souhaitez que la personne reçoive lorsqu’elle travaille sur des épreuves qui utilisent ce modèle.

   Pour plus d’informations sur les rôles sur une épreuve, voir [Configurer des rôles de relecture par défaut](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Pour plus d’informations sur les alertes d’épreuve par e-mail, voir la section [Configurer les paramètres par défaut d’une épreuve pour une personne](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) dans l’article [Configurer les paramètres de notification par e-mail dans Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Chaque personne ne peut être ajoutée qu’à une seule étape. Vous pouvez ajouter autant de personnes que vous le souhaitez à une étape.

   >[!TIP]
   >
   >Vous pouvez faire glisser et déposer les noms des réviseurs et réviseuses entre les étapes sur le diagramme des étapes. Les étapes disponibles sont mises en surbrillance en bleu.

1. Répétez les deux étapes précédentes pour toute autre étape que vous souhaitez ajouter au modèle.

   En haut de la section **Workflow**, vous pouvez voir un diagramme du workflow automatisé que vous configurez. Au fur et à mesure que vous continuez à ajouter des étapes, elles apparaissent sur le diagramme avec des lignes indiquant les dépendances entre elles. Vous pouvez cliquer sur une étape du diagramme pour afficher les paramètres de cette étape.

   Si vous n’avez pas besoin de voir le diagramme, vous pouvez cliquer sur **Masquer le diagramme**.

1. Dans la section **Partager le modèle avec**, cliquez sur une option (si le modèle n’est pas déjà partagé avec l’ensemble de l’organisation) pour spécifier qui pourra l’utiliser.

   Par défaut, les nouveaux modèles de workflow automatisé sont partagés avec toutes les personnes de votre entreprise.

1. Cliquez sur **Créer**.

## Modifier un modèle de workflow automatisé

En tant qu’administrateur ou administratrice Workfront proof, vous pouvez modifier un modèle de workflow automatisé. Vos modifications sont enregistrées automatiquement au fur et à mesure que vous les apportez.

{{step1-to-proofing}}

1. Cliquez sur **Workflows** dans le panneau de gauche.
1. Dans la liste **Modèles de workflow** qui s’affiche, cliquez sur le modèle à modifier.
1. Dans la section **Détails**, renseignez les informations suivantes :

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
      <td>Vous pouvez sélectionner l’administrateur ou l’administratrice Workfront ou Workfront Proof qui gérera le modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groupe de modèles</td> 
      <td> <p> Si les workflows automatisés de votre entreprise sont organisés en groupes, vous pouvez sélectionner le nom du groupe. Pour plus d’informations, consultez la section <a href="#create-automated-workflow-template-groups" class="MCXref xref">Créer des groupes de modèles de workflows automatisés</a> plus loin dans cet article.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fuseau horaire du modèle </td> 
      <td> <p>Le fuseau horaire par défaut du modèle est celui dans lequel vous travaillez. Si le fuseau horaire des personnes chargées de la création et de la révision des épreuves est différent, vous pouvez le modifier ici afin de vous assurer que les échéances des étapes sont correctement définies pour ces utilisateurs et ces utilisatrices. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser</td> 
      <td> <p>Sélectionnez les activités d’étape que vous souhaitez rendre accessibles aux personnes qui créent des épreuves à l’aide du modèle. </p> <p><b>AVERTISSEMENT</b> : si vous ne sélectionnez pas les options « Ajouter une étape » et « Ajouter des personnes aux étapes », aucune étape ne pourra être ajoutée par la personne propriétaire du modèle ou d’une épreuve utilisant ce modèle, et l’épreuve ne pourra pas être partagée.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Dans la section **Workflow**, modifiez le nom d’une étape et développez ses paramètres ![](assets/arrow-button.png) pour apporter les modifications nécessaires :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Date d’échéance calculée à partir de</td> 
      <td> <p>Indiquez le mode de calcul de la date d’échéance :</p> 
       <ul> 
        <li> <p><strong>Date d’échéance calculée à partir de la création de l’épreuve</strong> : dans la liste déroulante <strong>Définir une date d’échéance d’étape</strong>, sélectionnez le nombre de jours ouvrables à ajouter à la date de création de l’épreuve pour définir automatiquement une date d’échéance pour l’épreuve.</p> </li> 
        <li><strong>Date d’échéance calculée à partir de l’activation de l’épreuve</strong> : dans la liste déroulante <strong>Définir une date d’échéance d’étape</strong>, sélectionnez le nombre de jours ouvrables à ajouter à la date d’activation de l’épreuve pour définir automatiquement une date d’échéance pour l’épreuve.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activer l’étape</td> 
      <td> <p>Indiquez si l’étape est activée automatiquement ou manuellement. Pour la première étape, vous pouvez sélectionner <strong>Lors de la création de l’épreuve</strong>, <strong>À une date et une heure spécifiques</strong> ou <strong>Manuellement</strong>.</p> <p>Les autres options deviennent disponibles lorsque vous ajoutez une seconde étape, car elles vous obligent à sélectionner une étape parent. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’étape</td> 
      <td>Indiquez si vous souhaitez autoriser le verrouillage de l’étape pour les commentaires. Les options sont de verrouiller une étape manuellement ou automatiquement, au démarrage de l’étape suivante ou lorsque toutes les décisions sont prises sur l’étape parent.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décision</td> 
      <td>L’étape se termine dès que l’une des personnes décisionnaires soumet sa décision. Pour plus d’informations, consultez la section <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Configurer des paramètres d’épreuve dans Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Confidentialité</td> 
      <td>Masque les commentaires et les décisions des personnes qui n’ont pas été ajoutées à l’étape ou qui ne sont pas des personnes ayant un niveau de supervision ou supérieur dans le compte. Pour plus d’informations, consultez la section <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Vue d’ensemble du workflow automatisé</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer une étape</td> 
      <td>Rend l’étape obligatoire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Plus <img src="assets/more-icon.png"></td> 
      <td>Ajoutez des personnées chargées de la révision à l’étape ou supprimez l’étape.<p>Si chacune de vos épreuves est envoyée aux mêmes personnes à une étape donnée, vous pouvez spécifier leurs noms ici afin de ne pas avoir à les ajouter à chaque fois que vous créez une épreuve. Saisissez et sélectionnez le nom d’un utilisateur ou d’une utilisatrice que vous souhaitez ajouter à l’étape, puis définissez son <strong>Rôle</strong> sur l’épreuve ainsi que ses paramètres d’<strong>Alertes par e-mail</strong>. Pour plus d’informations sur les rôles de relecture, consultez la section <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Configurer des rôles de relecture par défaut</a>. Pour plus d’informations sur les alertes d’épreuve par e-mail, consultez la section <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Configurer les paramètres par défaut d’une épreuve pour un utilisateur ou une utilisatrice</a> dans l’article <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configurer les paramètres des notifications par e-mail des épreuves Workfront</a>.</p><p>Vous pouvez ajouter autant d’utilisateurs et d’utilisatrices que vous le souhaitez à une étape.</p><p>Conseil : vous pouvez faire glisser et déposer les noms des personnes chargées de la révision entre les étapes sur le diagramme des étapes. Les étapes disponibles sont mises en surbrillance en bleu.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Répétez l’étape pour toutes les autres étapes à ajouter au modèle.

   En haut de la section **Workflow**, vous pouvez voir un diagramme du workflow automatisé que vous configurez. Au fur et à mesure que vous continuez à ajouter des étapes, elles apparaissent sur le diagramme avec des lignes indiquant les dépendances entre elles. Vous pouvez cliquer sur une étape du diagramme pour afficher les paramètres de cette étape.

   Si vous n’avez pas besoin de voir le diagramme, vous pouvez cliquer sur **Masquer le diagramme**.

1. Si vous souhaitez supprimer un utilisateur ou une utilisatrice, cliquez sur le bouton Plus ![](assets/more-icon.png) à droite dans la section **Partagé avec**, puis cliquez sur **Supprimer**.

## Créer des groupes de modèles de workflow automatisé {#create-automated-workflow-template-groups}

En tant qu’administrateur ou administratrice Workfront, vous pouvez afficher et gérer tous les modèles de workflow automatisés dans le compte de votre entreprise. Organiser les modèles en groupes peut s’avérer utile.

Pour créer un groupe de modèles de workflow automatisé, procédez comme suit :

{{step1-to-proofing}}

1. Cliquez sur **Workflows** dans le panneau de gauche.
1. Sur l’onglet **Workflow**, cliquez sur **Nouveau** > **Nouveau groupe de modèles**.
1. Saisissez un nom explicite pour le nouveau groupe de modèles, puis appuyez sur **Entrée**.

Vous pouvez déplacer les modèles entre les groupes en les faisant glisser et en les déposant.

## Gérer des modèles de workflow automatisés

{{step1-to-proofing}}

1. Dans le panneau de gauche de Workfront Proof, cliquez sur **Workflows**.
1. Sur la page **Workflows** qui s’affiche, effectuez l’une des opérations suivantes :

   * Ajouter un nouveau modèle
   * Ajouter un nouveau groupe de modèles
   * Supprimer un ou plusieurs groupes de modèles
   * Accèder aux détails d’un modèle
   * Faire glisser un modèle vers un autre groupe de modèles
