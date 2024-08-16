---
title: Présentation de l’assistant de planification Adobe Workfront AI
description: Vous pouvez utiliser l’assistant d’IA pour générer, mettre à jour ou supprimer des enregistrements en fonction du contexte de page et de la structure d’enregistrement actuels. Les commandes de l’utilisateur et l’exécution de ces commandes par l’IA fonctionnent ensemble pour garantir que les modifications apportées par l’IA sont reflétées avec précision dans votre environnement.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: 57e0fe65180cec3fab5cb10b3afbc0ac0a1dbb55
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 6%

---

# Présentation de l’assistant de planification Adobe Workfront AI

<!-- update metadata above at GA-->

>[!IMPORTANT]
>
><span class="preview">L’assistant Workfront AI a été temporairement supprimé et sera disponible ultérieurement.</span>
>Les informations de cet article se rapportent à la planification Adobe Workfront et à l’assistant Workfront AI (version bêta), qui sont de nouvelles offres d’Adobe Workfront.
>
>Actuellement, Workfront Planning est en phase d’accès anticipé et l’assistant Workfront AI est en phase bêta.
>
>La planification de Workfront et l’assistant d’IA (version bêta) sont ouverts à un nombre limité de clients.
>
>Vous devez être une cliente ou un client Workfront pour utiliser ces fonctionnalités.
>
>Si vous participez à cette étape, le représentant du compte vous en informera.
>
>Pour plus d’informations, voir [Vue d’ensemble d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Vous pouvez utiliser l’assistant d’IA pour générer, mettre à jour ou supprimer des enregistrements en fonction du contexte de page et de la structure d’enregistrements actuels.

Les commandes de l’utilisateur et l’exécution de ces commandes par l’IA fonctionnent ensemble pour garantir que les modifications apportées par l’IA sont reflétées avec précision dans votre environnement.

## Remarques concernant l’assistant d’IA

* Par défaut, l’assistant d’IA est disponible pour l’administrateur Workfront principal. Pour plus d’informations, voir [Configuration des informations de base pour votre système](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* L’administrateur Workfront doit activer l’assistant d’IA pour tous les autres utilisateurs. Pour plus d’informations, voir [Activation ou désactivation de l’assistant d’IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* L’assistant d’IA fonctionne dans le contexte de chaque page. Les requêtes que vous envoyez pour l’assistant d’IA doivent référencer la fonctionnalité disponible dans la page que vous avez ouverte.

* Les actions effectuées par l’assistant d’IA dans la zone Planification se rapportent à vos autorisations de planification Workfront et à votre niveau d’accès Workfront. Pour plus d’informations, voir les articles suivants :

   * [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Les modifications apportées par l’assistant d’IA au nom de l’utilisateur sont suivies dans le panneau Historique des enregistrements.

* Vous pouvez utiliser des commandes pour annuler vos actions. Par exemple, vous pouvez saisir &quot;Annuler la dernière modification&quot; pour annuler la modification.

## Fonctionnalités actuellement disponibles pour l’assistant AI

Actuellement, l’assistant d’IA est disponible dans la zone Planification de Workfront pour les pages suivantes :

* Page Workspace
* Page de type d’enregistrement
* Enregistrer la page

Pour le moment, vous pouvez utiliser l’assistant d’IA pour effectuer les actions suivantes :

* Recherchez des enregistrements. Vous pouvez effectuer une recherche en fonction des informations contenues dans n’importe quel champ d’enregistrement.
* Créer des enregistrements. Un identifiant avec un lien vers le nouvel enregistrement s’affiche une fois l’enregistrement créé. Vous pouvez spécifier les champs que vous souhaitez mettre à jour au cours du processus de création, tels que les dates ou la description.
* Créez des enregistrements à partir d’un document que vous téléchargez. Workfront prend en charge les formats de document suivants pour l’assistant d’IA :

  .pptx, .pdf, .docx, .xlsx, .ppt, .doc, .txt et la plupart des formats d’image
* Mettre à jour les champs des enregistrements affichés à l’écran
* Supprimer des enregistrements
* Restaurer les enregistrements que vous venez de supprimer

## Accès à l’assistant d’IA

1. Connectez-vous à Workfront, puis accédez à la zone **Planning**.

1. Cliquez sur une carte **espace de travail**.

1. (Facultatif) Cliquez sur une **carte de type enregistrement**.

1. (Facultatif) Cliquez sur un **enregistrement** pour ouvrir la page **Détails** de l’enregistrement.

1. Cliquez sur l’icône **Assistant IA** dans le coin supérieur droit de l’écran dans la barre de navigation globale.

   ![](assets/ai-assistant-icon-highlighted.png)

1. Dans l’espace fourni, commencez à saisir des commandes pour l’assistant d’IA, puis cliquez sur Entrée lorsque vous avez terminé.

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   Par exemple, vous pouvez saisir l’une des valeurs suivantes :

   * Créez une campagne dont la date de début est le 4 juillet et la date de fin est le 30 juillet.
   * Mettre à jour le champ Description de l’enregistrement de campagne d’été avec la date à déterminer
   * Supprimer le dernier enregistrement
   * Restaurer l’enregistrement

   Un indicateur visuel s’affiche pendant que l’assistant d’IA traite les commandes, définissant les attentes en termes de temps de réponse.

   Après avoir reçu une réponse réussie, suivez les liens fournis ou notez les modifications sur la gauche.
