---
title: Utilisation de la promotion de l’environnement pour Adobe Workfront Planning
description: Vous pouvez copier des espaces de travail Workfront Planning, des types d’enregistrements, des champs et des vues d’un environnement Workfront à un autre à l’aide des fonctionnalités de promotion d’environnement. Au lieu de tout reconstruire manuellement, vous assemblez la configuration dans un package au sein de l’environnement source et vous l’installez dans l’environnement cible.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 1eaa497ba7e446f7fdf978f369205f309bbe231f
workflow-type: tm+mt
source-wordcount: '1277'
ht-degree: 4%
---

# Utilisation de la promotion de l’environnement pour Adobe Workfront Planning

<!--add to TOC-->
<!--add to miniTOC-->

<!--
Not sure if this bit will ever be needed because this only exists when both Preview and Prod have the features in parity. Features released here always come to both environments at the same time: 

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Workfront Planning. Votre société doit acheter un package Planning supplémentaire pour accéder à Workfront Planning.
>
>La fonctionnalité décrite ici n’est pas disponible si votre entreprise a acheté Workfront Planning en tant que produit autonome.
>
>Pour obtenir des informations générales sur Workfront Planning, voir [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>

<!--
Future - when they make it available in Planning: replace the above with this OR ... insert the snippet:

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning which your organization can purchase either as an Adobe Workfront package or a standalone product. 
>
>Not all capabilities included in the Planning package are available to Workfront Planning when it is purchased as a standalone product. 
>
>For general information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>For information about Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 
>
-->

Vous pouvez copier des espaces de travail Workfront Planning, des types d’enregistrements, des champs et des vues d’un environnement Workfront à un autre à l’aide des fonctionnalités de promotion d’environnement.

Au lieu de tout reconstruire manuellement, vous assemblez la configuration dans un package au sein de l’environnement source et vous l’installez dans l’environnement cible.

L’utilisation de la promotion de l’environnement avec Planning est similaire à son utilisation pour Workfront. Pour plus d’informations, consultez la section « Promotion de l’environnement » de l’article [Environnements de test &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-testing-environments.md).

## Remarques concernant l&#39;utilisation de la promotion de l&#39;environnement avec Planning

* Vous devez être un administrateur Workfront pour utiliser la promotion d’environnement.
* Les éléments suivants sont importés par le biais de la promotion de l’environnement :

  * Espaces de travail
  * Sections de Workspace
  * Types d’enregistrements
  * Champs
  * Vues
  * Hiérarchies
  * Partage des paramètres pour tous les objets
  * &#x200B;<!--this might not be part of it; Lilit is checking--> des automatisations
  * Formulaires de demande
  * Règles métier
  * Objets connectés
  * Objets dont dépend l&#39;espace de travail ou avec lesquels d&#39;autres objets sont partagés, tels que le groupe, les équipes, les fonctions. Les scénarios suivants sont possibles :

    * Si un objet portant le même nom existe déjà dans l’environnement cible, Workfront signale un conflit et vous décidez comment le gérer.
    * Si une équipe ou un groupe avec lequel un objet est partagé n’existe pas dans l’environnement cible, la promotion la crée.
* Pour chaque objet, vous pouvez effectuer les opérations suivantes :

  * Créez-le en tant que nouvel objet .
  * Utilisez l’objet existant, mais créez-le avec un nouveau nom
  * Remplacer un objet existant. Le remplacement remplace la configuration dans la cible.

* L’installation peut prendre quelques minutes. Si nécessaire, vous pouvez restaurer une installation à partir de la page de résultats.
* Nous vous recommandons de tester le processus avant de continuer, lorsque cela est possible. Vous pouvez effectuer l’installation dans un environnement de sandbox ou de prévisualisation avant de le promouvoir en production.

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
<p>Package de workflow Prime ou Ultimate avec un package Prime ou Ultimate Planning</p>
<!--This might come later: <p>Prime or Ultimate Planning package when purchased as a standalone product</p>-->
   </td> 
   </tr>
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Norme de workflow</p>    
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Planning</p></td> 
   <td><p>Norme de planification</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Vous devez ajouter un workflow et un type de licence Planning au niveau d'accès lorsque vous disposez à la fois d'un workflow et d'un package Planning</p>  
   <p>Vous devez être administrateur système</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gestion des autorisations relatives aux espaces de travail</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Importer la configuration Planning à l’aide de la promotion d’environnement

Les principales étapes pour promouvoir la configuration de Planning dans un autre environnement sont les suivantes :

* [Créer un package dans l’environnement source](#create-a-package-in-the-source-environment)
* [Préparer le package à l’installation](#make-the-package-ready-to-install)
* [Installation du package dans l’environnement cible](#install-the-package-in-the-target-environment)
* [Vérifier les résultats](#verify-the-results)

Suivez les instructions des sections suivantes pour copier une configuration Planning entre deux environnements Workfront.

### Création d’un package dans l’environnement source

1. disposer d’un environnement source dans lequel la configuration souhaitée est en place ;
1. Dans l’environnement source, cliquez sur le **Menu principal** ![Menu principal](assets/main-menu-shell.png), puis accédez à **Configuration** > **Système** > **Promotion de l’environnement**.
La liste **Packages de configuration** répertorie les packages existants avec leur statut, leur environnement source et l’emplacement de déploiement.
1. Cliquez sur **Créer un package**.

   >[!TIP]
   >
   >Un package nécessite au moins un objet avant de pouvoir être assemblé et installé.
1. Dans l’onglet **Détails du package**, saisissez un **Nom** et un **Description** pour le package. L’environnement source est déjà rempli avec l’environnement (source) actuel.
1. Dans la liste des types d&#39;objet sur la gauche, sélectionnez **Planning workspace**.
1. Recherchez l&#39;espace de travail à convertir, cochez sa case, puis cliquez sur **Ajouter un espace de travail Planning**. L’espace de travail s’affiche sous **Contenu du package**.

   ![Workspace sélectionné pour la promotion de l’environnement](assets/workspace-selected-for-environment-promotion.png)
1. Cliquez sur **Enregistrer et assembler**.

   Workfront assemble le package et ajoute une entrée dans l’onglet **Mises à jour** du package. Vous pouvez consulter les éléments inclus dans le package dans l’onglet Contenu .
1. (Conditionnel et facultatif) Cliquez sur **Enregistrer et fermer** au lieu de cela si vous souhaitez terminer plus tard.
1. (Facultatif) Cliquez sur **Contenu** pour consulter le contenu du package ou cliquez sur **Déploiements** pour voir si ce package a été déployé plusieurs fois.

   Continuez pour préparer le package à l’installation.

### Préparer le package à l’installation

Avant d’installer le package dans l’environnement cible, il est recommandé de le tester dans un environnement de test.

1. Une fois la création du package terminée, comme décrit dans la section précédente, cliquez sur **Détails du package**, puis sur **Modifier**, définissez **Statut** sur **Test**, puis cliquez sur **Enregistrer et fermer**.

   >[!TIP]
   >
   >Après avoir créé le package, son statut est défini sur **Brouillon**. Le statut **Actif** n’est pas disponible tant que vous n’avez pas testé le package pour la première fois.
1. (Recommandé) Cliquez sur **Installer** et sélectionnez l’un des environnements de test disponibles pour le déployer et tester la configuration.

   >[!TIP]
   >
   >L’environnement de production n’est pas disponible comme l’une des options lorsque le statut est défini sur **Tests**.

1. Après l’avoir installé dans un environnement de test, cliquez de nouveau sur **Modifier**, définissez le **Statut** sur **Actif**, puis cliquez sur **Enregistrer et fermer**.

   >[!TIP]
   >
   >L’installation du package dans un environnement de test est similaire à son installation en production, comme décrit dans la section suivante.

   Continuez avec la section suivante pour installer le package dans votre environnement cible.


### Installation du package dans l’environnement cible

1. Sur la page du package, après avoir vérifié, cliquez sur **Installer**.
1. Dans la liste **Environnement cible**, sélectionnez l’environnement dans lequel effectuer le déploiement (par exemple, votre environnement de production), puis cliquez sur **Continuer**. La cible par défaut est l’environnement actuel.
1. Sur la page **Informations sur le package**, confirmez l’environnement source et l’environnement sur lequel vous effectuez le déploiement.
1. Dans la section **Mappage d&#39;objets**, développez chaque regroupement d&#39;objets, tel que **Groupe** et **Espace de travail Planning**, pour passer en revue les objets.
1. Pour chaque objet, passez en revue les colonnes **Collision** et **Statut**, puis choisissez une **Action de déploiement** dans la liste. Choisissez l’une des options suivantes :

   * **Créer** : ajoute l’objet à la cible. Utilisez cette option lorsqu’aucune collision n’est détectée.
   * **Utiliser existant** : permet de mapper l’objet à un objet qui existe déjà dans la cible, comme un groupe portant le même nom.
   * **Créer avec un nouveau nom** : ajoute l’objet sous un nom que vous spécifiez.
   * **Remplacer** : permet de remplacer l’objet existant dans la cible par celui du package.
1. (Facultatif) Pour modifier plusieurs objets à la fois, cochez leurs cases, choisissez une action dans la liste Action de déploiement en haut du groupe, puis cliquez sur Appliquer à la sélection. Utilisez les filtres situés au-dessus de la liste, par exemple Afficher uniquement les erreurs, pour placer le focus sur des objets spécifiques.
1. Résolvez les indicateurs d’erreur. Si vous sélectionnez **Utiliser existant** pour un objet, vous devez également sélectionner l’objet auquel il correspond.  Dans le cas contraire, l’état affiche une erreur et le **Déployer** reste indisponible.
1. Cliquez sur **Déployer**, puis sur **Déployer** pour confirmer.

   Workfront affiche une page d’installation avec le message **Ce package est en cours d’installation**. Cela peut prendre quelques minutes.

   Une fois l’installation terminée, la page affiche un message de réussite, l’environnement dans lequel le package a été installé et une liste des objets installés, avec un statut pour chacun, tel que **Utilisé existant** ou **Installé (Créer)**.
1. (Facultatif) Cliquez sur **Restaurer l’installation**, si nécessaire, pour rétablir l’installation et supprimer la configuration de l’environnement cible.

   Continuez à vérifier les résultats de l’installation.

### Vérifier les résultats

1. Accédez à l’environnement cible > **Menu principal** > **Planification** et recherchez l’espace de travail importé.
1. Ouvrez les types d’enregistrements et les vues pour confirmer que les champs et la mise en page correspondent à la source. Les enregistrements n’étant pas inclus, les tables sont vides.


