---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Désactiver un utilisateur ou une utilisatrice via l’API
description: Désactiver un utilisateur ou une utilisatrice via l’API
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 9%

---


# Désactiver un utilisateur ou une utilisatrice via l’API

Lorsqu’un utilisateur quitte votre entreprise, vous pouvez désactiver l’utilisateur, rendre sa licence Adobe Workfront disponible pour un autre utilisateur et l’empêcher de se voir attribuer par inadvertance un travail. En désactivant un utilisateur, vous conservez son historique de travail, notamment ses affectations et son association à des notes, heures et documents.

Pour en savoir plus sur la désactivation d’un utilisateur, voir &quot; [Désactivation ou réactivation d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Pour plus d’informations sur l’utilisation de l’API Core, voir [Principes de base de l’API](../../wf-api/general/api-basics.md).

Pour désactiver un utilisateur via l’API :

1. Générez une clé API à l’aide de la requête API suivante :

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. Recherchez le GUID de l’utilisateur que vous souhaitez désactiver.

   1. Utilisez la requête d’API suivante pour récupérer le GUID pour tous les utilisateurs de votre système. Notez que le champ **isActive** affiche **true** pour les utilisateurs actuellement actifs et **false** pour les utilisateurs qui ont été désactivés :

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. Recherchez le GUID de l’utilisateur que vous souhaitez désactiver, utilisez la requête **PUT** suivante pour remplacer la valeur du champ **isActive** de l’utilisateur par **false** :

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. La réponse indiquera que la valeur du champ **isActive** a été changée de **true** à **false** indiquant que l’utilisateur a été désactivé :

<!-- [Copy](javascript:void(0);) -->
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
