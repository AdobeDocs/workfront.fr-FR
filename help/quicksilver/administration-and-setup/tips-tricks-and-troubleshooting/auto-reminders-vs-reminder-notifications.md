---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Reminders automatiques et notifications de rappel
description: Cet article décrit les différences entre les rappels automatiques et les notifications de rappel et fournit des scénarios pour chacun d’eux.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 26c6fa2c-5c3a-4f53-bd7e-e49a623ff60d
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 91%

---

# Rappels automatiques et notifications de rappel

Cet article décrit les différences entre les rappels automatiques et les notifications de rappel et fournit des scénarios pour chacun d’entre eux. Pour plus d’informations sur toutes les notifications [!DNL Adobe Workfront], consultez les notifications [[!DNL Adobe Workfront] ](../../workfront-basics/using-notifications/wf-notifications.md).

## Rappels automatiques

Les caractéristiques suivantes sont spécifiques aux rappels automatiques :

* Leur activation et leur modification ne peuvent être effectuées que par un administrateur ou une administratrice [!DNL Workfront].
* Ils sont déclenchés pour toutes les tâches et problèmes lorsqu’ils sont dus, en retard ou proches de la date d’achèvement prévue.
* Ils ne peuvent être envoyés qu’à la personne cessionnaire, à la personne responsable de la personne cessionnaire ou à la personne responsable de la personne responsable directe.
* Ils ne peuvent pas ne pas être accompagnés d’un modèle d’e-mail.

Scénario : si vous souhaitez que des rappels soient déclenchés pour toutes les tâches et problèmes dans l’ensemble du système, configurez des paramètres de rappel automatique. Pour plus d’informations, voir [Configurer des rappels automatiques](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

## Notifications de rappel

Les caractéristiques suivantes sont spécifiques aux notifications de rappel :

* Elles peuvent être créées par un administrateur ou une administratrice ou toute personne disposant d’une licence Plan et d’un accès administratif aux notifications de rappel.
* Elles ne peuvent être qu’associées manuellement à un objet.
* Elles ne peuvent notifier que par rapport à l’objet joint.
* Elles peuvent être envoyées à différentes parties prenantes de l’objet, telles que la personne propriétaire, le créateur ou la créatrice, l’approbateur ou l’approbatrice ou la personne cessionnaire.
* Il est possible d’utiliser l’e-mail par défaut ou un modèle d’e-mail personnalisé qui est joint.

Scénario : si vous souhaitez créer des rappels pour des projets ou des feuilles de temps, ou si vous voulez personnaliser les rappels pour les tâches et les problèmes, configurez des notifications de rappel. Pour plus d’informations, voir [Configurer des notifications de rappel](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
