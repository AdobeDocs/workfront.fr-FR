---
title: Présentation du type d’enregistrement de l’espace de travail croisé
description: Vous pouvez activer les types d’enregistrements pour qu’ils soient globaux ou connectables. Les types d'enregistrements globaux peuvent être ajoutés à plusieurs espaces de travail à partir d'un espace de travail principal ou central dans Adobe Workfront Planning, tandis que les types d'enregistrements connectables peuvent être connectés à partir d'autres espaces de travail que le leur.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: 895fcc9e8bfc6ef21e82ae6dab4c370b0e267cad
workflow-type: tm+mt
source-wordcount: '1663'
ht-degree: 3%

---


# Présentation du type d’enregistrement de l’espace de travail croisé

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, consultez la section [Activer ou désactiver les versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Vous pouvez activer les fonctionnalités inter-espaces de travail pour un type d’enregistrement dans Adobe Workfront Planning. Un type d’enregistrement entre espaces de travail peut être référencé ou accessible à partir de plusieurs espaces de travail.

>[!IMPORTANT]
>
>Votre entreprise doit acheter les packages suivants pour pouvoir activer les fonctionnalités inter-espaces de travail pour les types d’enregistrements :
>
>Pour configurer les types d’enregistrements connectables :
>
>
>* Tout package Workfront et tout package Planning
>
>   Ou
>
>* Tout workflow et un package Planning Prime ou Ultimate
>
><span class="preview">Pour configurer les types d’enregistrements globaux :</span>
>
>* <span class="preview">Tout package Workfront et un package Planning Plus</span>
>     
>   Ou
>
>* <span class="preview">Tout workflow et un package Prime ou Ultimate Planning</span>
>
>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront.
>Pour plus d’informations, consultez [Présentation de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).


Vous trouverez ci-dessous des fonctionnalités inter-espaces de travail de types d’enregistrements :

* <span class="preview">**Types d’enregistrements globaux** : les utilisateurs peuvent ajouter des types d’enregistrements globaux à d’autres espaces de travail qu’ils gèrent.</span>

* **Types d’enregistrement connectables** : les utilisateurs peuvent se connecter à ce type d’enregistrement à partir d’autres espaces de travail.

Cet article vous donne un aperçu des types d’enregistrements de l’ensemble des espaces de travail. Pour plus d’informations sur la définition des fonctionnalités inter-espaces de travail d’un type d’enregistrement, voir [Configuration des fonctionnalités inter-espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

<div class="preview">

## Présentation des types d’enregistrements globaux

Les types d’enregistrements globaux peuvent être ajoutés à plusieurs espaces de travail à partir d’un espace de travail principal ou central dans Workfront Planning.

Lors de l’implémentation de Workfront Planning pour une organisation multi-équipes avec des workflows communs, vous devrez peut-être définir une structure et des métadonnées cohérentes pour les types d’enregistrements clés (tels que les campagnes ou les éléments livrables) qui peuvent être ajoutés aux espaces de travail de chaque équipe pour capturer et gérer leur travail.

Vous pouvez également avoir besoin du travail de chaque équipe pour atteindre un niveau central.

Dans un tel workflow, vous pouvez vous assurer que les équipes capturent leur travail de manière cohérente tout en déverrouillant la visibilité entre les équipes, sans avoir à tout ajouter à un espace de travail ou à tous les membres de l’organisation à chaque espace de travail. Pour ce faire, vous pouvez utiliser des types d’enregistrements globaux.

Pour utiliser des types d’enregistrements globaux, procédez comme suit :

1. Dans un espace de travail que vous gérez, configurez un type d’enregistrement comme étant global.

   Un gestionnaire d’espace de travail peut accorder des autorisations aux utilisateurs disposant d’une licence Standard, ou aux équipes, groupes, rôles et sociétés pour ajouter un type d’enregistrement choisi aux espaces de travail qu’ils gèrent.

   Le type d’enregistrement d’origine existera dans son espace de travail d’origine, mais sera rendu visible dans d’autres espaces de travail.

   Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Ajoutez un type d’enregistrement à un espace de travail secondaire à partir d’un espace existant qui a été configuré en tant que type d’enregistrement global.

   Le type d’enregistrement existe dans les espaces de travail suivants :

   * Son espace de travail d’origine où il a été désigné comme type d’enregistrement global.
   * Un espace de travail secondaire.

   Pour plus d’informations, voir [Ajouter des types d’enregistrements existants depuis un autre espace de travail](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   Les sections suivantes décrivent les points à prendre en compte concernant les types d’enregistrements globaux et leur fonctionnement dans leurs espaces de travail d’origine ou secondaires.

### Considérations sur les types d’enregistrements globaux dans leur espace de travail d’origine

Le type d’enregistrement configuré pour être global possède les propriétés suivantes :

* Toutes ses informations (aspect, champs d’origine) ne peuvent être modifiées que dans l’espace de travail d’origine.

* Vous pouvez effectuer les actions suivantes sur le type d’enregistrement global à partir de son espace de travail d’origine :

   * Le modifier.

     La modification d’un type d’enregistrement global inclut la modification de son apparence, des fonctionnalités de plusieurs espaces de travail et de tous les champs créés dans l’espace de travail d’origine.
   * Partager

     Le partage d’un type d’enregistrement ajoute des utilisateurs à l’espace de travail et partage également les enregistrements avec ces utilisateurs.
   * Le supprimer.

     Vous ne pouvez supprimer un type d’enregistrement global de son espace de travail d’origine qu’après avoir supprimé toutes les instances de s’il dans tous les espaces de travail secondaires où il a été ajouté.

     Pour plus d’informations, consultez la section [Supprimer des types d’enregistrement](/help/quicksilver/planning/architecture/delete-record-types.md).
   * Rendre connectable depuis d’autres espaces de travail
   * Créer et gérer des formulaires de demande
   * Création et gestion des automatisations

* Les enregistrements que vous ajoutez à un type d&#39;enregistrement global ne sont visibles que par les utilisateurs qui disposent des autorisations d&#39;affichage sur l&#39;espace de travail dans lequel ils ont été ajoutés. <!-- this needs to be more specific: what does "o the workspace where they were added" mean? - added in which kind of workspaces? secondary or primary; asking Lilit-->
* Les enregistrements que vous ajoutez à partir d’un espace de travail secondaire sont cumulés et affichés dans l’espace de travail d’origine. Tous les membres de l’espace de travail d’origine obtiennent des autorisations d’affichage.
* Lorsque le type d’enregistrement global d’origine est ajouté à plusieurs espaces de travail secondaires, les scénarios suivants existent :

   * Les membres de l’espace de travail d’origine obtiennent automatiquement des autorisations d’affichage pour tous les enregistrements ajoutés depuis n’importe quel espace de travail, même s’ils ne sont pas membres de ces espaces de travail.
   * Les membres Secondaire de l&#39;espace de travail ne peuvent afficher que les enregistrements des espaces de travail dont ils sont membres. <!--change this to: Secondary workspace members can view only records from the workspace the records were added and where they have at least permissions to view the record workspace and the record type.-->

* Les types d’enregistrement connectés à un type d’enregistrement global seront disponibles pour la connexion à partir des espaces de travail où ce type d’enregistrement est ajouté.

  Par exemple, si vous disposez d’un type d’enregistrement global Campaign ayant une connexion avec un type d’enregistrement Régions et que vous ajoutez le type d’enregistrement Campaign à un espace de travail secondaire, les régions pourront être connectées entre espaces de travail à partir de l’espace de travail secondaire. Les membres secondaires de l’espace de travail peuvent désormais créer des campagnes et les lier à des régions.

* Les champs créés pour un type d’enregistrement global à partir de l’espace de travail d’origine sont visibles de tous les espaces de travail où le type d’enregistrement est ajouté.

  Vous ne pouvez modifier les paramètres de champ qu’à partir de l’espace de travail d’origine.

  Les paramètres des champs créés dans l’espace de travail d’origine sont en lecture seule dans les espaces de travail secondaires pour tous les membres, quelles que soient leurs autorisations sur l’espace de travail secondaire.

  Les gestionnaires d’espace de travail Secondaire ne peuvent pas modifier les paramètres des champs configurés dans l’espace de travail d’origine. Seuls les gestionnaires d’espace de travail de l’espace de travail d’origine peuvent modifier les paramètres de champ dans l’espace de travail d’origine.

### Considérations relatives aux types d’enregistrements globaux dans un espace de travail secondaire

* Les contributeurs Secondaire à l’espace de travail obtiennent l’autorisation Contribuer au type d’enregistrement global dans l’espace de travail de leur équipe. Ils peuvent y ajouter et y gérer des enregistrements à partir de l’espace de travail secondaire.

* Les observateurs de l’espace de travail Secondaire obtiennent l’autorisation d’affichage du type d’enregistrement global dans l’espace de travail de leur équipe. Ils ne peuvent pas y ajouter ni y gérer des enregistrements.

* Les gestionnaires d’espace de travail Secondaire peuvent effectuer les actions supplémentaires suivantes sur le type d’enregistrement ajouté à partir d’un type d’enregistrement global dans un espace de travail secondaire :

   * Supprimez-le.

     La suppression du type d’enregistrement d’un espace de travail secondaire le supprime uniquement de l’espace de travail secondaire. Les enregistrements et les champs qui lui ont été ajoutés à partir de l’espace de travail secondaire sont également supprimés. Le type d’enregistrement n’est pas supprimé de son espace de travail d’origine ni de tout autre espace de travail secondaire où il a été ajouté.

     Pour plus d’informations, consultez la section [Supprimer des types d’enregistrement](/help/quicksilver/planning/architecture/delete-record-types.md).
   * Partagez les vues des types d’enregistrements.

     Vous ne pouvez pas partager une vue publiquement à partir d’un type d’enregistrement global dans un espace de travail secondaire. Vous pouvez uniquement partager des vues en interne à partir d’un espace de travail secondaire. Vous pouvez partager une vue en interne et publiquement pour un type d’enregistrement global dans son espace de travail d’origine.

     Pour plus d’informations, voir [Partager des vues](/help/quicksilver/planning/access/share-views.md).

<!--Uncomment this at prod on Jan 15: * Share it-->

<!--You can share a global record type added to a secondary workspace from the secondary space. By sharing a global record type in a secondary workspace, the following also occur:

    * Users are added to the workspace with View permissions.
    * Users receive the same permissions to all the records of the global record type in the secondary workspace.-->

<!--when they will be able to add fields to the secondary space, this bullet will need this extra information: 
    After adding fields to the global record type in the secondary workspace, shared views might not open for other users in workspaces. The fields exist only in the secondary workspace and they would not be visible in any other workspace. Only fields created in the primary workspace are visible in all secondary workspaces where there the record type is added.-->

<!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
* Add new fields
    Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
* Add request forms to it
* Add automations to it-->

* Aucun utilisateur ne peut effectuer les actions suivantes sur un type d’enregistrement global dans un espace de travail secondaire :

   * Le modifier.

     Vous ne pouvez pas modifier son apparence, les fonctionnalités de l’espace de travail croisé ou les champs ajoutés à partir de l’espace de travail d’origine.
   * Partager <!-- remove this at Prod on Jan 15-->
   * Créer et gérer des formulaires de demande
   * Création et gestion des automatisations

* Les enregistrements ajoutés dans un espace de travail secondaire sont visibles à partir des espaces de travail suivants uniquement si vous disposez d&#39;autorisations d&#39;affichage ou supérieures pour ces espaces de travail :

   * Espace de travail secondaire dans lequel ils sont ajoutés.
   * Espace de travail d’origine du type d’enregistrement global.
   * Tous les autres espaces de travail auxquels l’espace de travail global est ajouté.

  <!--replace he above bullet with this: 
        * Records added in a secondary workspace are visible from the following workspaces, only if you have View or higher permissions to these workspaces:
        * The secondary place where they were added
        * The global record type's original workspace
    -->

* Les scénarios suivants existent pour les enregistrements créés dans les espaces de travail secondaires :

   * Si vous disposez d’autorisations de niveau Gérer sur l’espace de travail d’origine et d’aucune autorisation sur un espace de travail secondaire, vous pouvez afficher les enregistrements ajoutés à partir des espaces de travail secondaires dans l’espace de travail d’origine, mais vous ne pouvez pas les gérer à partir de l’espace de travail d’origine.
   * Si vous disposez des autorisations de niveau Gérer sur l’espace de travail secondaire, vous pouvez gérer les enregistrements à partir de l’espace de travail d’origine du type d’enregistrement global et de l’espace de travail secondaire où ils ont été ajoutés.
   * Vous pouvez afficher les enregistrements dans d&#39;autres espaces de travail secondaires auxquels le type d&#39;enregistrement global est ajouté uniquement si vous disposez des autorisations d&#39;affichage sur ces espaces de travail. <!-- take this bullet out when we change this functionality on Jan 15-->

### Accès aux connexions d’un type d’enregistrement global

Les types d’enregistrement connectés au type d’enregistrement global dans l’espace de travail d’origine deviennent visibles à partir d’autres espaces de travail où le type d’enregistrement global est ajouté et ils sont disponibles pour les connexions à partir des espaces de travail secondaires où le type d’enregistrement global est ajouté.

### Accès API d’un type d’enregistrement global

Lors de l’ajout d’enregistrements à un type d’enregistrement global à partir d’un espace de travail secondaire à l’aide de l’API Workfront Planning, le système vérifie si l’utilisateur a accès à la création d’enregistrements dans l’espace de travail d’origine du type d’enregistrement global.

Les cas suivants existent :

* Si l’utilisateur y a accès, l’enregistrement est créé dans l’espace de travail d’origine des types d’enregistrements globaux.

* Si l’utilisateur n’y a pas accès, il est prévenu qu’il n’a pas accès à l’espace de travail d’origine du type d’enregistrement global et doit fournir l’identifiant de l’espace de travail auquel il a accès pour créer des enregistrements.

</div>

## Présentation des types d’enregistrements connectables

Vous pouvez vous connecter à un type d’enregistrement défini comme pouvant être connecté à partir de n’importe quel espace de travail que vous gérez.

Vos équipes peuvent avoir besoin que leurs enregistrements soient liés à des types d&#39;enregistrements d&#39;autres espaces de travail ou afficher des informations capturées sur des enregistrements appartenant à des enregistrements d&#39;autres espaces de travail. Vous pouvez effectuer cette configuration en désignant un type d’enregistrement comme connectable.

Pour utiliser des types d’enregistrements connectables, procédez comme suit :

1. Configurez un type d’enregistrement à connecter dans un espace de travail spécifique.

   Un gestionnaire d’espace de travail peut sélectionner les espaces de travail auxquels un type d’enregistrement désigné peut se connecter.

   Le type d’enregistrement d’origine existe dans son espace de travail d’origine et il peut être accessible pour se connecter à partir d’un autre espace de travail.

   Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Connectez-vous à un type d’enregistrement désigné comme connectable à partir d’un autre espace de travail que vous gérez.

   Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).
