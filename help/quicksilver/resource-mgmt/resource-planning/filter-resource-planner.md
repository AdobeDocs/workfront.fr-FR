---
product-area: resource-management
navigation-topic: resource-planning
title: Filtrage des informations dans le planificateur de ressources
description: '"(AL :*Répétez sur cet article : filtrage par données personnalisées. Autres améliorations ? La mise en garde des caractères spéciaux peut changer - suivez l''histoire pour savoir quand. Il est d''abord sorti en version bêta 3 17.3)'''
author: Alina
feature: Resource Management
exl-id: 7186cae5-1e16-421e-b26d-afb50aa7f6eb
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '2442'
ht-degree: 0%

---

# Filtrage des informations dans le planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(AL:*Iterate on this article: filtering by custom data. Other enhancements? Special characters caveat might change - follow the story to know when. It originally came in Beta 3 17.3.)</p>
-->

Les filtres vous permettent de modifier les informations affichées dans le planificateur de ressources à partir de toutes les informations stockées dans le système.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage ou accès supérieur à la gestion des projets, des utilisateurs et des ressources </p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations ou plus pour les projets</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Présentation des filtres du planificateur de ressources

Pour minimiser la quantité d’informations affichées dans le planificateur de ressources, Adobe Workfront fournit un filtre par défaut avec des critères préconfigurés. Pour plus d’informations sur le filtre par défaut, voir la section [Présentation du filtre par défaut dans le planificateur de ressources](#overview-of-the-default-filter-in-the-resource-planner) dans cet article.

Vous pouvez également créer des filtres personnalisés. Pour plus d’informations sur la personnalisation des filtres dans le planificateur de ressources, voir la section [Création de filtres de planificateur de ressources](#create-resource-planner-filters) dans cet article.

Tenez compte des points suivants lors de l’utilisation de filtres dans le planificateur de ressources :

* Les filtres que vous créez ne sont visibles que par vous. Vous pouvez partager des filtres pour les rendre disponibles à d’autres utilisateurs.
* En tant qu’administrateur de Workfront, vous ne pouvez voir que les filtres que vous créez ou qui sont partagés avec vous.
* Les résultats filtrés ne changent pas lorsque vous sélectionnez une autre vue pour le planificateur de ressources.\
   Pour plus d’informations sur la modification de la vue dans le planificateur de ressources, voir la section de sélection &quot;Projet/Rôle/Vue utilisateur&quot; dans [Présentation de la navigation de Resource Planner](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

* L’application d’un filtre ne modifie pas les données d’affectation et de disponibilité du planificateur de ressources pour les projets, les rôles ou les utilisateurs. Un filtre modifie uniquement le nombre d’objets que vous voyez dans le planificateur de ressources.
* Le filtrage s’applique à tous les objets qui s’affichent simultanément dans le planificateur de ressources. Par exemple, si vous filtrez un utilisateur spécifique, le planificateur de ressources affiche uniquement les résultats suivants :

   * Projets dans lesquels cet utilisateur fait partie du pool de ressources (pour les vues Projet et Rôle) ou a une affectation sur le projet (pour la vue Utilisateur)
   * Rôles associés à l’utilisateur sur ces projets\
      Les autres rôles ou utilisateurs des projets auxquels l’utilisateur est associé ne s’affichent pas.

## Présentation du filtre par défaut dans le planificateur de ressources {#overview-of-the-default-filter-in-the-resource-planner}

Lorsque vous ouvrez le planificateur de ressources pour la première fois, Workfront applique le filtre Par défaut. Vous pouvez modifier le filtre par défaut pour ne filtrer que les éléments que vous souhaitez afficher. Pour plus d’informations sur la modification d’un filtre, voir la section [Modification d’un filtre dans le planificateur de ressources](#edit-a-filter-in-the-resource-planner) dans cet article.

Tenez compte des points suivants lors de l’utilisation du filtre Par défaut :

* Le filtre par défaut récupère les informations uniquement des projets avec les éléments suivants :

   * Date d’achèvement planifiée qui survient après la première date du mois en cours
   * Date de début planifiée qui se produit avant le dernier jour du quatrième mois à partir de la date actuelle
   * État de la planification ou de l’état actuel

   >[!IMPORTANT]
   >
   >Le filtre par défaut récupère les informations des projets qui se produisent toujours dans les quatre mois à compter du premier jour du mois en cours, quelle que soit la période que vous sélectionnez pour l’affichage dans le planificateur de ressources.

* Dans la vue Utilisateur, tous les utilisateurs du système s’affichent, mais seuls les utilisateurs associés aux projets filtrés affichent les informations sur l’heure.
* Vous pouvez éditer les informations du filtre Par défaut sans enregistrer le filtre.
* Vous pouvez dupliquer et modifier une copie du filtre Par défaut, y modifier les critères souhaités, puis l’enregistrer en tant que nouveau filtre.
* Vous ne pouvez pas supprimer ni partager le filtre Par défaut.

   ![RP_new_default_fitler_critères__1_.PNG](assets/rp-new-default-fitler-criteria--1--301x547.png)

## Création de filtres de planificateur de ressources {#create-resource-planner-filters}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: **^ This section is somewhat duplicated (format more than content) from the "Filtering Utilization Information" section in "Viewing Utilization Information for Projects, Programs, and Portfolios.")</p>
-->

La création d’un filtre dans le planificateur de ressources est identique pour toutes les vues.

Assurez-vous que les conditions préalables pour afficher les informations correctes dans le planificateur de ressources sont bien remplies avant de créer un filtre.\
Pour plus d’informations sur les conditions préalables requises pour travailler avec le planificateur de ressources, voir la section &quot;Conditions préalables requises pour travailler dans le planificateur de ressources&quot; dans la section [Présentation de Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md) article.

Tenez compte des points suivants lors de la création d’un filtre :

* Il n’existe aucune limite quant au nombre d’objets pour lesquels vous pouvez filtrer simultanément.
* Les champs disponibles que vous pouvez ajouter à un filtre changent en fonction de l’objet de la vue que vous appliquez au planificateur de ressources. Par exemple, vous pouvez filtrer les champs Problème ou Tâche uniquement dans la vue Utilisateur, car ces objets s’affichent uniquement dans la vue Utilisateur. Si vous créez un filtre pour Problèmes ou tâches dans la vue Utilisateur, puis l’appliquez aux vues Projet ou Rôle , il est ignoré car les champs n’existent pas dans les vues Projet ou Rôle. Dans ce cas, le filtre apparaît indisponible.

Pour créer un filtre dans le planificateur de ressources :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Ressource**.

   Le **Planificateur** s’affiche par défaut.

   Par défaut, la première fois que vous accédez au planificateur de ressources, la variable <strong>Filtre par défaut</strong> est appliquée.<br>Pour plus d’informations sur le filtre Par défaut, voir la section <a href="#overview-of-the-default-filter-in-the-resource-planner" class="MCXref xref">Présentation du filtre par défaut dans le planificateur de ressources</a> dans cet article.

1. Dans le coin supérieur gauche de , cliquez sur le bouton **Filtrer** icône .\
   ![filter_icon.png](assets/filter-icon.png)\
   Ou\
   Développez l’objet **Filtrer** menu déroulant, puis cliquez sur **Ajouter un nouveau filtre**.\
   ![](assets/rp-filter-dropdown-expanded-with-default-filter-selected-350x283.png)

1. Pour créer un filtre à l’aide des critères intégrés, spécifiez l’un des champs suivants :

   * **Portfolio**: Commencez à saisir le nom du portfolio qui contient les informations que vous souhaitez inclure dans le planificateur de ressources, puis cliquez sur le nom lorsqu’il apparaît dans la liste.\
      Répétez cette procédure pour inclure des informations provenant de plusieurs portefeuilles.

   * **État du projet**: Développez le menu déroulant État du projet et sélectionnez un ou plusieurs états de projet disponibles dans la liste.
   * **Équipe**: Commencez à saisir le nom d’une ou de plusieurs équipes associées aux utilisateurs affectés aux tâches dans les projets que vous souhaitez afficher.
   * **Rôle de tâche**: Commencez à saisir le nom d’un ou de plusieurs rôles de tâche associés aux utilisateurs affectés aux tâches dans les projets que vous souhaitez afficher.
   * **Pools**: Commencez à saisir le nom d’un ou de plusieurs groupes de ressources associés aux projets (pour la vue Projet), aux utilisateurs (pour la vue Utilisateur) ou associés aux projets et aux utilisateurs (pour la vue Rôle) que vous souhaitez afficher.
   * **Groupe**: Commencez à saisir le nom d’un ou de plusieurs groupes associés aux utilisateurs (dans la vue Utilisateur) ou aux projets (dans les vues Projet et Rôle) que vous souhaitez afficher.

1. Cliquez sur **Ajouter une règle de filtre**, puis commencez à saisir le nom du champ par lequel vous souhaitez filtrer les données dans la variable **Type pour le filtrage des éléments** de la boîte. Si le champ est disponible, il est renseigné pour chaque objet auquel il peut être associé.

   >[!IMPORTANT]
   >
   >Lorsque vous référencez des champs personnalisés, vous devez saisir le nom du champ et non le libellé du champ. Le libellé du champ s’affiche sur un formulaire personnalisé associé à un objet. Pour plus d’informations sur la différence entre le libellé et le nom d’un champ personnalisé, voir  [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

1. Cliquez sur le nom du champ à ajouter au filtre lorsqu&#39;il apparaît dans la liste.\
   Pour plus d’informations sur les champs que vous voyez dans la liste, voir [Glossaire de la terminologie Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. (Facultatif) Sélectionnez les modificateurs de condition et de filtre pour le filtre. Les modificateurs disponibles sont décrits dans la section [Modificateurs de filtre et de condition](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Vous pouvez utiliser des caractères génériques ou des caractères génériques basés sur des dates pour filtrer les informations associées à l’utilisateur connecté.\
   Pour plus d’informations sur les caractères génériques pris en charge dans les filtres, voir [Variables de filtre génériques](../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Cliquez sur **Enregistrer** pour enregistrer la règle de filtrage.
1. (Facultatif) Cliquez sur **Ajouter une règle de filtre** pour ajouter une nouvelle règle pour un autre objet ou champ.
1. Cliquez sur **Appliquer** pour appliquer le filtre sans l’enregistrer.

   Ou

   Cliquez sur **Enregistrer le filtre** pour enregistrer le filtre.\
   ![RP_Apply_or_Save_button_on_filters.png](assets/rp-apply-or-save-buttons-on-filters-320x79.png)

1. (Conditionnel) Après avoir cliqué sur **Enregistrer**, spécifiez un nom pour le filtre dans la variable **Nom du filtre** à l’intérieur de la zone **Enregistrer le filtre** de la boîte de dialogue Champ obligatoire.\
   ![RP_new_save_filter_box__with_Save_button__without_apply.png](assets/rp-new-save-filter-box--with-save-button--without-apply-350x175.png)

   >[!NOTE]
   >
   >Si le nom de votre filtre contient des caractères spéciaux, vous utilisez uniquement les caractères suivants :
   >
   >* Virgule
   >* Slash
   >* Trait d’union
   >* Soulignement


1. Cliquer sur **Enregistrer**.

   Les résultats du planificateur de ressources sont désormais filtrés par les informations que vous avez incluses dans les règles de filtrage.

## Appliquer un filtre existant

Lorsque vous ou une personne ayant accès au planificateur de ressources enregistrez un filtre, celui-ci devient disponible pour tous les utilisateurs du planificateur de ressources.

Pour appliquer un filtre existant :

1. Accédez au planificateur de ressources.
1. Dans le coin supérieur gauche, développez la variable **Filtrer** menu déroulant.

   Vous pouvez voir les filtres que vous avez créés ou d’autres qui ont été créés et partagés avec vous dans ce menu.\
   ![RP_filter_drop_down.png](assets/rp-filter-drop-down-350x152.png)

1. Sélectionnez un filtre dans le menu déroulant. Vous pouvez voir les filtres que vous ou d’autres utilisateurs avez créés dans ce menu.\
   Lorsque vous sélectionnez un filtre, la quantité d’informations affichées dans le planificateur de ressources est automatiquement réduite.

## Modification d’un filtre dans le planificateur de ressources {#edit-a-filter-in-the-resource-planner}

Vous pouvez modifier un filtre dans le planificateur de ressources en effectuant l’une des opérations suivantes :

* [Renommer un filtre](#rename-a-filter)
* [Editer les informations d&#39;un filtre](#edit-the-information-in-a-filter)
* [Dupliquer un filtre](#duplicate-a-filter)

Lorsque vous modifiez un filtre, celui-ci est mis à jour pour tous les utilisateurs du système ayant accès au planificateur de ressources.

### Renommer un filtre {#rename-a-filter}

Vous pouvez modifier le nom d’un filtre sans modifier ses critères. Nous vous recommandons de faire savoir à d’autres utilisateurs du système ce changement, car les filtres sont visibles par d’autres utilisateurs. Cette modification affecte les listes de filtres pour tous ceux qui peuvent voir le planificateur de ressources.

1. Accédez au planificateur de ressources et développez la variable **Filtrer** pour sélectionner un filtre enregistré.
1. Développez l’objet **Filtrer** menu déroulant. Recherchez le filtre que vous souhaitez renommer et survolez son nom avec la souris.
1. Sélectionnez la **Renommer le filtre** en regard du nom du filtre.

   ![](assets/rp-filter-options-edit-350x154.png)

1. Spécifiez un nouveau nom pour le filtre dans la variable **Nom du filtre** de la boîte.
1. Cliquer sur **Enregistrer**.\
   Les informations incluses dans le filtre sont les mêmes et le nom est mis à jour.

### Editer les informations d&#39;un filtre {#edit-the-information-in-a-filter}

Vous pouvez modifier les informations que vous incluez dans un filtre sans modifier son nom. Nous vous recommandons de faire savoir à d’autres utilisateurs du système ce changement, car les filtres leur sont visibles. Cette modification affecte les listes de filtres pour tous ceux qui peuvent voir le planificateur de ressources.

1. Accédez au planificateur de ressources et développez la variable **Filtrer** menu déroulant dans le coin supérieur gauche.
1. Sélectionnez un filtre existant à modifier.
1. Cliquez sur le bouton **Filtrer** icône .\
   ![filter_icon.png](assets/filter-icon.png)

1. Ajoutez de nouveaux champs au filtre.\
   Pour plus d’informations sur la création de filtres, voir [Création de filtres de planificateur de ressources](#create-resource-planner-filters).

1. Pointez sur les champs existants sélectionnés pour le filtre, puis cliquez sur l’icône **Modifier** pour sélectionner un autre champ, ou la variable **Supprimer** pour supprimer le champ.\
   ![RP_custom_filter_delete_and_edit_icons.png](assets/rp-custom-filter-delete-and-edit-icons-350x169.png)

1. (Facultatif) Cliquez sur **Ajouter une règle de filtre** pour ajouter de nouveaux champs au filtre.\
   Pour plus d’informations sur la définition des critères de filtre, voir [Création de filtres de planificateur de ressources](#create-resource-planner-filters).

1. Cliquez sur **Appliquer** pour appliquer le filtre sans l’enregistrer.

   Ou

   Cliquez sur **Enregistrer** pour enregistrer le filtre.\
   Le filtre est enregistré avec le même nom mais avec de nouveaux critères de filtrage.

### Dupliquer un filtre {#duplicate-a-filter}

Vous pouvez dupliquer un filtre existant. Les critères de filtrage d&#39;origine restent identiques dans le filtre dupliqué et vous pouvez enregistrer le nouveau filtre sous un nouveau nom.

1. Accédez au planificateur de ressources et développez la variable **Filtrer** menu déroulant dans le coin supérieur gauche.
1. Pointez sur le nom d’un filtre enregistré que vous souhaitez dupliquer.
1. Cliquez sur le bouton **Dupliquer** icône .

   ![](assets/rp-filter-options---duplicate-350x154.png)\
   La zone Dupliquer le filtre s’affiche.

1. Dans le **Nom du filtre** , indiquez un nouveau nom pour le filtre dupliqué.\
   Le nom par défaut du nouveau filtre est *`<Original Filter Name>`(copie)*.

1. Cliquer sur **Enregistrer**. Un nouveau filtre est créé avec les mêmes critères que le filtre d&#39;origine et un nouveau nom.

   >[!NOTE]
   >
   >Bien que vous puissiez avoir 2 filtres portant le même nom et des critères identiques, nous vous recommandons d’enregistrer les filtres avec des critères et des noms de filtrage uniques dans votre planificateur de ressources afin d’éviter toute confusion.

## Supprimer un filtre

Vous pouvez supprimer un filtre lorsqu’il n’est plus nécessaire. Vous ne pouvez pas supprimer le filtre par défaut.

Pour plus d’informations sur le filtre par défaut, voir [Présentation du filtre par défaut dans le planificateur de ressources](#overview-of-the-default-filter-in-the-resource-planner) dans cet article.

Lorsque vous supprimez un filtre, celui-ci est supprimé pour tous les utilisateurs Workfront ayant accès au planificateur de ressources. Avant de le supprimer, assurez-vous que le filtre que vous souhaitez supprimer n’est plus utilisé par quiconque travaille dans le planificateur de ressources. Un filtre supprimé ne peut pas être récupéré.

Pour supprimer un filtre :

1. Accédez au planificateur de ressources.
1. Développez l’objet **Filtrer** menu déroulant.
1. Recherchez le filtre à supprimer et survolez son nom avec la souris.
1. Sélectionnez la **Supprimer le filtre** en regard du nom du filtre.

   ![](assets/rp-filter-options---delete-350x154.png)

1. Cliquez sur **Supprimer** dans le **Supprimer le filtre** de la boîte de dialogue

1. Le filtre est supprimé et supprimé du planificateur de ressources.

## Partage d’un filtre

Vous pouvez partager un filtre que vous avez créé ou que vous avez accès à partager avec d’autres utilisateurs. Vous ne pouvez pas partager le filtre par défaut, mais vous pouvez le dupliquer et partager la copie.

>[!NOTE]
>
>Tous les utilisateurs, y compris les administrateurs Workfront, ne peuvent accéder qu’aux filtres qu’ils ont créés ou qui ont été partagés avec eux. Vous pouvez partager un filtre avec des utilisateurs spécifiques afin de rendre un filtre disponible pour tous les utilisateurs du planificateur de ressources.

Pour plus d’informations sur le filtre par défaut, voir [Présentation du filtre par défaut dans le planificateur de ressources](#overview-of-the-default-filter-in-the-resource-planner) dans cet article.

Pour plus d’informations sur la duplication de filtres, voir [Dupliquer un filtre](#duplicate-a-filter) dans cet article.

1. Accédez au planificateur de ressources.
1. Développez l’objet **Filtrer** menu déroulant.
1. Recherchez le filtre que vous souhaitez partager et survolez son nom avec la souris.
1. Sélectionnez la **Partager le filtre** en regard du nom du filtre.

   ![](assets/rp-filter-options---share-350x154.png)

   La boîte de dialogue Accès aux filtres s’affiche.

1. (Facultatif) Pour mettre le filtre à la disposition de tous les utilisateurs du planificateur de ressources, cliquez sur le bouton **Paramètres** puis sélectionnez **rendre visible à l’échelle du système ;**.

   ![](assets/make-this-visible-system-wide-350x119.png)

1. Dans le **Accédez à :** , commencez à saisir les noms des utilisateurs, équipes, rôles, groupes ou entreprises avec lesquels vous souhaitez partager le filtre.
1. Sélectionnez l’un des niveaux d’autorisation suivants :

   * Afficher
   * Gérer

      Pour plus d’informations sur les autorisations dans Workfront, voir [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

1. (Facultatif) Cliquez sur **Paramètres avancés** pour ajouter des autorisations pour chaque niveau en les sélectionnant ou supprimer des autorisations pour chaque niveau en les désélectionnant.

   ![](assets/rp-share-filter-manage-advanced-settings-350x271.png)

1. Cliquer sur **Enregistrer**.

   Le filtre est partagé avec les entités que vous avez sélectionnées et il apparaît dans la variable **Partagé avec moi** zone.

   ![](assets/rp-shared-with-me-area.png)
