---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Désactivation d’un utilisateur via l’API
description: Désactivation d’un utilisateur via l’API
author: Becky
feature: Workfront API
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Désactivation d’un utilisateur via l’API

Lorsqu’un utilisateur quitte votre entreprise, vous pouvez désactiver l’utilisateur, rendre sa licence Adobe Workfront disponible pour un autre utilisateur et l’empêcher de se voir attribuer par inadvertance un travail. En désactivant un utilisateur, vous conservez son historique de travail, notamment ses affectations et son association à des notes, heures et documents.

Pour en savoir plus sur la désactivation d’un utilisateur, voir &quot; [Désactivation ou réactivation d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Pour plus d’informations sur l’utilisation de l’API Core, voir [Principes de base des API](../../wf-api/general/api-basics.md).

Pour désactiver un utilisateur via l’API :

1. Générez une clé API à l’aide de la requête API suivante :

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. Recherchez le GUID de l’utilisateur que vous souhaitez désactiver.

   1. Utilisez la requête d’API suivante pour récupérer le GUID pour tous les utilisateurs de votre système. Notez que la variable **isActive** affichage des champs **true** pour les utilisateurs actuellement principaux et **false** pour les utilisateurs qui ont été désactivés :

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. Localisez le GUID de l’utilisateur que vous souhaitez désactiver. Utilisez les **PUT** demande de modification de la **isActive** valeur du champ à **false**:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. La réponse indique que la variable **isActive** la valeur du champ a changé de **true** to **false** indiquant que l’utilisateur a été désactivé :

<!-- [Copy](javascript:void(0);) -->
<pre></pre>
