---
product-area: resource-management
navigation-topic: resource-planning
title: Exporter des informations à partir du planificateur de ressources
description: Vous pouvez exporter des informations de n’importe quelle vue du planificateur de ressources vers un fichier Excel (.xlsx) enregistré sur votre ordinateur.
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 3%

---

# Exporter des informations à partir du planificateur de ressources

Vous pouvez exporter des informations de n’importe quelle vue du planificateur de ressources vers un fichier Excel (.xlsx) enregistré sur votre ordinateur.

>[!IMPORTANT]
>
>Les informations affichées et les informations que vous pouvez exporter à partir du planificateur de ressources sont limitées. Pour plus d’informations sur ces limites, voir [Limites d’affichage de Resource Planner](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage ou accès supérieur à la gestion des projets, des utilisateurs et des ressources</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations ou plus pour les projets</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Exporter des informations à partir du planificateur de ressources

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Ressource**. Le **Planificateur** s’affiche par défaut.

1. Sélectionnez la vue du planificateur. Vous pouvez sélectionner l’une des options suivantes :

   * Afficher par utilisateur
   * Afficher par projet
   * Afficher par fonction

1. Cliquez sur **Exporter**.

   La boîte de dialogue Options d’exportation s’affiche.

   ![](assets/rp-export-options-box-350x421.png)

1. Indiquez les informations suivantes :\
   **Date de début**: Date de début de l’exportation. Le fichier exporté contient des informations d&#39;attribution et de disponibilité commençant par le premier jour de la semaine qui contient le jour que vous indiquez ici.\
   **Nombre de périodes**: Le nombre de périodes que vous souhaitez inclure dans votre fichier. La valeur par défaut est de 4 points.\
   **Type**: Type de période par laquelle vous souhaitez afficher les informations dans le fichier exporté (semaines, mois ou trimestres).\
   Voici les périodes maximales que vous pouvez exporter :

   * 52 semaines
   * 36 mois
   * 12 trimestres

   **Sélectionner à exporter**: Selon la vue que vous avez sélectionnée, vous pouvez choisir d&#39;exporter les informations de disponibilité et de budget, soit pour tous les objets affichés à l&#39;écran, soit pour des objets spécifiques.
Vous pouvez choisir d&#39;exporter les informations suivantes :

   * Dans la vue Projet, sélectionnez pour exporter :

      * Projets
      * Projets et rôles
      * Tout (il s’agit de l’option par défaut)
   * Dans la vue Utilisateur, sélectionnez pour exporter :

      * Utilisateurs
      * Utilisateurs et projets
      * Tout (il s’agit de l’option par défaut)
   * Dans la vue Rôle, sélectionnez pour exporter :

      * Rôles
      * Rôles et projets
      * Tout (il s’agit de l’option par défaut)

   **Formatage des données**: Sélectionnez les options suivantes en fonction de l’affichage du fichier Excel :

   * **Brut**: Sélectionnez cette option pour afficher les informations de disponibilité et d&#39;allocation dégroupées par les objets auxquels il appartient dans le fichier Excel. (il s’agit de l’option par défaut)
   * **Regroupé**: Sélectionnez cette option pour afficher les informations de disponibilité et d&#39;allocation regroupées par les objets auxquels il appartient. Les informations exportées s’affichent alors à l’écran.

   Un exemple de l’aspect des informations dans le fichier exporté s’affiche dans la boîte de dialogue Options d’exportation .

1. Cliquez sur **Exporter** pour exporter les informations du planificateur de ressources.\
   Seules les informations que vous avez enregistrées sont exportées.

1. (Conditionnel) Si vous avez enregistré des heures budgétaires non enregistrées dans les vues Rôle ou Projet, cliquez sur **Enregistrez et continuez.**
Un fichier Excel (.xlsx) est téléchargé sur votre ordinateur.
\
   L’exportation depuis le planificateur de ressources n’est pas disponible lorsque le fichier est préparé pour le téléchargement.\
   (Conditionnel) Si vous exportez une grande quantité de données, vous recevez un courrier électronique contenant un lien pour télécharger le fichier.\
   ![RP_email_with_export_planner_attachment.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Conditionnel) Lorsque vous recevez le courrier électronique contenant le fichier exporté, cliquez sur **Télécharger** pour télécharger le fichier.\
   Vous revenez alors à Workfront où vous pouvez télécharger le fichier.\
   Vous devez être connecté à Workfront pour que le téléchargement soit terminé.\
   Si vous ne téléchargez pas le fichier lors de sa diffusion, le lien Télécharger reste principal pendant 7 jours après avoir lancé l’exportation.
