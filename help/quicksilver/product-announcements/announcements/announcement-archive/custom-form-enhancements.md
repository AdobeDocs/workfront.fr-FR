---
title: Améliorations apportées aux formulaires personnalisés
description: Les améliorations significatives suivantes ont été apportées à la gestion des formulaires personnalisés dans la version 22.2.
author: Luke
feature: Product Announcements, Custom Forms
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: 8dac7959919014d7bfbbbd39d193d026ca31c4b2
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 98%

---

# Améliorations apportées aux formulaires personnalisés

Les améliorations significatives suivantes ont été apportées à la gestion des formulaires personnalisés dans la version 22.2.

## Ajouter des widgets de ressources

Vous pouvez incorporer une image dans vos formulaires personnalisés. Vous pouvez ainsi communiquer avec les utilisateurs et utilisatrices de formulaires personnalisés de manière plus interactive et visuelle. D’autres types de widgets seront bientôt disponibles.

![](assets/image-in-custom-form.png)

Lorsqu’un formulaire personnalisé contenant un widget est associé à un objet, les utilisateurs et utilisatrices qui travaillent avec l’objet peuvent le voir dans les zones suivantes :

* La zone Détails de l’objet (par exemple, pour un projet, la zone Détails du projet)

  ![](assets/see-image-details-page.png)

* La boîte Modifier de l’objet, si l’aspect de l’expérience Adobe Workfront est nouvelle (par exemple, les boîtes Modifier le projet et Modifier la tâche)

  ![](assets/image-see-in-edit.png)

Actuellement, les utilisateurs et utilisatrices ne peuvent pas voir le widget dans les zones suivantes :

* Listes et rapports
* Accueil et Récapitulatif
* La zone Modifier de l’objet, s’il ne présente pas l’apparence de la nouvelle expérience Adobe Workfront (par exemple, la zone Modifier les dépenses).
* Application mobile Workfront

## Associer un formulaire personnalisé à plusieurs types d’objets

Vous pouvez associer plusieurs types d’objet à n’importe quel nouveau formulaire personnalisé :

![](assets/new-custom-form-object-types.png)

Ou tout formulaire personnalisé existant :

![](assets/add-object-type-existing-form.png)

Vous pouvez ainsi créer un formulaire personnalisé unique à utiliser sur les projets, les tâches, les problèmes et tout autre type d’objet pris en charge pour les formulaires personnalisés.

Cela s’avère particulièrement utile lorsque vous convertissez un problème ou une tâche, car vous pouvez transférer un formulaire personnalisé et ses données vers l’objet converti. Vous n’avez plus besoin de créer et de gérer des copies exactes d’un même formulaire personnalisé pour différents types d’objets. Ajoutez manuellement le formulaire personnalisé au projet.

>[!INFO]
>
>**Exemple :**
>
>Quelqu’un envoie une demande informatique interne (problème) et fournit des détails sur ce qui est nécessaire dans un formulaire personnalisé joint.
>
>Vous convertissez le problème en projet pour les utilisateurs et utilisatrices qui travailleront dessus.
>
>Comme le formulaire personnalisé contenant les détails de l’auteur ou autrice est associé aux types d’objet Problème et Projet, le formulaire personnalisé et tous ces détails sont transmis au projet pendant la conversion.

>[!NOTE]
>
>Lorsque la conversion a lieu, le formulaire personnalisé doit déjà être associé au type d’objet vers lequel vous convertissez.

Tenez compte des points suivants lorsque vous créez ou modifiez un formulaire personnalisé à plusieurs objets :

* [Options d’autorisation pour les sauts de section](#permission-options-for-section-breaks)
* [Compatibilité des champs personnalisés calculés](#calculated-custom-field-compatibility)
* [Attention à la suppression d’un type d’objet d’un formulaire personnalisé](#caution-about-deleting-an-object-type-from-a-custom-form)

### Options d’autorisation pour les sauts de section

L’ensemble des options d’autorisation de saut de section disponibles pour les types d’objets Problème, Tâche, Projet et Utilisation comporte une option d’autorisation en plus de l’ensemble des options d’autorisation pour tous les autres types d’objets : Modification limitée.

![](assets/section-break-permissions-limited-edit.png)

L’ensemble des autorisations de saut de section disponibles pour tous les autres types d’objets (Portfolio, Document, Programme, Dépenses, Entreprise, Itération, Enregistrement de facturation et Groupe) n’inclut pas l’option Modification limitée :

![](assets/section-break-permissions-no-limited-edit.png)

Dans un formulaire personnalisé associé aux types d’objets de ces deux groupes, le système utilise un ensemble commun d’autorisations de saut de section qui fonctionne pour tous les types d’objets. En particulier, au lieu d’utiliser l’option d’autorisation Modification limitée, cet ensemble commun remplace l’option d’autorisation Modifier par l’option d’autorisation Modification limitée. L’option Modifier est compatible avec tous les types d’objets.

Lorsque vous associez un type d’objet qui utilise des options d’autorisation différentes des autres types d’objet déjà présents sur un formulaire personnalisé, un message s’affiche et vous permet de passer à l’ensemble commun d’options d’autorisation qui sera utilisé pour le formulaire. Cette modification s’applique à tous les champs, même s’ils ne sont pas sous un saut de section.

### Compatibilité des champs personnalisés calculés

Dans un formulaire personnalisé à plusieurs objets, si un champ calculé fait référence à des champs pouvant être utilisés avec tous les types d’objets associés au formulaire (tels que {name}, {description} et {entryDate}, disponibles pour plusieurs types d’objets), les données sont correctement calculées, quel que soit l’objet auquel vous le joignez.

Par exemple, si vous disposez d’un formulaire à plusieurs objets pour les projets et les problèmes et que vous ajoutez un champ calculé contenant l’expression {name}, le champ affiche le nom du projet lorsque vous ajoutez le formulaire à un projet et le nom de la tâche lorsque vous ajoutez le formulaire à une tâche.

Les champs non compatibles avec l’objet s’affichent sous la forme N/A.

>[!INFO]
>
>**Exemple :** dans un formulaire personnalisé associé au type d’objet Tâche, vous créez un champ personnalisé calculé qui référence le champ intégré « Affecté à : nom » afin qu’il puisse afficher le nom de la personne cessionnaire principale chaque fois que le formulaire est joint à une tâche :
>
>```
>Assigned To: Name{assignedTo}.{name}
>```
>
>Par la suite, vous ajoutez le type d’objet Projet au formulaire personnalisé. Un message d’avertissement vous indique que le type d’objet Projet est incompatible avec le champ personnalisé calculé. En effet, le champ « Assigné à » n’est pas disponible pour les projets.

Dans ce cas, vous pouvez effectuer l’une des opérations suivantes :

* Supprimez l’un des deux éléments incompatibles du formulaire personnalisé : le type d’objet ou le champ référencé.
* Conservez les deux éléments et utilisez la variable de filtre de caractères génériques `$$OBJCODE` comme condition dans une expression IF pour créer deux versions différentes du champ « En charge ». Cela permet au champ de fonctionner correctement, quel que soit le type d’objet auquel le formulaire est associé.

  En reprenant l’exemple ci-dessus, bien qu’il n’existe pas de champ « Affecté à : nom » intégré pour les projets, il existe un champ « Propriétaire » intégré (qui renseigne automatiquement le nom de la personne qui a créé le projet, sauf si quelqu’un modifie manuellement ce champ). Ainsi, dans votre champ personnalisé « En charge », vous pouvez utiliser `$$OBJCODE` comme illustré ci-dessous pour faire référence au champ « Propriétaire » lorsque le formulaire personnalisé est joint à un projet, et au champ « Affecté à : nom » lorsque le formulaire est joint à une tâche :

  ```
  IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
  ```

>[!NOTE]
>
>  Si vous ajoutez un type d’objet devant un nom de champ, il fait référence à l’objet parent de l’objet. Vous ne pouvez donc pas utiliser `{project}.{name}` avec un projet, mais vous pouvez l’utiliser avec une tâche.


Pour plus d’informations sur les variables telles que `$$OBJCODE`, voir [Vue d’ensemble des variables de filtre de caractères génériques](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### Attention à la suppression d’un type d’objet d’un formulaire personnalisé

Vous pouvez à tout moment supprimer un type d’objet sur un formulaire personnalisé, mais cela doit être effectué avec précaution. Si les personnes ont déjà joint le formulaire personnalisé à des objets du type que vous souhaitez supprimer et y ont ajouté des données, ces données sont définitivement supprimées lorsque vous supprimez ce type d’objet sur le formulaire.

En outre, il n’existe aucun système de notification pour avertir les personnes qui utilisent le formulaire personnalisé qu’il a été supprimé.

Pour plus d’informations, voir [Supprimer un champ ou un widget personnalisé du système](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
