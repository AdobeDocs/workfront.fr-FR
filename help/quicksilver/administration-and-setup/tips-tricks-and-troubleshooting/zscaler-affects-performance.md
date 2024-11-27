---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Les paramètres de ZScaler peuvent réduire les performances
description: Après la création de l’utilisateur ou de l’utilisatrice, vous pouvez modifier l’utilisateur ou l’utilisatrice et activer l’option « Autoriser uniquement l’authentification SAML 2.0 » afin que son utilisateur ou utilisatrice et son mot de passe soient contrôlés par le système SAML. Lorsque cette option est activée, l’utilisateur n’est autorisé à se connecter que par SAML.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
source-git-commit: f66b219e9fd203f108844ad397bcfa848b8f1134
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 25%

---

# Workfront : les paramètres de ZScaler peuvent réduire les performances

>[!NOTE]
>
>Il s’agit d’un problème avec ZScaler, qui ne sera pas résolu par Workfront.

Le service Web de ZScaler utilise `http/1.1` par défaut, ce qui peut entraîner des performances réduites dans Workfront.

Pour vérifier et résoudre ce problème, configurez votre logiciel ZScaler pour utiliser `http/2`. Cette configuration ne peut pas être effectuée dans Workfront.

Vous trouverez des informations sur `http/2` dans la documentation de ZScaler.
