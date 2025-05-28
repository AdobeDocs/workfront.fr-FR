---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Lier des éléments entre  [!DNL Adobe Workfront]  et  [!DNL Jira]
description: Vous pouvez lier des problèmes  [!DNL Jira]  à des tâches ou problèmes  [!DNL Adobe Workfront]  automatiquement ou manuellement.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: 97d755c71eb1bdfa8a031fa387741318f9a7f261
workflow-type: tm+mt
source-wordcount: '1238'
ht-degree: 54%

---

# Lier des éléments entre [!DNL Adobe Workfront] et [!DNL Jira]

<!-- Audited: 5/2025 -->

Vous pouvez lier des problèmes [!DNL Jira] à des tâches ou problèmes [!DNL Adobe Workfront] automatiquement ou manuellement.

Un seul élément dans [!DNL Workfront] peut être lié à un élément dans [!DNL Jira]. Vous ne pouvez jamais lier un élément [!DNL Workfront] à plusieurs problèmes [!DNL Jira], ni un problème [!DNL Jira] à plusieurs éléments [!DNL Workfront].

## Conditions d’accès

Vous devez disposer des éléments suivants :

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a></td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences Adobe [!DNL Workfront]</a></td> 
   <td> 
   <p>Nouveau : Standard<p>
   <p>Ou</p>
   <p>Actuel : formule </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accès Jira</td> 
   <td> <p>Accès pour l’administration système</p> <p><b>IMPORTANT</b>

Nous vous recommandons de créer des comptes d’administrateur ou d’administratrice système distincts dans [!DNL Jira] et [!DNL Workfront] à dédier à cette intégration, plutôt que d’utiliser des comptes existants qui peuvent être associés à des utilisateurs et utilisatrices existants.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et administratrices [!DNL Workfront], voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif complet à une personne</a>.</p> <p><b>NOTE</b>

Si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour plus d’informations sur la manière dont un un administrateur ou une administratrice de [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de pouvoir lier des éléments entre [!DNL Workfront] et [!DNL Jira], vous devez effectuer les opérations suivantes :

* Installez [!DNL Workfront] pour [!DNL Jira].

  Pour obtenir des instructions, voir [Installation d’Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurez [!DNL Workfront] pour Jira.

  Pour obtenir des instructions, voir [Configuration d’Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Lier automatiquement des éléments [!DNL Workfront] à des problèmes [!DNL Jira]

En tant qu&#39;administrateur [!DNL Workfront], vous pouvez définir des déclencheurs qui créeront automatiquement un problème dans [!DNL Jira] chaque fois que certaines conditions seront remplies sur une tâche ou un problème dans [!DNL Workfront]. Les éléments Workfront et [!DNL Jira] sont ainsi liés.

Une fois la configuration de [!DNL Workfront] pour Jira terminée, lorsqu’un élément est créé ou mis à jour dans [!DNL Workfront] pour correspondre à vos déclencheurs, un nouvel élément est automatiquement créé dans [!DNL Jira].

Les utilisateurs ou utilisatrices de Workfront qui créent et mettent à jour des éléments Workfront n’ont pas besoin d’une licence [!DNL Jira] pour déclencher la création d’éléments dans [!DNL Jira].

Pour plus d’informations, voir [Configurer [!DNL Adobe Workfront] pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Vous pouvez créer des éléments [!DNL Jira] automatiquement en associant un modèle à un projet. Si le modèle contient des tâches avec des affectations qui correspondent aux déclencheurs [!DNL Jira], les nouvelles tâches génèrent de nouveaux problèmes [!DNL Jira].

La liaison automatique d’un problème [!DNL Workfront] à un problème [!DNL Jira] est identique à la liaison automatique d’une tâche [!DNL Workfront] à un problème [!DNL Jira].

Pour lier automatiquement une tâche [!DNL Workfront] à un problème [!DNL Jira] :

1. Assurez-vous que votre administrateur ou administratrice système [!DNL Jira] a configuré des déclencheurs pour la création automatique de problèmes [!DNL Jira] lors de l’affectation d’éléments [!DNL Workfront], puis connectez-vous à [!DNL Workfront] avec un niveau d’accès qui permet de créer une tâche.

   Pour plus d’informations sur l’accès aux tâches, voir [Accorder l’accès aux tâches](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.

1. Dans le panneau de gauche Projet, sélectionnez **[!UICONTROL Tâches]**.

1. Cliquez sur **+ Nouvelle tâche**.
   >[!NOTE]
   >
   >Pour lier un élément Workfront existant à un problème Jira, sélectionnez **Modifier** dans le menu **Plus** ![Icône Plus](assets/more-icon.png) de l’élément.

1. Spécifiez ou mettez à jour l’un des champs disponibles pour la tâche.
1. Dans le champ **[!UICONTROL Affectations]**, recherchez et sélectionnez l’utilisateur, le rôle ou l’équipe spécifié comme déclencheur dans l’intégration [!DNL Jira].

1. Cliquez sur **Créer une tâche**. La tâche est créée dans Workfront et un nouveau commentaire s’affiche dans l’onglet **Mises à jour** de la tâche pour indiquer qu’un nouveau problème a également été créé dans [!DNL Jira].

1. (Facultatif) Dans la zone **[!UICONTROL Intégrations]** de la section **[!UICONTROL Détails]** de l’en-tête de tâche ou d’événement, cliquez sur le lien **[!UICONTROL Accéder à Jira]** pour ouvrir l’événement dans Jira.

   Votre administrateur ou administratrice système ou groupe doit ajouter le champ [!UICONTROL Intégrations] à votre modèle de disposition pour l’afficher dans l’en-tête de la tâche ou du problème. Pour plus d’informations, consultez [Personnalisation des en-têtes d’objet à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   N’importe quelle personne utilisant [!DNL Jira] peut immédiatement commencer à travailler sur des éléments créés automatiquement à partir de [!DNL Workfront] et leurs mises à jour seront transférées vers [!DNL Workfront] sans avoir besoin d’une licence [!DNL Workfront] pour ce faire.

   Seuls les champs que vous avez configurés en tant qu’administrateur ou administratrice [!DNL Workfront] lors de la configuration du module complémentaire de [!DNL Workfront] sont mis à jour.

   Pour plus d’informations sur la synchronisation des champs entre Workfront et Jira, consultez la section Configuration de Workfront pour Jira dans [Configuration d’Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Le problème [!DNL Jira] n’est attribué à personne dans [!DNL Jira] lorsqu’il est automatiquement créé à partir de Workfront.

## Lier manuellement des problèmes [!DNL Jira] aux éléments [!DNL Workfront]

Une fois les éléments créés dans [!DNL Jira] et [!DNL Workfront] indépendamment les uns des autres, vous pouvez lier manuellement un événement [!DNL Jira] à une tâche ou un événement [!DNL Workfront] existant.

Vous ne pouvez pas lier manuellement un élément [!DNL Workfront] à partir de [!DNL Workfront] à un élément [!DNL Jira] existant.

>[!NOTE]
>
>Si le problème [!DNL Jira] ne se trouve pas sur un projet qui n’est pas identifié comme déclencheur dans l’intégration de [!DNL Workfront], vous ne pouvez pas le lier manuellement à un élément Workfront lors de l’utilisation de l’intégration avec [!DNL Jira] On-Premise.\
>Pour plus d’informations sur la configuration des déclencheurs pour le workflow Workfront vers Jira, consultez [Lier automatiquement les éléments Workfront aux problèmes Jira](#automatically-link-workfront-items-to-jira-issues).

Lorsque les éléments [!DNL Workfront] et [!DNL Jira] sont liés, certains champs d’un élément peuvent être automatiquement mis à jour sur l’autre.\
Pour plus d’informations sur la mise à jour des éléments liés, consultez [Mettre à jour des éléments liés entre Jira et Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Pour lier manuellement des problèmes [!DNL Jira] à des éléments [!DNL Workfront] :

1. (Conditionnel) Connectez-vous à [!DNL Workfront] et recherchez un problème ou une tâche que vous souhaitez lier à un problème [!DNL Jira].
1. (Conditionnel) Dans la section **Informations de base** de l’onglet **Détails de la tâche** ou **Détails de l’événement**, copiez le **[!UICONTROL Numéro de référence]** de l’élément dans Workfront.

   Ou

   Dans la barre d’adresse de l’élément, copiez l’**URL** de l’élément dans Workfront.

   >[!IMPORTANT]
   >
   >Si votre organisation a été intégrée à l’expérience unifiée Adobe, vous devez utiliser le **Numéro de référence** pour lier les éléments Workfront à Jira. (L’option URL est disponible, mais elle renvoie une erreur si vous l’utilisez.) Pour plus d’informations sur l’expérience unifiée, voir [Expérience unifiée Adobe pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >Pour les organisations qui ne disposent pas d’une expérience unifiée Adobe, il n’est pas recommandé d’utiliser l’option URL, car les URL peuvent changer.

   >[!NOTE]
   >
   >Vous devez disposer d’une licence [!DNL Workfront] pour vous connecter à [!DNL Workfront]. Sinon, un autre utilisateur ou utilisatrice [!DNL Workfront] doit vous fournir ces informations.

1. Dans [!DNL Jira], accédez à un problème que vous souhaitez lier manuellement à l’élément [!DNL Workfront].
1. Dans le panneau de droite [!DNL Workfront], collez le **[!UICONTROL Numéro de référence]** ou le **URL** de l’élément de [!DNL Workfront] auquel vous souhaitez le lier.

1. Cliquez sur **[!UICONTROL Lien]**. Les deux éléments sont liés et le panneau de droite de [!DNL Workfront] contient les informations relatives à l’élément [!DNL Workfront].

   Par défaut, les champs de [!DNL Workfront] suivants sont visibles dans les [!DNL Jira] du panneau [!DNL Workfront] droit :

   * **[!UICONTROL Nom]** de l’élément. Vous pouvez accéder à l’élément de [!DNL Workfront] en cliquant sur son nom dans le panneau.
   * Le **[!UICONTROL Nom Du Projet]**.
   * **[!UICONTROL Statut]** de l’élément.
   * **[!UICONTROL Priorité]** de l’élément.
   * Date à laquelle elle a été créée en [!DNL Workfront].
   * **[!UICONTROL heures prévues]** de l’élément.
   * Le **[!UICONTROL Numéro De Référence]**. Vous pouvez accéder à l’élément de [!DNL Workfront] en cliquant sur le **Numéro de référence** dans le panneau.

   Pour plus d’informations sur l’activation de champs supplémentaires à afficher dans le panneau de droite, voir la section Configurer la synchronisation des champs entre les éléments [!DNL Jira] et [!DNL Workfront] dans [Configurer [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Un commentaire de l’administrateur ou l’administratrice [!DNL Workfront] associé à l’intégration est publié dans l’onglet **[!DNL Workfront]** du problème [!DNL Jira] pour confirmer qu’un nouvel élément [!DNL Jira] a été créé. Le commentaire contient un lien vers le problème [!DNL Jira].

## Dissocier des éléments entre [!DNL Jira] et [!DNL Workfront]

Les éléments liés entre [!DNL Jira] et [!DNL Workfront] peuvent être dissociés manuellement dans [!DNL Jira]. Vous ne pouvez pas dissocier un élément [!DNL Workfront] de son homologue [!DNL Jira] dans [!DNL Workfront].

Vous avez besoin de l’accès suivant pour dissocier l’élément lié manuellement :

* Vous êtes l’utilisateur qui a lié manuellement les éléments.
* Vous êtes l’administrateur système [!DNL Jira].

>[!NOTE]
>
>Un administrateur ou une administratrice [!DNL Workfront] uniquement peut dissocier des éléments qui ont été liés automatiquement.

Pour dissocier un problème [!DNL Jira] d’un élément [!DNL Workfront] :

1. Connectez-vous à Jira.
1. Accédez au problème lié à une tâche ou à un événement [!DNL Workfront].
1. Accédez au panneau de droite **Workfront**.
1. Cliquez sur l’icône **[!UICONTROL Dissocier]**, puis sur **[!UICONTROL Dissocier]**. Les éléments [!DNL Jira] et [!DNL Workfront] précédemment liés sont dissociés.

   Leurs champs, commentaires ou documents mis à jour ultérieurement ne sont pas mis à jour par rapport à leurs équivalents précédents dans l’autre application.
