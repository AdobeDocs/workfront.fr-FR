---
title: Présentation de l’assistant de planification AI d’Adobe Workfront
description: Vous pouvez utiliser l’assistant d’IA pour générer, mettre à jour ou supprimer des enregistrements en fonction du contexte de page et de la structure d’enregistrement actuels. Les commandes de l’utilisateur et l’exécution de ces commandes par l’IA fonctionnent ensemble pour garantir que les modifications apportées par l’IA sont reflétées avec précision dans votre environnement.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 6%

---


# Présentation de l’assistant de planification Adobe Workfront AI

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Vous pouvez utiliser l’assistant d’IA pour générer, mettre à jour ou supprimer des enregistrements en fonction du contexte de page et de la structure d’enregistrements actuels.

Les commandes de l’utilisateur et l’exécution de ces commandes par l’IA fonctionnent ensemble pour garantir que les modifications apportées par l’IA sont reflétées avec précision dans votre environnement.

## Remarques concernant l’assistant d’IA

* L’assistant d’IA doit être activé pour votre organisation avant d’être disponible pour les utilisateurs de votre entreprise. Pour plus d’informations, voir [Présentation de l’assistant d’IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* Une fois que Workfront a activé l’assistant d’IA pour votre organisation, il est disponible pour l’administrateur Workfront principal. Pour plus d’informations, voir [Configurer les informations de base de votre système](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

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


## Localisation de l’assistant d’IA dans la planification Workfront

Vous pouvez localiser l’assistant d’IA dans les zones suivantes de la planification Workfront :

* La barre de navigation principale, dans le coin supérieur droit de l’écran.
* <span class="preview">Dans la zone de détails d’un enregistrement, après avoir ouvert l’enregistrement dans l’aperçu ou après avoir ouvert la page de l’enregistrement.</span>

## Accès à l’assistant d’IA dans la zone Planification

1. Connectez-vous à Workfront, puis cliquez sur l’icône **Menu principal** ![](assets/dots-main-menu.png) dans le coin supérieur droit de l’écran, ou sur l’icône **Menu principal** ![](assets/lines-main-menu.png) dans le coin supérieur gauche, le cas échéant.

. Cliquez sur **Planning**. La zone Planification s’ouvre.

1. Cliquez sur une carte **espace de travail**.

1. (Facultatif) Cliquez sur une **carte de type enregistrement**.

1. (Facultatif) Cliquez sur un **enregistrement** pour ouvrir la page **Détails** de l’enregistrement.

1. Cliquez sur l’icône **Assistant IA** dans le coin supérieur droit de l’écran dans la barre de navigation globale <span class="preview"> ou dans le coin supérieur droit de l’aperçu ou de la page de l’enregistrement.</span>

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



