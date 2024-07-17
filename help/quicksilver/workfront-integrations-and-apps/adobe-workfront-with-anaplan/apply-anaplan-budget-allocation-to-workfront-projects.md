---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Appliquer une allocation de budget  [!DNL Anaplan]  à un projet  [!DNL Adobe Workfront]
description: Ce scénario d’intégration synchronise toutes les allocations budgétaires qui ont été effectuées dans  [!DNL Anaplan] vers [!DNL Workfront]. Le scénario récupère tous les éléments de budget de l’opération liés, puis transmet la valeur budgétaire au projet Workfront lié si la valeur du budget a été modifiée.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 7%

---

# Application d’une allocation budgétaire [!DNL Anaplan] à un projet [!DNL Adobe Workfront]

Ce scénario d’intégration synchronise toutes les allocations budgétaires qui ont été effectuées dans [!DNL Anaplan] avec [!DNL Workfront]. Le scénario récupère tous les éléments de budget de campagne liés, puis transmet la valeur budget au projet [!DNL Workfront] lié si la valeur du budget a été modifiée.

>[!IMPORTANT]
>
>&quot;Campaign&quot; dans cet article fait référence au cas d’utilisation de campagne marketing que ce scénario représente et n’est en aucun cas connecté au connecteur Adobe Campaign [!DNL Workfront Fusion] ou à l’objet [!UICONTROL Campaign] récemment obsolète dans [!DNL Workfront].

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td> <p>[!UICONTROL Fusion Workfront pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

&#42;&#42; Pour plus d’informations sur les [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Événement de déclenchement

Ce scénario est planifié pour s’exécuter toutes les 15 minutes.

## Configuration [!DNL Workfront] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Workfront] :

* Un profil utilisateur de [!DNL Workfront] nommé **Intégration Anaplan**, disposant des droits d’administrateur système.

  Pour plus d&#39;informations sur la création d&#39;un utilisateur dans [!DNL Workfront], voir [Ajout d&#39;utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configuration [!DNL Anaplan] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Anaplan] :

* Un profil utilisateur dans [!DNL Anaplan] nommé **[!DNL Workfront]Integration**, disposant des droits d’administrateur système.
* Le modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* Liste du modèle [!DNL Anaplan] qui capture les budgets de campagne.

  Le module de la liste doit prendre en charge la réception des attributs suivants :

   * [!UICONTROL GUID de projet Workfront]
   * [!UICONTROL Nom de la campagne]
   * [!UICONTROL Fonds de main-d’oeuvre requis]
   * [!UICONTROL Recettes estimées]
   * [!UICONTROL Brand]

  Cette liste et ce module doivent stocker les détails supplémentaires nécessaires à la fonctionnalité normale de [!DNL Anaplan], y compris la possibilité de définir un budget et de signaler que l&#39;élément de liste de budget est prêt à être resynchronisé sur [!DNL Workfront].

* Une vue dans [!DNL Anaplan] nommée **[!UICONTROL Campaigns.Update Campaigns dans Adobe Workfront]**.

  Cette vue doit contenir les colonnes suivantes, dans cet ordre :

   1. [!UICONTROL Nom de l’élément]

   2. [!UICONTROL [!DNL Workfront] GUID de projet ]

   3. [!UICONTROL Nom de la campagne]

   4. [!UICONTROL Budget]

   5. [!UICONTROL Recettes estimées]

   6. [!UICONTROL Brand]

  La vue doit être filtrée pour afficher les éléments qui ont un [!UICONTROL [!DNL Workfront] GUID de projet ] et certains indicateurs que les allocations budgétaires doivent être transmises à [!DNL Workfront].

Pour obtenir des instructions sur l’une de ces actions, consultez la documentation [!DNL Anaplan].

## Déploiement sur [!DNL Workfront Fusion]

Effectuez les étapes suivantes pour déployer ce scénario d’intégration sur votre compte [!DNL Fusion]. Cette opération ne doit être effectuée qu’après avoir terminé la configuration [!DNL Workfront] et [!DNL Anaplan] requise.

1. Accédez au menu [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur le modèle de scénario **[!UICONTROL Appliquez [!DNL Anaplan] les allocations budgétaires aux projets Workfront]** .
1. Remplacez les valeurs de variable pour les variables [!DNL Anaplan] suivantes :

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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>L’identifiant d’un espace de travail de votre compte [!DNL Anaplan].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID de modèle] </td> 
      <td>L’identifiant d’un modèle de votre compte [!DNL Anaplan] et l’espace de travail sélectionné.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nom du module]</td> 
      <td>Nom du module qui décrit les attributs de campagne dans la liste sélectionnée [!DNL Anaplan].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Nom de la liste de votre compte [!DNL Anaplan] et de l’espace de travail et du modèle sélectionnés.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nom de la vue]</td> 
      <td> <p>Nom de la vue qui contient les budgets de campagne prêts à être transmis à [!DNL Workfront].</p> <p>(Exemple : [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Vous trouverez des détails sur la configuration des fichiers et des processus dans la documentation de configuration de [!DNL Anaplan].

1. Sélectionnez ou ajoutez un profil de connexion [!DNL Anaplan].
1. Mettez à jour tous les modules [!DNL Anaplan] restants avec une connexion [!DNL Anaplan] lorsque vous y êtes invité.
1. Sur le **[!UICONTROL module Convertir un fichier CSV en objet JSON]**, ajoutez une nouvelle structure de données pour mapper les colonnes CSV à un objet JSON utilisable.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. Lorsque vous y êtes invité, sélectionnez cette structure de données pour les autres modules du déploiement de ce scénario.
1. Sur le module **[!UICONTROL Vérifier le projet lié]** , sélectionnez ou ajoutez un profil de connexion [!DNL Workfront].
1. Mettez à jour tous les modules [!DNL Workfront] restants avec une connexion [!DNL Workfront] lorsque vous y êtes invité.

## Autres modèles de scénario recommandés

Pour terminer le workflow représenté par ce modèle, vous devez également déployer le modèle supplémentaire suivant :

* [[!UICONTROL  Créez un  [!DNL Anaplan] élément de liste à partir d&#39;une  [!DNL Adobe Workfront] requête de budget]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Voici d’autres scénarios d’optimisation des dépenses :

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] des mises à jour de projet à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] des mises à jour en heures réelles à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyez [!DNL Adobe Workfront] des dépenses à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
