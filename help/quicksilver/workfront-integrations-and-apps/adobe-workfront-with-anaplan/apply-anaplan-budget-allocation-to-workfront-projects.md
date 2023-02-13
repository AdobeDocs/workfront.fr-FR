---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Appliquez une [!DNL Anaplan] allocation d’un budget à un [!DNL Adobe Workfront] project
description: Ce scénario d’intégration synchronise toutes les allocations budgétaires qui ont été effectuées dans [!DNL Anaplan] Retour à [!DNL Workfront]. Le scénario récupère tous les éléments de budget de l’opération liés, puis transmet la valeur budgétaire au projet Workfront lié si la valeur du budget a été modifiée.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Appliquez une [!DNL Anaplan] allocation d’un budget à un [!DNL Adobe Workfront] project

Ce scénario d’intégration synchronise toutes les allocations budgétaires qui ont été effectuées dans [!DNL Anaplan] Retour à [!DNL Workfront]. Le scénario récupère tous les éléments de budget de l’opération liés, puis transmet la valeur budget à l’élément lié. [!DNL Workfront] project si la valeur du budget a été modifiée.

>[!IMPORTANT]
>
>Dans cet article, &quot;Campaign&quot; fait référence au cas d’utilisation de la campagne marketing que ce scénario représente et n’est en aucun cas connecté à la variable [!DNL Workfront Fusion] Connecteur Adobe Campaign ou vers le connecteur récemment obsolète [!UICONTROL Campagne] dans [!DNL Workfront].

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
   <td> <p>[!UICONTROL Fusion Workfront pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

&#42;&#42;Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Événement de déclenchement

Ce scénario est planifié pour s’exécuter toutes les 15 minutes.

## Valeur attendue [!DNL Workfront] Configuration

Vous devez avoir les éléments suivants dans [!DNL Workfront] pour utiliser ce scénario :

* Un profil utilisateur dans [!DNL Workfront] named **Intégration Anaplan**, qui dispose des droits d’administrateur système.

   Pour plus d’informations sur la création d’un utilisateur dans [!DNL Workfront], voir [Ajout d’utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Valeur attendue [!DNL Anaplan] Configuration

Vous devez avoir les éléments suivants dans [!DNL Anaplan] pour utiliser ce scénario :

* Un profil utilisateur dans [!DNL Anaplan] named **[!DNL Workfront]Intégration**, qui dispose des droits d’administrateur système.
* Le [!DNL Anaplan] Modèle que vous souhaitez utiliser pour ce scénario.
* La liste dans la variable [!DNL Anaplan] Modèle qui capture les budgets de campagne.

   Le module de la liste doit prendre en charge la réception des attributs suivants :

   * [!UICONTROL GUID de projet Workfront]
   * [!UICONTROL Nom de la campagne]
   * [!UICONTROL Fonds de main-d&#39;oeuvre requis]
   * [!UICONTROL Recettes estimées]
   * [!UICONTROL Marque]

   Cette liste et ce module doivent stocker les détails supplémentaires nécessaires au bon fonctionnement de la fonction [!DNL Anaplan], y compris la possibilité de définir un budget et de signaler que l’élément de liste des budgets est prêt à être resynchronisé sur [!DNL Workfront].

* Une vue dans [!DNL Anaplan] named **[!UICONTROL Campagnes.Mettre à jour les campagnes dans Adobe Workfront]**.

   Cette vue doit contenir les colonnes suivantes, dans cet ordre :

   1. [!UICONTROL Nom de l’élément]

   2. [!UICONTROL [!DNL Workfront] GUID du projet]

   3. [!UICONTROL Nom de la campagne]

   4. [!UICONTROL Budget]

   5. [!UICONTROL Recettes estimées]

   6. [!UICONTROL Marque]
   La vue doit être filtrée pour afficher les éléments qui ont une [!UICONTROL [!DNL Workfront] GUID du projet] et certains indicateurs selon lesquels les allocations budgétaires doivent être transmises à [!DNL Workfront].

Pour obtenir des instructions sur l’une de ces actions, voir [!DNL Anaplan] documentation.

## Déploiement sur [!DNL Workfront Fusion]

Procédez comme suit pour déployer ce scénario d’intégration dans votre [!DNL Fusion] compte . Cette opération ne doit être effectuée qu’après avoir terminé les [!DNL Workfront] et [!DNL Anaplan] configuration.

1. Accédez au [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur le bouton **[!UICONTROL Appliquer [!DNL Anaplan] allocations budgétaires pour les projets Workfront]** modèle de scénario.
1. Remplacez les valeurs de variable pour les éléments suivants : [!DNL Anaplan] variables :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Nom de variable</th> 
      <th>Remplacer la valeur par</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID de l’espace de travail]</td> 
      <td>L’identifiant d’un espace de travail de votre [!DNL Anaplan] compte .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID de modèle] </td> 
      <td>L’identifiant d’un modèle de votre [!DNL Anaplan] et l’espace de travail sélectionné.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nom du module]</td> 
      <td>Nom du module qui décrit les attributs de campagne dans le [!DNL Anaplan] Liste.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Le nom de la liste de votre [!DNL Anaplan] et l’espace de travail et le modèle sélectionnés.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nom de la vue]</td> 
      <td> <p>Nom de la vue qui contient les budgets de campagne prêts à être transmis à [!DNL Workfront].</p> <p>(Exemple : [!UICONTROL Campagnes.Charger des campagnes dans [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Vous trouverez des informations détaillées sur la configuration des fichiers et des processus dans la section [!DNL Anaplan] documentation de configuration.

1. Sélectionnez ou ajoutez une [!DNL Anaplan] profil de connexion.
1. Mettre à jour tout le reste [!DNL Anaplan] modules avec un [!DNL Anaplan] connexion, lorsque vous y êtes invité.
1. Sur le **[!UICONTROL Conversion de CSV en module d’objet JSON]**, ajoutez une nouvelle structure de données pour mapper les colonnes CSV à un objet JSON utilisable.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Lorsque vous y êtes invité, sélectionnez cette structure de données pour les autres modules du déploiement de ce scénario.
1. Sur le **[!UICONTROL Vérifier le projet lié]** , sélectionnez ou ajoutez un [!DNL Workfront] profil de connexion.
1. Mettre à jour tout le reste [!DNL Workfront] modules avec un [!DNL Workfront] connexion, lorsque vous y êtes invité.

## Autres modèles de scénario recommandés

Pour terminer le workflow représenté par ce modèle, vous devez également déployer le modèle supplémentaire suivant :

* [[!UICONTROL Créez un [!DNL Anaplan] élément d’une liste à partir d’un [!DNL Adobe Workfront] requête budget]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Voici d’autres scénarios d’optimisation des dépenses :

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] mises à jour de projet à une [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] mises à jour des heures réelles à une [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] dépenses d’un [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
