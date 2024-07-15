---
product-area: workfront-integrations
keywords: google,doc,document,sheet,diapositive
navigation-topic: workfront-for-g-suite
title: Confidentialité et autorisations dans Workfront pour Google Workspace
description: Confidentialité et autorisations dans Workfront pour Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Confidentialité et autorisations dans Workfront pour Google Workspace

La confidentialité des clients étant importante, Adobe Workfront ne stocke ni ne collecte aucune donnée client d’identification résultant d’une autorisation tierce d’une application de module externe Google. Workfront for Google Workspace L’utilisation et le transfert des informations reçues des API Google vers toute autre application seront conformes à la [stratégie de données utilisateur des services d’API Google](https://developers.google.com/terms/api-services-user-data-policy), y compris les conditions d’utilisation limitées.

Nous avons besoin des autorisations suivantes afin que le module externe Workfront for Google Workspace puisse fournir sa valeur maximale :

* **Affichez vos e-mails lorsque le module complémentaire est en cours d’exécution** : le plug-in Workfront for Google Workspace permet aux utilisateurs d’économiser d’innombrables heures de travail en double en convertissant les e-mails en nouvelles tâches dans Workfront et en renseignant automatiquement le titre et la description de la tâche avec l’objet et le corps de l’e-mail. Le plug-in permet également de publier vos emails dans Workfront en tant que nouveaux commentaires. Le plug-in doit afficher vos e-mails lorsque le module complémentaire est en cours d’exécution pour fournir cette valeur.
* **Exécuter en tant que module complémentaire Gmail / non sensible** : des autorisations sont nécessaires pour que le module complémentaire Workfront for Google Workspace fonctionne dans l’environnement Gmail. Le plug-in nécessite un environnement Gmail pour fonctionner. Il nécessite donc l’autorisation `Run as a Gmail add-on / non-sensitive`.
* **Affichez les métadonnées de votre message électronique lorsque le module complémentaire est en cours d’exécution** : pour améliorer les workflows, le module externe Workfront for Google Workspace confirme si un message électronique est une notification Workfront et identifie le type de notification Workfront (nouvelle demande de travail, demande d’approbation, nouveau commentaire, etc.). Le plug-in nécessite l’autorisation `View your email message metadata when the add-on is running` pour fournir cette valeur.
* **Le module externe doit s’exécuter en tant que module complémentaire de calendrier / non sensible** : le module externe Workfront for Google Workspace se connecte à votre calendrier, afin que vous puissiez visualiser l’impact des tâches sur les plannings. Pour ce faire, le plug-in doit disposer de l’autorisation `Run as a Calendar add-on / non-sensitive` .
* **Connectez-vous à une autorisation de service externe :** En fin de compte, le plug-in doit se connecter à l’API Workfront, qui est la colonne vertébrale de la valeur du plug-in. L’API Workfront est un service externe à Google. Par conséquent, le plug-in nécessite `Connect to an external service permission` pour que le plug-in fonctionne.

Pour plus d’informations sur le dévouement Adobe Workfront à la vie privée des clients, voir [Workfront la notification de confidentialité](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Pour plus d’informations, voir [Stratégie de données utilisateur des services d’API Google](https://developers.google.com/terms/api-services-user-data-policy).
