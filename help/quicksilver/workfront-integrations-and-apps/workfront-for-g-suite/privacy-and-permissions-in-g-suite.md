---
product-area: workfront-integrations
keywords: google,doc,document,feuille,diapositive
navigation-topic: workfront-for-g-suite
title: Confidentialité et autorisations dans Workfront pour Google Workspace
description: Confidentialité et autorisations dans Workfront pour Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 32%

---

# Confidentialité et autorisations dans Workfront pour Google Workspace

>[!IMPORTANT]
>
>Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de Workfront Automation and Integration (Fusion). Dans le cadre de ce processus de transition, la fonctionnalité Workfront for Google Workspace suivante ne sera plus disponible après le **28 février 2026** :
>
>* Accès à la fonctionnalité Google Workspace depuis Workfront
>
>* Affichage et gestion des tâches Workfront à partir de Gmail ou du panneau du site Calendrier Google
>
>Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre entreprise avec Google Workspace.
>
>Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez [Présentation d’Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Pour plus d’informations sur les fonctionnalités spécifiques des modules d’automatisation et d’intégration de Workfront pour Google Workspace, voir [Modules Gmail](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) et [Modules de calendrier Google](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

La confidentialité des clientes et clients étant importante, Adobe Workfront ne stocke ni ne collecte aucune donnée client d’identification résultant d’une autorisation tierce d’une application de plug-in Google. L’utilisation et le transfert des informations reçues des API de Google vers une autre application de Workfront for Google Workspace sont conformes à la politique de données de l’utilisateur des services d’API de Google [&#128279;](https://developers.google.com/terms/api-services-user-data-policy), y compris les exigences en matière d’utilisation limitée.

Nous avons besoin des autorisations ci-dessous pour que le plug-in Workfront for Google Workspace puisse délivrer sa valeur maximale :

* **Affichez vos e-mails lorsque le module complémentaire est en cours d’exécution** : le plug-in Workfront for Google Workspace peut permettre aux utilisateurs de gagner d’innombrables heures de travail en double en convertissant les e-mails en nouvelles tâches dans Workfront et en renseignant automatiquement le titre et la description de la tâche avec l’objet et le corps de l’e-mail. Le plug-in permet également de publier vos e-mails dans Workfront en tant que nouveaux commentaires. Le plug-in doit afficher vos e-mails lorsque le module complémentaire est en cours d’exécution pour fournir cette valeur.
* **Exécuté en tant que module complémentaire Gmail/non sensible** : des autorisations sont nécessaires pour que le module complémentaire Workfront for Google Workspace fonctionne dans l’environnement Gmail. Le plug-in nécessite un environnement Gmail pour fonctionner. Il nécessite donc l’autorisation `Run as a Gmail add-on / non-sensitive`.
* **Affichez les métadonnées de votre e-mail lorsque le module complémentaire est en cours d’exécution** : pour améliorer les workflows, le plug-in Workfront for Google Workspace confirme si un e-mail est une notification Workfront et identifie le type de notification Workfront (nouvelle demande de travail, demande d’approbation, nouveau commentaire, etc.). Le plug-in nécessite l’autorisation `View your email message metadata when the add-on is running` pour fournir cette valeur.
* **Le plug-in doit s’exécuter en tant que module complémentaire de calendrier/non sensible** : le plug-in Workfront for Google Workspace se connecte à votre calendrier afin que vous puissiez visualiser l’impact des tâches sur les plannings. Le plug-in a besoin de l’autorisation `Run as a Calendar add-on / non-sensitive` pour faire cela.
* **Se connecter à une autorisation de service externe :** en fin de compte, le plug-in doit se connecter à l’API Workfront, qui est la colonne vertébrale de la valeur du plug-in. L’API Workfront est un service externe à Google. Par conséquent, le plug-in nécessite l’`Connect to an external service permission` pour que le plug-in fonctionne.

Pour plus d’informations sur l’attachement d’Adobe Workfront à la confidentialité des clientes et clients, voir [Politique de confidentialité de Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Pour plus d’informations, voir [Politique de données utilisateur des services d’API Google](https://developers.google.com/terms/api-services-user-data-policy).
