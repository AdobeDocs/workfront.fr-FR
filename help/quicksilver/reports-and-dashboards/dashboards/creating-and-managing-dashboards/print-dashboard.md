---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Imprimer un tableau de bord
description: Vous pouvez imprimer ou exporter un tableau de bord vers un fichier .PDF. Pour imprimer un tableau de bord, vous devez disposer des autorisations nécessaires pour le Visualiser.
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: efae17458f2aa08ca2286ef5e43c68d1f9334b7b
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 18%

---

# Imprimer un tableau de bord

Vous pouvez imprimer ou exporter un tableau de bord vers un fichier .PDF. Pour imprimer un tableau de bord, vous devez disposer des autorisations nécessaires pour le Visualiser.

>[!NOTE]
>
>Cette fonctionnalité est réservée à l’utilisation avec la vue standard Tableau de bord . Elle n’est pas disponible pour les tableaux de bord qui sont incorporés dans la zone Projets ou définis comme des onglets personnalisés.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Forfait Adobe Workfront*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Travail ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>Affichage de l’accès aux rapports, aux tableaux de bord et aux calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong>/td&gt; 
   <td> <p>Affichage des autorisations pour le tableau de bord</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Le tableau de bord doit être créé avant de pouvoir être imprimé.

Pour plus d’informations sur la création de tableaux de bord, voir [Création d’un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Comprendre les informations imprimées lors de l’impression d’un tableau de bord

Lors de l’impression d’un tableau de bord ou de son enregistrement en tant que fichier .PDF, certaines informations du tableau de bord, telles qu’elles apparaissent dans l’application web Adobe Workfront, peuvent ne pas apparaître sur le fichier imprimé ou exporté.

* [Qu’est-ce qui s’affiche ?](#what-is-displayed)
* [Que ne s’affiche pas ?](#what-is-not-displayed)

### Que s’affiche-t-il ? {#what-is-displayed}

Les informations suivantes sont incluses dans le fichier de tableau de bord imprimé ou exporté :

* Titre du tableau de bord
* Titres des rapports
* Horodatage du dernier rapport généré
* Tous les objets du tableau de bord, y compris les vues de liste, les pages web externes, les rapports et les calendriers
* Le logo de votre société, si votre administrateur Workfront l’a personnalisé dans votre barre de navigation globale. Pour plus d’informations sur l’identité graphique du site Workfront, voir [Marquez votre instance Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### Que ne s’affiche pas ? {#what-is-not-displayed}

Les informations suivantes ne sont pas incluses dans le fichier de tableau de bord imprimé ou exporté :

* La barre de navigation de Workfront
* Toute autre mise en forme spécifique à Workfront
* Selon la taille de vos rapports et le nombre et la largeur des colonnes individuelles, l’exportation et l’impression d’un tableau de bord peuvent entraîner la suppression de certaines colonnes.

## Imprimer un tableau de bord

1. Accédez au tableau de bord que vous souhaitez imprimer.
1. Effectuez l’une des opérations suivantes :

   * Cliquez sur **Actions du tableau de bord** > **Imprimer**

   * Appuyez sur **Ctrl+P** (sous Windows) ou **Commande+P** (sous Mac).

     >[!IMPORTANT]
     >
     >* Aucune de ces options n’est disponible lorsque le tableau de bord est incorporé à un onglet personnalisé. Pour plus d’informations sur la création d’onglets personnalisés, voir [Création d’onglets ou de sections personnalisés](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
     >* L’option de raccourci clavier n’est pas disponible lors de l’utilisation du navigateur Internet Explorer.

1. Dans le champ **Destination** , sélectionnez l’une des différentes options d’impression disponibles.\
   Les options d’impression varient en fonction du navigateur et de la version du navigateur que vous utilisez.

1. (Facultatif) Enregistrez le tableau de bord en tant que fichier .PDF, puis cliquez sur **Enregistrer** pour enregistrer le fichier .PDF.\
   Pour savoir comment enregistrer le tableau de bord en tant que fichier .PDF, voir [Exporter un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. Cliquez sur **Imprimer**.
