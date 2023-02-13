---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Rappels automatiques par rapport aux notifications de rappel
description: Cet article décrit les différences entre les rappels automatiques et les notifications de rappel et fournit des scénarios pour chacun d’eux. Pour plus d’informations sur tous les [!DNL Adobe Workfront] notifications, voir Adobe [!DNL Workfront] notifications.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 26c6fa2c-5c3a-4f53-bd7e-e49a623ff60d
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Rappels automatiques par rapport aux notifications de rappel

Cet article décrit les différences entre les rappels automatiques et les notifications de rappel et fournit des scénarios pour chacun d’eux. Pour plus d’informations sur tous les [!DNL Adobe Workfront] notifications, voir [[!DNL Adobe Workfront] notifications](../../workfront-basics/using-notifications/wf-notifications.md).

## Rappels automatiques

Les caractéristiques suivantes sont spécifiques aux rappels automatiques :

* Ne peuvent être activés et modifiés que par une [!DNL Workfront] administrator
* sont déclenchés sur toutes les tâches et problèmes lorsqu’ils sont dus, en retard ou près de la date d’achèvement prévue ;
* Ne peuvent être envoyés qu’au responsable désigné, au responsable du responsable ou au responsable du responsable immédiat.
* Impossible d’y joindre un modèle d’email.

Scénario : Si vous souhaitez que les rappels soient déclenchés sur toutes les tâches et problèmes du système, configurez les paramètres de rappel automatique. Pour plus d’informations, voir [Configuration de rappels automatiques](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

## Notifications de rappel

Les caractéristiques suivantes sont spécifiques aux notifications de rappel :

* Peut être créé par un administrateur ou tout utilisateur disposant d’une licence Plan et d’un accès administratif aux notifications de rappel
* Ne peut être associé manuellement qu’à un objet
* Peut uniquement avertir concernant l’objet joint
* Peut être envoyé à différents intervenants d’objets, tels que propriétaire, créateur, approbateur ou cessionnaire
* Peut utiliser l’email par défaut ou utiliser un modèle d’email personnalisé joint

Scénario : Si vous souhaitez créer des rappels pour des projets, des feuilles de temps ou personnaliser des rappels pour des tâches et des problèmes, configurez les notifications de rappel. Pour plus d’informations, voir [Configuration des notifications de rappel](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
