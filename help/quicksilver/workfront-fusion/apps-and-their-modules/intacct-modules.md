---
title: Installer les modules
description: Installer les modules
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# Installer les modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Analysis Workspace et les connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr>
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules d’installation, vous devez disposer d’un compte d’installation.

## Connexion à Workfront Fusion

### Autorisation [!DNL Workfront Fusion] pour apporter des modifications à Target

Avant [!DNL Workfront Fusion] peut se connecter à [!DNL Intacct], vous devez l’autoriser.

Dans votre compte d’installation, accédez à la **[!UICONTROL Société]** .

1. Cliquez sur **Informations sur la société**.
1. Accédez au **Sécurité** .
1. Cliquez sur [!UICONTROL Modifier] dans le coin supérieur droit
1. Sélectionnez Autorisations des services Web.
1. Cliquez sur l’icône Plus
1. Saisissez AzuquaMPP comme sender_id.
1. (Facultatif) Saisissez une description pour la connexion.

### Configurer une connexion dans [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

Vous pouvez créer une connexion à votre [!DNL Intacct] compte directement depuis l’intérieur d’une [!DNL Intacct] module .

1. Dans n’importe quel module d’installation, cliquez sur **[!UICONTROL Ajouter]** en regard du champ Connexion .
1. Entrez vos informations d’identification d’intégration

   * ID d&#39;entreprise
   * ID d’utilisateur
   * Mot de passe

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et revenir au module .

## Installer les modules et leurs champs

Lorsque vous configurez [!DNL Intacct] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En outre, d’autres champs d’intégration peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Effectuer un appel API personnalisé]](#make-a-custom-api-call)
* [[!UICONTROL Recherche d’enregistrements]](#search-records)

### [!UICONTROL Effectuer un appel API personnalisé] {#make-a-custom-api-call}

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers le [!DNL Intacct] API. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par l’autre [!DNL Intacct] modules.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connexion</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte d’installation à [!DNL Workfront Fusion] 2.0, voir <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Configuration d’une connexion dans Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body XML</td> 
   <td> <p>Inclure uniquement le code XML dans le corps. La requête inclut automatiquement des en-têtes d’authentification.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Recherche d’enregistrements]

Ce module de recherche récupère une liste d’enregistrements correspondant à des critères de recherche spécifiques.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connexion</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte d’installation à [!DNL Workfront Fusion] 2.0, voir <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Configuration d’une connexion dans Workfront Fusion</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’enregistrement]</td> 
   <td> <p>Sélectionnez le type d’enregistrement à rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Critères de recherche</p> </td> 
   <td> 
    <ul> 
     <li> <p>Sélectionnez le champ par lequel vous souhaitez effectuer une recherche.</p> </li> 
     <li> <p>Sélectionnez l’opérateur que vous souhaitez utiliser pour la recherche.</p> </li> 
     <li> <p>Saisissez la valeur à rechercher.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jeu de résultats</td> 
   <td>Indiquez si vous souhaitez renvoyer tous les enregistrements correspondants ou uniquement le premier enregistrement correspondant.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limite</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Classer par</td> 
   <td>Sélectionnez le champ selon lequel vous souhaitez trier les résultats. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ordre</td> 
   <td>Indiquez si vous souhaitez trier par ordre croissant ou décroissant.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sorties</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Respect de la casse</td> 
   <td>Activez cette option pour rendre votre requête sensible à la casse.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Interrogation des entités privées</td> 
   <td>Activez cette option pour permettre au module de rechercher des entités privées.</td> 
  </tr> 
 </tbody> 
</table>
