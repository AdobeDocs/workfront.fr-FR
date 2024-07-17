---
title: Configurer  [!DNL Workfront] avec  [!DNL Adobe Experience Manager] connecteur hérité
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: En tant qu'administrateur  [!DNL Adobe Workfront] , vous pouvez intégrer  [!DNL Workfront]  à Adobe Experience Manager (AEM) Assets et fournir à votre entreprise une solution de gestion de contenu complète pour la création, le partage et la maintenance des ressources dans votre workflow.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '1890'
ht-degree: 5%

---

# Configurer [!DNL Workfront] avec [!DNL Adobe Experience Manager] connecteur hérité

En tant qu’administrateur [!DNL Adobe Workfront], vous pouvez intégrer [!DNL Workfront] à [!UICONTROL Adobe Experience Manager (AEM) Assets] et fournir à votre entreprise une solution de gestion de contenu complète pour la création, le partage et la maintenance de ressources dans votre workflow.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et les administratrices [!DNL Workfront], voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à un utilisateur ou à une utilisatrice un accès administratif complet</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## [!DNL Workfront for AEM Assets]

L’ [!DNL Workfront for AEM Assets connector] permet à votre entreprise d’effectuer les opérations suivantes :

* Collaborez et gérez le contenu créatif en liant AEM ressources et dossiers aux projets, tâches, problèmes et demandes dans [!DNL Workfront].

  Pour plus d’informations sur la configuration des intégrations de documentation avec des applications tierces, voir [Configuration des intégrations de documents](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* S’intégrer au référentiel [!DNL AEM Digital Asset Managemen]t (DAM) , ce qui vous permet d’utiliser [!DNL Workfront] pour gérer et partager des ressources numériques stockées dans DAM.

  Pour plus d’informations sur la liaison de documents et de dossiers de ressources, voir   [Lier des documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Combinez et appliquez des métadonnées des deux applications à une ressource.
* Affichez un flux de communication global pour une ressource. Les mises à jour et commentaires apportés à une ressource dans [!DNL Workfront] ou [!UICONTROL AEM Assets] sont synchronisés avec l’autre application, ce qui crée un historique complet des communications effectuées à la ressource.

  Pour plus d&#39;informations sur la création de commentaires dans [!DNL Workfront], voir [Ajout d&#39;une mise à jour à un document](../../documents/managing-documents/add-update-documents.md).

## Prérequis pour l’installation du connecteur [!DNL AEM Assets]

Avant d’installer le connecteur [!DNL Workfront] pour [!UICONTROL AEM Assets], assurez-vous que les conditions préalables suivantes sont remplies :

* [!UICONTROL AEM Assets] installé et configuré, version 6.5 ou ultérieure. Pour plus d&#39;informations sur l&#39;installation de [!UICONTROL AEM Assets], consultez la [[!DNL Adobe Experience Manager] documentation](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Conditionnel) Si les règles de pare-feu n’autorisent pas le trafic comme prévu, ajoutez l’adresse IP et/ou le domaine de votre grappe à votre liste autorisée. Pour plus d’informations, voir [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Installer le package connecteur [!DNL Workfront for AEM Assets] {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>Les instructions suivantes concernent un connecteur hérité [!DNL Workfront with AEM Assets] qui a été remplacé par le [[!DNL Workfront for Experience Manager] connecteur amélioré](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Pour plus d’informations, contactez votre représentant de compte.

Pour installer le connecteur [!DNL Workfront for AEM Assets], vous devez importer le connecteur dans AEM sous la forme d’un package à l’aide du [!UICONTROL  gestionnaire de modules CRX].

1. Téléchargez le fichier d&#39;installation du connecteur [!DNL Workfront for AEM Assets] sur un poste de travail où vous avez déjà installé AEM.

   Vous pouvez obtenir le connecteur [!DNL Workfront for AEM Assets] auprès de votre représentant [!DNL Workfront].

1. Connectez-vous à AEM à l’aide d’un compte administrateur.
1. Cliquez sur **[!UICONTROL Outils]** > **[!UICONTROL Déploiement]** > **[!UICONTROL Modules]**.

   Le [!UICONTROL Gestionnaire de modules CRX] s’ouvre.

1. Cliquez sur **[!UICONTROL Télécharger le package].**

1. Dans la boîte de dialogue [!UICONTROL Télécharger le package], recherchez et sélectionnez le package [!UICONTROL Workfront Connector], puis cliquez sur **[!UICONTROL OK]**.\
   Le package s’affiche dans le [!UICONTROL Gestionnaire de modules CRX].

1. Cliquez sur **[!UICONTROL Install].**

1. Dans la boîte de dialogue [!UICONTROL Package], ignorez les paramètres avancés et cliquez sur **[!UICONTROL Installer]**.
1. (Facultatif) Pour confirmer l’installation du connecteur, assurez-vous que l’instruction suivante s’affiche dans le [!UICONTROL Journal d’activité] :

   ```
   Package installed in <time>
   ```

1. Fermez le [!UICONTROL Gestionnaire de modules CRX].

   Le connecteur est installé et vous pouvez maintenant configurer [!DNL AEM Assets] pour l’intégration à [!DNL Workfront].

1. Passez à [Configurer [!DNL AEM Assets]  pour l’intégrer à [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## Configurer [!DNL AEM Assets] à intégrer à [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

Après avoir installé le connecteur, importez le package connecteur pour AEM et configurez AEM pour qu’il se connecte aux documents dans [!DNL Workfront].

Pour plus d’informations sur l’installation du connecteur, voir [Installation du [!DNL Workfront for AEM Assets] package connecteur](#install-the-workfront-for-aem-assets-connector-package).

* [Conditions préalables](#prerequisites)
* [Intégrer l’AEM à  [!DNL Workfront]](#integrate-aem-with-workfront)
* [Configuration de l’[!UICONTROL Externalizer d’AEM]](#configure-the-aem-externalizer)

### Conditions préalables {#prerequisites}

Avant de commencer, vous devez activer les autorisations pour le service front-service :

1. Dans AEM, accédez à **[!UICONTROL Outils]**> **[!UICONTROL Sécurité]**> **[!UICONTROL Autorisations]**.
1. Dans le coin supérieur gauche, sélectionnez **[!UICONTROL Users]** &#x200B; dans le menu déroulant et saisissez *[!UICONTROL workfront-service]* dans le champ **[!UICONTROL Recherche]** &#x200B;. Sélectionnez l’utilisateur [!UICONTROL workfront-service].
1. Sur le côté droit de l’écran, sélectionnez **[!UICONTROL Ajouter ACE]** pour créer de nouvelles entrées.
1. Dans la fenêtre &#x200B;**[!UICONTROL Ajouter une nouvelle entrée]** &#x200B;, sélectionnez l’icône de case à cocher dans le champ **[!UICONTROL Chemin]** et choisissez le dossier : */conf*
1. Dans le champ Privilèges , saisissez : *jcr:read*
1. Sélectionnez **[!UICONTROL Ajouter]** &#x200B; dans le coin supérieur droit.
1. (Facultatif) Répétez les étapes pour créer d’autres entrées.

### Intégration de l’AEM avec [!DNL Workfront] {#integrate-aem-with-workfront}

1. Connectez-vous à AEM Assets en tant qu’administrateur.
1. Cliquez sur **[!UICONTROL Outils]** >**[!UICONTROL Cloud Service]**>**[!UICONTROL Configuration de l’intégration Workfront]** >**[!UICONTROL Global-Workfront].** &#x200B;**&#x200B;**

1. (Conditionnel) Si vous ne l’avez pas encore fait, créez un fichier de configuration cloud [!DNL Workfront].

   1. Cliquez sur **[!UICONTROL Créer]** dans le coin supérieur droit de la page [!DNL Global-Workfront].
   1. Dans la zone **[!UICONTROL Workfront URL]**, spécifiez l’URL de votre instance [!DNL Workfront].

      Par exemple, [!DNL https]://`<account>`.my.workfront.com, où `<account>` est le compte que vous utilisez pour les intégrations avec AEM.

   1. Dans le champ &#x200B;**[!UICONTROL Dossier de base]** , sélectionnez l’icône en forme de case à cocher, puis, dans le menu déroulant, sélectionnez le chemin d’accès où sont stockés les documents liés aux objets [!DNL Workfront].
   1. Dans le modal d’AEM qui s’affiche, suivez le chemin d’accès au dossier avec les documents connectés aux objets [!DNL Workfront]. Sélectionnez le dossier et appuyez sur **[!UICONTROL Sélectionner]** &#x200B; dans le coin supérieur droit.

      Vous pouvez créer un lien vers n’importe quel dossier sous la racine /content/dam/.

   1. Dans la zone **[!UICONTROL Workfront API Key]**, spécifiez votre clé d’API [!UICONTROL Workfront].

      Pour récupérer votre clé d’API [!DNL Workfront] :

      1. Ouvrez un onglet de navigateur et connectez-vous à votre compte [!DNL Workfront] en tant qu&#39;administrateur [!DNL Workfront].
      1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

      1. Cliquez sur **[!UICONTROL System]** >**[!UICONTROL Customer Info]**.

         Si vous avez déjà généré une clé d’API, votre clé d’API [!DNL Workfront] s’affiche sous le libellé de clé d’API de votre utilisateur.

      1. (Conditionnel) Si vous n’avez pas encore généré de clé API, vous devez en générer une :

         1. Dans la section **[!UICONTROL Paramètres de clé API]**, assurez-vous que l’option **[!UICONTROL Après la création, les clés d’API expirent dans]** est définie sur Aucun.

            Si vous sélectionnez une période d’expiration, le connecteur cessera de fonctionner après l’expiration de la clé API. Vous devrez ensuite générer à nouveau une clé API et mettre à jour votre configuration [!DNL Workfront].

         1. Sous l’étiquette **[!UICONTROL Your User’s API Key]**, cliquez sur **[!UICONTROL Générer la clé API]**.

            Une clé API pour [!DNL Workfront] génère et s’affiche.
      1. Copiez la clé API dans le presse-papiers.
      1. Ouvrez l’onglet du navigateur pour AEM Connector et, dans la zone **[!DNL Workfront API Key]**, collez la clé API que vous avez copiée.
   1. (Conditionnel) Cliquez sur l’onglet **[!UICONTROL Avancé]** dans le coin supérieur gauche de la page [!UICONTROL [!DNL Workfront] Configuration de l’intégration ] et sélectionnez les options suivantes, le cas échéant :

      **[!UICONTROL Autoriser la navigation dans les collections] :** &#x200B; Sélectionnez cette option si votre organisation permet à [!DNL Workfront] utilisateurs de lier les collections AEM Assets à [!DNL Workfront] objets.

      **[!UICONTROL Federated ID utilisateur] :** Sélectionnez cette option si votre entreprise utilise des Federated ID ou une authentification unique (SSO) lors de sa connexion à Workfront.

      **[!UICONTROL Ignorer le domaine de messagerie] :** Sélectionnez cette option si vos utilisateurs AEM n’utilisent pas le nom de domaine dans leur ID utilisateur.

      **[!UICONTROL Limiter l’accès] :** Sélectionnez cette option pour spécifier les [!DNL Workfront] adresses IP appropriées à ajouter à la liste autorisée. Pour plus d’informations sur la liste autorisée, voir [Configuration de la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Cliquez sur l’onglet **[!UICONTROL Basic]** dans le coin supérieur gauche de la page Configuration de l’intégration Workfront, puis cliquez sur **[!UICONTROL Connect]**.

      >[!NOTE]
      >
      >Les modifications peuvent prendre un certain temps pour s’appliquer. Le redémarrage du lot peut accélérer le processus.



1. (Conditionnel) Si vous avez déjà créé un fichier de configuration cloud [!DNL Workfront], sélectionnez **[!UICONTROL Global-[!DNL Workfront]]**, puis, dans le coin supérieur gauche, cliquez sur **[!UICONTROL Propriétés]**.

1. Générez la clé d’API AEM en cliquant sur **[!UICONTROL Générer la clé],**, puis copiez la clé d’API AEM dans votre presse-papiers.

   Vous aurez besoin de la clé API d’AEM ultérieurement lorsque vous configurerez [!UICONTROL Workfront] pour l’intégration à [!UICONTROL AEM Assets]. Pour plus d’informations, voir [Configuration de Workfront pour l’intégration avec AEM ressources](#configure-workfront-to-integrate-with-aem-assets).

1. Dans le coin supérieur droit, cliquez sur **[!UICONTROL Enregistrer]**.

   La fenêtre [!UICONTROL Global-[!DNL Workfront]] s’affiche.

   ![Properties.png](assets/properties-350x117.png)

1. (Facultatif) Synchronisez la communication bidirectionnelle entre AEM et [!DNL Workfront].

   1. Cliquez sur **[!UICONTROL Global-[!DNL Workfront]].**
   1. Dans le coin supérieur gauche de la fenêtre, cliquez sur **[!UICONTROL Propriétés]**.

      La page [!UICONTROL [!DNL Workfront] Configuration de l’intégration ] s’affiche.

      ![Properties2.png](assets/properties2-350x444.png)

   1. (Facultatif) Pour activer la synchronisation des commentaires entre [!UICONTROL AEM Assets] et [!DNL Workfront], cliquez sur **[!UICONTROL Activer la synchronisation des commentaires]**.

      >[!IMPORTANT]
      >
      >Vous devez activer la [!UICONTROL synchronisation du document] pour synchroniser les ressources.

   1. (Facultatif) Pour désactiver la synchronisation des commentaires, cliquez sur **[!UICONTROL Désactiver la synchronisation des commentaires].**

      Ou

      Supprimez l&#39;abonnement à l&#39;événement [!UICONTROL REMARQUE CREATE] enregistré sur votre instance AEM.

      Pour plus d’informations sur les abonnements aux événements, voir [API d’abonnement à un événement](../../wf-api/general/event-subs-api.md).

1. Passez à [Configuration de l’externaliseur d’AEM [!UICONTROL .]](#configure-the-aem-externalizer)

### Configuration de l’[!UICONTROL Externalizer d’AEM] {#configure-the-aem-externalizer}

L’externaliseur d’AEM [!UICONTROL  permet à AEM de transmettre des URL dans un format utilisable dans [!DNL Workfront]. ] Si la configuration n’est pas correcte, [!DNL Workfront] ne peut pas appeler l’API AEM et les URL liant AEM documents dans Workfront ne fonctionneront pas.

1. Dans AEM, cliquez sur **[!UICONTROL Outils]** > **[!UICONTROL Opérations]** >**[!UICONTROL Console web]**.

1. Cliquez sur **[!UICONTROL OSGI]**, puis sur **[!UICONTROL Configuration]** dans le menu déroulant.

1. Dans la liste de configuration, sélectionnez &#x200B;**[!UICONTROL Day CQ Link Externalizer].**

   La page [!UICONTROL Externalizer] s’affiche.

1. Dans la section **[!UICONTROL Domaines]** , assurez-vous que le domaine répertorié dans le champ [!UICONTROL Auteur] est le nom de domaine accessible en externe pour AEM utilisateurs.

   Le nom de domaine dans le champ [!UICONTROL author] doit correspondre au domaine répertorié dans la ligne d’URL de votre instance AEM.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Conditionnel) Si nécessaire, mettez à jour le domaine dans le champ [!UICONTROL Auteur] .
1. Cliquer sur **[!UICONTROL Enregistrer]**.

   [!UICONTROL AEM Assets] est maintenant configuré pour lier des documents à [!DNL Workfront]

1. Passez à [Configurer [!DNL Workfront]  pour l’intégrer à [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## Configurer [!DNL Workfront] à intégrer à [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

Après avoir installé le connecteur [!UICONTROL Workfront for AEM Assets] (comme décrit dans [Installation du package connecteur [!UICONTROL Workfront for AEM Assets]](#install-the-workfront-for-aem-assets-connector-package)) et configuré [!UICONTROL AEM Assets] (comme décrit dans [Configuration[!UICONTROL  d’AEM Assets] pour l’intégration avec  [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)), vous devez configurer [!DNL Workfront] pour lier des documents entre [!DNL Workfront] et [!DNL AEM Assets] 4}.

1. Connectez-vous à [!DNL Workfront] en tant qu&#39;administrateur [!UICONTROL Workfront].

   >[!TIP]
   >
   >[!UICONTROL Workfront] recommande de créer un administrateur [!UICONTROL Workfront] dédié uniquement à votre intégration AEM. Pour plus d&#39;informations sur l&#39;attribution du niveau d&#39;accès administrateur [!UICONTROL Workfront] à un utilisateur, voir [Octroi aux utilisateurs d&#39;un accès administratif à certaines zones](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Documents]**> **[!UICONTROL Intégration personnalisée].**

1. Cliquez sur **[!UICONTROL Ajouter une intégration personnalisée]**.
1. Dans la zone **[!UICONTROL Name]**, indiquez le nom de l’intégration personnalisée.

   Il s’agit du nom que les utilisateurs voient lors de l’utilisation de l’intégration dans [!UICONTROL Workfront] ; par exemple, vous pouvez saisir *&quot;[!DNL AEM Assets]&quot;* pour le nom.

1. Dans la zone **[!UICONTROL URL de l’API de base]**, spécifiez l’URL de votre instance AEM.

   L’URL de l’API de base se compose de l’URL de votre instance AEM suivie du chemin d’accès : /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. Dans le menu déroulant **[!UICONTROL Type d&#39;authentification]**, sélectionnez **[!UICONTROL ApiKey].**

1. Dans la zone &#x200B;**[!UICONTROL Clé API]**, collez la clé API AEM que vous avez copiée lorsque vous avez configuré [!UICONTROL AEM Assets].
1. Cliquer sur **[!UICONTROL Enregistrer]**.
1. (Facultatif) Assurez-vous que l’intégration est marquée comme [!UICONTROL Active].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] est désormais configuré pour fonctionner avec [!DNL AEM Assets].

   Pour accéder aux ressources dans AEM, chaque utilisateur [!DNL Workfront] qui doit utiliser le connecteur doit être configuré en tant qu’utilisateur dans AEM. Pour plus d&#39;informations sur la création d&#39;utilisateurs, voir [Configuration des utilisateurs pour utiliser le connecteur](#set-up-users-to-use-the-connector).

## Configuration des utilisateurs pour l’utilisation du connecteur {#set-up-users-to-use-the-connector}

Pour que les utilisateurs puissent accéder au connecteur, ils doivent disposer d’un profil utilisateur dans AEM et appartenir à un groupe [!DNL Workfront] dont les niveaux d’accès incluent les autorisations [!UICONTROL Create] et [!UICONTROL Delete].

Pour plus d’informations sur les autorisations [!DNL Workfront], voir [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Configuration des utilisateurs dans [!DNL AEM assets]](#set-up-users-in-aem-assets)

### Configuration des utilisateurs dans [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Connectez-vous à [!DNL AEM Assets] en tant qu’administrateur [!DNL Workfront].
1. Cliquez sur **[!UICONTROL Outils]** >**&#x200B;** &#x200B;**[!UICONTROL Sécurité]** >**[!UICONTROL Utilisateurs]**.

1. (Conditionnel) Si l’utilisateur n’a pas de profil utilisateur dans AEM, créez un profil utilisateur AEM.

   1. Cliquez sur **[!UICONTROL Créer un utilisateur].**
   1. Saisissez les informations personnelles de l’utilisateur.

      ![64NewUser.png](assets/64newuser-350x524.png)

      Le seul champ obligatoire est le champ ID. L’ID d’AEM de l’utilisateur doit correspondre à son ID [!DNL Workfront], qui est l’adresse électronique de l’utilisateur [!DNL Workfront].

      Si vous avez sélectionné l’option [!UICONTROL Ignorer le domaine de messagerie] lorsque vous avez configuré l’AEM à intégrer à [!DNL Workfront], l’ID d’AEM ne correspondra pas à l’adresse électronique [!DNL Workfront].

1. (Conditionnel) Si l’utilisateur dispose d’un profil d’AEM, ouvrez son profil d’AEM.

   1. Cliquez sur &#x200B;**[!UICONTROL User].**

      La page [!UICONTROL User Management] s’affiche.

   1. Cliquez sur l’utilisateur que vous souhaitez ajouter, puis sur **[!UICONTROL Propriétés]**.

      La page des paramètres de l’utilisateur s’affiche.

1. Cliquez sur l’onglet **[!UICONTROL Groupes]** .

   ![](assets/groupstab.png)

1. Assurez-vous que l’utilisateur appartient à au moins un groupe [!DNL Workfront] disposant de niveaux d’accès comprenant les autorisations [!UICONTROL Create] et [!UICONTROL Delete] .

   1. Pour ajouter l’utilisateur à un groupe existant, commencez à saisir le nom du groupe dans la zone **[!UICONTROL Type Group Name]**, puis sélectionnez le groupe lorsqu’il apparaît dans le menu déroulant.

      Ou

      Pour sélectionner un groupe auquel l’utilisateur est membre, sélectionnez un groupe dans la section **[!UICONTROL Groupes auxquels cet utilisateur est membre de]** .

1. Cliquez sur **[!UICONTROL Enregistrer].**
