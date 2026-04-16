---
title: Présentation des profils métier
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: add-users-to-workfront
description: Les profils métier constituent un modèle d’autorisation amélioré qui permet aux clients, tels que les agences, de gérer efficacement l’accès des utilisateurs et d’assurer un contrôle précis des autorisations au niveau du groupe. Dans un profil d’entreprise, les utilisateurs disposent d’autorisations distinctes pour les objets spécifiques à un groupe. D’autres objets peuvent également être partagés directement avec le profil d’entreprise.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7f62de33-e544-4be9-8dcf-03a2e09e8a05
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b190de6b6ef9ce53e96475d426a4d39cfbd4df4
workflow-type: tm+mt
source-wordcount: '1443'
ht-degree: 1%

---

# Présentation des profils professionnels

Les profils métier constituent un modèle d’autorisation amélioré qui permet aux clients, tels que les agences, de gérer efficacement l’accès des utilisateurs et d’assurer un contrôle précis des autorisations au niveau du groupe. Dans un profil d’entreprise, les utilisateurs disposent d’autorisations distinctes pour les objets spécifiques à un groupe. D’autres objets peuvent également être partagés directement avec le profil d’entreprise.

Un profil professionnel pour un utilisateur est similaire à un utilisateur ayant un rôle spécifique dans un groupe, tel qu’un contrôleur financier ou un chef de projet, et recevant les autorisations associées à ce rôle pour le groupe spécifié. Le profil d’entreprise peut être temporaire, ce qui permet d’accorder des autorisations pour une période qui va expirer et de maintenir des restrictions sur les données pour le groupe ou l’agence.

L’administrateur système de Workfront :

* Crée les niveaux d&#39;accès et définit les champs restreints selon les besoins
* Met à jour le profil utilisateur avec le groupe et le niveau d’accès pour ce groupe (il s’agit du profil professionnel)
* Définit des dates d’entrée en vigueur pour le profil professionnel, le cas échéant
* Attribue des modèles de mise en page aux niveaux d’accès

Tout utilisateur disposant de l’accès nécessaire pour partager des objets peut les partager avec le profil d’entreprise et tous les utilisateurs disposant du profil verront l’objet .

## Exemple de profil professionnel

>[!BEGINSHADEBOX]

Sam a besoin d&#39;un accès différent aux projets pour l&#39;Agence A et l&#39;Agence B. Les deux agences sont configurées en tant que groupes dans Workfront. (Pour plus d’informations sur les groupes, voir la présentation des groupes.)

Pour l’agence A, Sam agit en tant que contrôleur financier et doit avoir accès à tous les champs financiers de ses projets. Pour l&#39;Agence B, Sam agit en tant que chef de projet et doit gérer les tâches et les problèmes, mais ne devrait pas être en mesure d&#39;afficher les informations financières.

L’administrateur système de Workfront crée de nouveaux niveaux d’accès appelés Contrôleur financier et Gestionnaire de projets. Ces niveaux d’accès sont correctement accessibles pour les données financières. Ensuite, l’administrateur ouvre le profil utilisateur de Sam et sélectionne « Agence A » en tant que groupe avec le niveau d’accès « Contrôleur financier » pour créer le premier profil commercial, et « Agence B » en tant que groupe avec le niveau d’accès « Gestionnaire de projets » pour créer le second profil commercial.

Une fois les profils métier configurés, lorsque Sam accède à la liste des projets, tous les projets de l’Agence A et de l’Agence B s’affichent (ainsi que tous les autres projets que Sam a créés ou pour lesquels il a reçu des autorisations). Les champs financiers des projets de l&#39;Agence A sont visibles pour Sam dans la vue Liste et dans les détails du projet, mais les champs financiers des projets de l&#39;Agence B sont masqués. Les noms des champs s’affichent, mais les données des champs sont vides.

Si d’autres utilisateurs de l’une ou l’autre des agences partagent des projets avec les profils métier « Contrôleur financier - Agence A » ou « Gestionnaire de projets - Agence B », ces projets sont visibles pour Sam. Les champs financiers des projets de l&#39;Agence B resteront toujours masqués, car ils sont définis dans le niveau d&#39;accès.

>[!ENDSHADEBOX]

## Définition des profils métier

L’administrateur système Adobe Workfront est chargé de définir tous les domaines d’un profil d’entreprise.

### Créer un niveau d&#39;accès

L’administrateur système de Workfront crée le niveau d’accès avec l’accès nécessaire et définit les champs restreints selon les besoins.

Pour plus d’informations, consultez [Créer et modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Ajouter un profil professionnel à l’utilisateur

L’administrateur système Workfront ajoute le profil professionnel à un profil utilisateur en sélectionnant un groupe et un niveau d’accès. La combinaison des deux crée le profil d’entreprise. Chaque groupe ne peut être utilisé que dans un seul profil professionnel par utilisateur. <!--how does this combine with more than one access level per group. As far as I can see a business profile is one level and one group-->

Le profil d’entreprise peut avoir plusieurs niveaux d’accès par groupe. Le niveau disposant de l’accès le plus élevé est prioritaire.

L’administrateur peut attribuer des dates d’entrée en vigueur à un profil professionnel, de sorte que l’accès de l’utilisateur expirera à une date ultérieure. Les dates de début et de fin indiquent les dates auxquelles l’utilisateur commence et se termine en tenant le profil dans ce groupe. L’utilisation de dates d’effet pour mettre fin à l’accès au lieu de supprimer le profil permet au profil d’être activé à nouveau à l’avenir.

Plusieurs profils professionnels sont autorisés pour un utilisateur.

<!--image?-->

Pour plus d’informations, voir [Modifier le profil d’un utilisateur](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). <!--may be separate article now since it's not in the profile-->

### Attribuer des modèles de mise en page au niveau d’accès

L’administrateur système de Workfront peut éventuellement affecter un modèle de mise en page au niveau d’accès, afin de s’assurer que les utilisateurs et utilisatrices disposant du profil professionnel associé voient les informations et actions pertinentes en fonction de leur rôle dans le système.

Pour plus d’informations, voir [Affecter des utilisateurs et utilisatrices à un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

## Fonctionnement des profils métier

Lorsqu’un profil professionnel est ajouté à un utilisateur, les autorisations dans la combinaison du groupe et du niveau d’accès déterminent ce que l’utilisateur verra dans Workfront.

### Disposition Workfront

Lorsque le groupe du profil professionnel est associé à un projet, le modèle de mise en page pour le niveau d&#39;accès dans le profil professionnel est appliqué. Tous les utilisateurs disposant du profil professionnel verront les éléments de menu, la page d’accueil et d’autres éléments de disposition inclus dans le modèle. Le modèle de mise en page du profil professionnel est prioritaire sur un modèle de mise en page affecté à l&#39;utilisateur.

Si le profil professionnel comporte plusieurs niveaux d’accès avec le même groupe, les modèles de mise en page des deux niveaux d’accès sont combinés. Tous les éléments de disposition disponibles s’affichent. Si un élément de menu est affiché dans un modèle, mais masqué dans un autre, il s’affiche. Seuls les éléments masqués dans tous les modèles du profil professionnel sont masqués.

Dans les cas où les mêmes éléments sont affichés dans plusieurs modèles de mise en page, mais que l’ordre des éléments est différent (comme dans le volet de navigation de gauche ou les épingles), l’ordre à partir du modèle du niveau d’accès répertorié en premier dans le profil professionnel est utilisé.

### Projets et autres objets partagés

Lorsqu’un projet est associé à un groupe, un utilisateur disposant d’un profil professionnel pour ce groupe peut afficher le projet. La visibilité des champs dans le projet est basée sur le niveau d’accès dans le profil métier. Si plusieurs niveaux d’accès sont affectés au groupe dans le profil professionnel de l’utilisateur, le niveau avec les autorisations les plus élevées s’applique.

Par exemple, un utilisateur possède deux profils métier : le premier fournit un accès de contrôleur financier à un groupe (pour afficher les champs finances) et le second fournit un accès de gestionnaire de projet sous un autre groupe (où les champs finances ne doivent pas être affichés).

L’utilisateur verrait les projets des deux groupes dans la liste de tous les projets. Dans la vue Liste et dans les détails du projet, l’utilisateur ne voit les données financières que pour le premier groupe. Les champs financiers des projets du deuxième groupe seraient vides.

Tout utilisateur autorisé à partager des objets peut partager ces objets avec un profil d’entreprise. Tous les utilisateurs affectés au profil disposeront des autorisations spécifiées pour l’objet . Cependant, si l&#39;accès est limité dans le niveau d&#39;accès affecté par l&#39;administrateur dans le profil d&#39;entreprise, le niveau d&#39;accès prévaut sur les autorisations accordées dans le partage. Par exemple, si le niveau d’accès ne permet pas de créer des tâches, l’utilisateur ne peut pas ajouter de tâches à un projet, même s’il dispose d’autorisations de niveau Gérer pour un projet lorsqu’il est partagé avec le profil d’entreprise.

Si un profil professionnel est affecté à un utilisateur après qu’un objet a déjà été partagé avec le profil, l’utilisateur voit l’objet avec l’accès spécifié.

Lorsqu’un profil professionnel comporte plusieurs niveaux d’accès, le niveau avec le plus grand nombre d’accès est prioritaire.

Pour plus d’informations sur le partage, voir [Partager un objet](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Pour plus d&#39;informations sur la façon dont les niveaux d&#39;accès et les autorisations fonctionnent ensemble, voir [Présentation des niveaux d&#39;accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

## Considérations relatives aux profils professionnels

* Il n’est pas nécessaire d’être membre d’un groupe pour qu’un profil professionnel lui soit affecté.
* Le niveau d’accès au profil professionnel ne peut mettre à niveau que le niveau d’accès de « base » d’un utilisateur. Le profil d’entreprise ne peut pas retirer les autorisations de niveau d’accès de base.
* Dans les listes d’objets et les rapports, l’utilisateur dispose de toutes les autorisations disponibles à partir de tous les profils professionnels qui lui sont attribués dans les groupes fusionnés avec son niveau d’accès de base. Dans d’autres pages, l’utilisateur dispose des autorisations de niveau d’accès de base.
* Lorsqu’un groupe est supprimé de Workfront, tous les profils professionnels attribués à ce groupe sont supprimés des utilisateurs associés.
* Si un niveau d’accès fait partie d’un profil professionnel et que vous supprimez le niveau d’accès, vous êtes invité à choisir un nouveau niveau d’accès à utiliser à la place.
* Les mises à jour des profils métier sont suivies dans les journaux d’audit Workfront. Pour plus d’informations, voir Présentation des journaux d’audit.
