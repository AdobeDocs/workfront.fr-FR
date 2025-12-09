---
title: Prise en main de l’intégration de Workfront Planning and GenStudio for Performance Marketing
description: L’espace de travail GenStudio for Performance Marketing est disponible dans Adobe Workfront Planning lorsque votre société a acheté les deux produits. Découvrez quelques principes de base sur la manière de rationaliser vos workflows à l’aide de cette intégration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: e6fc6def1553df3faa8e1200f7ec2ca2bb97eb04
workflow-type: tm+mt
source-wordcount: '2063'
ht-degree: 1%

---

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->


# Prise en main de l’intégration d’Adobe Workfront Planning et d’Adobe GenStudio for Performance Marketing

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Les organisations qui utilisent à la fois Adobe Workfront Planning et Adobe GenStudio for Performance Marketing définissent souvent des concepts marketing tels que des campagnes, des produits, des activations et des rôles de manière plus détaillée que ce que GenStudio prend en charge par défaut.

Il existe une intégration native entre GenStudio for Performance Marketing et Workfront Planning. Cette intégration permet aux utilisateurs de Workfront Planning de gérer les campagnes, produits, rôles, activations, canaux et régions utilisés dans GenStudio. Il leur permet également de configurer GenStudio pour référencer les types d’enregistrements existants à partir de Workfront Planning, ce qui crée un workflow marketing plus connecté et plus cohérent.

L’espace de travail GenStudio for Performance Marketing est disponible dans Adobe Workfront Planning lorsque votre société a acheté les deux produits.

## Avantages de l’intégration

Grâce à l’intégration entre Workfront Planning et GenStudio for Performance Marketing, vous pouvez :

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Affichez l’espace de travail GenStudio dans Workfront Planning.
* Modifiez vos campagnes, produits, personnages et activations dans GenStudio for Performance Marketing et disposez des mises à jour en temps réel des mêmes informations dans Workfront Planning.
* Modifiez vos campagnes, produits, personnages et activations dans Workfront Planning et disposez des mises à jour en temps réel des mêmes informations dans GenStudio for Performance Marketing.
* Évitez la saisie de données en double.
* Maintenir l’alignement des efforts de planification et d’activation.
* Connecter les marques GenStudio et leurs informations aux enregistrements Workfront Planning.

## Exigences d’intégration

Votre entreprise doit répondre aux exigences suivantes pour que l’intégration entre Workfront Planning et GenStudio for Performance Marketing existe :

* Workfront et GenStudio for Performance Marketing doivent être activés pour la même organisation.

  Pour plus d’informations sur GenStudio, consultez le [Guide de l’utilisateur d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/home).

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* Votre instance Workfront fait partie de l’expérience unifiée Adobe, y compris l’utilisation du système Identity Management (IMS).

  Pour plus d’informations, voir [Expérience unifiée Adobe pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Les utilisateurs qui utilisent à la fois Workfront Planning et GenStudio for Performance Marketing ne doivent appartenir qu’à une seule instance Workfront au sein de l’organisation IMS.

  Les utilisateurs de Workfront uniquement peuvent afficher l’espace de travail GenStudio, même s’ils ne sont pas des utilisateurs de GenStudio for Performance Marketing.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Conditions d’accès

Le tableau suivant décrit les exigences en matière d’accès et d’autorisations pour utiliser Adobe Workfront Planning avec Adobe GenStudio for Performance Marketing :

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront et tout package Planning</p> <p>Tout workflow et tout package Planning</p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
   <tr> 
<td> 
   <p> Produits supplémentaires</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Rôles utilisateur Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Tout rôle d’utilisateur GenStudio pour accéder aux campagnes, aux produits et aux rôles</li>
   <li>GenStudio System Manager pour accéder aux activations <!--and Events--></li></ul>
   Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> Rôles utilisateur et autorisations </a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>  
   <p>Dans Workfront Planning : </p>
   <ul>
   <li><p>Gérez les autorisations de l’espace de travail GenStudio pour ajouter de nouveaux champs ou types d’enregistrements à l’espace de travail GenStudio</p></li>
   <li><p>Autorisations de contribution à l’espace de travail GenStudio pour ajouter, mettre à jour ou supprimer des enregistrements dans l’espace de travail GenStudio</p> </li>  
   </ul>
   <p>Aucun utilisateur ne peut supprimer des types d’enregistrements ou des champs GenStudio for Performance Marketing de l’espace de travail GenStudio dans Workfront Planning</p>
   <p>Dans Adobe GenStudio for Performance Marketing : <p>
   <ul>
   <li><p> Toutes les autorisations dans Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Création d’autorisations dans Adobe GenStudio for Performance Marketing pour créer des éléments</p></li></ul>
   </td>  
</tbody> 
</table>

Pour plus d’informations sur l’accès à Adobe Workfront Planning, consultez [Présentation de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Pour plus d’informations sur Adobe GenStudio for Performance Marketing, consultez le [Guide de l’utilisateur d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/home).

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront package</p>
<p>Any Planning package</p>  

   </td> </tr>
   <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
   
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenSudio System Manager to access Activations ****and Events****</li></ul>
   For information, see <a href="https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Manage permissions to the GenStudio workspace to add new fields or record types to the GenStudio workspace</p></li>
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   </ul>
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> -->

## Présentation des fonctionnalités de Workfront Planning et d’intégration de GenStudio for Performance Marketing

En fonction du nombre d’instances Workfront dont dispose votre organisation, vous disposez automatiquement des autorisations suivantes sur l’espace de travail GenStudio dans Planning :

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Une instance de Workfront</p></td> 
   <td> 
<p>L’espace de travail GenStudio est visible dans votre instance de Workfront Planning</p>
<p>Tous les utilisateurs, y compris les administrateurs de Workfront, ont par défaut un accès de type Contributeur à l’espace de travail GenStudio dans Planning</p>
<p>Les administrateurs et administratrices de Workfront peuvent modifier l’espace de travail GenStudio et accorder des autorisations de gestion à tout le monde</p>
</td> </tr>
   <tr> 
<td> 
   <p> Instances multiples de Workfront</p> </td> 
   <td> 
   <p>Voici les scénarios possibles lorsque votre organisation dispose de plusieurs instances de Workfront avec Workfront Planning :</p>
   <ul><li>Si votre société dispose de plusieurs instances de Workfront au moment de l’achat d’Adobe GenStudio for Performance Marketing, l’espace de travail GenStudio est visible à partir de toutes les instances de Workfront.</li>
   <li>Si votre société ajoute d’autres instances Workfront après l’intégration de leur instance d’origine à Adobe GenStudio for Performance Marketing, l’espace de travail GenStudio n’est visible qu’à partir de l’instance Workfront d’origine. Pour plus d’informations sur la connexion d’une instance Workfront supplémentaire à Adobe GenStudio, contactez votre représentant de compte. </li></ul>    
</td> 
  </tr>
   </tbody> 
</table>

<!--Old for the second row in the table:

<p>The GenStudio workspace is visible from all Workfront instances</p>
<p>All users with access to GenStudio for Performance Marketing and Workfront Planning have Contribute permissions on the GenStudio in Planning by default</p> 
<p>Workfront administrators cannot grant Manage permissions to the GenStudio workspace to anyone</p>-->

Pour plus d’informations sur les autorisations Workfront Planning, voir [Présentation des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Les sections ci-dessous décrivent les éléments suivants :

* Fonctionnalités de mise à jour des informations de planification Workfront depuis GenStudio for Performance Marketing
* Fonctionnalités de mise à jour des informations GenStudio for Performance Marketing à partir de Workfront Planning
* Limites de ce que vous pouvez et ne pouvez pas gérer dans un espace de travail GenStudio à partir de Workfront Planning.

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Espace de travail GenStudio dans Workfront Planning

* L’espace de travail GenStudio affiche un indicateur visuel dans Workfront Planning afin de l’identifier comme représentant l’espace de travail GenStudio for Performance Marketing.

  ![Carte GenStudio dans Planning](assets/genstudio-card-with-tag-highlighted.png)

  Pour plus d’informations, voir [Gérer l’espace de travail GenStudio dans Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Lorsque vous disposez d’autorisations de niveau Gérer pour l’espace de travail GenStudio dans Planning, vous pouvez :

   * Mise à jour de l’espace de travail GenStudio dans Planning (nom, description, icône)
   * Créer des sections
   * Ajouter des types d’enregistrements
   * Partager avec d’autres personnes

     Vous pouvez partager l’espace de travail GenStudio avec d’autres personnes qui ne disposent pas d’un compte GenStudio. Vous ne pouvez le partager qu’avec les utilisateurs disponibles dans le système Identity Management (IMS) de votre organisation.

     <!--
        >[!NOTE]
        >
        >You cannot remove GenStudio users from the GenStudio workspace or its record types' sharing. -->
     <!--check to see this is correct-->
     <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* Si vous disposez des autorisations de niveau Contribution pour l&#39;espace de travail GenStudio dans Planning, vous ne pouvez pas modifier l&#39;espace de travail à partir de Workfront Planning.

### Types d’enregistrements dans l’espace de travail GenStudio

* Les types d’enregistrements visibles dans GenStudio for Performance Marketing et Planning comportent un indicateur GenStudio dans Workfront Planning.

  ![Carte de type d’enregistrement GenStudio dans Workfront Planning](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* Lorsque vous disposez d’autorisations de niveau Gérer pour l’espace de travail GenStudio dans Planning, vous pouvez effectuer les opérations suivantes à partir de Workfront Planning :
   * Modifier les informations sur les types d’enregistrements GenStudio (leur apparence, paramètres avancés).
   * Partagez des types d’enregistrements GenStudio avec d’autres utilisateurs.
   * Créer des types d’enregistrements. Ces types d’enregistrements restent uniquement dans Workfront Planning. Elles ne s’affichent pas dans GenStudio.
   * Activez les enregistrements de l’espace de travail GenStudio pour vous connecter à partir d’autres espaces de travail.
   * Autorisez l’ajout d’enregistrements de l’espace de travail GenStudio à d’autres espaces de travail.
* Si vous disposez des autorisations de niveau Contribution pour l&#39;espace de travail GenStudio dans Planning, vous ne pouvez pas modifier les types d&#39;enregistrements GenStudio à partir de Planning.

### Enregistrements dans l’espace de travail GenStudio

* Lorsque vous modifiez des enregistrements GenStudio à partir de GenStudio for Performance Marketing, les modifications sont visibles dans l’espace de travail GenStudio dans toutes vos instances de Workfront.
* Vous ne pouvez pas créer ni supprimer des enregistrements d’activation de l’espace de travail GenStudio dans Workfront Planning.
* Lorsque vous disposez d’autorisations de niveau Gérer ou Contribuer pour l’espace de travail GenStudio dans Planning, vous pouvez effectuer les opérations suivantes à partir de Workfront Planning :
   * Ajoutez ou supprimez des enregistrements pour qu’ils soient visibles dans GenStudio for Performance Marketing (ou en soient supprimés).

     Les enregistrements supprimés de Workfront Planning ou GenStudio for Performance Marketing sont placés dans la classe Workfront Planning récemment supprimé pendant 30 jours. GenStudio for Performance Marketing ne comporte pas de classe Récemment supprimé.
   * Restaurer un enregistrement à partir de la classe Récemment supprimé. La restauration des enregistrements supprimés les replace dans Workfront Planning et GenStudio for Performance Marketing.
   * Ajoutez des enregistrements des manières suivantes :

      * Manuellement, à partir de zéro, depuis n’importe quel affichage à l’aide du bouton Nouvel enregistrement .
      * En les important à l’aide d’un fichier CSV ou Excel en mode Tableau
      * Manuellement, dans n&#39;importe quel affichage de Workfront Planning
      * En soumettant une demande à un formulaire de demande de type enregistrement dans Workfront.

  Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* Vous pouvez modifier les informations d’enregistrement de tous les enregistrements de l’espace de travail GenStudio à partir de Workfront Planning.

  Pour plus d’informations, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

### Champs de type d’enregistrement dans l’espace de travail GenStudio

Par défaut, les champs de type enregistrement sont importés de GenStudio for Performance Marketing vers Workfront Planning.

Tenez compte des points suivants à propos des champs de type d’enregistrement GenStudio :

* Lorsque vous disposez d’autorisations de niveau Gérer pour l’espace de travail GenStudio dans Planning, vous pouvez effectuer les opérations suivantes à partir de Workfront Planning :

   * Modifiez les paramètres du champ GenStudio.
   * Créez des champs pour les types d’enregistrements GenStudio.

     Lorsque vous créez des champs pour des types d&#39;enregistrements GenStudio dans Planning, ils sont visibles à partir des zones suivantes :

      * Vues Workfront Planning
      * Pages de détails des enregistrements Workfront Planning
      * Pages de détails des enregistrements GenStudio

     >[!TIP]
     >
     >Les champs créés dans Workfront Planning ne sont pas visibles dans GenStudio.

   * Masquez les champs dans la vue Tableau d’un type d’enregistrement GenStudio dans Workfront Planning.
&lt;!—* Supprimez les champs créés dans Workfront Planning pour les types d’enregistrements GenStudio de Workfront Planning. — ce n&#39;est pas possible, par Iskuhi ; le lien est là mais il va générer une erreur—>

  <!--this is not true: You cannot delete fields imported from GenStudio from Workfront Planning.-->

* Si vous disposez des autorisations de niveau Contribution pour l&#39;espace de travail GenStudio dans Planning :

   * Vous ne pouvez pas modifier les paramètres des champs, ni supprimer ou ajouter des champs de l’espace de travail GenStudio dans Workfront Planning.
   * Vous pouvez masquer des champs de la vue Tableau dans Workfront Planning.

#### Les champs Créé par et Approuvé par

* Vous pouvez ajouter les champs Créé par et Approuvé par pour les types d’enregistrements GenStudio dans Workfront Planning à partir de Workfront Planning.
* Les enregistrements qui s&#39;affichent dans les types d&#39;enregistrements Canal et Région afficheront « Système » comme le Créé par l&#39;utilisateur. Ces enregistrements sont créés automatiquement lors de la création de l’espace de travail GenStudio dans Workfront Planning.
* Les enregistrements créés dans GenStudio après la mise à disposition de l&#39;espace de travail dans Workfront Planning affichent le nom de l&#39;utilisateur IMS qui a créé l&#39;enregistrement dans le champ Créé par , même si l&#39;utilisateur a créé les enregistrements dans GenStudio et n&#39;est pas un utilisateur Workfront.
* Le champ Approuvé par affiche le nom de l&#39;approbateur lorsqu&#39;un formulaire de demande est envoyé pour créer un enregistrement dans le type d&#39;enregistrement GenStudio dans Workfront Planning.
* Les champs Créé par et Approuvé par s’affichent dans les détails des enregistrements dans GenStudio for Performance Marketing. Elles ne s’affichent pas dans la vue Liste.

### Vues d’enregistrement dans l’espace de travail GenStudio

>[!NOTE]
>
>Les types d’enregistrements GenStudio s’affichent dans la vue de tableau par défaut importée depuis la vue de liste GenStudio for Performance Marketing.
>
>Vous ne pouvez pas supprimer la vue de tableau d’origine importée par défaut depuis GenStudio for Performance Marketing.

* Vous ne pouvez pas créer plusieurs vues dans GenStudio for Performance Marketing.

* Lorsque vous disposez d’autorisations de niveau Gérer pour l’espace de travail GenStudio dans Planning, vous pouvez effectuer les opérations suivantes à partir de Workfront Planning :

   * Créez des vues pour les types d’enregistrements GenStudio.

     Pour plus d’informations, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   * Renommez, partagez, exportez, dupliquez ou supprimez toute vue personnalisée à partir des types d’enregistrements GenStudio.

* Lorsque vous disposez des autorisations de niveau Contribution pour l’espace de travail GenStudio dans Planning, vous pouvez effectuer les opérations suivantes à partir de Workfront Planning :

   * Créez des vues pour les types d’enregistrements GenStudio.

     Pour plus d’informations, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   * Renommez, exportez, dupliquez ou supprimez des vues personnalisées à partir des types d&#39;enregistrements GenStudio.

     Vous ne pouvez pas partager de vues depuis l’espace de travail GenStudio dans Workfront Planning

### Enregistrer les connexions dans l’espace de travail GenStudio

Vous pouvez créer des connexions entre les types d’enregistrements dans les espaces de travail GenStudio pour lesquels vous disposez des autorisations de gestion.

Dans Workfront Planning, vous pouvez établir les connexions suivantes entre les types d&#39;enregistrements GenStudio et d&#39;autres types d&#39;enregistrements ou d&#39;objets :

* Deux types d’enregistrements GenStudio
* Un type d’enregistrement GenStudio et un type d’enregistrement Planning du même espace de travail
* Un type d’enregistrement GenStudio et un type d’enregistrement Planning d’un autre espace de travail, si les types d’enregistrement sont configurés pour se connecter à partir d’un autre espace de travail.
* Un type d’enregistrement GenStudio et un type d’objet Workfront (projets, portfolios, programmes, sociétés, groupes)
* Un type d’enregistrement GenStudio et un type d’objet AEM Assets.

### Formulaires de demande et automatisations dans le type d’enregistrement GenStudio

* Vous pouvez ajouter des formulaires de demande à un type d’enregistrement GenStudio dans Workfront Planning.

  Pour plus d’informations, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* Vous pouvez configurer des automatisations pour un type d’enregistrement GenStudio dans Workfront Planning.

  Pour plus d’informations, voir [Configuration des automatisations d’Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

### Connexion à GenStudio Brands à partir des espaces de travail Workfront Planning

Lorsque votre entreprise dispose d’une intégration entre Workfront Planning et Adobe GenStudio, vous pouvez connecter les types d’enregistrements Planning aux marques GenStudio à partir de n’importe quel type d’enregistrement dans n’importe quel espace de travail de Workfront Planning.

Les marques ne sont pas visibles en tant que cartes de type enregistrement dans l’espace de travail GenStudio. Les marques sont disponibles pour créer de nouvelles connexions à partir de n’importe quel type d’enregistrement Workfront Planning, y compris celles de l’espace de travail GenStudio.

<!-- when this releases, replace the paragraph above with these:

Brands are connected by default to the following GenStudio workspace record types:

    * Products
    * Personas

Brands are available for manually connecting to all other GenStudio workspace record types, or record types from all other workspaces you have permissions to manage. 

-->

## Environnement de prévisualisation

* L’espace de travail GenStudio accessible à partir de votre environnement de production s’affiche également dans votre environnement de prévisualisation de la même instance Workfront.
* Vous pouvez effectuer toutes les activités décrites dans cet article sur l’espace de travail GenStudio dans la planification Workfront dans votre environnement de prévisualisation, mais ces modifications ne seront pas visibles à partir de GenStudio.

  Seules les modifications apportées aux éléments de l’environnement de production synchronisent Workfront Planning et GenStudio.

  GenStudio ne dispose pas d’un environnement de prévisualisation.

