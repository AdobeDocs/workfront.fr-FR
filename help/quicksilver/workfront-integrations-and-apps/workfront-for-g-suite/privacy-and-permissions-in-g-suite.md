---
product-area: workfront-integrations
keywords: google,doc,document,sheet,diapositive
navigation-topic: workfront-for-g-suite
title: Confidentialité et autorisations dans Workfront pour G Suite
description: Confidentialité et autorisations dans Workfront pour G Suite
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 90d088846e72f1632274043c8d8ca7807ff05b4a
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Confidentialité et autorisations dans Workfront pour G Suite

La confidentialité des clients étant importante, Adobe Workfront ne stocke ni ne collecte aucune donnée client d’identification résultant d’une autorisation tierce d’une application de module externe Google. Workfront for G Suite est conforme à la politique de données utilisateur des services d’API de Google, y compris aux exigences d’utilisation limitée.

Nous avons besoin des autorisations suivantes afin que le module externe Workfront for G Suite puisse fournir sa valeur maximale :

* **Afficher vos messages électroniques lorsque le module complémentaire est en cours d’exécution**: Le plug-in Workfront for G Suite permet aux utilisateurs d’économiser d’innombrables heures de travail en double en convertissant les emails en nouvelles tâches dans Workfront et en renseignant automatiquement le titre et la description de la tâche avec l’objet et le corps du message. Le plug-in permet également de publier vos emails dans Workfront en tant que nouveaux commentaires. Le plug-in doit afficher vos e-mails lorsque le module complémentaire est en cours d’exécution pour fournir cette valeur.
* **Exécuter en tant que module complémentaire Gmail / non sensible**: Des autorisations sont nécessaires pour que le module complémentaire Workfront for G Suite fonctionne dans l’environnement Gmail. Le plug-in nécessite un environnement Gmail pour fonctionner. Il nécessite donc la fonction `Run as a Gmail add-on / non-sensitive` autorisation.
* **Affichage des métadonnées de votre message électronique lorsque le module complémentaire est en cours d’exécution**: Pour améliorer les workflows, le plug-in Workfront for G Suite confirme si un email est une notification Workfront et identifie le type de notification Workfront (nouvelle demande de travail, demande d’approbation, nouveau commentaire, etc.). Le plug-in nécessite la fonction `View your email message metadata when the add-on is running` autorisation de fournir cette valeur.
* **Le module externe doit s’exécuter en tant que module complémentaire de calendrier/non sensible**: Le plug-in Workfront for G Suite se connecte à votre calendrier afin que vous puissiez visualiser l’impact des tâches sur les plannings. Le module externe a besoin de la fonction `Run as a Calendar add-on / non-sensitive` autorisation de le faire.
* **Connectez-vous à une autorisation de service externe :** En fin de compte, le plug-in doit se connecter à l’API Workfront, qui est la colonne vertébrale de la valeur du plug-in. L’API Workfront est un service externe à Google. Par conséquent, le plug-in nécessite la variable `Connect to an external service permission` pour que le module externe fonctionne.

Pour plus d’informations sur le dévouement d’Adobe Workfront à la vie privée des clients, voir [Notification de confidentialité Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Pour plus d’informations, voir [Stratégie de données utilisateur des services d’API Google](https://developers.google.com/terms/api-services-user-data-policy).
