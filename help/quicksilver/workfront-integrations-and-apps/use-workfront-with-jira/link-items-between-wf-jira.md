---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Lier des éléments entre  [!DNL Adobe Workfront]  et  [!DNL Jira]
description: Vous pouvez lier des problèmes  [!DNL Jira]  à des tâches ou problèmes  [!DNL Adobe Workfront]  automatiquement ou manuellement.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 89%

---

# Lier des éléments entre [!DNL Adobe Workfront] et [!DNL Jira]

Vous pouvez lier des problèmes [!DNL Jira] à des tâches ou problèmes [!DNL Adobe Workfront] automatiquement ou manuellement.

Un seul élément dans [!DNL Workfront] peut être lié à un élément dans [!DNL Jira]. Vous ne pouvez jamais lier un élément [!DNL Workfront] à plusieurs problèmes [!DNL Jira], ni un problème [!DNL Jira] à plusieurs éléments [!DNL Workfront].

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences Adobe [!DNL Workfront]</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accès Jira</td> 
   <td> <p>Accès pour l’administration système</p> <p><b>IMPORTANT</b>

Nous vous recommandons de créer des comptes d’administrateur ou d’administratrice système distincts dans [!DNL Jira] et [!DNL Workfront] à dédier à cette intégration, plutôt que d’utiliser des comptes existants qui peuvent être associés à des utilisateurs et utilisatrices existants.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et administratrices [!DNL Workfront], voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif complet à une personne</a>.</p> <p><b>NOTE</b>

Si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Avant de pouvoir lier des éléments entre [!DNL Workfront] et [!DNL Jira], vous devez effectuer les actions suivantes :

* Installer [!DNL Workfront] pour [!DNL Jira].

  Pour obtenir des instructions sur l’installation de Workfront pour Jira, voir [Installer Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurer [!DNL Workfront] pour Jira.

  Pour obtenir des instructions sur la configuration de Workfront pour Jira, voir [Configurer Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Lier automatiquement des éléments [!DNL Workfront] à des problèmes [!DNL Jira]

En tant qu’administrateur ou administratrice [!DNL Workfront], vous pouvez définir des déclencheurs permettant de créer automatiquement un problème dans [!DNL Jira] chaque fois que certaines conditions sont remplies sur une tâche ou un problème dans [!DNL Workfront]. Les éléments Workfront et [!DNL Jira] sont ainsi liés.

Une fois la configuration de [!DNL Workfront] pour Jira terminée, lorsqu’un élément est créé ou mis à jour dans [!DNL Workfront] pour correspondre à vos déclencheurs, un nouvel élément est automatiquement créé dans [!DNL Jira].\
Les utilisateurs ou utilisatrices de Workfront qui créent et mettent à jour des éléments Workfront n’ont pas besoin d’une licence [!DNL Jira] pour déclencher la création d’éléments dans [!DNL Jira].

Pour plus d’informations sur la définition de déclencheurs pour la création automatique de problèmes Jira, voir [Configurer  [!DNL Adobe Workfront]  pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Vous pouvez créer des éléments [!DNL Jira] automatiquement en associant un modèle à un projet. Si le modèle contient des tâches avec des affectations qui correspondent aux déclencheurs [!DNL Jira], les nouvelles tâches génèrent de nouveaux problèmes [!DNL Jira].

La liaison automatique d’un problème [!DNL Workfront] à un problème [!DNL Jira] est identique à la liaison automatique d’une tâche [!DNL Workfront] à un problème [!DNL Jira].

Pour lier automatiquement une tâche [!DNL Workfront] à un problème [!DNL Jira] :

1. Assurez-vous que votre administrateur ou administratrice système [!DNL Jira] a configuré des déclencheurs pour la création automatique de problèmes [!DNL Jira] lors de l’affectation d’éléments [!DNL Workfront], puis connectez-vous à [!DNL Workfront] avec un niveau d’accès qui permet de créer une tâche.

   Pour plus d’informations sur l’accès aux tâches, voir [Accorder l’accès aux tâches](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Accédez à un projet et sélectionnez **[!UICONTROL Tâches]** ![Icône Tâches](assets/tasks-icon-in-left-panel-14x14.png) dans le panneau de gauche.

1. Cliquez sur **[!UICONTROL Nouvelle tâche]**.

   Ou

   Sélectionnez une tâche existante, puis cliquez sur **Modifier**.

1. Spécifiez ou mettez à jour l’un des champs disponibles pour la tâche.
1. Cliquez sur **[!UICONTROL Affectations]** et affectez la tâche à un utilisateur ou une utilisatrice, un rôle ou une équipe spécifié(e) comme déclencheur dans l’intégration [!DNL Jira].

1. Cliquez sur **Enregistrer les modifications**.

   Une nouvelle tâche est créée dans Workfront.

   Dans la zone **[!UICONTROL Mises à jour]** de la nouvelle tâche, un commentaire indique qu’un nouveau problème a également été créé dans [!DNL Jira].

1. (Facultatif) Cliquez sur le lien vers le problème Jira pour l’ouvrir dans Jira.

   Ou

   Cliquez sur le lien **[!UICONTROL Accéder à Jira]** dans la zone **[!UICONTROL Intégrations]** de la section **[!UICONTROL Détails]** ou de l’en-tête de la tâche ou du problème pour ouvrir le problème [!DNL Jira].

   Votre administrateur ou administratrice système ou groupe doit ajouter le champ [!UICONTROL Intégrations] à votre modèle de disposition pour l’afficher dans l’en-tête de la tâche ou du problème. Pour plus d’informations, consultez [Personnalisation des en-têtes d’objet à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   N’importe quelle personne utilisant [!DNL Jira] peut immédiatement commencer à travailler sur des éléments créés automatiquement à partir de [!DNL Workfront] et leurs mises à jour seront transférées vers [!DNL Workfront] sans avoir besoin d’une licence [!DNL Workfront] pour ce faire.

   Seuls les champs que vous avez configurés en tant qu’administrateur ou administratrice [!DNL Workfront] lors de la configuration du module complémentaire de [!DNL Workfront] sont mis à jour.

   Pour plus d’informations sur la synchronisation de champs entre Workfront et Jira, consultez la section [Configuration de Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) dans [Configuration d’Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Le problème [!DNL Jira] n’est attribué à personne dans [!DNL Jira] lorsqu’il est automatiquement créé à partir de Workfront.

## Lier manuellement des problèmes [!DNL Jira] aux éléments [!DNL Workfront]

Une fois les éléments créés dans [!DNL Jira] et [!DNL Workfront], indépendamment l’un de l’autre, vous pouvez lier manuellement un problème [!DNL Jira] lié à une tâche ou un problème [!DNL Workfront] qui existe déjà.\
Vous ne pouvez pas lier manuellement un élément [!DNL Workfront] à partir de [!DNL Workfront] à un élément [!DNL Jira] existant.

>[!NOTE]
>
>Si le problème [!DNL Jira] ne se trouve pas sur un projet qui n’est pas identifié comme déclencheur dans l’intégration de [!DNL Workfront], vous ne pouvez pas le lier manuellement à un élément Workfront lors de l’utilisation de l’intégration avec [!DNL Jira] On-Premise.\
>Pour plus d’informations sur la configuration des déclencheurs pour le workflow Workfront vers Jira, consultez [Lier automatiquement les éléments Workfront aux problèmes Jira](#automatically-link-workfront-items-to-jira-issues).

Lorsque les éléments [!DNL Workfront] et [!DNL Jira] sont liés, certains champs d’un élément peuvent être automatiquement mis à jour sur l’autre.\
Pour plus d’informations sur la mise à jour des éléments liés, consultez [Mettre à jour des éléments liés entre Jira et Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Pour lier manuellement des problèmes [!DNL Jira] à des éléments [!DNL Workfront] :

1. (Le cas échéant) Connectez-vous à [!DNL Workfront] et recherchez un problème ou une tâche que vous souhaitez lier à un problème [!DNL Jira].
1. (Conditionnel) Dans la zone [!UICONTROL Détails], copiez le **[!UICONTROL Numéro de référence]** de l’élément dans Workfront.

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
1. Dans le panneau de droite [!DNL Workfront], collez le **[!UICONTROL Numéro de référence]** ou le **URL** de l’élément de [!DNL Workfront] auquel vous souhaitez créer un lien.

1. Cliquez sur **[!UICONTROL Lier]**.

   Les deux éléments sont liés et le panneau de droite de [!DNL Workfront] contient les informations relatives à l’élément [!DNL Workfront].

   Les champs [!DNL Workfront] suivants sont visibles dans [!DNL Jira], par défaut, dans le panneau de droite de [!DNL Workfront] :

   * **[!UICONTROL Nom]** de l’élément : vous pouvez accéder à l’élément [!DNL Workfront] en cliquant sur son nom dans le panneau.
   * **[!UICONTROL Nom du projet]**
   * **[!UICONTROL Statut]** de l’élément
   * **[!UICONTROL Priorité]** de l’élément
   * Date à laquelle il a été créé dans [!DNL Workfront]
   * **[!UICONTROL Nombre d’heures prévues]** de l’élément
   * **[!UICONTROL Numéro de référence]** : vous pouvez accéder à l’élément [!DNL Workfront] en cliquant sur [!UICONTROL Numéro de référence] dans le panneau.

Pour plus d’informations sur l’activation de champs supplémentaires à afficher dans le panneau de droite, consultez la section [Configurer la synchronisation des champs entre  [!DNL Jira]  et les éléments  [!DNL Workfront] ](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) dans [Configurer [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Un commentaire de l’administrateur ou l’administratrice [!DNL Workfront] associé à l’intégration est publié dans l’onglet **[!DNL Workfront]** du problème [!DNL Jira] pour confirmer qu’un nouvel élément [!DNL Jira] a été créé. Le commentaire contient un lien vers le problème [!DNL Jira].

## Dissocier des éléments entre [!DNL Jira] et [!DNL Workfront]

Des éléments liés entre [!DNL Jira] et [!DNL Workfront] peuvent être dissociés manuellement de [!DNL Jira].\
Vous ne pouvez pas dissocier un élément [!DNL Workfront] de son homologue [!DNL Jira] dans [!DNL Workfront].

Vous avez besoin de l’accès suivant pour dissocier l’élément lié manuellement :

* Vous êtes l’utilisateur ou l’utilisatrice qui a lié manuellement les éléments.
* Vous êtes l’administrateur ou l’administratrice système [!DNL Jira].

Un administrateur ou une administratrice [!DNL Workfront] uniquement peut dissocier des éléments qui ont été liés automatiquement.

Pour dissocier un problème [!DNL Jira] d’un élément [!DNL Workfront] :

1. Dans [!DNL Jira], accédez à un problème lié à une tâche ou un problème [!DNL Workfront].
1. Accédez au panneau de droite de [!DNL Workfront], cliquez sur l’icône **[!UICONTROL Dissocier]** puis cliquez sur **[!UICONTROL Dissocier]**.

   Les éléments précédemment liés [!DNL Jira] et [!DNL Workfront] ne sont désormais plus liés. Les champs, commentaires ou documents qui pourraient être mis à jour individuellement à l’avenir ne sont pas mis à jour sur leur homologue précédent dans l’autre application.
