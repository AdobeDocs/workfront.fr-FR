---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Créer des  [!DNL Adobe Workfront]  projets à partir d'objets  [!DNL Salesforce]
description: Après avoir installé  [!DNL Adobe Workfront] pour Salesforce, vous pouvez définir des déclencheurs qui créent des projets  [!DNL Workfront] lorsque certains critères sont satisfaits sur [!DNL Salesforce] Opportunités et comptes.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 5%

---

# Créer des projets [!DNL Adobe Workfront] à partir d’objets [!DNL Salesforce]

Après avoir installé [!DNL Adobe Workfront] pour Salesforce, vous pouvez définir des déclencheurs qui créent des projets [!DNL Workfront] lorsque certains critères sont satisfaits sur les [!DNL Salesforce] [!UICONTROL opportunités] et les [!UICONTROL comptes].

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Pour envoyer une requête [!DNL Workfront] à partir d&#39;une [!DNL Salesforce] [!UICONTROL Opportunity] ou d&#39;un compte
vérifiez que vous disposez des éléments suivants dans votre environnement :

* Votre administrateur [!DNL Workfront] a installé [!DNL Workfront for Salesforce].\
   Pour plus d&#39;informations sur l&#39;installation de [!DNL Workfront for Salesforce], voir [Installation [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Votre administrateur [!DNL Workfront] a ajouté la section [!DNL Workfront] à votre [!UICONTROL opportunité] et votre compte
mises en page.\
   Pour plus d’informations sur l’ajout de la section [!DNL Workfront] à une mise en page, voir [Configuration de la section  [!DNL Adobe Workfront] pour les  [!DNL Salesforce] utilisateurs](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Vous disposez d&#39;un compte [!DNL Workfront] et vous pouvez vous y connecter à partir de la section [!DNL Workfront] de votre [!UICONTROL Opportunité] ou de votre compte
.

## Configuration de la création de [!DNL Workfront] projets à partir de [!DNL Salesforce]

* [Présentation de la création automatique de projets](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Configuration des Triggers](#configuring-triggers-configuring-triggers)
* [Présentation des noms de projet](#understanding-project-names-understanding-project-names)

### Présentation de la création automatique de projets {#understanding-the-automatic-creation-of-projects}

En tant qu&#39;administrateur système [!DNL Salesforce], vous pouvez définir des déclencheurs qui peuvent automatiquement créer des projets dans [!DNL Workfront] lorsque les événements suivants se produisent dans [!DNL Salesforce] :

* L’ [!UICONTROL état] d’une [!UICONTROL opportunité] est mis à jour.
* [!UICONTROL Type] d’un compte
est mise à jour.

Les déclencheurs ne peuvent être configurés qu&#39;après l&#39;installation de [!DNL Workfront for Salesforce].  \
Pour plus d&#39;informations sur l&#39;installation de [!DNL Workfront for Salesforce], voir [Installation [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Tenez compte de ce qui suit lors de la configuration des déclencheurs pour créer automatiquement des projets [!DNL Workfront] lorsque des éléments [!DNL Salesforce] sont créés ou mis à jour :

* Pour configurer des déclencheurs, vous devez être un administrateur système [!DNL Salesforce] et [!DNL Workfront].
* Une fois que vous avez configuré les déclencheurs, toute personne qui met à jour l’[!UICONTROL état] d’une [!UICONTROL opportunité] ou le [!UICONTROL type] d’un compte
peut déclencher la création d’un projet [!DNL Workfront]. Cela inclut les utilisateurs de [!DNL Salesforce] qui n&#39;ont pas de compte [!DNL Workfront].
* Le nombre de déclencheurs que vous pouvez avoir n’est pas limité.
* Vous ne pouvez pas créer plusieurs déclencheurs en fonction des mêmes conditions. Les déclencheurs sont uniques par défaut.
* Une fois le projet créé, il est automatiquement lié à l&#39;opportunité ou au compte sur lequel il a été généré. Une fois établi, ce lien ne peut pas être rompu.
* Une opportunité ou un compte peut être lié à plusieurs projets dans [!DNL Workfront] lorsqu’une condition déclenchée a été remplie plusieurs fois au cours de la vie de l’opportunité ou du compte.

  Par exemple, si vous définissez plusieurs [!UICONTROL Étape] pour qu’une [!UICONTROL Opportunité] déclenche un projet, un projet est créé pour chaque étape définie à laquelle l’opportunité atteint, pour la durée de vie de cette opportunité. En outre, si vous mettez à jour l’[!UICONTROL état] d’une [!UICONTROL opportunité] d’une étape définie vers une autre, puis que vous la remettez à jour vers l’étape définie, un deuxième projet est créé pour la deuxième fois que vous mettez à jour le champ [!UICONTROL état] vers la même étape définie.

* Un projet de [!DNL Workfront] ne peut être lié qu’à une seule opportunité ou à un seul compte de [!DNL Salesforce] à un moment donné, mais pas aux deux en même temps.

### Configuration des Triggers {#configuring-triggers}

Une fois que vous avez configuré les déclencheurs, le processus de création de projets [!DNL Workfront] est activé pour les structures [!UICONTROL Salesforce Classic] ou [!DNL Lightning Experience].

Pour configurer des déclencheurs dans [!UICONTROL Salesforce] :

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur système.
1. (Conditionnel) Dans [!DNL Salesforce Classic], cliquez sur **[!UICONTROL Configuration]**, puis, sous la section **[!UICONTROL Build]** , développez **[!UICONTROL Éclair de foudre]**.

   Ou

   Dans [!DNL Salesforce] Lightning Experience, cliquez sur l&#39;icône **[!UICONTROL Setup]**, puis sur **[!UICONTROL Setup]**, et sous **[!UICONTROL PLATFORM TOOLS]**, développez **[!UICONTROL Apps]**.

1. Cliquez sur **[!UICONTROL Packages installés]**.

   Notez que le package **[!DNL Workfront]** a été installé.

1. Cliquez sur **[!UICONTROL Configurer]** en regard de **[!DNL Workfront]**.

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur système.

   La page **[!UICONTROL Triggers]** s’affiche.

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Cliquez sur **[!UICONTROL New Trigger]**.
1. Dans le menu déroulant **[!UICONTROL [!DNL Salesforce]Object]**, sélectionnez **[!UICONTROL Opportunity]**.

   Il s’agit d’un champ obligatoire.

1. (Conditionnel) Indiquez les informations suivantes :

   1. Dans le menu déroulant **[!UICONTROL Stage]**, sélectionnez un **[!UICONTROL Stage]**.\

      Lorsqu’une opportunité atteint l’[!UICONTROL état] spécifié ici, un projet est créé dans [!DNL Workfront]. Il s’agit d’un champ obligatoire.

   1. Dans le champ **[!UICONTROL Portfolio ou Programme]** , commencez à saisir le nom d’un Portfolio ou d’un programme dans lequel vous souhaitez que le projet soit placé dans [!DNL Workfront], puis sélectionnez-le lorsqu’il apparaît dans la liste.\

      Si vous ne spécifiez aucun Portfolio ou programme, le nouveau projet est créé et ajouté à la liste [!UICONTROL Projets que je possède] de l’utilisateur connecté à [!DNL Workfront] lors de la configuration des déclencheurs. Cet utilisateur est également le propriétaire du projet.

   1. Commencez à saisir le nom d’un modèle que vous souhaitez associer au nouveau projet [!DNL Workfront], puis sélectionnez-le lorsqu’il apparaît dans la liste.\

      Il s’agit d’un champ obligatoire.


      >[!NOTE]
      >
      >Si vous avez spécifié un propriétaire de modèle sur le modèle que vous prévoyez d’utiliser pour cette intégration, cela devient le propriétaire du projet du nouveau projet. Les nouveaux projets apparaissent sous la liste [!UICONTROL Projets que je possède] de l’utilisateur propriétaire du nouveau projet, selon le modèle.

   1. (Facultatif) Sélectionnez le champ **[!UICONTROL Créer un projet pour chaque type de produit vendu]** si vous souhaitez créer un projet pour chaque type de produit vendu à une occasion donnée.
   1. (Conditionnel) Sélectionnez un **[!UICONTROL Produit]** dans le menu déroulant **[!UICONTROL Produit]** .

      Il s’agit d’un champ obligatoire.

   1. (Conditionnel) Commencez à saisir le nom d’un **[!UICONTROL modèle]** que vous souhaitez associer au nouveau projet [!DNL Workfront] si le produit spécifié se trouve sur l’ [!UICONTROL opportunité]. Sélectionnez-le lorsqu’il apparaît dans la liste.

      Il s’agit d’un champ obligatoire.

      Le projet créé lorsqu’un nouveau produit est ajouté à l’opportunité [!DNL Salesforce] est placé dans le même Portfolio ou programme que celui sélectionné pour l’opportunité.

      >[!IMPORTANT]
      >
      >Le projet est créé uniquement lorsque l’étape est mise à jour sur l’ [!UICONTROL opportunité]. Un projet unique est créé pour chaque produit spécifié lorsque le champ Stage est mis à jour, et non lorsque les produits sont ajoutés à [!UICONTROL Opportunités].

1. (Facultatif) Cliquez sur **[!UICONTROL New Trigger]**.
1. (Facultatif) Dans le menu déroulant **[!UICONTROL [!DNL Salesforce]Object]**, sélectionnez **Account
**.

   Il s’agit d’un champ obligatoire.
1. (Conditionnel) Indiquez les informations suivantes :

   1. Sélectionnez un **[!UICONTROL Type]** dans le menu déroulant **[!UICONTROL Type]** .

      Lorsqu’un compte **
** est désigné comme **[!UICONTROL Type]** spécifié ici dans [!DNL Salesforce], un **[!UICONTROL Projet]** est créé dans [!DNL Workfront].

      Il s’agit d’un champ obligatoire.

   1. (Facultatif) Commencez à saisir le nom d’un **[!UICONTROL Portfolio]** ou **[!UICONTROL Programme]** où vous souhaitez placer le projet dans [!DNL Workfront] dans le champ **[!UICONTROL Portfolio ou Programme]** , puis sélectionnez-le lorsqu’il apparaît dans la liste.

      Si vous ne spécifiez aucun Portfolio ou programme, le nouveau projet est créé et ajouté à la liste **[!UICONTROL Projets que je possède]** de l’utilisateur connecté à [!DNL Workfront] à partir de [!DNL Salesforce]. L’utilisateur est également le propriétaire du projet pour le nouveau projet.

   1. Commencez à saisir le nom d’un **[!UICONTROL modèle]** que vous souhaitez associer au nouveau projet [!DNL Workfront], puis sélectionnez-le lorsqu’il apparaît dans la liste.

      Il s’agit d’un champ obligatoire.

      >[!NOTE]
      >
      >Si vous avez spécifié un propriétaire de modèle sur le modèle que vous prévoyez d’utiliser pour cette intégration, cela devient le propriétaire du projet du nouveau projet. Les nouveaux projets apparaissent sous la liste **[!UICONTROL Projets que je possède]** de l’utilisateur propriétaire du nouveau projet, selon le modèle.

   ![salesforce_triggers_page_with_cleaned_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Les projets [!DNL Workfront] sont désormais générés chaque fois que l’un des déclencheurs est satisfait.

### Présentation des noms de projet {#understanding-project-names}

Selon le déclencheur qui a généré les projets, les noms des projets dans [!DNL Workfront] peuvent suivre l’un de ces modèles :

* Si le projet est créé en fonction d’une opportunité ou d’un déclencheur de compte, le nom du projet est : *`<Salesforce object name>`: `<Project template name>` (via [!DNL Salesforce])*.
* Si le projet est créé à partir d’un déclencheur d’opportunité qui inclut également l’ajout d’un nouveau produit, le nom du projet est : *`<Salesforce object name>`: `<Salesforce product name>` (via [!DNL Salesforce])*.

## Affichage de [!DNL Workfront] projets

Si votre administrateur [!DNL Workfront] a ajouté la section [!DNL Workfront] à votre [!UICONTROL opportunité] ou compte
mise en page, vous pouvez voir les projets créés automatiquement dans l’onglet [!UICONTROL Projets] de cette section.\
Pour plus d’informations sur l’ajout de la section [!DNL Workfront] à la mise en page d’une [!UICONTROL opportunité] ou d’un compte
, voir [Configuration de la section  [!DNL Adobe Workfront] pour les  [!DNL Salesforce] utilisateurs](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Vous devez disposer d’un compte [!DNL Workfront] et être connecté à [!DNL Workfront] pour afficher l’onglet [!UICONTROL Projets].

Pour afficher les projets créés à partir d’une [!UICONTROL opportunité] ou d’un compte
:

1. Accédez à une [!UICONTROL opportunité] ou à un compte
.
1. Accédez à la section **[!DNL Workfront]** .

   >[!NOTE]
   >
   >Selon la façon dont votre administrateur [!DNL Workfront] a configuré cette section, elle peut porter un nom différent.

1. Sélectionnez l’onglet **[!UICONTROL Projets]** .

   Tous les projets créés par des déclencheurs définis sont répertoriés dans cet onglet. Tout utilisateur de [!DNL Salesforce] qui dispose également d’un compte [!DNL Workfront] et qui peut être autorisé à voir ces projets dans [!DNL Workfront] peut également les voir dans [!DNL Salesforce] pour l’ [!UICONTROL opportunité] ou le compte
qui les ont générés.

   Vous pouvez afficher les informations suivantes sur les projets créés par l’intégration :

   * Nom du projet
   * Numéro de référence
   * Date d’entrée
   * Nom du propriétaire
   * Statut
   * Condition
   * Date d&#39;achèvement prévue
   * Pourcentage d’achèvement

     Lorsque ces informations sont mises à jour dans [!DNL Workfront], vous pouvez voir les champs mis à jour dans cette liste.

1. (Facultatif) Cliquez sur le nom d’un projet pour l’ouvrir dans Workfront.
1. (Facultatif) Cliquez sur [!UICONTROL **[!UICONTROL Accéder à Salesforce]**] dans la zone [!UICONTROL Détails du projet] ou dans l’en-tête du projet pour accéder à l’[!UICONTROL opportunité] ou au compte
d’où provient le projet. L’administrateur du système ou du groupe doit ajouter le champ [!UICONTROL Intégrations] à votre modèle de mise en page pour le trouver dans l’en-tête du projet.

   >[!NOTE]
   >
   >Le lien [!UICONTROL Aller à Salesforce] est visible par tous les utilisateurs de [!DNL Workfront] qui peuvent afficher le projet. Vous devez disposer d’un compte [!DNL Salesforce] pour pouvoir accéder à l’opportunité ou au compte [!DNL Salesforce] à partir duquel le projet a été généré.
