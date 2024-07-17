---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Lier des éléments entre [!DNL Adobe Workfront] et [!DNL Jira]
description: Vous pouvez lier les  [!DNL Jira] problèmes aux  [!DNL Adobe Workfront] tâches ou problèmes automatiquement ou manuellement.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 8%

---

# Lier des éléments entre [!DNL Adobe Workfront] et [!DNL Jira]

Vous pouvez lier des problèmes [!DNL Jira] à des tâches [!DNL Adobe Workfront] ou des problèmes automatiquement ou manuellement.

Un seul élément de [!DNL Workfront] peut être lié à un élément de [!DNL Jira]. Vous ne pouvez jamais lier un élément [!DNL Workfront] à plusieurs problèmes [!DNL Jira], ni un problème [!DNL Jira] à plusieurs éléments [!DNL Workfront].

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans?lang=fr" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] licences </a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accès Jira</td> 
   <td> <p>Accès administrateur système</p> <p><b>IMPORTANT</b>

Nous vous recommandons de créer des comptes d’administrateur système distincts dans [!DNL Jira] et [!DNL Workfront] afin de vous consacrer à cette intégration, plutôt que d’utiliser des comptes existants qui peuvent être joints aux utilisateurs.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et les administratrices [!DNL Workfront], voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à un utilisateur ou à une utilisatrice un accès administratif complet</a>.</p> <p><b>NOTE</b>

Si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Avant de pouvoir lier des éléments entre [!DNL Workfront] et [!DNL Jira], vous devez :

* Installer [!DNL Workfront] pour [!DNL Jira]

  Pour plus d’informations sur l’installation de Workfront pour Jira, voir [Installation d’Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configuration de [!DNL Workfront] pour Jira

  Pour plus d’informations sur la configuration de Workfront pour Jira, voir [Configuration d’Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Lier automatiquement [!DNL Workfront] éléments à [!DNL Jira] problèmes

En tant qu&#39;administrateur [!DNL Workfront], vous pouvez définir des déclencheurs qui peuvent automatiquement créer un problème dans [!DNL Jira] chaque fois que certaines conditions sont remplies sur une tâche ou un problème dans [!DNL Workfront]. Les éléments Workfront et [!DNL Jira] deviennent liés.

Une fois la configuration de [!DNL Workfront] pour Jira terminée, lorsqu’un élément est créé ou mis à jour dans [!DNL Workfront] pour correspondre à vos déclencheurs, un nouvel élément est automatiquement créé dans [!DNL Jira].\
Les utilisateurs de Workfront qui créent et mettent à jour des éléments Workfront n’ont pas besoin d’une licence [!DNL Jira] pour déclencher la création d’éléments dans [!DNL Jira].

Pour plus d’informations sur la définition des déclencheurs pour la création automatique de problèmes Jira, voir [Configuration [!DNL Adobe Workfront] pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Vous pouvez créer automatiquement [!DNL Jira] éléments en joignant un modèle à un projet. Si le modèle contient des tâches avec des affectations qui répondent aux déclencheurs [!DNL Jira], les nouvelles tâches génèrent de nouveaux problèmes [!DNL Jira].

La liaison automatique d’un problème [!DNL Workfront] à un problème [!DNL Jira] est identique à la liaison automatique d’une tâche [!DNL Workfront] à un problème [!DNL Jira].

Pour associer automatiquement une tâche [!DNL Workfront] à un problème [!DNL Jira] :

1. Assurez-vous que votre administrateur système [!DNL Jira] a configuré des déclencheurs pour créer automatiquement des problèmes [!DNL Jira] lorsque des éléments [!DNL Workfront] sont affectés, puis connectez-vous à [!DNL Workfront] avec un niveau d’accès qui vous permet de créer une tâche.

   Pour plus d’informations sur l’accès aux tâches, voir [Accorder l’accès aux tâches](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Accédez à un projet et sélectionnez **[!UICONTROL Tâches]** ![](assets/tasks-icon-in-left-panel-14x14.png) dans le panneau de gauche.

1. Cliquez sur **[!UICONTROL Nouvelle tâche]**

   Ou

   Sélectionnez une tâche existante, puis cliquez sur **Modifier**.

1. Spécifiez ou mettez à jour l’un des champs disponibles pour la tâche.
1. Cliquez sur **[!UICONTROL Affectations]** et affectez la tâche à un utilisateur, un rôle ou une équipe qui est spécifié comme déclencheur dans l’intégration [!DNL Jira].

1. Cliquez sur **Enregistrer les modifications**.

   Une nouvelle tâche est créée dans Workfront.

   Dans la zone **[!UICONTROL Mises à jour]** de la nouvelle tâche, un commentaire indique qu’un nouveau problème a également été créé dans [!DNL Jira].

1. (Facultatif) Cliquez sur le lien vers le problème Jira pour l’ouvrir dans Jira.

   Ou

   Cliquez sur le lien **[!UICONTROL Aller à Jira]** dans la zone **[!UICONTROL Intégrations]** de la section **[!UICONTROL Détails]** ou dans l’en-tête de la tâche ou du problème, pour ouvrir le problème [!DNL Jira].

   L’administrateur du système ou du groupe doit ajouter le champ [!UICONTROL Intégrations] à votre modèle de mise en page pour l’afficher dans l’en-tête de la tâche ou du problème. Pour plus d’informations, voir [Personnaliser les en-têtes d’objet à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Tout utilisateur de [!DNL Jira] peut immédiatement commencer à travailler sur des éléments créés automatiquement à partir de [!DNL Workfront] et leurs mises à jour seront transférées vers [!DNL Workfront] sans avoir besoin d’une licence pour que [!DNL Workfront] puisse le faire.

   Seuls les champs que vous, administrateur [!DNL Workfront] configuré lors de la configuration du module complémentaire [!DNL Workfront] sont mis à jour.

   Pour plus d’informations sur la synchronisation des champs entre Workfront et Jira, consultez la section [Configuration de Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) dans [Configuration d’Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Le problème [!DNL Jira] n’est attribué à personne dans [!DNL Jira] lorsqu’il est automatiquement créé à partir de Workfront.

## Lier manuellement les problèmes [!DNL Jira] aux éléments [!DNL Workfront]

Une fois les éléments créés dans [!DNL Jira] et [!DNL Workfront], indépendamment les uns des autres, vous pouvez lier manuellement un problème [!DNL Jira] à une tâche ou à un problème [!DNL Workfront] existant.\
Vous ne pouvez pas lier manuellement un élément [!DNL Workfront] de [!DNL Workfront] à un élément [!DNL Jira] existant.

>[!NOTE]
>
>Si le problème [!DNL Jira] ne concerne pas un projet qui n’est pas identifié comme déclencheur dans l’intégration [!DNL Workfront], vous ne pouvez pas le lier manuellement à un élément Workfront lors de l’utilisation de l’intégration avec [!DNL Jira] On-Premise.\
>Pour plus d’informations sur la configuration des déclencheurs pour le workflow Workfront vers Jira, voir [Lier automatiquement les éléments Workfront aux problèmes Jira](#automatically-link-workfront-items-to-jira-issues).

Lorsque des éléments [!DNL Workfront] et [!DNL Jira] sont liés, certains champs d’un élément peuvent être automatiquement mis à jour sur l’autre.\
Pour plus d’informations sur la mise à jour des éléments liés, voir [Mise à jour des éléments liés entre Jira et Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Pour lier manuellement des problèmes [!DNL Jira] à des éléments [!DNL Workfront] :

1. (Conditionnel) Connectez-vous à [!DNL Workfront] et recherchez un problème ou une tâche que vous souhaitez lier au problème [!DNL Jira].
1. (Conditionnel) Dans la barre d’adresse de l’élément, copiez l’ **URL** de l’élément dans Workfront.

   Ou

   Dans la zone [!UICONTROL Details], copiez le **[!UICONTROL numéro de référence]** de l’élément dans Workfront.

   >[!NOTE]
   >
   >Vous devez disposer d’une licence [!DNL Workfront] pour vous connecter à [!DNL Workfront]. Dans le cas contraire, un utilisateur [!DNL Workfront] doit vous fournir ces informations.

1. Dans [!DNL Jira], accédez à un problème que vous souhaitez lier manuellement à l’élément [!DNL Workfront].
1. Dans le panneau de droite [!DNL Workfront], collez l’ **URL** ou le **[!UICONTROL numéro de référence]** de l’élément [!DNL Workfront] auquel vous souhaitez créer un lien.

1. Cliquez sur **[!UICONTROL Lien]**.

   Les deux éléments sont liés et le panneau de droite [!DNL Workfront] est rempli avec des informations de l’élément [!DNL Workfront].

   Les champs [!DNL Workfront] suivants sont visibles dans [!DNL Jira], par défaut, dans le panneau de droite [!DNL Workfront] :

   * **[!UICONTROL Nom]** de l’élément : vous pouvez accéder à l’élément [!DNL Workfront] en cliquant sur le nom dans le panneau.
   * **[!UICONTROL Nom du projet]**
   * **[!UICONTROL Status]** de l’élément
   * **[!UICONTROL Priorité]** de l’élément
   * Date à laquelle il a été créé dans [!DNL Workfront]
   * **[!UICONTROL Heures planifiées]** de l’élément
   * Le **[!UICONTROL numéro de référence]** : vous pouvez accéder à l’élément [!DNL Workfront] en cliquant sur le [!UICONTROL numéro de référence] dans le panneau.

Pour plus d’informations sur l’activation de champs supplémentaires à afficher dans le panneau de droite, voir la section [Configurer la synchronisation des champs entre [!DNL Jira]  et  [!DNL Workfront] Éléments](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) dans [Configurer [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) . Un commentaire de l’administrateur [!DNL Workfront] associé à l’intégration est publié dans l’onglet **[!DNL Workfront]** du problème [!DNL Jira] pour confirmer qu’un nouvel élément [!DNL Jira] a été créé. Le commentaire contient un lien vers le problème [!DNL Jira].

## Dissocier des éléments entre [!DNL Jira] et [!DNL Workfront]

Les éléments liés entre [!DNL Jira] et [!DNL Workfront] peuvent être dissociés manuellement de [!DNL Jira].\
Vous ne pouvez pas dissocier un élément [!DNL Workfront] de leur contrepartie [!DNL Jira] dans [!DNL Workfront].

Vous avez besoin de l’accès suivant pour dissocier l’élément lié manuellement :

* Vous êtes l’utilisateur qui a lié manuellement les éléments.
* Vous êtes l’administrateur système [!DNL Jira].

Seul un administrateur [!DNL Workfront] peut dissocier des éléments qui ont été automatiquement liés.

Pour dissocier un problème [!DNL Jira] d’un élément [!DNL Workfront] :

1. Dans [!DNL Jira], accédez à un problème lié à une tâche [!DNL Workfront] ou à un problème.
1. Accédez au panneau de droite [!DNL Workfront], cliquez sur l’icône **[!UICONTROL Dissocier]** , puis sur **[!UICONTROL Dissocier]**.

   Les éléments [!DNL Jira] et [!DNL Workfront] précédemment liés ne sont désormais plus liés. Les champs, commentaires ou documents qui pourraient être mis à jour individuellement à l’avenir ne sont pas mis à jour sur leur contrepartie précédente dans l’autre application.
