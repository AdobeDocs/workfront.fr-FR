---
content-type: release-notes
title: Activité de mise à jour du troisième trimestre 2026 pour Adobe Workfront Planning
description: Il s’agit de l’activité de publication du produit Planification d’Adobe Workfront pour le troisième trimestre 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: bd1c8dfc4b03b4b8d9948da278406addf801d226
workflow-type: tm+mt
source-wordcount: '1665'
ht-degree: 1%

---

# Activité de mise à jour du troisième trimestre 2026 pour Adobe Workfront Planning

<!--
take the next sentence out when we start listing features
-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

Cet article décrit les nouvelles fonctionnalités de Workfront Planning de la version du troisième trimestre 2026.

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning, voir [Activité de version d’Adobe Workfront Planning : index des articles](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).



<!--

## New Sample workspaces tab added to the Planning landing page

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added the Sample workspaces tab in the Planning landing area where you can view example of best-practice workspaces. The workspaces are not editable and we recommend that you use them as examples to create your own.  

We also recommend that you use the multi-workspace template to create, and edit and share workspaces that result as a use of that template.  The template contains the same workspaces as the Sample workspaces tab.   

Workspace managers can modify views in sample workspaces.     

For information, see Workspaces overview (/help/quicksilver/planning/architecture/workspaces-overview.md). 

-->

## Nouvel onglet Exemples d’espaces de travail ajouté à la page de destination Planification

>[!NOTE]
>
>Aperçu : 1er juin 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Nous avons ajouté l’onglet Exemples d’espaces de travail à la zone de destination Planification où vous pouvez afficher des exemples d’espaces de travail des bonnes pratiques. Les espaces de travail ne sont pas modifiables. Les responsables Workspace peuvent modifier les vues dans les exemples d’espaces de travail. L’onglet est visible pour les utilisateurs d’Administration standard et système.

Nous vous recommandons d’afficher les exemples d’espaces de travail et d’utiliser le lot de modèles multi-espaces de travail pour créer, modifier et partager les espaces de travail résultant de l’utilisation de ce modèle.  Le lot du modèle contient les mêmes espaces de travail que l’onglet Exemples d’espaces de travail .

Pour plus d’informations, voir [ Présentation des espaces de travail ](/help/quicksilver/planning/architecture/workspaces-overview.md).

## API Workfront Planning version 2

>[!NOTE]
>
>Disponible pour tous les clients et clientes : 28 mai 2026>[!BADGE horaire de congés]{type=Neutral}

La version 2 de l’API Workfront Planning est désormais disponible et étend considérablement les fonctionnalités de la version 1.

Les améliorations suivantes ont été apportées à la version 2 :

* Créez, mettez à jour et supprimez des espaces de travail, des types d’enregistrements et des champs par programmation.

* Gérer entièrement les enregistrements.
* Améliorations de la structure de l’URL, de la gestion des erreurs, de la pagination, du filtrage et des autorisations.
* Inclut des mises à jour partielles via PATCH
* Inclut les opérations d’enregistrement en bloc.

La version 1 reste disponible, bien que nous vous recommandons de passer à l’utilisation de la version 2.

>[!NOTE]
>
>Le connecteur Workfront Planning pour Fusion n’a pas été mis à jour vers la version 2 de l’API et continuera à utiliser la version 1 jusqu’à nouvel ordre.

Pour plus d’informations, voir [Principes de base de l’API Adobe Workfront Planning](/help/quicksilver/planning/general/planning-api-basics.md).

Pour connaître les spécifications de l’API Workfront Planning, consultez la documentation destinée aux développeurs de l’[API Workfront Planning](https://developer.adobe.com/wf-planning/).

## Octroi d’autorisations pour les enregistrements

>[!NOTE]
>
>Aperçu : 28 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Vous pouvez désormais ajuster les autorisations d’enregistrements individuels pour contrôler qui peut les gérer dans un type d’enregistrement.

Les utilisateurs héritent par défaut des autorisations d’enregistrement de l’espace de travail et du type d’enregistrement. Pour n’accorder des autorisations de type enregistrement qu’à certains utilisateurs spécifiques Gérer les autorisations pour certains enregistrements uniquement, vous pouvez désactiver les autorisations héritées pour certains enregistrements et n’accorder à ces utilisateurs qu’un accès Gérer à ces enregistrements. Vous pouvez ajuster en bloc les autorisations pour un enregistrement ou pour plusieurs enregistrements en même temps.

Vous pouvez accorder aux utilisateurs les niveaux d’autorisation suivants :

* Afficher
* Gérer

>[!NOTE]
>
>* Les autorisations au niveau des enregistrements d’un utilisateur ne peuvent pas dépasser ses autorisations de type enregistrement. Par exemple, un utilisateur disposant d’un accès en lecture seule à un type d’enregistrement ne peut pas se voir accorder un accès en gestion à des enregistrements individuels de ce type.
>* Vous ne pouvez pas supprimer les autorisations d’un utilisateur d’un enregistrement pour le moment. Tout utilisateur disposant au moins d’un accès en lecture seule au type d’enregistrement peut afficher tous les enregistrements de ce type.

Pour plus d’informations, voir [Partager des enregistrements](/help/quicksilver/planning/access/share-records.md).

## Ajout d’un type d’enregistrement global rationalisé

>[!NOTE]
>
>Aperçu : 28 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Pour réduire les clics et vous aider à trouver rapidement les types d’enregistrements dont vous avez besoin, nous avons amélioré l’expérience d’ajout d’enregistrements afin qu’ils soient plus rapides et plus intuitifs lorsque vous ajoutez des types d’enregistrements globaux à un autre espace de travail.

Lorsque vous choisissez d&#39;ajouter un enregistrement à partir de types d&#39;enregistrements existants, vous verrez désormais immédiatement une liste de tous les types d&#39;enregistrements globaux disponibles.

Vous pouvez sélectionner et ajouter un ou plusieurs types d’enregistrements globaux en même temps directement à partir de cet écran.

Pour plus d’informations, voir [Ajouter des types d’enregistrements existants depuis un autre espace de travail](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

## Planning Designer est désormais disponible dans Beta pour tous les clients Workfront Planning

>[!NOTE]
>
>Aperçu : 28 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026>[!BADGE Dans Beta]{type=Neutral}

Vous pouvez désormais utiliser Adobe Planning Designer optimisé par l’IA pour configurer facilement vos espaces de travail et vos structures de données. Planning Designer prend en charge de nombreux éléments, de la création et la configuration des espaces de travail à la définition de champs et de formules, la gestion des enregistrements, la révision de l&#39;historique des modifications et la création de vues personnalisées.

Utilisé directement ou par l’intermédiaire de l’assistant d’IA, Planning Designer offre un environnement flexible et puissant pour créer et maintenir des informations structurées et connectées.

Un administrateur Workfront peut gérer la disponibilité de Planning Designer à partir de la zone Préférences système de la Configuration.

Pour plus d’informations, voir [Prise en main d’Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).


## Synchronisation des métadonnées de Planning vers AEM Assets

>[!NOTE]
>
>Aperçu : 28 mai 2026>Mise à jour rapide de la production : 28 mai 2026>Production pour tous : 28 mai 2026>[!BADGE Horaire réduit]{type=Neutral}

Pour améliorer l’intégrité des données, nous avons publié une synchronisation transparente des métadonnées entre les types d’enregistrements GenStudio for Performance Marketing et AEM Assets lorsque les AEM Assets sont liés à des types d’enregistrements GenStudio dans Workfront Planning.

Les types d’enregistrements GenStudio for Performance Marketing suivants peuvent être connectés à AEM Assets : Campagne, Produit, Persona, Région et Canal.

Les informations ajoutées à un type d’enregistrement GenStudio dans Workfront Planning s’affichent dans un onglet Campaign distinct d’une ressource AEM dans AEM. Les informations sur le produit, le persona, la région et le canal de cette campagne s’affichent également dans cet onglet, en mode lecture seule.

Grâce à cette version, les métadonnées clés sont cohérentes sur les deux plateformes et reflètent les mises à jour en temps quasi réel, ce qui réduit la réconciliation manuelle.

Pour plus d’informations, voir [Gérer l’espace de travail GenStudio dans Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).

## Synchronisation des métadonnées entre Planning et les fragments de contenu AEM

>[!NOTE]
>
>Aperçu : 28 mai 2026>Mise à jour rapide de la production : 28 mai 2026>Production pour tous : 28 mai 2026>[!BADGE Horaire réduit]{type=Neutral}

Pour améliorer l’intégrité des données, nous avons publié une synchronisation transparente des métadonnées entre les types d’enregistrements Planning dans l’espace de travail GenStudio et les fragments de contenu AEM lorsque les fragments de contenu sont liés à des campagnes GenStudio for Performance Marketing.

Les informations de campagne GenStudio s’affichent désormais dans l’onglet Métadonnées d’un fragment de contenu dans AEM.  Les informations sur le produit, le persona, la région et le canal de cette campagne s’affichent également dans cet onglet, en mode lecture seule.

Grâce à cette version, les métadonnées clés sont cohérentes sur les deux plateformes et reflètent les mises à jour en temps quasi réel, ce qui réduit la réconciliation manuelle.

Pour plus d’informations, voir [Gérer l’espace de travail GenStudio dans Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).


## Mises à jour de la vue Liste

>[!NOTE]
>
>Aperçu : 27 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Plusieurs types de champs dans la vue Liste ont été mis à jour afin d’inclure la navigation au clavier et d’autres améliorations.

Les champs à sélection multiple, à sélection unique et Personne désignée offrent désormais une navigation au clavier dans la vue Liste :

* Utilisez les flèches vers le haut et vers le bas de votre clavier pour vous déplacer dans la liste des personnes.

* Appuyez sur la barre d’espace pour sélectionner une personne ou pour supprimer une personne sélectionnée.

Sur les champs à sélection unique et multiple dans la vue Liste :

* Vous pouvez ajouter de nouvelles options directement à partir de l’éditeur si aucun résultat n’est trouvé. Notez que cette fonctionnalité peut ne pas être disponible sur toutes les listes.

* L’interaction avec les champs est désormais accessible à l’aide du clavier. Cela inclut la navigation entre les balises, les options de recherche et la liste à l’aide des flèches haut et bas. Appuyez sur la barre d’espace pour sélectionner un élément ou supprimer un élément sélectionné.

L’interface des champs de référence, tels que la saisie semi-automatique et les champs de recherche externe, a été améliorée.

En outre, lorsque disponible, l’expérience de glisser-déposer de colonnes a été améliorée visuellement.

Pour plus d’informations, voir [Gérer la vue Liste dans Adobe Workfront Planning](/help/quicksilver/planning/views/manage-the-list-view.md).

## Les champs de référence Workfront sont activés comme champs de recherche pour les connexions Planning

>[!NOTE]
>
>Aperçu : 27 mai 2026>Version rapide de production : 11 juin 2026\
>Production pour tous : 16 juillet 2026

Vous pouvez désormais ajouter des champs de référence Workfront en tant que champs de recherche lors de la connexion d&#39;un type d&#39;enregistrement Planning à un type d&#39;objet Workfront.

Par exemple, vous pouvez ajouter les informations sur le Portfolio, le Programme, le Groupe ou la Société de l&#39;objet Projet dans un champ de connexion au projet d&#39;une campagne dans Planning.

Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

## Nouveaux filtres pour la fonctionnalité de répartition de la vue du journal

>[!NOTE]
>
>Aperçu : 27 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Vous pouvez désormais filtrer les informations dans la vue chronologique en fonction de critères correspondant aux objets inclus dans la répartition des enregistrements.

Avant cette amélioration, vous ne pouviez appliquer des filtres que pour les enregistrements principaux dans la vue chronologique.

Pour plus d’informations, consultez [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Nouvelle indication indiquant que les champs modifiés et supprimés affectent les formulaires de demande

>[!NOTE]
>
>Aperçu : 27 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Nous vous rappelons que les champs d’enregistrement que vous modifiez ou supprimez peuvent avoir une incidence sur les formulaires de demande qui contiennent ces champs. Vous aurez désormais la possibilité de passer en revue les formulaires concernés et de vous assurer que les modifications que vous souhaitez apporter aux champs n’auront aucune incidence sur les informations existantes.

Pour plus d’informations, voir [Modifier les paramètres de champ](/help/quicksilver/planning/fields/edit-fields.md).

## Modifier les demandes Planning envoyées

>[!NOTE]
>
>Aperçu : 27 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Vous pouvez désormais modifier les demandes Planning après les avoir envoyées, avant qu&#39;un enregistrement ne soit créé à partir de la demande.

Les utilisateurs suivants peuvent modifier une demande envoyée :

* Créateur de la requête
* Gestionnaires Workspace de l’espace de travail dans lequel la demande a été envoyée
* Administrateurs et administratrices système

Avant cette amélioration, vous ne pouviez pas modifier les requêtes envoyées.

Pour plus d’informations, voir [Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## Nouvelle fenêtre d’aperçu pour les fragments de contenu AEM

>[!NOTE]
>
>Aperçu : 14 mai 2026>Mise à jour rapide de la production : 14 mai 2026>Production pour tous : 14 mai 2026>[!BADGE Horaire réduit]{type=Neutral}

Pour une meilleure visibilité lorsque vous utilisez des fragments de contenu AEM connectés à des enregistrements Workfront Planning, nous avons ajouté une fenêtre d’aperçu qui affiche des informations sur les fragments dans Workfront Planning.

Cette fonctionnalité était auparavant disponible pour les ressources AEM et nous l’avons maintenant ajoutée aux fragments de contenu.

Pour plus d’informations, consultez [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

## Champs de recherche désormais disponibles pour les fragments de contenu AEM dans Workfront Planning

>[!NOTE]
>
>Aperçu : 14 mai 2026>Mise à jour rapide de la production : 14 mai 2026>Production pour tous : 14 mai 2026>[!BADGE Horaire réduit]{type=Neutral}

Vous pouvez désormais ajouter les champs de recherche suivants lorsque vous connectez un type d’enregistrement Planning à un fragment de contenu AEM :

* Créé par
* Date de création
* Modifié par
* Modifié le

Avant cette amélioration, les champs de recherche n’étaient disponibles que pour les ressources et dossiers AEM.

Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).



## Vues personnalisées pour la page Détails d&#39;un enregistrement

>[!NOTE]
>
>Aperçu : 14 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Pour une meilleure flexibilité de visualisation de vos informations dans la page de détails d&#39;un enregistrement, nous avons introduit la possibilité de créer des vues personnalisées pour cette page.

Outre l&#39;ajout de deux vues de page de détails déjà créées, qui contiennent tous les champs d&#39;enregistrement ou uniquement les champs visibles en mode Tableau, vous pouvez désormais créer des vues personnalisées pour les pages de détails d&#39;un enregistrement. Les vues que vous créez sont visibles par tous ceux qui peuvent accéder à l&#39;enregistrement.

Cette mise à jour supprime le paramètre **Afficher tous les champs** et le remplace par des vues détaillées personnalisées.

Pour plus d’informations, voir [ Gérer la page d’enregistrement ](/help/quicksilver/planning/records/manage-the-record-page.md).

## Ajouter des regroupements à une page d’enregistrement connecté Projets

>[!NOTE]
>
>Aperçu : 14 mai 2026\
>Production rapide : 11 juin 2026>Production pour tous : 16 juillet 2026

Vous pouvez désormais regrouper vos informations dans la page Enregistrements connectés à des projets d’un enregistrement dans Workfront Planning. Cette fonctionnalité n&#39;existait pas dans ce domaine avant cette amélioration.

Pour plus d’informations, voir [ Gérer la vue Liste ](/help/quicksilver/planning/views/manage-the-list-view.md).
