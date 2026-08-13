---
content-type: release-notes
title: Activité de mise à jour du quatrième trimestre 2026 pour Adobe Workfront Planning
description: Il s’agit de l’activité de publication du produit Planification d’Adobe Workfront pour le quatrième trimestre 2026.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: c34c4f351010980098b3efece8643a5f5620917f
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 3%

---

# Activité de mise à jour du quatrième trimestre 2026 pour Adobe Workfront Planning

Cet article décrit les nouvelles fonctionnalités de Workfront Planning de la version du quatrième trimestre 2026.

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning, voir [Activité de version d’Adobe Workfront Planning : index des articles](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Améliorations de la vue Tableau lors du glisser-déposer de plusieurs lignes

>[!NOTE]
>
>Aperçu : 13 août 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

De nouveaux indicateurs visuels s’affichent lorsque vous faites glisser et déposez plusieurs lignes dans la vue Tableau. Un signe plus important et un indicateur numérique indiquent désormais le nombre de lignes sélectionnées pour l’action de glisser-déposer.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Collapse and expand all groupings in the timeline view

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Timeline views now include Collapse all and Expand all options for grouped timelines. This makes it easier to navigate large roadmap views: you can quickly reduce the view to grouping headings, then expand only the sections you want to review.

For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

-->

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

<!--

## Updated column headers for dependent connected record fields

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

We've made visual improvements to the column headers for a dependent connected record field in the table view.

For information, see [Manage dependent connections](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

-->

## Présentation de la compétence d’architecte de solution Workfront Planning

>[!NOTE]
>
>Aperçu : 10 août 2026
>Production : 10 Août 2026

Nous mettons à disposition une nouvelle compétence, l’architecte de solution de planification Workfront, qui apporte des conseils d’agent et de bonne pratique pour la planification Workfront directement dans Claude. Dans l’interface Claude, vous pouvez désormais effectuer les opérations suivantes :

* Configurez un nouvel espace de travail Planning pour répondre aux besoins de votre entreprise, le serveur Workfront MCP exécutant la configuration dans votre environnement.
* Effectuez l’audit d’une configuration existante pour détecter des antimodèles à grande échelle.
* Vérifiez l’utilisation par rapport aux limites recommandées.
* Posez des questions sur Planning.

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
