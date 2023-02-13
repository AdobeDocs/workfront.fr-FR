---
content-type: reference
navigation-topic: announcements
title: Nouveau système géré Adobe Workfront pour remplacer les courriers électroniques POP des files d’attente de requête par la version 21.1
description: Nous remplaçons l’option de messagerie POP pour les files d’attente de demandes par un nouveau système géré par Adobe Workfront. Vous pourrez toujours envoyer des demandes par courrier électronique, mais vous devrez configurer une nouvelle adresse électronique gérée par Workfront dans la zone File d’attente des demandes à la place.
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Nouveau système géré Adobe Workfront pour remplacer les courriers électroniques POP des files d’attente de requête par la version 21.1

Nous remplaçons l’option de messagerie POP pour les files d’attente de demandes par un nouveau système géré par Adobe Workfront. Vous pourrez toujours envoyer des demandes par courrier électronique, mais vous devrez configurer une nouvelle adresse électronique gérée par Workfront dans la zone File d’attente des demandes à la place.

## Pourquoi supprimez-vous l’option de courrier électronique POP ?

La technologie POP est une option d&#39;email peu fiable et moins sécurisée. De plus, nous voyons de nombreux problèmes liés aux clients, spécifiquement aux emails POP. Apporter une modification à un système géré Workfront permet d’obtenir une expérience plus fiable.

## Quelle action dois-je entreprendre ?

Vous devez configurer une nouvelle adresse électronique pour chaque file d’attente de demandes configurée avec des courriers électroniques POP dans votre environnement de production et distribuer la nouvelle adresse électronique selon vos besoins. Pour plus d’informations, voir [Autorisation des utilisateurs à envoyer par courrier électronique un problème dans un projet de file d’attente des demandes](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Quel est le plan de transition ?

À compter de la version 21.1 au début du mois de février, vous aurez 60 jours pour faire passer vos utilisateurs vers la nouvelle *@intake.workfront.com* adresse électronique que vous créez. Pendant la période de 60 jours, l&#39;email POP utilisé précédemment continuera à fonctionner.

## Comment puis-je le tester dans Aperçu ?

Pour tester cette modification dans la prévisualisation, vous devez activer les emails dans votre environnement Aperçu . Pour ce faire, suivez les instructions de la section Gestion des emails dans l’aperçu de la section [Activation de la diffusion des emails à partir de l’environnement Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>Ce que vous définissez ici ne sera pas transféré vers votre environnement de production. Vous devrez recommencer cette procédure une fois la fonctionnalité mise en production.
