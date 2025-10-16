---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: 'Créer des projets  [!DNL Adobe Workfront]  à partir d’objets  [!DNL Salesforce] '
description: Après l’installation d’ [!DNL Adobe Workfront] pour Salesforce, vous pouvez définir des déclencheurs qui créent des projets  [!DNL Workfront]  lorsque certains critères sont remplis sur les Opportunités et Comptes  [!DNL Salesforce] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '1573'
ht-degree: 94%

---

# Créer des projets [!DNL Adobe Workfront] à partir d’objets [!DNL Salesforce]

>[!IMPORTANT]
>
>Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de Workfront Automation and Integration (Fusion). Dans le cadre de ce processus de transition, l’intégration de Workfront for Salesforce ne sera plus disponible après le **28 février 2026**.
>
>Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre entreprise avec Salesforce.
>
>Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez [Présentation d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Pour plus d’informations sur les fonctionnalités spécifiques des modules d’automatisation et d’intégration de Workfront pour Salesforce, consultez [Modules Salesforce](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Après l’installation d’[!DNL Adobe Workfront] pour Salesforce, vous pouvez définir des déclencheurs qui créent des projets [!DNL Workfront] lorsque certains critères sont remplis sur [!UICONTROL Opportunités] et [!UICONTROL Comptes] [!DNL Salesforce].

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Pour envoyer une demande [!DNL Workfront] à partir d’une [!UICONTROL Opportunité] ou d’un Compte [!DNL Salesforce], assurez-vous que les éléments suivants sont présents dans votre environnement :

* Votre administrateur ou administratrice [!DNL Workfront] a installé [!DNL Workfront for Salesforce].\
   Pour plus d’informations sur l’installation de [!DNL Workfront for Salesforce], voir [Installer  [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

* Votre administrateur ou administratrice [!DNL Workfront] a ajouté la section [!DNL Workfront] à vos dispositions de page [!UICONTROL Opportunité] et Compte.\
   Pour plus d’informations sur l’ajout de la section [!DNL Workfront] à une disposition de page, voir [Configurer la section  [!DNL Adobe Workfront]  pour les utilisateurs et utilisatrices de  [!DNL Salesforce] &#x200B;](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Vous avez un compte [!DNL Workfront] et vous pouvez vous y connecter à partir de la section [!DNL Workfront] dans votre [!UICONTROL Opportunité] ou Compte.

## Configurer la création de projets [!DNL Workfront] à partir de [!DNL Salesforce]

* [Comprendre la création automatique de projets](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Configurer des déclencheurs](#configuring-triggers-configuring-triggers)
* [Présentation des noms de projet](#understanding-project-names-understanding-project-names)

### Comprendre la création automatique de projets {#understanding-the-automatic-creation-of-projects}

En tant qu’administrateur ou administratrice système de [!DNL Salesforce], vous pouvez définir des déclencheurs pouvant créer automatiquement des projets dans [!DNL Workfront] lorsque les événements suivants se produisent dans [!DNL Salesforce] :

* L’[!UICONTROL étape] d’une [!UICONTROL Opportunité] est mise à jour.
* Le [!UICONTROL Type] d’un compte est mis à jour.

Les déclencheurs ne peuvent être configurés qu’après l’installation de [!DNL Workfront for Salesforce].  \
Pour plus d’informations sur l’installation de [!DNL Workfront for Salesforce], voir [Installer  [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Tenez compte des points suivants lors de la configuration de déclencheurs pour créer automatiquement des projets [!DNL Workfront] lorsque des éléments [!DNL Salesforce] sont créés ou mis à jour :

* Vous devez être un administrateur ou une administratrice système de [!DNL Salesforce] et [!DNL Workfront] pour configurer des déclencheurs.
* Une fois que vous avez configuré des déclencheurs, toute personne qui met à jour l’[!UICONTROL étape] d’une [!UICONTROL Opportunité] ou le [!UICONTROL type] d’un compte peut déclencher la création d’un projet [!DNL Workfront]. Cela inclut les utilisateurs et utilisatrices de [!DNL Salesforce] qui n’ont pas de compte [!DNL Workfront].
* Le nombre de déclencheurs que vous pouvez avoir n’est pas limité.
* Vous ne pouvez pas créer plusieurs déclencheurs en fonction des mêmes conditions. Les déclencheurs sont uniques par défaut.
* Une fois le projet créé, il est automatiquement lié à l’opportunité ou au compte sur lequel il a été généré. Une fois établi, ce lien ne peut pas être rompu.
* Une opportunité ou un compte peut être lié à plusieurs projets dans [!DNL Workfront] lorsqu’une condition déclenchée a été remplie plusieurs fois au cours de la durée de vie de l’opportunité ou du compte.

  Par exemple, si vous définissez plusieurs [!UICONTROL étapes] pour qu’une [!UICONTROL Opportunité] déclenche un projet, un projet est créé pour chaque étape définie que l’opportunité atteint, pour la durée de vie de cette opportunité. En outre, si vous mettez à jour l’[!UICONTROL étape] d’une [!UICONTROL Opportunité] en passant d’une étape définie à une autre, puis effectuez une mise à jour vers l’étape définie, un second projet est créé pour la deuxième mise à jour du champ [!UICONTROL Étape] de la même étape définie.

* Un projet dans [!DNL Workfront] ne peut être lié qu’à une seule opportunité ou à un seul compte dans [!DNL Salesforce] à un moment donné, mais pas aux deux en même temps.

### Configurer des déclencheurs {#configuring-triggers}

Une fois que vous avez configuré des déclencheurs, le processus de création de projets [!DNL Workfront] est activé pour les deux frameworks [!UICONTROL Salesforce Classic] ou [!DNL Lightning Experience].

Pour configurer des déclencheurs dans [!UICONTROL Salesforce], procédez comme suit :

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur ou administratrice système.
1. (Le cas échéant) Dans [!DNL Salesforce Classic], cliquez sur **[!UICONTROL Configuration]** et sous la section **[!UICONTROL Créer]**, développez **[!UICONTROL Éclair]**.

   Ou

   Dans Expérience éclair de [!DNL Salesforce], cliquez sur l’icône **[!UICONTROL Configuration]**, puis sur **[!UICONTROL Configuration]** et sous **[!UICONTROL OUTILS DE PLATEFORME]** développez **[!UICONTROL Applications]**.

1. Cliquez sur **[!UICONTROL Packages installés]**.

   Remarquez que le package **[!DNL Workfront]** a été installé.

1. Cliquez sur **[!UICONTROL Configurer]** en regard de **[!DNL Workfront]**.

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur ou administratrice système.

   La page **[!UICONTROL Déclencheurs]** s’affiche.

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Cliquez sur **[!UICONTROL Nouveau déclencheur]**.
1. Dans le menu déroulant Objet **[!UICONTROL [!DNL Salesforce]]**, sélectionnez **[!UICONTROL Opportunité]**.

   Champ obligatoire.

1. (Le cas échéant) Indiquez les informations suivantes :

   1. Dans le menu déroulant **[!UICONTROL Étape]**, sélectionnez une **[!UICONTROL Étape]**.

      Lorsqu’une opportunité atteint l’[!UICONTROL étape] spécifiée ici, un projet est créé dans [!DNL Workfront]. Champ obligatoire.

   1. Dans le champ **[!UICONTROL Portfolio ou programme]**, commencez à saisir le nom d’un portfolio ou d’un programme dans lequel vous souhaitez placer le projet dans [!DNL Workfront], puis sélectionnez-le lorsqu’il apparaît dans la liste.

      Si vous ne spécifiez aucun portfolio ou programme, le nouveau projet est créé et ajouté à la liste [!UICONTROL Projets dont je suis propriétaire] de la personne connectée à [!DNL Workfront] lors de la configuration des déclencheurs. Cette personne est également propriétaire du nouveau projet.

   1. Commencez à saisir le nom d’un modèle que vous souhaitez associer au nouveau projet [!DNL Workfront], puis sélectionnez-le lorsqu’il apparaît dans la liste.

      Champ obligatoire.


      >[!NOTE]
      >
      >Si vous avez spécifié une personne propriétaire de modèle sur le modèle que vous prévoyez d’utiliser pour cette intégration, elle devient la personne propriétaire du nouveau projet. Les nouveaux projets s’affichent sous la liste [!UICONTROL Projets dont je suis propriétaire] de l’utilisateur ou de l’utilisatrice propriétaire du nouveau projet, en fonction du modèle.

   1. (Facultatif) Sélectionnez le champ **[!UICONTROL Créez un projet pour chaque type de produit vendu]**, si vous souhaitez créer un projet pour chaque type de produit vendu dans le cadre d’une opportunité.
   1. (Le cas échéant) Sélectionnez un **[!UICONTROL produit]** dans le menu déroulant **[!UICONTROL Produit]**.

      Champ obligatoire.

   1. (Le cas échéant) Commencez à saisir le nom d’un **[!UICONTROL Modèle]** que vous souhaitez associer au nouveau projet [!DNL Workfront] si le produit spécifié se trouve sur l’[!UICONTROL Opportunité]. Sélectionnez le nom qui apparaît dans la liste.

      Champ obligatoire.

      Le projet créé lorsqu’un nouveau produit ajouté à l’opportunité [!DNL Salesforce] est placé dans le même portfolio ou programme sélectionné pour l’opportunité.

      >[!IMPORTANT]
      >
      >Le projet est créé uniquement lorsque l’étape est mise à jour sur l’[!UICONTROL Opportunité]. Un projet unique est créé pour chaque produit spécifié lors de la mise à jour du champ Étape, et non au fur et à mesure que les produits sont ajoutés aux [!UICONTROL Opportunités].

1. (Facultatif) Cliquez sur **[!UICONTROL Nouveau déclencheur]**.
1. (Facultatif) Dans le menu déroulant **[!UICONTROL [!DNL Salesforce]Objet]**, sélectionnez **Compte**.

   Champ obligatoire.
1. (Le cas échéant) Indiquez les informations suivantes :

   1. Sélectionnez un **[!UICONTROL Type]** de le menu déroulant **[!UICONTROL Type]**.

      Lorsqu’un **Compte** est désigné comme le **[!UICONTROL Type]** spécifié ici dans [!DNL Salesforce], un **[!UICONTROL Projet]** est créé dans [!DNL Workfront].

      Champ obligatoire.

   1. (Facultatif) Commencez à saisir le nom d’un **[!UICONTROL portfolio]** ou **[!UICONTROL programme]** où vous souhaitez placer le projet dans [!DNL Workfront] dans le champ **[!UICONTROL Portfolio ou programme]**, puis sélectionnez-le lorsqu’il apparaît dans la liste.

      Si vous ne spécifiez aucun portfolio ou programme, le nouveau projet est créé et ajouté à la liste **[!UICONTROL Projets dont je suis propriétaire]** des personnes connectées à [!DNL Workfront] à partir de [!DNL Salesforce]. La personne est également propriétaire du nouveau projet.

   1. Commencez à saisir le nom d’un **[!UICONTROL modèle]** que vous souhaitez associer au nouveau projet [!DNL Workfront], puis sélectionnez-le lorsqu’il apparaît dans la liste.

      Champ obligatoire.

      >[!NOTE]
      >
      >Si vous avez spécifié une personne propriétaire de modèle sur le modèle que vous prévoyez d’utiliser pour cette intégration, elle devient la personne propriétaire du nouveau projet. Les nouveaux projets s’affichent dans la liste **[!UICONTROL Projets dont je suis propriétaire]** de la personne propriétaire du nouveau projet, en fonction du modèle.

   ![salesforce_triggers_page_with_cleaned_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Les projets [!DNL Workfront] sont désormais générés chaque fois que l’un des déclencheurs est satisfait.

### Présentation des noms de projet {#understanding-project-names}

Selon le déclencheur qui a généré les projets, les noms des projets dans [!DNL Workfront] peuvent suivre l’un de ces modèles :

* Si le projet est créé en fonction d’une opportunité ou d’un déclencheur de compte, le nom du projet est : *`<Salesforce object name>` : `<Project template name>` (via [!DNL Salesforce])*.
* Si le projet est créé en fonction d’un déclencheur d’opportunité qui inclut également l’ajout d’un nouveau produit, le nom du projet est : *`<Salesforce object name>` : `<Salesforce product name>` (via [!DNL Salesforce])*.

## Afficher les projets [!DNL Workfront]

Si votre équipe d’administration [!DNL Workfront] a ajouté la section [!DNL Workfront] à votre disposition de page d’[!UICONTROL Opportunité] ou de compte, vous pouvez voir les projets créés automatiquement dans l’onglet [!UICONTROL Projets] de cette section.\
Pour plus d’informations sur l’ajout de la section [!DNL Workfront] à la disposition de la page d’une [!UICONTROL Opportunité] ou d’un compte, voir [Configurer la section  [!DNL Adobe Workfront]  pour les utilisateurs et utilisatrices de  [!DNL Salesforce] &#x200B;](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Vous devez disposer d’un compte [!DNL Workfront] et d’une connexion à [!DNL Workfront] pour afficher l’onglet [!UICONTROL Projets].

Pour afficher les projets créés à partir d’une [!UICONTROL Opportunité] ou d’un compte, procédez comme suit :

1. Accédez à une [!UICONTROL Opportunité] ou à un compte.
1. Accédez à la section **[!DNL Workfront]**.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur ou administratrice [!DNL Workfront] a configuré cette section. elle peut porter un nom différent.

1. Sélectionnez l’onglet **[!UICONTROL Projets]**.

   Tous les projets créés par des déclencheurs définis sont répertoriés dans cet onglet. N’importe quelle personne dans [!DNL Salesforce] qui a également un compte [!DNL Workfront] et qui peut être autorisée à voir ces projets dans [!DNL Workfront] peut également les voir dans [!DNL Salesforce] pour l’[!UICONTROL Opportunité] ou le compte qui les a générés.

   Vous pouvez afficher les informations suivantes sur les projets créés par l’intégration :

   * Nom du projet
   * Numéro de référence
   * Date d’entrée
   * Nom de la personne propriétaire
   * Statut
   * Condition
   * Date d&#39;achèvement prévue
   * Pourcentage d’achèvement

     Lorsque ces informations sont mises à jour dans [!DNL Workfront], vous pouvez voir les champs mis à jour dans cette liste.

1. (Facultatif) Cliquez sur le nom d’un projet pour l’ouvrir dans Workfront.
1. (Facultatif) Cliquez sur [!UICONTROL **[!UICONTROL Accéder à Salesforce]**] dans la zone [!UICONTROL Détails du projet] ou dans l’en-tête de projet pour accéder à l’[!UICONTROL Opportunité] ou au compte d’origine du projet. Votre administrateur ou administratrice système ou de groupes doit ajouter le champ [!UICONTROL Intégrations] à votre modèle de mise en page pour le trouver dans l’en-tête du projet.

   >[!NOTE]
   >
   >Le lien [!UICONTROL Accéder à Salesforce] est visible pour toutes les personnes utilisant [!DNL Workfront] qui peuvent afficher le projet. Vous devez disposer d’un compte [!DNL Salesforce] pour pouvoir accéder à l’opportunité ou au compte [!DNL Salesforce] à partir de l’emplacement où le projet a été généré.
