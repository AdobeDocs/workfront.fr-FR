---
title: Création et gestion d’un formulaire de demande dans Adobe Workfront Planning
description: Après avoir sélectionné un type d’enregistrement dans la zone Adobe Workfront Planning, vous pouvez créer un formulaire de demande et l’associer à ce type d’enregistrement. Vous pouvez ensuite partager un lien vers celle-ci avec d’autres utilisateurs internes ou externes. Les utilisateurs disposant d’un lien vers le formulaire peuvent remplir les valeurs de champ et, en l’envoyant, ajouter un nouvel enregistrement pour le type d’enregistrement qui y est associé.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 2ffd06f2f50d14b6d33bc79c92616ebed1d58fed
workflow-type: tm+mt
source-wordcount: '3518'
ht-degree: 4%

---

# Création et gestion d’un formulaire de demande dans Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Vous pouvez créer un formulaire de demande et l&#39;associer à un type d&#39;enregistrement dans Adobe Workfront Planning. Vous pouvez ensuite partager le formulaire avec d’autres utilisateurs qui peuvent envoyer des demandes pour créer des enregistrements de ce type.

Cet article décrit comment un gestionnaire d’espace de travail peut créer un formulaire de demande associé à un type d’enregistrement.

Pour plus d’informations sur la soumission d’une demande à un type d’enregistrement pour créer un enregistrement, voir [&#x200B; Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Packages Adobe Workfront</p></td> 
   <td> 
<p>Tout package Workfront et tout package Planning</p>
Ou
<p>Tout package de workflow et tout package Planning</p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérez les autorisations d’un espace de travail ou d’un type d’enregistrement</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limites d’affichage des champs et des valeurs dans les formulaires de demande

Il existe des limitations dans l’affichage de certains champs sur le formulaire de demande et dans l’affichage ultérieur de leurs valeurs sur les enregistrements ou la page des détails de la demande, après l’envoi d’une demande.

Pour plus d’informations sur l’envoi de demandes Workfront Planning, voir [Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

* Vous trouverez ci-dessous les limites d’affichage de certains champs dans les formulaires de demande, les enregistrements créés par un formulaire de demande ou sur la page des détails de la demande :

   * Vous ne pouvez pas ajouter de champs des types suivants à un formulaire de demande :

      * Créé par, Dernière modification par, Approuvé par
      * Date de création, Date de dernière modification, Date d’approbation
      * Champs de recherche d’objets Workfront
      * Champs de recherche des enregistrements connectés de Workfront Planning

* Voici les différences entre la façon dont les formats de champ s’affichent dans le créateur de formulaires de demande et la façon dont les valeurs des champs sont formatées dans l’enregistrement ou dans la page des détails de la demande :

   * Les champs Devise, Nombre et Pourcentage s’affichent sous la forme d’un type de champ de texte monoligne dans le créateur de formulaires.

     Cependant, le format des champs est conservé et les valeurs des champs s’affichent sous la forme de devise, de nombres et de pourcentages une fois la demande soumise, sur le type d’enregistrement et dans la page des détails de la demande.

* Vous trouverez ci-dessous une description de l’affichage de certaines valeurs de champ dans les formulaires de demande et les pages de détails de la demande :

   * Le formatage spécial des champs Devise, Nombre et Pourcentage n’est pas conservé. Par exemple, la précision décimale n’est pas conservée pour les valeurs de ces champs dans ces zones.
   * Les valeurs des champs Personnes s’affichent sous la forme d’identifiants.
   * Les champs de formule qui ne font pas référence à d’autres champs ou calculs n’affichent aucune valeur. Par exemple, un champ avec une formule `STRING` affiche une valeur « N/A ».
   * Les champs de formule qui font référence à des champs Devise affichent les valeurs sans tenir compte des taux de change.
   * Les valeurs des champs de paragraphe affichent une valeur « S/O » sur le formulaire de demande et affichent des balises HTML au lieu du texte formaté dans la page des détails de la demande.

## Création d’un formulaire de demande

Pour créer un formulaire de demande, vous devez commencer par créer le formulaire, configurer les détails du formulaire et terminer en publiant et en partageant le formulaire.

### Commencer à créer un formulaire de demande

Vous pouvez créer un formulaire de demande à partir du type d’enregistrement associé au formulaire<!--span class="preview">, or from the Requests area of Workfront.</span>-->.

#### Création d’un formulaire de demande à partir d’un type d’enregistrement

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails. Pour plus d’informations sur la création d’un type d’enregistrement, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page du type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type d’enregistrement s’ouvre en mode Tableau.

1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Créer un formulaire de demande** ou **Gérer les formulaires de demande**, si vous disposez déjà d’un formulaire et que vous souhaitez en créer d’autres.
1. (Conditionnel) Si vous souhaitez ajouter un autre formulaire, cliquez sur **Nouveau formulaire de demande**.

   La zone Créer un formulaire de demande s’ouvre.

1. Dans la zone Créer un formulaire de demande, mettez à jour le nom du formulaire de demande. Par défaut, le nom du formulaire est **Formulaire sans titre**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Facultatif) Ajoutez une **Description** pour le formulaire de demande.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Cliquez sur **Créer**.

   Le formulaire de demande pour le type d’enregistrement sélectionné s’ouvre dans l’onglet Formulaire .
1. Passez à [&#x200B; Configurer les détails du formulaire de demande &#x200B;](#set-up-details-for-the-request-form).

<!--

<div class="preview">

#### Create a request form from the Requests area of Workfront

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Requests**.
1. In the upper-right corner of the screen, click **Request forms**.
1. (Conditional) If you are editing an existing request form, select it from the list, then continue to [Configure the form](#confgure-the-form).
1. If you are creating a new request form, in the upper-right corner of the screen, click **New request form**.

   The Create request form box opens

1. In the Create request form box, update the name of the request form. By default, the name of the form is **Untitled form**. 
1. In the Object types field, select the record type that the request form will be associated with. Record types are grouped into the workspace that they exist within.
1. (Optional) Add a **Description** for the request form. 

1. Click **Create**. 

   The request form for the selected record type opens in the Form tab.
1. Continue to [Set up details for the request form](#set-up-details-for-the-request-form).



</div>

-->

### Configurer les détails du formulaire de demande

Les détails du formulaire sont divisés en onglets.

* L’onglet **Formulaire** vous permet d’ajouter des champs et des éléments de contenu au formulaire
* L’onglet **Configuration** vous permet de définir un processus d’approbation du formulaire et de définir les options de remplissage de la demande.

  >[!NOTE]
  >
  ><span class="preview">Dans l’environnement de Prévisualisation, l’onglet Paramètres remplace l’onglet Configuration </span>.
  <!--* <span class="preview">The **Automations** tab allows you to automate what will occur based on features of the request made with the form.</span>-->

#### Configurer les détails du formulaire

1. Commencez à créer ou à modifier un formulaire de demande, comme décrit dans la section [Commencer à créer un formulaire de demande](#begin-creating-a-request-form).

   Ou

   Recherchez le formulaire dans la liste Formulaires de demande, cliquez sur la zone en regard du nom du formulaire, puis cliquez sur **Modifier le formulaire** dans la barre bleue en bas de l’écran.

   Le formulaire de demande pour le type d’enregistrement sélectionné s’ouvre dans l’onglet Formulaire .

   ![Mode de modification du formulaire de demande de campagne](assets/campaigns-request-form-edit-mode.png)

   Le formulaire de demande contient par défaut les informations suivantes :

   * Champs d’enregistrement disponibles dans la vue Tableau du type d’enregistrement sélectionné. <!--they are working on removing the limitation below-->

   * **Section par défaut** : il s’agit du saut de section par défaut que Workfront applique au formulaire de demande. Tous les champs d’enregistrement s’affichent dans la zone **Section par défaut**.
   * Champ **Subject** : champ qui identifiera la demande dans Workfront. La configuration et la valeur du champ Objet ne sont pas modifiables.

     >[!NOTE]
     >
     >* Le champ **Objet** nécessite une valeur lorsqu’il est visible sur le formulaire de demande. Cependant, vous pouvez supprimer le champ **Objet** si nécessaire, et les demandeurs ne le verront pas dans le formulaire lorsqu’ils soumettent la demande.
     >* Lorsque le champ Objet est manquant dans un formulaire de demande, mais qu&#39;il existe un champ Nom pour le nom de l&#39;enregistrement futur, le nom de la demande est automatiquement attribué au même nom que l&#39;enregistrement créé.
     >* Lorsque les champs Objet et Nom sont manquants dans le formulaire de demande, la demande est nommée selon le modèle suivant : `< Record name > request form < Entry date of the request >` ; l’enregistrement est nommé **Sans titre**.

   * Tous les champs associés au type d’enregistrement.

     Les champs contenus dans le formulaire de demande seront visibles pour toutes les personnes soumettant une demande à ce type d&#39;enregistrement.

1. (Facultatif) Pointez sur un champ du formulaire à supprimer, puis cliquez sur l’icône **x** pour le supprimer. Elles sont ajoutées à l’onglet **Champs** situé à gauche du formulaire.

1. (Facultatif) Pour supprimer la **section Par défaut** du formulaire, procédez comme suit :

   1. Supprimez tous les champs de la section Par défaut.
   1. Cliquez sur **Éléments de contenu** et ajoutez une nouvelle section, puis ajoutez un nom pour la section.
   1. Ajoutez des champs à la nouvelle section.
   1. Cliquez sur l’icône **x** pour supprimer la **section par défaut**.
1. Cliquez sur n’importe quel champ, puis utilisez les commandes du panneau de droite du formulaire pour définir leur taille ou l’une des informations suivantes :

   * **Libellé** : il s&#39;agit du nom du champ tel qu&#39;il apparaîtra sur le formulaire de demande. Le nom du champ d’enregistrement n’est pas modifié.
   * **Instructions** : ajoutez plus d’informations sur le champ .
   * **Rendre un champ obligatoire** : lorsqu’il est sélectionné, le champ doit avoir une valeur. Dans le cas contraire, le formulaire ne peut pas être envoyé.
   * **Ajouter une logique** : définissez les conditions qui doivent être remplies pour que le champ s’affiche ou soit masqué.

   >[!TIP]
   >
   >   Le type de champ de chaque champ s’affiche dans la partie supérieure du panneau de droite, une fois que vous avez sélectionné le champ dans le formulaire.
   >     

1. (Facultatif) Cliquez sur l’onglet **Éléments de contenu** sur le côté gauche du formulaire, puis ajoutez l’un des éléments suivants :

   * **Texte descriptif**
   * **Saut de section**

   Pour plus d’informations sur la création d’un formulaire personnalisé, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Facultatif) Cliquez sur **Aperçu** pour voir comment le formulaire s’affichera pour les autres utilisateurs lorsqu’ils l’utiliseront pour envoyer un nouvel enregistrement.
1. Passez à l’un des éléments suivants :

   * [Configurer les détails de configuration](#set-up-configuration-details) si vous souhaitez configurer plus de détails pour le formulaire dans l’environnement d’Exploitation
   * <span class="preview">[Configurer les paramètres](#configure-settings) si vous souhaitez configurer plus de détails pour le formulaire dans l’environnement de production</span>
   * [Complétez la création du formulaire de demande](#complete-request-form-creation) si vous ne souhaitez pas configurer d’autres paramètres.

#### Configurer les détails de configuration

>[!NOTE]
>
>Cet onglet est disponible uniquement dans l’environnement de production.

Dans l’onglet Configuration , vous pouvez définir le processus d’approbation et configurer le moment où une demande créée à partir de ce formulaire sera marquée comme Terminée.

1. Commencez à créer ou à modifier un formulaire de demande, comme décrit dans la section [Commencer à créer un formulaire de demande](#begin-creating-a-request-form).

   Le formulaire de demande pour le type d’enregistrement sélectionné s’ouvre dans l’onglet Formulaire .
1. (Facultatif) Configurez tous les détails du formulaire, comme décrit dans la section [Configurer les détails du formulaire](#set-up-form-details).

1. (Facultatif) Si vous souhaitez ajouter des approbateurs, cliquez sur l’onglet **Configuration**, puis ajoutez au moins un utilisateur ou une équipe au champ **Approbateurs** pour approuver les nouvelles demandes de ce formulaire d’enregistrement.

   ![Onglet Configuration](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Vous pouvez ajouter un ou plusieurs approbateurs à un formulaire de demande.
   * Si au moins un approbateur rejette la demande, celle-ci est rejetée et l&#39;enregistrement n&#39;est pas créé. La demande reste dans la zone des Demandes de Workfront.
   * Si vous ajoutez plusieurs approbateurs et que l&#39;option Une seule décision est obligatoire n&#39;est pas activée, tous les approbateurs doivent prendre une décision avant qu&#39;une demande ne soit approuvée ou rejetée.
   * Si une équipe est définie en tant qu&#39;approbateur, une seule décision est requise de la part de l&#39;équipe.

   Pour plus d’informations sur l’ajout d’approbations à des formulaires de demande, voir [&#x200B; Ajouter une approbation à un formulaire de demande &#x200B;](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Conditionnel) Si vous souhaitez que l&#39;enregistrement soit créé après son approbation par l&#39;un des approbateurs, cochez la case **Une seule décision est requise**.

1. Choisissez si vous souhaitez qu&#39;une demande créée à partir de ce formulaire soit marquée comme terminée lorsque l&#39;objet demandé est créé ou lorsque l&#39;objet demandé est terminé.
1. (Conditionnel) Si vous avez sélectionné pour que la demande soit marquée comme terminée une fois l’objet demandé terminé, sélectionnez le champ et la valeur qui indiquent quand l’objet est terminé. Par exemple, vous pouvez sélectionner le champ Statut et la valeur Terminé pour terminer la demande lorsque le statut de l&#39;objet créé est défini sur Terminé.
1. Passez à <!--[Set up Automations details](#set-up-configuration-details) if you want to configure more details for the form, or go to -->[Terminer la création du formulaire de demande](#complete-request-form-creation).

<div class="preview">

### Configurer les paramètres

>[!NOTE]
>
>Cet onglet est disponible uniquement dans l’environnement de Prévisualisation.

Dans l’onglet Paramètres , vous pouvez définir des règles d’approbation et configurer le moment où une demande créée à partir de ce formulaire sera marquée comme Terminée.

#### Configuration des règles de validation

Les règles d’approbation définissent le processus d’approbation en fonction des valeurs de champ sur dans les demandes envoyées.

Par exemple, si un formulaire de demande comporte le champ « Type de campagne », il est possible de créer une règle qui envoie la demande à une personne lorsque le champ comporte la valeur « Numérique » et à une autre personne lorsqu’il comporte la valeur « Imprimer ».

Tenez compte des points suivants lors de l’ajout de règles d’approbation :

* Les règles sont hiérarchisées par ordre de priorité. Si les conditions de la première règle sont remplies, cette règle est appliquée, même si les conditions des règles situées plus bas dans la liste sont également remplies.
* Si aucune condition n’est remplie, la règle par défaut est appliquée.
* Vous pouvez ajouter un ou plusieurs approbateurs à une règle d&#39;approbation.
* Si au moins un approbateur rejette la demande, celle-ci est rejetée et l&#39;enregistrement n&#39;est pas créé. La demande reste dans la zone des Demandes de Workfront.
* Si vous ajoutez plusieurs approbateurs et que l&#39;option Une seule décision est obligatoire n&#39;est pas activée, tous les approbateurs doivent prendre une décision avant qu&#39;une demande ne soit approuvée ou rejetée.
* Si une équipe est définie en tant qu&#39;approbateur, une seule décision est requise de la part de l&#39;équipe.

Pour plus d’informations sur l’ajout d’approbations, voir [&#x200B; Ajouter une approbation à un formulaire de demande &#x200B;](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

Pour définir des règles d&#39;approbation pour un formulaire de demande :

1. Commencez à créer ou à modifier un formulaire de demande, comme décrit dans la section [Commencer à créer un formulaire de demande](#begin-creating-a-request-form).

   Le formulaire de demande pour le type d’enregistrement sélectionné s’ouvre dans l’onglet Formulaire .
1. (Facultatif) Configurez tous les détails du formulaire, comme décrit dans la section [Configurer les détails du formulaire](#set-up-form-details).

1. Pour commencer à configurer les règles d’approbation, cliquez sur Approbations ![icône Approbations](assets/approvals-icon-on-form.png) dans le volet de navigation de gauche.

1. (Facultatif) Si vous souhaitez définir un processus d&#39;approbation par défaut, ajoutez au moins un utilisateur ou une équipe au champ **Approbateurs** de la zone Règle d&#39;approbation par défaut, puis cochez la case **Une seule décision est requise** si vous souhaitez que l&#39;enregistrement soit créé après son approbation par l&#39;un des approbateurs par défaut.

   ![Zone de règle d&#39;approbation par défaut](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. (Facultatif) Pour chaque règle d’approbation supplémentaire, procédez comme suit :

   1. Cliquez sur **Ajouter une règle d’approbation**
   1. Cliquez sur le titre de l’espace réservé « Règle d’approbation sans titre » et saisissez un nom pour la règle d’approbation.
   1. Cliquez sur **Sélectionner un champ** et sélectionnez le champ qui active la règle.
   1. Sélectionnez l’opérateur de la règle. Les opérateurs varient en fonction du type de champ.
   1. Si l’opérateur sélectionné requiert une valeur, cliquez sur l’icône plus et ajoutez une ou plusieurs valeurs.
   1. (Facultatif) Ajoutez d’autres conditions à l’aide de l’opérateur AND ou OR en cliquant sur Ajouter une condition et en configurant la condition supplémentaire.
   1. Dans la zone Actions de la règle d&#39;approbation, dans le champ **Approbateurs**, ajoutez au moins un utilisateur ou une équipe à définir au niveau de l&#39;approbateur lorsque la condition est remplie.
   1. (Conditionnel) Si vous souhaitez que l&#39;enregistrement soit créé après son approbation par l&#39;un des approbateurs, cochez la case **Une seule décision est requise**.

1. (Facultatif) Pour réorganiser les règles de routage, cliquez sur la poignée située à gauche de la règle et faites-la glisser jusqu&#39;à l&#39;emplacement souhaité.

   Impossible de réorganiser la règle par défaut.

1. (Facultatif) Pour supprimer une règle de transmission, cliquez sur le **X** situé à droite de la règle.
1. Cliquez sur **Enregistrer** pour enregistrer les règles d’approbation.
1. Passez à [Définir les options d’achèvement de la demande](#set-request-completion-options)

#### Définir les options d’achèvement de la demande

Les options d&#39;achèvement vous permettent de définir si une demande est marquée comme terminée lorsque l&#39;objet demandé est créé ou lorsque l&#39;objet créé est terminé. Vous définissez le moment où l’objet est terminé en fonction d’une condition spécifiée.

1. Commencez à créer ou à modifier un formulaire de demande, comme décrit dans la section [Commencer à créer un formulaire de demande](#begin-creating-a-request-form).

   Le formulaire de demande pour le type d’enregistrement sélectionné s’ouvre dans l’onglet Formulaire .
1. (Facultatif) Configurez tous les détails du formulaire, comme décrit dans la section [Configurer les détails du formulaire](#set-up-form-details).

1. Choisissez si vous souhaitez qu&#39;une demande créée à partir de ce formulaire soit marquée comme terminée lorsque l&#39;objet demandé est créé ou lorsque l&#39;objet demandé est terminé.
1. (Conditionnel) Si vous avez sélectionné pour que la demande soit marquée comme terminée une fois l’objet demandé terminé, sélectionnez le champ et la valeur qui indiquent quand l’objet est terminé. Par exemple, vous pouvez sélectionner le champ Statut et la valeur Terminé pour terminer la demande lorsque le statut de l&#39;objet créé est défini sur Terminé.
1. Passez à <!--[Set up Automations details](#set-up-configuration-details) if you want to configure more details for the form, or go to -->[Terminer la création du formulaire de demande](#complete-request-form-creation).

</div>

<!--
 
<div class="preview">

#### Set up Automations

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. 

For information on creating automations in other areas of Workfront Planning, see [Configure Adobe Workfront Planning automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. Currently, the only available trigger for request form automation is `When request object status equals pending creation`.

1. Update the following fields in the **Actions** section: 

   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Currently, the only available Action for request form automation is `Create record`.

     >[!TIP]
     >
     >After you saved the automation, you can no longer change the action selected in this field.
1. Continue to  [Complete request form creation](#complete-request-form-creation).


</div>

-->

### Terminer la création du formulaire de demande

1. Créez et configurez le formulaire comme décrit dans [Commencer à créer un formulaire de demande](#begin-creating-a-request-form) et [Configurer les détails du formulaire de demande](#set-up-details-for-the-request-form).
1. (Facultatif) Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du formulaire dans l’en-tête, puis cliquez sur **Modifier** pour mettre à jour le nom du formulaire.

1. Cliquez sur **Publier** pour publier le formulaire et obtenir un lien unique pour celui-ci.

   Les événements suivants se produisent :

   * Le bouton **Publier** est supprimé.
   * Le bouton **Dépublier** est ajouté au formulaire. Cliquez dessus pour empêcher l’accès au formulaire.
   * Un bouton **Partager** est ajouté au formulaire.
   * Le formulaire est alors disponible dans la zone Demandes du menu principal de Workfront.

1. Cliquez sur **Partager** pour partager le formulaire avec d’autres personnes.

   Pour plus d’informations sur le partage d’un formulaire de demande, consultez la section [Partager un formulaire de demande](#share-a-request-form) de cet article
1. Cliquez sur la flèche pointant vers la gauche du nom du formulaire dans l’en-tête pour fermer le formulaire.

   La vue du tableau **Formulaires de demande** s’ouvre et le formulaire y est ajouté.

## Gestion des formulaires de demande existants


1. Cliquez sur l’espace de travail dans lequel vous souhaitez gérer les formulaires de demande.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails. Pour plus d’informations sur la création d’un type d’enregistrement, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page du type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type d’enregistrement s’ouvre en mode Tableau.

1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Gérer les formulaires de demande**.

   Tous les formulaires de demande associés au type d’enregistrement s’affichent dans une vue tabulaire.

1. (Facultatif) Passez la souris sur le nom d’un formulaire de demande en mode Tableau, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du formulaire, puis cliquez sur l’une des options suivantes :

   * **Modifier le formulaire** : cliquez sur cette option pour modifier davantage les informations du formulaire.
   * **Dépublier** : cliquez sur cette option pour dépublier le formulaire et le supprimer de la zone des Demandes dans Workfront.
   * **Partager** : cliquez sur cette option pour modifier la personne qui a accès au formulaire.
   * **Copier le lien** : cliquez sur cette option pour copier rapidement le lien du formulaire de demande sans ouvrir le formulaire.
   * **Supprimer** : cliquez sur cette icône pour supprimer le formulaire. Toutes les demandes et tous les enregistrements ajoutés à l’aide du formulaire ne sont pas supprimés. Le formulaire ne peut pas être récupéré.

   ![Menu Plus sur le formulaire de demande de la liste des formulaires de demande](assets/more-menu-on-request-form-from-request-forms-list.png)

1. Cliquez sur la flèche pointant vers la gauche de **Formulaires de demande** dans l’en-tête pour fermer le tableau des formulaires de demande.

   La page de type d’enregistrement s’ouvre.
1. (Facultatif et conditionnel) Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement dans l’en-tête, puis effectuez l’une des opérations suivantes :

   1. Cliquez sur **Mettre à jour le formulaire de demande** pour apporter des modifications au formulaire de demande, puis cliquez sur un formulaire de demande pour l’ouvrir et le modifier.
   1. Cliquez sur **Copier le lien pour demander un formulaire** pour partager le lien vers le formulaire avec d’autres personnes.

1. (Facultatif) Accédez à la zone **Demandes** dans Workfront et recherchez le formulaire partagé pour envoyer une demande. Pour plus d’informations, voir [Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## Partager un formulaire de demande

1. Créez un formulaire de demande comme décrit dans la section [Créer un formulaire de demande pour un type d’enregistrement](#create-a-request-form-for-a-record-type) de cet article.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du formulaire de demande sur la page du type d’enregistrement.
1. Cliquez sur **Partager** pour partager le formulaire avec d’autres personnes.

1. Pour partager le formulaire en interne, sélectionnez l’onglet **Partage interne**, recherchez le nom d’un utilisateur, d’une équipe, d’une fonction, d’un groupe ou d’une entreprise dans le champ **Accorder l’accès pour envoyer ce formulaire**, puis sélectionnez-le lorsqu’il apparaît dans la liste. L’autorisation **Envoyer** est sélectionnée par défaut pour chaque entité.

   ![Zone de partage pour le formulaire de demande](assets/share-box-for-request-form.png)

1. (Facultatif) Cliquez sur le menu déroulant situé après le nom d’une entité, puis cliquez sur **Supprimer** pour la supprimer de la liste et arrêter de partager le formulaire avec elle.

   >[!NOTE]
   >
   >Outre les équipes, les groupes, les entreprises et les fonctions, vous ne pouvez partager qu’avec des utilisateurs qui ont été ajoutés au Adobe Admin Console. Vous ne pouvez pas ajouter des utilisateurs Workfront uniquement. Pour plus d’informations, voir [Gestion des utilisateurs dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

1. Dans la section **Qui peut soumettre des demandes via ce formulaire**, sélectionnez l’une des options suivantes pour indiquer quels types d’utilisateurs peuvent accéder à ce formulaire :

   * Accessible par les personnes invitées uniquement
   * Toute personne disposant d’un accès en affichage ou supérieur à l’espace de travail
   * Toute personne disposant d’un accès en contribution ou supérieur à l’espace de travail
1. (Facultatif) Cliquez sur **Copier le lien** pour partager le lien vers le formulaire avec des personnes qui y ont accès. Le lien est copié dans le presse-papiers.
1. Pour partager le formulaire publiquement, sélectionnez l’onglet **Partage public** puis activez le paramètre **Créer un lien public**.

   ![Partage public pour le formulaire de demande](assets/share-request-form-publicly-tab.png)

   >[!WARNING]
   >
   >* Lorsque vous activez le paramètre **Créer un lien public**, n’importe qui peut accéder au formulaire et envoyer un nouvel enregistrement, même les personnes extérieures à votre organisation qui ne disposent pas d’un compte Workfront.
   >
   >* Un formulaire contenant les types de champs suivants ne peut pas être partagé publiquement :
   >
   >     * Connexions Workfront ou AEM Assets
   >     * Personnes
   >

1. Choisissez une **date d’expiration du lien**.

   Vous pouvez sélectionner des dates futures dans les 180 jours à compter de la date actuelle.

   >[!TIP]
   >
   >Une fois la date de partage expirée, le formulaire de demande n’est plus disponible dans la zone des Demandes de Workfront et les liens partagés avec d’autres utilisateurs ne sont plus accessibles.

   Les personnes recevront une erreur après l’expiration du lien et vous devez mettre à jour la date du lien et générer un nouveau lien à partager avant que les personnes puissent à nouveau accéder au formulaire.


1. (Facultatif et conditionnel) Cliquez sur **Enregistrer** pour enregistrer les détails de partage du formulaire.
1. (Conditionnel) Si le formulaire a été précédemment enregistré, cliquez sur **Copier le lien**.

   Les options de partage de formulaire sont enregistrées et le lien est copié dans le presse-papiers. Vous pouvez maintenant le partager avec d’autres personnes.

   Pour plus d&#39;informations sur la création d&#39;enregistrements à l&#39;aide d&#39;un lien vers un formulaire de demande, voir [Soumettre des demandes Adobe Workfront Planning](/help/quicksilver/planning/requests/submit-requests.md).

1. Cliquez sur **Enregistrer** dans le coin inférieur droit de l’onglet **Formulaire** pour enregistrer le formulaire.
