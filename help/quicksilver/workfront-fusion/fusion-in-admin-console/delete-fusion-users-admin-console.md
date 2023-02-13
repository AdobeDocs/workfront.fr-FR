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
hidefromtoc: true
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Suppression d’utilisateurs via le [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>La fonctionnalité de cet article n’est disponible que si l’instance de [!DNL Adobe Workfront Fusion] a été intégré au [!DNL Adobe Business Platform].
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à la variable [!DNL Adobe Business Platform], voir [Différences d’administration basées sur les plateformes ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

Vous pouvez supprimer un utilisateur de [!DNL Adobe Workfront Fusion] uniquement, en laissant l’accès à tout autre [!DNL Adobe] profils de produit, ou vous pouvez supprimer l’utilisateur de la variable [!DNL Adobe Admin Console] entièrement.

## Suppression d’un utilisateur dans [!DNL Adobe Workfront Fusion]

Pour supprimer un utilisateur dans [!DNL Adobe Workfront Fusion], vous devez désactiver l’utilisateur par l’intermédiaire de la fonction [!DNL Adobe Admin Console].

Un utilisateur est désactivé à partir de la fonction [!DNL Adobe Admin Console] lorsque l’une des conditions suivantes s’applique :

* L’utilisateur est déplacé d’un produit ou d’un profil de produit et n’est affecté à aucun autre produit ou profil de produit.
* L’utilisateur est supprimé d’un groupe lié à un profil de produit et n’est inclus dans aucun autre groupe lié à un profil de produit.
* L’utilisateur est supprimé d’un profil de produit et n’est affecté à aucun autre profil de produit.
* L’utilisateur est supprimé ou désactivé dans l’organisation qui inclut Workfront Fusion.

   Pour obtenir des instructions, reportez-vous à la section &quot;Suppression d’utilisateurs&quot; de la section [Gérer les utilisateurs individuellement](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

Dans [!DNL Workfront Fusion], la désactivation affecte l’utilisateur de l’une des manières suivantes :

* Si l’utilisateur se trouve dans une seule organisation, il est désactivé.
* Si l’utilisateur se trouve dans plusieurs organisations, il est supprimé de l’organisation dans laquelle il a été modifié dans la variable [!DNL Adobe Admin Console].
* Pour d’autres considérations lors de la suppression d’un utilisateur dans [!DNL Workfront Fusion], voir [Remarques concernant la suppression d’un utilisateur dans [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
