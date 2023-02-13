---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Les dossiers liés ne sont pas pris en charge pour l’objet DOCU
description: Les dossiers liés ne sont pas pris en charge pour l’objet DOCU
author: Becky
feature: Workfront API
source-git-commit: 9bdc433158e471729bd27d701947d6ae41aa06e7
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---


# L’utilisation de l’API pour ajouter un dossier lié n’est pas prise en charge

L’utilisation de l’API pour ajouter un dossier lié au tableau de dossiers pour un objet Document (DOCU) n’est pas prise en charge. La requête aboutira, mais le document peut être supprimé du système par certains fournisseurs externes. C&#39;est parce que le système externe sera utilisé comme la source finale de vérité. Par conséquent, si le document est supprimé du fournisseur externe, le document est considéré comme n’existant plus. Les documents qui ne figurent pas dans le dossier lié (externe) peuvent être supprimés automatiquement de [!DNL Workfront] sans moyen de les récupérer.
