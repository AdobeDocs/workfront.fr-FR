---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Les dossiers liés ne sont pas pris en charge pour l’objet DOCU
description: Les dossiers liés ne sont pas pris en charge pour l’objet DOCU
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 9%

---

# L’utilisation de l’API pour ajouter un dossier lié n’est pas prise en charge.

L’utilisation de l’API pour ajouter un dossier lié au tableau de dossiers pour un objet Document (DOCU) n’est pas prise en charge. La requête aboutira, mais le document peut être supprimé du système par certains fournisseurs externes. C&#39;est parce que le système externe sera utilisé comme la source finale de vérité. Par conséquent, si le document est supprimé du fournisseur externe, le document est considéré comme n’existant plus. Tous les documents introuvables dans le dossier lié (externe) peuvent être supprimés automatiquement de [!DNL Workfront] sans possibilité de les récupérer.
