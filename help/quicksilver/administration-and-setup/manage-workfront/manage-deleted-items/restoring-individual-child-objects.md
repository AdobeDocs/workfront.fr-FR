---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restaurer des objets enfant individuels
description: Cet article décrit comment obtenir de l’aide pour récupérer des objets enfants individuels qui ont été supprimés de vos environnements de production ou de prévisualisation Adobe Workfront moins de 30 jours auparavant.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 90%

---

# Restaurer des objets enfants individuels

Cet article décrit comment obtenir de l’aide pour récupérer des objets enfants individuels qui ont été supprimés de vos environnements de production ou de prévisualisation Adobe Workfront moins de 30 jours auparavant.

Un administrateur ou une administratrice Workfront peut restaurer des projets, des tâches, des problèmes et des documents dans chaque instance Workfront, comme décrit dans la section [Restaurer des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). Cependant, seule l’équipe de base de données Workfront peut restaurer des objets tels que des tâches, des problèmes, des documents, des formulaires personnalisés, des heures et des notes indépendamment de leur objet parent.

Les données de votre environnement en ligne sont disponibles dans l’environnement sandbox de prévisualisation pendant 7 jours au maximum. Cela signifie que vous pouvez exporter les données autonomes à partir de l’environnement sandbox de prévisualisation à l’aide des méthodes suivantes :

* Lancements
* Créer un rapport et exporter les résultats

Pour plus d’informations sur l’export de données à partir de Workfront, voir [Exporter des données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Vous pouvez importer les données exportées de la manière suivante :

* Manuellement, si vous utilisez des rapports exportés.
* En masse, si vous utilisez des kickstart

  Pour plus d’informations sur l’import de données dans Workfront à l’aide des kickstart, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle de kickstart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

L’environnement sandbox de prévisualisation est actualisé pendant les fenêtres de maintenance du week-end.

Pour plus d’informations sur les fenêtres de maintenance de l’environnement sandbox de prévisualisation, voir [le site des statuts Adobe](https://status.adobe.com/fr).

>[!IMPORTANT]
>
>Les documents constituent une exception à ces méthodes de restauration. Vous pouvez les télécharger manuellement à partir de l’environnement de prévisualisation et les charger à nouveau dans l’environnement de production. Si vous souhaitez télécharger et charger des documents en masse, vous devez demander une restauration des données à Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informations nécessaires à la restauration des données

Une fois que vous avez déterminé qu’un objet supprimé doit être restauré par notre équipe de base de données, collectez autant d’informations que possible à son sujet. Les informations suivantes sont requises pour que les administrateurs et administratrices de base de données trouvent l’objet et lancent une restauration :

* Nom de l&#39;objet
* Type d’objet (tâche, problème, projet, etc.)
* Date et heure estimées de la suppression
* GUID de l’objet (si possible)

  Reportez-vous aux informations suivantes pour trouver le GUID d’un objet :

   * Le GUID est accessible en référençant des notifications par e-mail déclenchées en interagissant avec l’objet (affectations, commentaires, etc.).
   * Exemple de GUID situé à la fin d’une URL : `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Une fois que vous avez rassemblé ces informations ou si vous avez besoin d’aide, contactez notre équipe d’assistance clientèle au 844-306-HELP(4357) ou soumettez un ticket en ligne.

## Processus de restauration des données

1. Une fois que notre équipe d’assistance clientèle aura reçu vos informations, elle les transmettra à notre équipe d’assistance clientèle.
1. Notre équipe d’assistance clientèle contactera notre équipe de base de données.
1. Une fois que l’équipe de base de données a eu la possibilité de passer en revue les données à restaurer, une estimation plus précise de l’ETA pourra être fournie. Une restauration prend généralement trois jours, mais peut prendre plus de temps en fonction du type et du volume des données à restaurer.
1. L’équipe de base de données restaurera les informations dans votre environnement sandbox de prévisualisation où vous aurez la possibilité de passer en revue les données restaurées. Notre équipe d’assistance clientèle vous contactera lorsque les données seront disponibles dans l’environnement sandbox de prévisualisation.
1. Si la restauration dans l’environnement sandbox vous convient, faites-le savoir à notre équipe d’assistance clientèle. Elle contactera notre équipe de base de données pour l’informer qu’elle peut restaurer les données dans votre environnement de production.
1. Vous aurez la possibilité de consulter les données restaurées avant que la demande ne soit fermée.
