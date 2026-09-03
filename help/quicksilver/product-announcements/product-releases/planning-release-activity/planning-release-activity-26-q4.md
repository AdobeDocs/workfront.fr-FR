---
content-type: release-notes
title: Activité de mise à jour du quatrième trimestre 2026 pour Adobe Workfront Planning
description: Il s’agit de l’activité de publication du produit Planification d’Adobe Workfront pour le quatrième trimestre 2026.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 3f0a939e9de6436117fcb8242449793dcef73205
workflow-type: tm+mt
source-wordcount: '1770'
ht-degree: 3%

---

# Activité de mise à jour du quatrième trimestre 2026 pour Adobe Workfront Planning

Cet article décrit les nouvelles fonctionnalités de Workfront Planning de la version du quatrième trimestre 2026.

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning, voir [Activité de version d’Adobe Workfront Planning : index des articles](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Gérer la visibilité des miniatures et des couleurs des enregistrements à partir de la colonne du champ principal dans la vue Tableau

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Vous pouvez désormais gérer la visibilité des miniatures et des couleurs des enregistrements lors de la modification de la colonne du champ principal en mode Tableau.

Avec cette mise à jour, la miniature et les paramètres de couleur sont supprimés de l’icône Champs dans la barre d’outils du mode Tableau.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

## Créer des règles métier pour les types d’enregistrements

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

En tant que gestionnaire d’espace de travail, vous pouvez désormais définir des règles métier pour les types d’enregistrements qui se répercuteront ultérieurement sur la manière dont les enregistrements de ce type sont gérés. Vous pouvez définir des règles qui permettent aux utilisateurs de modifier ou de supprimer des enregistrements uniquement lorsque certaines conditions sont remplies ou que certains champs sont renseignés.

Vous pouvez créer une condition pour votre règle métier qui fait référence à tous les types de champ, à l’exception des suivants :

* Champs de formule
* Champs de recherche
* Champs de référence

Vous ne pouvez pas ajouter de règles métier aux types d’enregistrements globaux.

Pour plus d’informations, voir [Configurer des règles métier de type enregistrement](/help/quicksilver/planning/architecture/configure-business-rules.md).

>[!NOTE]
>
>Avec cette mise à jour, les options de menu suivantes du menu Plus d’un type d’enregistrement ont également été mises à jour :
>
>* **Créer des formulaires de demande** et **Gérer les formulaires de demande** est devenu **Formulaires de demande**
>* **Gérer les automatisations** est devenu **Automatisations**

## Introduction de semaines personnalisées pour la vue chronologique

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

En tant qu’administrateur Workfront, vous pouvez désormais configurer des semaines personnalisées, en plus des trimestres personnalisés. Les semaines et les trimestres personnalisés sont visibles à partir de la vue chronologique de Workfront Planning. Workfront génère des semaines séquentielles à partir de la semaine 1 au début du trimestre personnalisé 1.

Vous pouvez personnaliser les libellés des semaines qui sont visibles dans la vue chronologique. Vous pouvez choisir un format prédéfini ou en saisir un personnalisé.

Les semaines personnalisées ne sont pas visibles dans Workfront. Ils ne sont visibles que dans la vue chronologique Planification de Workfront.

Pour plus d’informations, voir [Activer les trimestres personnalisés](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Filtres pour les champs d’enregistrement connectés dépendants

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Vous pouvez désormais filtrer certains types d&#39;enregistrements qui répondent à un critère de filtre lorsque vous ajoutez des connexions dépendantes dans Planning.

Au lieu que tous les types d’enregistrement soient disponibles dans les champs connectés dépendants, seuls ceux qui répondent à vos critères de filtrage s’afficheront.

Pour cette fonctionnalité, nous avons ajouté une nouvelle option Règles de filtrage des enregistrements dans l&#39;onglet Nouvelle connexion lors de la connexion des types d&#39;enregistrements.

Pour plus d’informations, voir [Gestion des connexions dépendantes](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Réduire et développer tous les regroupements dans la vue chronologique

>[!NOTE]
>
>Aperçu : 27 août 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Les vues de chronologie incluent désormais les options Réduire tout et Développer tout pour les chronologies regroupées. Il est ainsi plus facile de parcourir les vues de feuille de route volumineuses : vous pouvez rapidement réduire la vue en en-têtes de regroupement, puis développer uniquement les sections que vous souhaitez examiner.

Pour plus d’informations, voir [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Afficher les noms complets des groupes et redimensionner le panneau de regroupement dans la vue chronologique

>[!NOTE]
>
>Aperçu : 27 août 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Dans la vue chronologique, le survol d’un libellé de groupe tronqué avec la souris affiche désormais le texte complet dans une info-bulle, à la fois dans le plan directeur et dans les regroupements empilés. Les libellés non tronqués n’affichent pas d’info-bulle.

Le panneau de gauche du regroupement dans l’affichage Couloir peut désormais être redimensionné en faisant glisser sa division. La vue est mise à jour en temps réel, ce qui est cohérent avec la vue du tableau. La largeur de panneau de chaque utilisateur est enregistrée entre les sessions, avec une largeur par défaut pour les nouveaux utilisateurs.

Pour plus d’informations, consultez [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Amélioration des performances du calendrier pour les jeux d’enregistrements volumineux dans la vue Semaine

>[!NOTE]
>
>Aperçu : 27 août 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

La vue Semaine du calendrier affiche désormais uniquement les 1 000 premiers enregistrements sur la période hebdomadaire visible. S’il existe d’autres enregistrements, le message suivant s’affiche au bas du calendrier pour indiquer que d’autres enregistrements sont disponibles : « Il existe d’autres enregistrements. Charger plus. »

Pour plus d’informations, voir [ Gérer la vue Calendrier ](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Mise à jour des en-têtes de colonne pour les champs d’enregistrement connectés dépendants

>[!NOTE]
>
>Aperçu : 20 août 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Nous avons apporté des améliorations visuelles aux en-têtes de colonne pour un champ d’enregistrement connecté dépendant dans la vue Tableau.

Pour plus d’informations, voir [Gestion des connexions dépendantes](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

## Améliorations de la vue Tableau lors du glisser-déposer de plusieurs lignes

>[!NOTE]
>
>Aperçu : 13 août 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026
>[!BADGE Hors planning]{type=Neutral}

De nouveaux indicateurs visuels s’affichent lorsque vous faites glisser et déposez plusieurs lignes dans la vue Tableau. Un signe plus important et un indicateur numérique indiquent désormais le nombre de lignes sélectionnées pour l’action de glisser-déposer.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

## Acheminez l’objet de requête envoyé vers l’espace de travail correct lors de l’utilisation de types d’enregistrements globaux

>[!NOTE]
>
>Aperçu : 13 août 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Les enregistrements créés pour les types d&#39;enregistrements globaux en soumettant un formulaire de demande sont désormais automatiquement acheminés vers l&#39;espace de travail à partir duquel ils ont été soumis.

Les enregistrements créés en soumettant une demande depuis un espace de travail secondaire d&#39;un type d&#39;enregistrement global sont ajoutés à cet espace de travail secondaire. Les enregistrements créés par l’envoi d’une demande depuis l’espace de travail d’origine ou depuis la zone des Demandes principale sont ajoutés à l’espace de travail d’origine.

Si le formulaire de saisie comprend un champ Workspace et qu’un utilisateur sélectionne un espace de travail avant l’envoi, la demande est acheminée vers l’espace de travail sélectionné, quel que soit l’endroit où le formulaire a été lancé. Cela permet de s’assurer que les enregistrements sont organisés dans l’espace de travail prévu à partir du moment où ils sont créés.

Pour plus d’informations, voir [Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## Présentation de la compétence d’architecte de solution Workfront Planning

>[!NOTE]
>
>Aperçu : 10 août 2026
>Production : 10 Août 2026

Nous publions une nouvelle compétence, l’architecte de solution Workfront Planning, qui apporte des conseils agentiques et de bonnes pratiques pour Workfront Planning directement dans Claude :

* **Configurer** nouveaux espaces de travail Planning aux spécifications, avec le serveur MCP Workfront exécutant le programme d’installation dans votre environnement.
* **Audit** configurations existantes pour les antimodèles à grande échelle.
* **Vérifiez l’utilisation** par rapport aux limites recommandées (enregistrements, connexions, profondeur de hiérarchie).
* **Posez des questions** sur Planning à tout moment.

Au-delà de la configuration initiale, la compétence soutient la gouvernance continue en capturant la dérive de configuration avant qu&#39;elle ne provoque des frictions, en signalant les limites avant qu&#39;elles ne deviennent des bloqueurs, en appliquant des normes cohérentes dans chaque espace de travail, indépendamment de qui le configure et en donnant des réponses précises à toute personne de l&#39;équipe sans attendre un spécialiste. Ensemble, ils couvrent tout le cycle de vie de la configuration correcte d’un espace de travail et de son maintien à mesure que l’utilisation augmente.

Pour plus d’informations, voir [Compétences disponibles pour une installation directe](/help/quicksilver/workfront-basics/workfront-mcp-server/direct-skills.md).

## Glisser-déposer des lignes en mode Tableau

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

L’expérience de glisser-déposer de lignes en mode Tableau a été améliorée visuellement.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).


## Champs d’enregistrement connectés dépendants

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Les gestionnaires de Workspace peuvent désormais définir des dépendances entre les types d’enregistrements connectés. Par exemple, s’assurer qu’un champ Région affiche uniquement les valeurs liées à la zone géographique sélectionnée. Cette configuration s’effectue directement dans la configuration du champ de connexion : lors de l’ajout d’une connexion d’un type d’enregistrement Géographique à un type d’enregistrement dépendant (comme Région), un nouveau paramètre permet aux gestionnaires de l’espace de travail de la marquer comme dépendante du type d’enregistrement Géographique, en utilisant les relations déjà établies entre ces types d’enregistrement.

Une fois configuré, tout type d’enregistrement qui fait référence aux deux champs (une campagne, par exemple) voit immédiatement l’effet : la sélection d’une valeur Géo limite le sélecteur de Région aux régions réellement liées à cette zone géographique. Cela permet d’appliquer automatiquement la structure des enregistrements, d’éliminer les combinaisons incohérentes et de réduire le nettoyage manuel.

Les fonctionnalités suivantes sont incluses dans cette mise à jour :

* Nous avons ajouté la nouvelle section Paramètres de connexion dans l’onglet Nouvelle connexion, lors de la connexion de types d’enregistrements
* Nous avons ajouté un paramètre Rendre cette connexion dépendante dans la nouvelle section .


Pour plus d’informations, voir [Gestion des connexions dépendantes](/help/quicksilver/planning/architecture/manage-dependent-connections.md).




## Afficher un nouvel indicateur de commentaire pour un enregistrement en mode Tableau

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Nous avons ajouté un nouvel indicateur qui s’affiche lorsqu’un enregistrement contient des commentaires non lus. L&#39;indicateur s&#39;affiche dans le coin supérieur droit du champ principal de l&#39;enregistrement en mode Tableau.

Pour plus d’informations, consultez la section [Gérer les commentaires d’enregistrements](/help/quicksilver/planning/records/manage-record-comments.md).

## Couleur d’enregistrement personnalisable et codage des couleurs basé sur les connexions

>[!NOTE]
> 
>Aperçu : 23 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Les enregistrements prennent désormais en charge les palettes de couleurs personnalisables qui vous permettent de mettre à jour les couleurs automatiquement attribuées aux nouveaux enregistrements vers des couleurs standard ou personnalisées.

Les modifications suivantes sont incluses dans cette amélioration : 

* Nous avons ajouté l’option Couleur aux zones suivantes :
  * L’icône Champs en mode Tableau. 
  * La section Style de barre de la zone Paramètres d’une chronologie et d’un calendrier

    Lorsque le paramètre Couleur est activé, la couleur affectée au nouvel enregistrement s&#39;affiche partout où l&#39;enregistrement s&#39;affiche dans ces vues. 

* Un cercle de couleurs est ajouté à la page Détails de l’enregistrement. 
* Vous pouvez désormais ajouter des champs d’enregistrement connectés, à sélection unique et multiple au codage de couleur des barres dans les vues Chronologie et Calendrier lors de la coloration par les valeurs de champ. 
* Vous pouvez activer l’affichage de la couleur, en plus du nom et de l’image d’un enregistrement lorsque vous créez des champs d’enregistrement connectés. 
* La section Couleur de la zone Paramètres a également été rationalisée en supprimant l’option « Aucun ».  

Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md). 

## Planning Designer nécessite désormais l’acceptation du contrat Beta

>[!NOTE]
>Prévisualisation et production pour tous les clients : 20 juillet 2026
>[!BADGE Hors planning]{type=Neutral}

Planning Designer nécessite désormais un accord Beta accepté pour être utilisé. Votre entreprise n’est pas tenue de signer un accord d’IA. Cette option est disponible pour tous les clients.

Pour cela, nous avons déplacé l’option Planning Designer dans la section Configuration sous la section Souscription aux versions bêta de l’IA.

Le lancement de Planning Designer sans accord Beta accepté vous invite désormais à l’accepter avant l’ouverture du créateur d’espace de travail.

Pour plus d’informations, voir [Prise en main d’Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).
