---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Suivre les relevés d’heures avec l’API Adobe Workfront
description: Si votre organisation utilise Adobe Workfront pour saisir les heures travaillées, mais utilise un autre outil comme système d’enregistrement pour ces données, vous pouvez utiliser l’API Workfront pour synchroniser les données entre les deux systèmes.
author: Alina
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 100%

---

# Suivre les relevés d’heures avec l’API Adobe Workfront

Si votre organisation utilise Adobe Workfront pour saisir les heures travaillées, mais utilise un autre outil comme système d’enregistrement pour ces données, vous pouvez utiliser l’API Workfront pour synchroniser les données entre les deux systèmes.

Le simple suivi de l’enregistrement d’heure n’est pas possible, car si l’entrée d’heure est supprimée, l’enregistrement entier est supprimé, ce qui nécessite d’extraire le jeu de données entier et de le comparer à l’ancien jeu de données. Heureusement, toutes les transactions d’heure sont enregistrées dans les entrées du journal Workfront.

Après avoir récupéré un jeu initial de toutes les heures actuelles dans le système, vous pouvez effectuer le suivi de toutes les modifications par le biais des entrées de journal.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&amp;fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler",<br>"newNumberVal": 2,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>Voici une description des champs inclus :

* **changeType :** type de modification apportée à l’objet :

   * **A :** ajouter

   * **E :** modifier

   * **D :** supprimer

* **aux2 :** nom de la personne pour laquelle l’enregistrement d’heure est destiné.

* **newNumberVal :** nouvelle valeur de l’enregistrement d’heure (cette valeur est nulle si le changementType a la valeur D).

* **oldNumberVal :** valeur précédente de l’enregistrement d’heure.

* **subObjCode :** type d’enregistrement modifié (Doit toujours être HOUR).

* **subObjID :** identifiant de l’enregistrement de l’heure.

Vous pouvez utiliser ces informations pour découvrir quels enregistrements d’heure ont été modifiés, édités ou supprimés. Vous pouvez ensuite utiliser subObjID pour récupérer plus d’informations à partir des enregistrements d’heure, si nécessaire.
