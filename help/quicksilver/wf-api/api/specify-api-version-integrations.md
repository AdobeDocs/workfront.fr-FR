---
content-type: api
navigation-topic: api-navigation-topic
title: Spécification d’une version d’API dans vos intégrations
description: Spécification d’une version d’API dans vos intégrations
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Spécification d’une version d’API dans vos intégrations

Tous les URI Adobe Workfront sont nécessaires pour référencer une version spécifique de l’API après la partie &quot;tâche/api&quot; de l’URI. L’exemple suivant appelle la version 7.0 :
`attask/api/v7.0/<objectName>/<objectId>` Vérifiez que toutes vos intégrations appellent les API Workfront actuellement prises en charge.

## Calendrier des versions et des obsolescences des API Workfront

Les nouvelles versions de l’API sont publiées tous les six à huit mois. Chaque version est prise en charge pendant trois ans après sa date de publication, avec une année supplémentaire dans un état obsolète où la version est disponible mais pas prise en charge.

Pour plus d’informations sur la cadence de publication et le planning d’obsolescence des API Workfront, voir [Contrôle de version des API et planification de la prise en charge](../../wf-api/api/api-version-support-schedule.md).

Workfront a rendu obsolète la version par défaut de l’API à compter de juillet 2017. Cela signifie que Workfront ne désigne plus une version spécifique de l’API comme version par défaut. Tous les futurs URI d’API doivent spécifier une version de l’API pour être valides.

>[!IMPORTANT]
>
> Toutes les intégrations utilisant la version d’API par défaut doivent être mises à jour afin d’appeler une version d’API prise en charge spécifique d’ici le 1er juillet 2018.

## Détermination de la version d’API que vous utilisez

Vous pouvez déterminer la version de l’API que vous utilisez en vérifiant l’URI d’une requête HTTP envoyée à l’API Workfront. L’exemple suivant illustre un URI de demande Workfront qui spécifie la version 7 de l’API :

`https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Si un URI ne spécifie pas de version, il utilise la version par défaut de l’API, comme illustré dans l’exemple suivant :

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Les intégrations qui ne spécifient pas de version de l’API dans l’URI sont automatiquement acheminées vers la version par défaut de l’API et ne fonctionneront pas après le 1er juillet 2018.

## Mise à jour des intégrations pour utiliser les versions d’API prises en charge

Lorsque vous créez ou gérez des intégrations Workfront, vous devez inclure une méthode pour mettre à jour dynamiquement la version de l’API et d’autres propriétés susceptibles d’être modifiées (telles que votre clé d’API).

Pour rendre la mise à jour des intégrations plus efficace, tenez compte des suggestions suivantes pour enregistrer les valeurs d’intégration :

* Stocker les valeurs sujettes à de futures modifications dans un fichier de propriétés que vous conservez à jour
* Créer un service Web pour gérer les propriétés en temps réel
* Stocker les valeurs de propriété dans un entrepôt de données que votre application peut lire

La conception de vos intégrations Workfront à cet effet permet d’éviter un travail de développement intensif lorsque ces valeurs changent inévitablement.
