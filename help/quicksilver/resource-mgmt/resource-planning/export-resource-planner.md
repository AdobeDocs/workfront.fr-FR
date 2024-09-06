---
product-area: resource-management
navigation-topic: resource-planning
title: Exporter des informations à partir du planificateur de ressources
description: Vous pouvez exporter des informations à partir de n’importe quelle vue du planificateur de ressources vers un fichier Excel (.xlsx) enregistré sur votre ordinateur.
author: Lisa
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 96%

---

# Exporter des informations du planificateur de ressources

Vous pouvez exporter des informations à partir de n’importe quelle vue du planificateur de ressources vers un fichier Excel (.xlsx) enregistré sur votre ordinateur.

>[!IMPORTANT]
>
>Les informations affichées et celles que vous pouvez exporter à partir du planificateur de ressources sont limitées. Pour plus d’informations sur ces limitations, voir la section [Limitations d’affichage du planificateur de ressources](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td><p>Nouveau : Tous</p>
       <p>ou</p>
       <p>Actuel : Pro ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Light ou supérieur</p>
       <p>ou</p>
       <p>Actuel : Révision ou supérieur</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Afficher l’accès ou une version ultérieure à Projets, Utilisateurs et Gestion des ressources</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou niveau supérieur pour les projets</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exporter des informations du planificateur de ressources

{{step1-to-resourcing}}

Le **planificateur** s’affiche par défaut.

1. Sélectionnez la vue du planificateur. Vous pouvez sélectionner l’une des options suivantes :

   * Par utilisateur
   * Par projet
   * Par fonction

1. Cliquez sur **Exporter**.

   La boîte de dialogue Options d’export s’affiche.

   ![](assets/rp-export-options-box-350x421.png)

1. Indiquez les informations suivantes :\
   **Date de début** : la date de début de votre export. Le fichier exporté contient des informations sur l’attribution et la disponibilité, en partant du premier jour de la semaine qui contient le jour que vous spécifiez ici.\
   **Nombre de périodes** : le nombre de périodes que vous souhaitez inclure dans votre fichier. La valeur par défaut est de 4 périodes.\
   **Type** : le type de périodes pour lesquelles vous souhaitez afficher les informations dans le fichier exporté (semaines, mois ou trimestres).\
   Les périodes maximales que vous pouvez exporter sont les suivantes :

   * 52 semaines
   * 36 mois
   * 12 trimestres

   **Sélectionner pour exporter** : en fonction de la vue sélectionnée, vous pouvez choisir d’exporter les informations de disponibilité et de budgétisation pour tous les objets listés à l’écran ou pour certains d’entre eux seulement.
Vous pouvez choisir d’exporter les informations suivantes :

   * Dans la vue du projet, sélectionnez pour export :

      * Projets
      * Projets et rôles
      * Tout (option par défaut)

   * Dans la vue de l’utilisateur ou l’utilisatrice, sélectionnez pour export :

      * Utilisateurs
      * Utilisateurs et projets
      * Tout (option par défaut)

   * Dans la vue Rôle, sélectionnez pour export :

      * Rôles
      * Rôles et projets
      * Tout (option par défaut)

   **Formatage des données** : selon la manière dont vous souhaitez afficher votre fichier Excel, sélectionnez les options suivantes :

   * **Brut** : sélectionnez cette option pour afficher les informations de disponibilité et d’affectation non regroupées par les objets auxquels elles appartiennent dans le fichier Excel. (Il s’agit de l’option par défaut.)
   * **Regroupement** : sélectionnez cette option pour afficher les informations de disponibilité et d’affectation regroupées par les objets auxquelles elles appartiennent. Les informations exportées sont affichées telles qu’elles apparaissent à l’écran.

   Un exemple de l’aspect des informations dans le fichier exporté est présenté dans la boîte de dialogue Options d’export.

1. Cliquez sur **Export** pour exporter les informations du planificateur de ressources.\
   Seules les informations que vous avez enregistrées sont exportées.

1. (Le cas échéant) Si vous avez des heures budgétées non enregistrées dans les vues Rôle ou Projet, cliquez sur **Enregistrer et continuer.** Un fichier Excel (.xlsx) est téléchargé sur votre ordinateur.\
   L’export à partir du planificateur de ressources n’est pas disponible pendant que le fichier est préparé pour le téléchargement.\
   (Le cas échéant) Si vous exportez une grande quantité de données, vous recevez un e-mail contenant un lien qui vous permet de télécharger le fichier.\
   ![RP_eamil_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Le cas échéant) Lorsque vous recevez l’e-mail contenant le fichier exporté, cliquez sur **Télécharger** pour télécharger le fichier.\
   Cela vous ramène à Workfront où vous pouvez télécharger le fichier.\
   Vous devez vous connecter à Workfront pour que le téléchargement s’effectue.\
   Si vous ne téléchargez pas le fichier lorsqu’il est livré, le lien de téléchargement reste actif pendant 7 jours après le lancement de l’export.
