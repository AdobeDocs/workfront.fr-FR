---
content-type: reference
navigation-topic: get-started-with-workfront
title: Préparation du HIPAA pour Workfront
description: Un client Workfront qui est, comme défini dans la loi HIPAA, un associé commercial et/ou l’entité couverte pour le compte de laquelle l’associé commercial fournit Adobe Workfront doit suivre les instructions suivantes pour configurer Workfront pour une utilisation conforme à la loi HIPAA.
feature: Get Started with Workfront
author: Courtney
hide: true
hidefromtoc: true
source-git-commit: a984038eea41d249cb0ad0d2ec6ba47025c56a65
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---


# Préparation du HIPAA pour Workfront

Un client Workfront qui est, comme défini dans la loi HIPAA, un associé commercial et/ou l’entité couverte pour le compte de laquelle l’associé commercial fournit Adobe Workfront doit suivre les instructions suivantes pour configurer Workfront pour une utilisation conforme à la loi HIPAA :


## Exigences de mot de passe

| **Paramètre de sécurité** | **Qu&#39;Est-Ce Que C&#39;Est ?** | **Exigence** |
|----------------------|------------------|------------------|
| Efficacité minimale du mot de passe pour les contrats | Quelle est la force minimale des mots de passe d&#39;accord ? | Pas moins de 8 caractères |
| Efficacité minimale du mot de passe pour les mots de passe utilisateur | Quelle est la force minimale des mots de passe des utilisateurs ? | Caractères appartenant à trois des catégories suivantes :<br>* Lettres majuscules (alphabet latin)<br>* Lettres minuscules (alphabet latin)<br>* Base 10 chiffres<br>* Caractères non alphanumériques |
| Durée du mot de passe | Pendant combien de temps les mots de passe doivent-ils rester inchangés ? | Les mots de passe doivent être modifiés au moins tous les 90 jours |
| Historique du mot de passe | Combien de mots de passe passés doivent être mémorisés et interdits ? | Pas moins de 5 |


## Exigences de connexion

| **Paramètre de sécurité** | **Qu&#39;Est-Ce Que C&#39;Est ?** | **Exigence** |
|----------------------|------------------|------------------|
| Nbre max. d&#39;échecs de connexion | Combien de tentatives de connexion ayant échoué l&#39;utilisateur a-t-il été verrouillé ? | Pas plus de 5 tentatives au cours d’une période de 5 minutes ; nouvelle tentative autorisée après 30 minutes |
| Nombre maximal d’échecs de vérification de l’authentification unique | Combien de tentatives de vérification de l&#39;authentification unique ayant échoué provoquent un verrouillage ? | Pas plus de 5 (s’applique uniquement aux clients utilisant la connexion unique) |


## Exigences de session

| **Paramètre de sécurité** | **Qu&#39;Est-Ce Que C&#39;Est ?** | **Exigence** |
|----------------------|------------------|------------------|
| Timeout de session | Combien de minutes d’inactivité entraînent une déconnexion ? | 15 minutes maximum |

## Responsabilités du client

Assurez-vous que tous les employés, représentants et/ou agents connaissent et comprennent les termes des contrats de licence et/ou de service signés entre les parties, le cas échéant, relatifs à l’utilisation des données avec Workfront.

En particulier, les responsabilités et obligations suivantes devraient être examinées et communiquées : 

* Le client est responsable de l’utilisation du service Workfront par tous ses utilisateurs. 

* Le client est tenu de respecter tous les termes de son contrat avec Adobe qui incluent des éléments de données interdits de chargement dans Workfront. 

* Toutes les données sensibles, y compris, mais sans s&#39;y limiter, les ePHI, sont téléchargées aux risques et périls du client.  Le client est en permanence responsable de toutes les données client. 


## Protection des données et conformité

>[!IMPORTANT]
>
>Workfront n’est pas conçu pour être un dépôt de dossiers de santé électroniques (DSE). ePHI ne peut être traité que si Adobe l&#39;a expressément autorisé par écrit. 

* Pour toute base de données Workfront où l’ePHI peut être accessible, assurez-vous que le **chiffrement au repos (EAR)** est activé.
   * Contactez votre chargé de compte (AE) pour vérifier que l’EAR est incluse dans votre achat Workfront.
   * Configurez les systèmes/bases de données accessibles via Workfront pour respecter les obligations de conformité.
* Assurez-vous que l’ePHI n’est pas transféré, lié ou partagé avec d’autres solutions Adobe.
* Veiller à ce que les photos des patients traitées via Workfront soient stockées en toute sécurité et non accessibles au public.