---
content-type: api
navigation-topic: api-navigation-topic
title: Spécifier une version de l’API dans vos intégrations
description: Spécifier une version de l’API dans vos intégrations
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 100%

---

# Spécifier une version de l’API dans vos intégrations

Tous les URI Adobe Workfront doivent référencer une version spécifique de l’API après la partie « attask/api » de l’URI. L’exemple suivant appelle la version 15.0 :

`attask/api/v15.0/<objectName>/<objectId>`

Vérifiez que toutes vos intégrations appellent les API Workfront actuellement prises en charge.

## Calendrier des versions et des obsolescences des API Workfront

Les nouvelles versions de l’API sont publiées régulièrement, généralement deux fois par an. Chaque version est prise en charge pendant trois ans après sa date de publication, avec une année supplémentaire dans un état obsolète où la version est disponible mais non prise en charge.

Pour plus d’informations sur la cadence de publication et le planning d’obsolescence des API Workfront, voir [Calendrier des versions de l’API et de la prise en charge](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* La version par défaut de l’API est définie sur la version la plus récente. Tout appel API sans la version spécifiée utilise la version par défaut. Chaque fois que Workfront publie une nouvelle version de l’API, la version par défaut est mise à jour vers la dernière version. **Par conséquent, après la publication d’une nouvelle version de l’API Workfront, tous les appels API qui utilisent la version par défaut doivent être vérifiés pour s’assurer que la fonctionnalité est toujours prise en charge.**
>
>* Si votre organisation utilise actuellement l’API par défaut, votre administrateur ou administratrice Workfront a reçu un message du centre d’annonces contenant des instructions supplémentaires sur l’API par défaut.
>
>Pour consulter la version la plus récente de l’API, voir [Calendrier des versions de l’API et de la prise en charge](../../wf-api/api/api-version-support-schedule.md).


## Déterminer la version de l’API que vous utilisez

Vous pouvez déterminer la version de l’API que vous utilisez en vérifiant l’URI d’une demande HTTP envoyée à l’API Workfront. L’exemple suivant illustre un URI de demande Workfront qui indique la version 15 de l’API :

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Si un URI ne spécifie pas de version, il utilise la version par défaut de l’API, comme illustré dans l’exemple suivant :

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Les intégrations qui ne spécifient pas de version de l’API dans l’URI sont automatiquement acheminées vers la version par défaut de l’API.

## Mise à jour des intégrations pour utiliser les versions d’API prises en charge

Lorsque vous créez ou gérez des intégrations Workfront, vous devez inclure une méthode pour mettre à jour dynamiquement la version de l’API et d’autres propriétés susceptibles d’être modifiées (telles que votre clé API).

Pour rendre la mise à jour des intégrations plus efficace, tenez compte des suggestions suivantes pour enregistrer les valeurs d’intégration :

* Stockez les valeurs susceptibles d’être modifiées à l’avenir dans un fichier de propriétés que vous maintenez à jour.
* Créez un service web pour gérer les propriétés en temps réel.
* Stockez les valeurs de propriété dans un magasin de données que votre application peut lire.

La conception de vos intégrations Workfront à cet effet permet d’éviter un travail de développement intensif lorsque ces valeurs changent inévitablement.
