---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Rechercher des éléments  [!DNL Adobe Workfront]  à partir de  [!DNL Slack]
description: Vous pouvez rechercher des éléments  [!DNL Adobe Workfront]  à partir de l’application  [!DNL Slack], if your instance of Slack has had the [!DNL Workfront]  installée.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
TQID: https://experienceleague.adobe.com/JulYq173XQa6mG93qzUwfBDn4TPVEafD2OVpcIAXxi8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 209
ht-degree: 100%

---

# Rechercher des éléments sur [!DNL Adobe Workfront] à partir de [!DNL Slack]

Vous pouvez rechercher des éléments sur [!DNL Adobe Workfront] à partir de [!DNL Slack], si l’application [!DNL Workfront] a été installée sur votre instance de [!DNL Slack].

Pour plus d’informations sur la configuration de [!DNL Workfront] avec [!DNL Slack], voir [Configurer  [!DNL Adobe Workfront]  pour  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Tous</p>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de pouvoir rechercher des éléments [!DNL Workfront] à partir de [!DNL Slack], vous devez effectuer les opérations suivantes :

* Configurer [!DNL Workfront] pour [!DNL Slack]\
   Pour obtenir des instructions sur la configuration de [!DNL Workfront for Slack], voir [Configurer  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Rechercher des éléments [!DNL Workfront] à partir de [!DNL Slack] :

1. Connectez-vous à votre instance [!DNL Slack] et connectez-vous à [!DNL Workfront] à partir de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section « Se connecter à [!DNL Workfront] à partir de [!DNL Slack] » sur la page [Accéder à  [!DNL Adobe Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Choisissez un canal et commencez à saisir l’une des commandes suivantes dans le champ de message :

   `/workfront search <keyword>`

   Ou

   `/wf search <keyword>`

   >[!NOTE]
   >
   >Les commandes respectent la casse. Le mot-clé n’est pas sensible à la casse et doit être saisi sans crochets ni guillemets.

1. Dans le champ qui s’affiche, sélectionnez un type d’objet parmi les suivants :

   * Projet
   * Tâche
   * Problème
   * Rapport
   * Personnes
   * Modèle
   * Document
   * Portfolio
   * Programme
   * Tableau de bord
   * Entreprise
   * Note

     Vous ne pouvez sélectionner qu’un seul type d’objet à la fois.\
      Une liste d’éléments correspondant aux critères de recherche s’affiche.

1. Cliquez sur le nom d’un élément pour l’ouvrir dans [!DNL Workfront] dans un nouvel onglet du navigateur.
