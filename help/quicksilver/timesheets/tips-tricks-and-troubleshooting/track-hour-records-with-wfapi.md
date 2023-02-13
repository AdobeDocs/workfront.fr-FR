---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Suivi des enregistrements d’heure avec l’API Adobe Workfront
description: Si votre entreprise utilise Adobe Workfront pour saisir les heures travaillées, mais utilise un autre outil comme système d’enregistrement pour ces données, vous pouvez utiliser l’API Workfront pour synchroniser les données entre les deux systèmes.
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Suivi des enregistrements d’heure avec l’API Adobe Workfront

Si votre entreprise utilise Adobe Workfront pour saisir les heures travaillées, mais utilise un autre outil comme système d’enregistrement pour ces données, vous pouvez utiliser l’API Workfront pour synchroniser les données entre les deux systèmes.

Le simple suivi de l’enregistrement d’heure n’est pas possible, car si l’entrée d’heure est supprimée, l’enregistrement entier est supprimé, ce qui nécessite d’extraire le jeu de données entier et de le comparer à l’ancien jeu de données. Heureusement, toutes les transactions d’heure sont enregistrées dans les entrées du journal Workfront.

Après avoir récupéré un jeu initial de toutes les heures actuelles dans le système, vous pouvez effectuer le suivi de toutes les modifications via les entrées de journal.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID" : "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2" : "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HEURE",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID" : "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2" : "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "HEURE",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID" : "5785416f008db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2" : "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HEURE",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID" : "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2" : "Brad Littler",<br>"newNumberVal": 2,<br>"oldNumberVal": 1,<br>"subObjCode": "HEURE",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>Voici une description des champs inclus :

* **changeType :** Type de modification apportée à l’objet :

   * **A :** Ajouter

   * **E :** Modifier

   * **D :** Supprimer

* **aux2 :** Nom de l’utilisateur pour lequel l’enregistrement d’heure est destiné.

* **newNumberVal :** Nouvelle valeur de l’enregistrement d’heure (cette valeur est nulle si le changementType a la valeur D).

* **oldNumberVal :** Valeur précédente de l’enregistrement d’heure.

* **subObjCode :** Type d’enregistrement modifié (Doit toujours être HEURE).

* **subObjID :** Identifiant de l’enregistrement de l’heure.

Vous pouvez utiliser ces informations pour découvrir les enregistrements d’heure modifiés, modifiés ou supprimés. Vous pouvez ensuite utiliser subObjID pour récupérer plus d’informations à partir des enregistrements d’heure, si nécessaire.
