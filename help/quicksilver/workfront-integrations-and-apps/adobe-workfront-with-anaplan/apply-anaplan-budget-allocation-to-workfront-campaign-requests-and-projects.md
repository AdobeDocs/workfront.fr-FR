---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Appliquer une affectation de budget  [!DNL Anaplan]  à une demande de campagne ou un projet de campagne  [!DNL Adobe Workfront] '
description: Ce scénario d’intégration synchronise toutes les attributions budgétaires effectuées dans  [!DNL Anaplan]  avec  [!DNL Workfront]. Le scénario extrait tous les postes budgétaires de campagne liés, puis transmet la valeur budgétée au projet Workfront lié si la valeur du budget a été modifiée.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 99%

---

# Appliquer une affectation de budget [!DNL Anaplan] à une demande de campagne ou un projet de campagne [!DNL Adobe Workfront]

Ce scénario d’intégration synchronise toutes les attributions budgétaires effectuées dans [!DNL Anaplan] avec [!DNL Workfront]. Le scénario extrait tous les postes budgétaires de campagne liés, puis transmet la valeur budgétée au projet [!DNL Workfront] lié si la valeur du budget a été modifiée.

>[!IMPORTANT]
>
>Dans cet article, le terme « campagne » fait référence au cas d’utilisation de la campagne marketing que ce scénario représente, et n’est en aucun cas lié au connecteur Adobe Campaign [!DNL Workfront Fusion] ou à l’objet [!UICONTROL Campaign] de [!DNL Workfront], qui a récemment été supprimé.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package de workflow Adobe Workfront et tout package d’automatisation et d’intégration Adobe Workfront</p><p>Workfront Ultimate</p><p>Packages Workfront Prime et Select, avec l’achat supplémentaire de Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licences Adobe Workfront</td> 
   <td> <p>Standard</p><p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront Fusion</td> 
   <td>
   <p>Basé sur les opérations : aucune exigence de licence Workfront Fusion</p>
   <p>Basé sur un connecteur (hérité) : Workfront Fusion pour l’automatisation et l’intégration du travail </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Si votre organisation dispose d’un package Workfront Select ou Prime qui n’inclut pas l’automatisation et l’intégration de Workfront, elle doit acquérir Adobe Workfront Fusion.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, consultez [Conditions d’accès requises dans la documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences Adobe Workfront Fusion, consultez [Licences Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Événement de déclenchement

Ce scénario est planifié pour s’exécuter toutes les 15 minutes.

## Configuration [!DNL Workfront] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Workfront] :

* Un profil d’utilisation dans [!DNL Workfront] nommé **[!DNL Anaplan Integration]**, qui dispose des droits d’administration du système.

  Pour plus d’informations sur la création d’un utilisateur ou d’une utilisatrice dans [!DNL Workfront], voir [Ajouter des utilisateurs ou des utilisatrices](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configuration [!DNL Anaplan] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Anaplan] :

* Profil d’utilisateur ou d’utilisatrice dans [!DNL Anaplan] nommé Intégration **[!UICONTROL [!DNL Workfront]]**, disposant de droits d’administration système.
* Modèle [!DNL Anaplan] à utiliser pour ce scénario.
* Liste dans le modèle [!DNL Anaplan] qui capture les budgets de campagne.

  Le module de la liste doit permettre de recevoir les attributs suivants :

   * GUID de demande [!UICONTROL [!DNL Workfront]]
   * GUID du projet [!UICONTROL [!DNL Workfront]]
   * [!UICONTROL Nom de la campagne]
   * [!UICONTROL Fonds demandés pour la main-d’œuvre]
   * [!UICONTROL Revenus estimés]
   * [!UICONTROL Marque]

  Cette liste et ce module doivent stocker les détails supplémentaires nécessaires au bon fonctionnement de [!DNL Anaplan], notamment la possibilité de définir un budget et de signaler que l’élément de liste budgétaire est prêt à être resynchronisé sur [!DNL Workfront].

* Une vue dans [!DNL Anaplan] appelée **[!UICONTROL Campagnes Campaigns.Update dans Adobe Workfront]**.

  Cette vue doit contenir les colonnes suivantes, dans cet ordre :

   1. [!UICONTROL Nom de l’élément]

   2. [!UICONTROL [!DNL Workfront]GUID de demande]

   3. GUID du projet [!UICONTROL [!DNL Workfront]]

   4. [!UICONTROL Nom de la campagne]

   5. [!UICONTROL Budget]

   6. [!UICONTROL Revenus estimés]

   7. [!UICONTROL Marque]

  La vue doit être filtrée pour afficher les éléments qui ont un GUID du projet [!UICONTROL [!DNL Workfront]] et un indicateur que les affectations budgétaires doivent être transmises à Workfront.

Pour obtenir des instructions sur l’une de ces actions, consultez la documentation [!DNL Anaplan].

## Déployer vers Workfront Fusion

Pour déployer ce scénario d’intégration dans votre compte Fusion, procédez comme suit. Cette opération ne doit être effectuée qu’après avoir terminé les configurations requises de [!DNL Workfront] et [!DNL Anaplan].

1. Accédez au menu des [!UICONTROL modèles] dans [!DNL Workfront Fusion] et cliquez sur le modèle de scénario **[!UICONTROL Appliquer les affectations budgétaires [!DNL Anaplan] aux demandes de campagne et aux projets Workfront]**.
1. Remplacez les valeurs des variables [!DNL Anaplan] suivantes :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Nom de la variable</th> 
      <th>Remplacer la valeur par</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>ID d’un espace de travail de votre compte [!DNL Anaplan].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model ID] </td> 
      <td>ID d’un modèle de votre compte [!DNL Anaplan] et de l’espace de travail sélectionné.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Le nom de la liste de votre compte [!DNL Anaplan] et l’espace de travail et le modèle sélectionnés.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] View Name]</td> 
      <td> <p>Nom de la vue qui contient les budgets de campagne prêts à être transmis à [!DNL Workfront].</p> <p>(Exemple : [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Vous trouverez des informations détaillées sur la configuration des fichiers et des processus dans la documentation de configuration d’[!DNL Anaplan].

1. Sélectionnez ou ajoutez un profil de connexion [!DNL Anaplan].
1. Mettez à jour tous les modules [!DNL Anaplan] restants avec une connexion [!DNL Anaplan], lorsque l’application vous y invite.
1. Dans le module **[!UICONTROL Convertir les CSV en objet JSON]**, ajoutez une nouvelle structure de données pour convertir les colonnes CSV en un objet JSON utilisable.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Request GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. Lorsque l’on vous y invite, sélectionnez cette structure de données pour les autres modules de ce déploiement de scénarios.
1. Dans le module **[!UICONTROL Vérifier le projet lié]**, sélectionnez ou ajoutez un profil de connexion [!DNL Workfront].
1. Mettez à jour tous les modules [!DNL Workfront] restants avec une connexion [!DNL Workfront], lorsque l’application vous y invite.

## Autres modèles de scénario recommandés

Pour compléter le workflow représenté par ce modèle, vous devez également déployer le modèle supplémentaire suivant :

* [[!UICONTROL Créer un élément de liste  [!DNL Anaplan]  à partir d’une demande de campagne  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

Parmi les autres scénarios d’optimisation des dépenses figurent :

* [[!UICONTROL Envoyer des mises à jour de projet  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyer des mises à jour des heures effectives  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyer des dépenses  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
