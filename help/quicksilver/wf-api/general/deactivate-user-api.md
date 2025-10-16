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
source-git-commit: f9a154fa92217810b762ac48169512bc0bca7305
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 80%

---


# Désactiver un utilisateur ou une utilisatrice via l’API

Lorsqu’un utilisateur ou une utilisatrice quitte votre entreprise, vous pouvez désactiver cette personne, rendre sa licence Adobe Workfront disponible pour un autre utilisateur ou une autre utilisatrice et empêcher qu’un travail lui soit affecté par inadvertance. En désactivant un utilisateur ou une utilisatrice, vous conservez son historique de travail, qui inclut ses affectations et son association aux notes, aux heures et aux documents.

Pour en savoir plus sur la désactivation d’un utilisateur ou d’une utilisatrice, voir [Désactiver ou réactiver un utilisateur ou une utilisatrice](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Pour plus d’informations sur l’utilisation de l’API Core, voir [Principes de base des API](../../wf-api/general/api-basics.md).

Pour désactiver un utilisateur ou une utilisatrice via l’API :

1. Générez une clé API à l’aide de la requête API suivante :

   ```
   <domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
   ```

1. Recherchez le GUID de l’utilisateur ou de l’utilisatrice que vous souhaitez désactiver.

   Utilisez la requête d’API suivante pour récupérer le GUID de tous les utilisateurs et utilisatrices de votre système. Notez que le champ **isActive** affiche **true** pour les utilisateurs et les utilisatrices actuellement actifs et **false** pour les utilisateurs et les utilisatrices qui ont été désactivés :

   ```
   <domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
   ```

1. Utilisez la requête **PUT** suivante pour modifier la valeur du champ **isActive** de l’utilisateur en **false** :

   ```
   <domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
   ```

1. La réponse indique que la valeur du champ **isActive** est passée de **true** à **false**, ce qui indique que l’utilisateur a été désactivé :

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
