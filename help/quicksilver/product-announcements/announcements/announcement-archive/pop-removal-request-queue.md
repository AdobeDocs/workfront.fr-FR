---
content-type: reference
navigation-topic: announcements
title: Nouveau système Adobe Workfront pour remplacer les e-mails POP par des files d’attente des demandes avec la version 21.1
description: Nous remplaçons l’option de messagerie POP des files d’attente des demandes par un nouveau système géré par Adobe Workfront. Vous pourrez toujours envoyer des demandes par e-mail, mais vous devrez configurer une nouvelle adresse e-mail gérée par Workfront dans la zone File d’attente des demandes.
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
TQID: https://experienceleague.adobe.com/zzr53eiyA6o-VpZQnFQt-xCXZBKaScZUz8jDmOgX-Ns
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 100%

---

# Nouveau système géré Adobe Workfront pour remplacer la messagerie POP des files d’attente des demandes avec la version 21.1

Nous remplaçons l’option de messagerie POP des files d’attente des demandes par un nouveau système géré par Adobe Workfront. Vous pourrez toujours envoyer des demandes par e-mail, mais vous devrez configurer une nouvelle adresse e-mail gérée par Workfront dans la zone File d’attente des demandes.

## Pourquoi supprimez-vous l’option de messagerie POP ?

La technologie POP est une option de messagerie peu fiable et moins sécurisée. De plus, nous avons constaté que de nombreux problèmes de nos clientes et clients sont liés à la messagerie POP. Passer à un système géré Workfront permet d’obtenir une expérience plus fiable.

## Quelle action dois-je entreprendre ?

Vous devez configurer une nouvelle adresse e-mail pour chaque file d’attente des demandes configurée avec la messagerie POP dans votre environnement de production et distribuer la nouvelle adresse e-mail selon vos besoins. Pour plus d’informations, voir [Autoriser les utilisateurs et utilisatrices à envoyer par e-mail un problème dans un projet de file d’attente des demandes](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Quel est le plan de transition ?

À compter de la version 21.1 au début du mois de février, vous aurez 60 jours pour faire passer vos utilisateurs et utilisatrices à la nouvelle adresse e-mail *@intake.workfront.com* que vous aurez créée. Pendant la période de 60 jours, la messagerie POP utilisée précédemment continuera de fonctionner.

## Comment puis-je faire l’essai en prévisualisation ?

Pour tester cette modification en prévisualisation, vous devez activer les e-mails dans votre environnement de prévisualisation. Pour ce faire, suivez les instructions dans la section Gérer les e-mails en prévisualisation dans [Activer la diffusion des e-mails à partir de l’environnement sandbox de prévisualisation](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>Ce que vous définissez ici ne sera pas transféré vers votre environnement de production. Vous devrez recommencer cette procédure une fois la fonctionnalité mise en production.
