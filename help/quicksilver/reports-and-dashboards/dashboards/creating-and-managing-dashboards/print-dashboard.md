---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Imprimer un tableau de bord
description: Vous pouvez imprimer ou exporter un tableau de bord vers un fichier PDF. Pour imprimer un tableau de bord, vous devez disposer des autorisations nécessaires pour le visualiser.
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 98%

---

# Imprimer un tableau de bord

<!-- Audited: 1/2025 -->

Vous pouvez imprimer ou exporter un tableau de bord vers un fichier PDF. Pour imprimer un tableau de bord, vous devez disposer des autorisations nécessaires pour le visualiser.

>[!NOTE]
>
>Cette fonctionnalité est réservée à la vue standard Tableau de bord. Elle n’est pas disponible pour les tableaux de bord qui sont incorporés dans la zone Projets ou définis comme des onglets personnalisés.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
      <p>Standard</p>
      <p>Travail ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux rapports, aux tableaux de bord et aux calendriers</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher des autorisations pour le tableau de bord</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Le tableau de bord doit être créé avant de pouvoir être imprimé.

Pour plus d’informations sur la création de tableaux de bord, voir [Créer un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Comprendre les informations imprimées lors de l’impression d’un tableau de bord

Lors de l’impression d’un tableau de bord ou de son enregistrement en tant que fichier PDF, certaines informations du tableau de bord, telles qu’elles apparaissent dans l’application web Adobe Workfront, peuvent ne pas apparaître sur le fichier imprimé ou exporté.

* [Quels sont les éléments affichés ?](#what-is-displayed)
* [Quels sont les éléments qui ne s’affichent pas ?](#what-is-not-displayed)

### Quels sont les éléments affichés ? {#what-is-displayed}

Les informations suivantes sont incluses dans le fichier de tableau de bord imprimé ou exporté :

* Titre du tableau de bord
* Titres des rapports
* Date et heure de la dernière génération du rapport
* Tous les objets du tableau de bord, y compris les vues de liste, les pages web externes, les rapports et les calendriers
* Le logo de votre société, si votre administration Workfront l’a personnalisé dans votre barre de navigation globale. Pour plus d’informations sur le placement d’une image de marque sur le site Workfront, voir [Appliquer votre image de marque à votre instance Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### Quels sont les éléments qui ne s’affichent pas ? {#what-is-not-displayed}

Les informations suivantes ne sont pas incluses dans le fichier de tableau de bord imprimé ou exporté :

* La barre de navigation de Workfront
* Toute autre mise en forme spécifique à Workfront
* Selon la taille de vos rapports et le nombre et la largeur des colonnes individuelles, l’export et l’impression d’un tableau de bord peuvent entraîner la suppression de certaines colonnes.

## Imprimer un tableau de bord

1. Accédez au tableau de bord que vous souhaitez imprimer.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur **Actions du tableau de bord** > **Aperçu avant impression**

   * Appuyez sur **Ctrl+P** (sous Windows) ou **Commande+P** (sur Mac).

     >[!IMPORTANT]
     >
     >* Aucune de ces options n’est disponible lorsque le tableau de bord est incorporé à un onglet personnalisé. Pour plus d’informations sur la création d’onglets personnalisés, voir [Créer des onglets ou des sections personnalisés](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
     >* L’option de raccourci clavier n’est pas disponible lors de l’utilisation du navigateur Internet Explorer.

1. Dans le champ **Destination**, sélectionnez parmi les différentes options d’impression disponibles.\
   Les options d’impression varient en fonction du navigateur et de la version du navigateur que vous utilisez.

1. (Facultatif) Enregistrez le tableau de bord en tant que fichier PDF, puis cliquez sur **Enregistrer** pour enregistrer le fichier PDF.\
   Pour savoir comment enregistrer le tableau de bord en tant que fichier PDF, voir [Exporter un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. Cliquez sur **Imprimer**.
