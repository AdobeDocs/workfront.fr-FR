---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Suppression d’utilisateurs via Adobe Admin Console
description: Vous pouvez supprimer un utilisateur d’Adobe Workfront Fusion uniquement, en laissant l’accès à tout autre profil de produit Adobe, ou vous pouvez entièrement le supprimer de Adobe Admin Console.
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Supprimer des utilisateurs par l’intermédiaire de l’élément [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>La fonctionnalité de cet article n’est disponible que si l’instance de [!DNL Adobe Workfront Fusion] de votre organisation a été intégrée à [!DNL Adobe Business Platform].
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à [!DNL Adobe Business Platform], voir [Différences d’administration basées sur les plateformes ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

Vous pouvez supprimer un utilisateur de [!DNL Adobe Workfront Fusion] uniquement, en laissant l’accès à tout autre profil de produit [!DNL Adobe], ou vous pouvez supprimer entièrement l’utilisateur de [!DNL Adobe Admin Console].

## Suppression d’un utilisateur dans [!DNL Adobe Workfront Fusion]

Pour supprimer un utilisateur dans [!DNL Adobe Workfront Fusion], vous devez le désactiver par le biais de [!DNL Adobe Admin Console].

Un utilisateur est désactivé à partir de [!DNL Adobe Admin Console] lorsque l’une des conditions suivantes s’applique :

* L’utilisateur est déplacé d’un produit ou d’un profil de produit et n’est affecté à aucun autre produit ou profil de produit.
* L’utilisateur est supprimé d’un groupe lié à un profil de produit et n’est inclus dans aucun autre groupe lié à un profil de produit.
* L’utilisateur est supprimé d’un profil de produit et n’est affecté à aucun autre profil de produit.
* L’utilisateur est supprimé ou désactivé dans l’organisation qui inclut Workfront Fusion.

  Pour obtenir des instructions, reportez-vous à la section &quot;Suppression d’utilisateurs&quot; dans la section [Gestion des utilisateurs individuellement](https://helpx.adobe.com/fr/enterprise/using/manage-users-individually.html).

Dans [!DNL Workfront Fusion], la désactivation affecte l’utilisateur de l’une des façons suivantes :

* Si l’utilisateur se trouve dans une seule organisation, il est désactivé.
* Si l’utilisateur se trouve dans plusieurs organisations, il est supprimé de l’organisation dans laquelle il a été modifié sur le [!DNL Adobe Admin Console].
* Pour d’autres considérations à prendre en compte lors de la suppression d’un utilisateur dans [!DNL Workfront Fusion], voir [Considérations à prendre en compte lors de la suppression d’un utilisateur dans [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
