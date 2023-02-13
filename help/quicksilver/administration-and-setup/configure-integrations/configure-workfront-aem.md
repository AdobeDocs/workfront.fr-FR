---
title: Configurer [!DNL Workfront] avec [!DNL Adobe Experience Manager] connecteur hérité
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: En tant que [!DNL Adobe Workfront] administrateur, vous pouvez intégrer [!DNL Workfront] avec Adobe Experience Manager (AEM) Assets et fournissez à votre entreprise une solution de gestion de contenu complète pour la création, le partage et la maintenance des ressources dans votre workflow.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '1893'
ht-degree: 0%

---

# Configurer [!DNL Workfront] avec [!DNL Adobe Experience Manager] connecteur hérité

En tant que [!DNL Adobe Workfront] administrateur, vous pouvez intégrer [!DNL Workfront] avec [!UICONTROL Adobe Experience Manager (AEM) Assets] et fournir à votre entreprise une solution de gestion de contenu complète pour la création, le partage et la maintenance des ressources dans votre workflow.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## [!DNL Workfront for AEM Assets]

Le [!DNL Workfront for AEM Assets connector] permet à votre entreprise d’effectuer les opérations suivantes :

* Collaborez et gérez le contenu créatif en liant AEM ressources et dossiers aux projets, tâches, problèmes et requêtes dans [!DNL Workfront].

   Pour plus d’informations sur la configuration des intégrations de documentation avec des applications tierces, voir  [Configuration des intégrations de documents](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Intégrez à la variable [!DNL AEM Digital Asset Managemen]référentiel t (DAM), ce qui vous permet d’utiliser [!DNL Workfront] pour gérer et partager des ressources numériques stockées dans la gestion des ressources numériques.

   Pour plus d’informations sur la liaison de documents et de dossiers de ressources, voir   [Liaison de documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Combinez et appliquez des métadonnées des deux applications à une ressource.
* Affichez un flux de communication global pour une ressource. Mises à jour et commentaires effectués sur une ressource dans [!DNL Workfront] ou [!UICONTROL AEM Assets] sont synchronisés avec l’autre application, ce qui crée un historique complet des communications effectuées à la ressource.

   Pour plus d’informations sur la création de commentaires dans [!DNL Workfront], voir [Ajouter une mise à jour à un document](../../documents/managing-documents/add-update-documents.md).

## Prérequis pour l’installation du [!DNL AEM Assets] connector

Avant d’installer le [!DNL Workfront] connecteur pour [!UICONTROL AEM Assets], assurez-vous que les conditions préalables suivantes sont remplies :

* [!UICONTROL AEM Assets] installé et configuré, version 6.5 ou ultérieure. Pour plus d’informations sur l’installation [!UICONTROL AEM Assets], reportez-vous à la section [[!DNL Adobe Experience Manager] documentation](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Conditionnel) Si les règles de pare-feu n’autorisent pas le trafic comme prévu, ajoutez l’adresse IP et/ou le domaine de votre grappe à votre liste autorisée. Pour plus d’informations, voir [Configuration de la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Installez le [!DNL Workfront for AEM Assets] package connecteur {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>Les instructions suivantes concernent un [!DNL Workfront with AEM Assets] connecteur hérité qui a été remplacé par [[!DNL Workfront for Experience Manager] connecteur amélioré](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Pour plus d’informations, contactez votre représentant de compte.

Pour installer le [!DNL Workfront for AEM Assets] connecteur, vous devez importer le connecteur dans AEM sous la forme d&#39;un package à l&#39;aide de la fonction [!UICONTROL Gestionnaire de modules CRX].

1. Sur un poste de travail où vous avez déjà installé AEM, téléchargez le fichier [!DNL Workfront for AEM Assets] Fichier d&#39;installation du connecteur.

   Vous pouvez obtenir le [!DNL Workfront for AEM Assets] connecteur depuis votre [!DNL Workfront] représentant.

1. Connectez-vous à AEM à l’aide d’un compte administrateur.
1. Cliquez sur **[!UICONTROL Outils]** > **[!UICONTROL Déploiement]** > **[!UICONTROL Packages]**.

   Le [!UICONTROL Gestionnaire de modules CRX] s’ouvre.

1. Cliquez sur **[!UICONTROL Télécharger le module].**

1. Dans le [!UICONTROL Télécharger le module] , recherchez et sélectionnez la variable [!UICONTROL Connecteur Workfront] module, puis cliquez sur **[!UICONTROL OK]**.\
   Le module s’affiche dans la variable [!UICONTROL Gestionnaire de modules CRX].

1. Cliquez sur **[!UICONTROL Installer].**

1. Sur le [!UICONTROL Package] , ignorez les paramètres avancés et cliquez sur **[!UICONTROL Installer]**.
1. (Facultatif) Pour confirmer l’installation du connecteur, vérifiez que l’instruction suivante s’affiche dans la variable [!UICONTROL Journal d’activité]:

   ```
   Package installed in <time>
   ```

1. Fermez la [!UICONTROL Gestionnaire de modules CRX].

   Le connecteur est installé et vous pouvez maintenant configurer [!DNL AEM Assets] pour intégrer à [!DNL Workfront].

1. Passez à la [Configurer [!DNL AEM Assets] pour intégrer à [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## Configurer [!DNL AEM Assets] pour intégrer à [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

Après avoir installé le connecteur, importez le package connecteur pour AEM et configurez AEM pour lier les documents dans [!DNL Workfront].

Pour plus d’informations sur l’installation du connecteur, voir  [Installez le [!DNL Workfront for AEM Assets] package connecteur](#install-the-workfront-for-aem-assets-connector-package).

* [Conditions préalables](#prerequisites)
* [Intégration d’AEM à [!DNL Workfront]](#integrate-aem-with-workfront)
* [Configurez la variable [!UICONTROL Externalizer AEM]](#configure-the-aem-externalizer)

### Conditions préalables {#prerequisites}

Avant de commencer, vous devez activer les autorisations pour le service front-service :

1. Dans AEM, accédez à **[!UICONTROL Outils]**> **[!UICONTROL Sécurité]**> **[!UICONTROL Autorisations]**.
1. Dans le coin supérieur gauche, choisissez **[!UICONTROL Utilisateurs]**&#x200B; dans le menu déroulant et saisissez *[!UICONTROL workfront-service]* dans le **[!UICONTROL Rechercher]** Champ &#x200B;. Sélectionnez la [!UICONTROL workfront-service] utilisateur.
1. Dans la partie droite de l’écran, sélectionnez **[!UICONTROL Ajouter ACE]** pour créer de nouvelles entrées.
1. Dans le &#x200B;**[!UICONTROL Ajouter une nouvelle entrée]**&#x200B; fenêtre, sélectionnez l’icône de case à cocher dans la **[!UICONTROL Chemin]**&#x200B; et choisissez le dossier : */conf*
1. Dans le champ Privilèges , saisissez : *jcr:read*
1. Sélectionner **[!UICONTROL Ajouter]**&#x200B; dans le coin supérieur droit
1. (Facultatif) Répétez les étapes pour créer d’autres entrées.

### Intégration d’AEM à [!DNL Workfront] {#integrate-aem-with-workfront}

1. Connectez-vous à AEM Assets en tant qu’administrateur.
1. Cliquez sur **[!UICONTROL Outils]** >**[!UICONTROL Cloud Services]**>**[!UICONTROL Configuration de l’intégration Workfront]** >**[!UICONTROL Global-Workfront].**&#x200B;**&#x200B;**

1. (Conditionnel) Si vous ne l’avez pas encore fait, créez une [!DNL Workfront] fichier de configuration cloud.

   1. Cliquez sur  **[!UICONTROL Créer]** dans le coin supérieur droit du [!DNL Global-Workfront] page.
   1. Dans le **[!UICONTROL URL Workfront]** , spécifiez l’URL de votre [!DNL Workfront] instance.

      Par exemple : [!DNL https]:/`<account>`.my.workfront.com, où `<account>` est le compte que vous utilisez pour les intégrations avec AEM.

   1. Dans le &#x200B;**[!UICONTROL Dossier de base]** , sélectionnez l’icône de case à cocher, puis, dans le menu déroulant, sélectionnez le chemin d’accès aux documents liés. [!DNL Workfront] sont stockés.
   1. Dans le modal d’AEM qui s’affiche, suivez le chemin d’accès au dossier avec les documents auxquels vous êtes connecté. [!DNL Workfront] objets. Sélectionnez le dossier et appuyez sur **[!UICONTROL Sélectionner]**&#x200B; dans le coin supérieur droit.

      Vous pouvez créer un lien vers n’importe quel dossier sous la racine /content/dam/.

   1. Dans le **[!UICONTROL Clé API Workfront]** , indiquez vos [!UICONTROL Workfront] Clé API.

      Pour récupérer votre [!DNL Workfront] Clé API :

      1. Ouvrez un onglet de navigateur et connectez-vous à [!DNL Workfront] compte en tant que [!DNL Workfront] administrateur.
      1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

      1. Cliquez sur **[!UICONTROL Système]** >**[!UICONTROL Informations sur le client]**.

         Si vous avez déjà généré une clé API, votre [!DNL Workfront] La clé API s’affiche sous le libellé Clé API de votre utilisateur.

      1. (Conditionnel) Si vous n’avez pas encore généré de clé API, vous devez en générer une :

         1. Dans le **[!UICONTROL Paramètres de clé API]** , assurez-vous que la variable **[!UICONTROL Après la création, les clés d’API expirent dans]** est définie sur Aucun.

            Si vous sélectionnez une période d’expiration, le connecteur cessera de fonctionner après l’expiration de la clé API. Vous devrez ensuite générer à nouveau une clé API et mettre à jour votre [!DNL Workfront] configuration.

         1. Sous , **[!UICONTROL Votre clé API d’utilisateur]** libellé, cliquez sur **[!UICONTROL Générer la clé API]**.

            Une clé API pour [!DNL Workfront] génère et s’affiche.
      1. Copiez la clé API dans le presse-papiers.
      1. Ouvrez l’onglet du navigateur pour AEM Connector et dans le **[!DNL Workfront API Key]** , collez la clé API que vous avez copiée.
   1. (Conditionnel) Cliquez sur le bouton **[!UICONTROL Avancé]** dans le coin supérieur gauche de la [!UICONTROL [!DNL Workfront] Configuration de l’intégration] et sélectionnez les options suivantes, le cas échéant :

      **[!UICONTROL Autoriser la navigation dans les collections]:**&#x200B; Sélectionnez cette option si votre organisation autorise [!DNL Workfront] utilisateurs pour lier des collections AEM Assets à [!DNL Workfront] objets.

      **[!UICONTROL Federated ID utilisateur]:** Sélectionnez cette option si votre entreprise utilise des Federated ID ou une authentification unique (SSO) lors de sa connexion à Workfront.

      **[!UICONTROL Ignorer le domaine de messagerie]:** Sélectionnez cette option si vos utilisateurs AEM n’utilisent pas le nom de domaine dans leur ID utilisateur.

      **[!UICONTROL Limitation de l’accès]:** Sélectionnez cette option pour spécifier les [!DNL Workfront] Adresses IP à ajouter à la liste autorisée. Pour plus d’informations sur la liste autorisée, voir [Configuration de la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Cliquez sur le bouton **[!UICONTROL De base]** dans le coin supérieur gauche de la page Configuration de l’intégration Workfront, puis cliquez sur **[!UICONTROL Connexion]**.

      >[!NOTE]
      >
      >Les modifications peuvent prendre du temps à s’appliquer. Le redémarrage du lot peut accélérer le processus.



1. (Conditionnel) Si vous avez déjà créé une [!DNL Workfront] fichier de configuration cloud, sélectionnez **[!UICONTROL Global-[!DNL Workfront]]**, puis, dans le coin supérieur gauche, cliquez sur **[!UICONTROL Propriétés]**.

1. Générez la clé API AEM en cliquant sur **[!UICONTROL Générer la clé],** copiez ensuite la clé API AEM dans le presse-papiers.

   Vous aurez besoin de la clé API AEM ultérieurement lorsque vous configurerez [!UICONTROL Workfront] pour intégrer à [!UICONTROL AEM Assets]. Pour plus d’informations, voir [Configuration de Workfront pour l’intégration à AEM ressources](#configure-workfront-to-integrate-with-aem-assets).

1. Dans le coin supérieur droit, cliquez sur **[!UICONTROL Enregistrer]**.

   Le [!UICONTROL Global-[!DNL Workfront]] s’affiche.

   ![Properties.png](assets/properties-350x117.png)

1. (Facultatif) Synchroniser la communication bidirectionnelle entre AEM et [!DNL Workfront].

   1. Cliquez sur **[!UICONTROL Global-[!DNL Workfront]].**
   1. Dans le coin supérieur gauche de la fenêtre, cliquez sur **[!UICONTROL Propriétés]**.

      Le [!UICONTROL [!DNL Workfront] Configuration de l’intégration] s’affiche.

      ![Properties2.png](assets/properties2-350x444.png)

   1. (Facultatif) Pour activer la synchronisation des commentaires entre les [!UICONTROL AEM Assets] et [!DNL Workfront], cliquez sur **[!UICONTROL Activation de la synchronisation des commentaires]**.

      >[!IMPORTANT]
      >
      >Vous devez activer [!UICONTROL Synchronisation des documents] pour synchroniser les ressources.

   1. (Facultatif) Pour désactiver la synchronisation des commentaires, cliquez sur **[!UICONTROL Désactiver la synchronisation des commentaires].**

      Ou

      Supprimez la variable [!UICONTROL REMARQUE CREATE] abonnement d’événement enregistré sur votre instance AEM.

      Pour plus d’informations sur les abonnements aux événements, voir [API d’abonnement à un événement](../../wf-api/general/event-subs-api.md).

1. Passez à la [Configurez la variable [!UICONTROL Externalizer AEM]](#configure-the-aem-externalizer).

### Configurez la variable [!UICONTROL Externalizer AEM] {#configure-the-aem-externalizer}

Le [!UICONTROL Externalizer AEM] permet à AEM de transmettre des URL dans un format pouvant être utilisé dans [!DNL Workfront]. Si elle n’est pas correctement configurée, [!DNL Workfront] ne peut pas effectuer d’appels vers l’API AEM et les URL liant AEM documents dans Workfront ne fonctionneront pas.

1. Dans AEM, cliquez sur **[!UICONTROL Outils]** > **[!UICONTROL Opérations]** >**[!UICONTROL Console web]**.

1. Cliquez sur **[!UICONTROL OSGI]**, puis cliquez sur **[!UICONTROL Configuration]** dans le menu déroulant.

1. Dans la liste des configurations, sélectionnez &#x200B;**[!UICONTROL Externalisateur de lien Day CQ].**

   Le [!UICONTROL Externalizer] s’affiche.

1. Dans le **[!UICONTROL Domaines]** , assurez-vous que le domaine répertorié dans la section [!UICONTROL Auteur] est le nom de domaine accessible en externe aux utilisateurs AEM.

   Le nom de domaine dans la variable [!UICONTROL author] doit correspondre au domaine répertorié dans la ligne URL de votre instance AEM.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Conditionnel) Si nécessaire, mettez à jour le domaine dans la variable [!UICONTROL Auteur] champ .
1. Cliquer sur **[!UICONTROL Enregistrer]**.

   [!UICONTROL AEM Assets] est maintenant configuré pour lier des documents à [!DNL Workfront]

1. Passez à la [Configurer [!DNL Workfront] pour intégrer à [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## Configurer [!DNL Workfront] pour intégrer à [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

Après avoir installé la variable [!UICONTROL Workfront pour AEM Assets] Connecteur (comme décrit dans [Installez le [!UICONTROL Workfront pour AEM Assets] package connecteur](#install-the-workfront-for-aem-assets-connector-package)) et configurez [!UICONTROL AEM Assets] (comme décrit dans la section [Configurer[!UICONTROL  AEM Assets] pour intégrer à [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)), vous devez configurer [!DNL Workfront] pour lier des documents entre [!DNL Workfront] et [!DNL AEM Assets].

1. Connectez-vous à [!DNL Workfront] as a [!UICONTROL Workfront] administrateur.

   >[!TIP]
   >
   >[!UICONTROL Workfront] recommande de créer une [!UICONTROL Workfront] administrateur dédié uniquement à votre intégration AEM. Pour plus d’informations sur l’attribution de la variable [!UICONTROL Workfront] niveau d’accès administrateur à un utilisateur, voir [Octroi aux utilisateurs un accès administratif à certaines zones](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Documents]**> **[!UICONTROL Intégration personnalisée].**

1. Cliquez sur **[!UICONTROL Ajout d’une intégration personnalisée]**.
1. Dans le **[!UICONTROL Nom]** , indiquez le nom de l’intégration personnalisée.

   Il s’agit du nom que les utilisateurs voient lors de l’utilisation de l’intégration dans [!UICONTROL Workfront]; par exemple, vous pouvez saisir *&quot;[!DNL AEM Assets]&quot;* pour le nom.

1. Dans le **[!UICONTROL URL de l’API de base]** , spécifiez l’URL de votre instance AEM.

   L’URL de l’API de base se compose de l’URL de votre instance AEM suivie du chemin d’accès : /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. Dans le **[!UICONTROL Type d’authentification]** menu déroulant, sélectionnez **[!UICONTROL ApiKey].**

1. Dans le &#x200B;**[!UICONTROL Clé API]** , collez la clé API AEM que vous avez copiée lors de la configuration. [!UICONTROL AEM Assets].
1. Cliquer sur **[!UICONTROL Enregistrer]**.
1. (Facultatif) Assurez-vous que l’intégration est marquée [!UICONTROL Principal].\
   ![aem_custom_integration_principal.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] est maintenant configuré pour fonctionner avec [!DNL AEM Assets].

   Pour accéder aux ressources dans AEM, chaque [!DNL Workfront] un utilisateur qui doit utiliser le connecteur doit être configuré en tant qu’utilisateur dans AEM. Pour plus d’informations sur la création d’utilisateurs, voir  [Configuration des utilisateurs pour l’utilisation du connecteur](#set-up-users-to-use-the-connector).

## Configuration des utilisateurs pour l’utilisation du connecteur {#set-up-users-to-use-the-connector}

Pour que les utilisateurs puissent accéder au connecteur, ils doivent disposer d’un profil utilisateur dans AEM et appartenir à un [!DNL Workfront] groupe ayant des niveaux d’accès qui incluent la variable [!UICONTROL Créer] et [!UICONTROL Supprimer] autorisations.

Pour plus d’informations sur [!DNL Workfront] autorisations, voir [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Configuration des utilisateurs dans [!DNL AEM assets]](#set-up-users-in-aem-assets)

### Configuration des utilisateurs dans [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Connectez-vous à [!DNL AEM Assets] as a [!DNL Workfront] administrateur.
1. Cliquez sur **[!UICONTROL Outils]** >**&#x200B;**&#x200B;**[!UICONTROL Sécurité]** >**[!UICONTROL Utilisateurs]**.

1. (Conditionnel) Si l’utilisateur n’a pas de profil utilisateur dans AEM, créez un profil utilisateur AEM.

   1. Cliquez sur **[!UICONTROL Créer un utilisateur].**
   1. Renseignez les informations personnelles de l’utilisateur.

      ![64NewUser.png](assets/64newuser-350x524.png)

      Le seul champ obligatoire est le champ ID. L’identifiant AEM de l’utilisateur doit correspondre à son [!DNL Workfront] ID, qui est l’identifiant de l’utilisateur [!DNL Workfront] adresse électronique.

      Si vous avez sélectionné la variable [!UICONTROL Ignorer le domaine de messagerie] lorsque vous avez configuré AEM pour l’intégration avec [!DNL Workfront], alors l’identifiant AEM ne correspondra pas à la variable [!DNL Workfront] adresse électronique.

1. (Conditionnel) Si l’utilisateur dispose d’un profil d’AEM, ouvrez son profil d’AEM.

   1. Cliquez sur &#x200B;**[!UICONTROL Utilisateur].**

      Le [!UICONTROL Gestion des utilisateurs] s’affiche.

   1. Cliquez sur l’utilisateur à ajouter, puis cliquez sur **[!UICONTROL Propriétés]**.

      La page des paramètres de l’utilisateur s’affiche.

1. Cliquez sur le bouton **[!UICONTROL Groupes]** .

   ![](assets/groupstab.png)

1. Assurez-vous que l’utilisateur appartient à au moins une [!DNL Workfront] groupe ayant des niveaux d’accès qui incluent la variable [!UICONTROL Créer] et [!UICONTROL Supprimer] autorisations.

   1. Pour ajouter l’utilisateur à un groupe existant, commencez à saisir le nom du groupe dans le champ **[!UICONTROL Type Group Name]** , puis sélectionnez le groupe lorsqu’il apparaît dans le menu déroulant.

      Ou

      Pour sélectionner un groupe auquel l’utilisateur est membre, sélectionnez un groupe dans la variable **[!UICONTROL Groupes dont cet utilisateur est membre]** .

1. Cliquer sur **[!UICONTROL Enregistrer].**
