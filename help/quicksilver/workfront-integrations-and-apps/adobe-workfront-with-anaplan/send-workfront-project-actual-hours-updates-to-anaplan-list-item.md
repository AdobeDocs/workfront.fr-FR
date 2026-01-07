---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Envoyer les mises à jour des heures effectives [!DNL Adobe Workfront] à un élément de liste [!DNL Anaplan] '
description: Ce scénario d’intégration partage les détails sur les heures effectives capturés dans un projet  [!DNL Adobe Workfront]  avec un élément de liste de budgets  [!DNL Anaplan] . Le partage de ces informations vous permet de tirer le meilleur parti de l’optimisation des dépenses et de l’analyse financière que fournit  [!DNL Anaplan] .
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 99%

---

# Envoyer les mises à jour des heures effectives d’[!DNL Adobe Workfront] à un élément de liste [!DNL Anaplan]

Ce scénario d’intégration partage les détails sur les heures effectives capturés dans un projet [!DNL Adobe Workfront] avec un élément de liste de budgets [!DNL Anaplan]. Le partage de ces informations vous permet de tirer le meilleur parti de l’optimisation des dépenses et de l’analyse financière que fournit [!DNL Anaplan].

Ce modèle de scénario fournit une liste des heures, résumées par projet, jour et rôle, enregistrées sur les projets actifs au cours des 3 derniers mois.

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

Pour plus d’informations sur les licences Adobe Workfront Fusion, consultez [Licences Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Événement de déclenchement

Ce scénario est planifié pour s’exécuter toutes les 15 minutes.

## Configuration [!DNL Workfront] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Workfront] :

* Un profil d’utilisateur ou d’utilisatrice dans [!DNL Workfront] nommé **[!UICONTROL Intégration Anaplan]**, disposant de droits d’administration système.

  Pour plus d’informations sur la création d’un utilisateur ou d’une utilisatrice dans [!DNL Workfront], voir [Ajouter des utilisateurs ou des utilisatrices](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configuration [!DNL Anaplan] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Anaplan] :

* Profil d’utilisateur ou d’utilisatrice dans [!DNL Anaplan] nommé Intégration **[!UICONTROL [!DNL Workfront]]**, disposant de droits d’administration système.
* Modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* La liste dans le modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* Un fichier dans [!DNL Anaplan] nommé **[!UICONTROL Importation des heures effectives Anaplan]** qui contient les colonnes suivantes, dans cet ordre :

   1. [!UICONTROL GUID de projet Workfront]

   2. [!UICONTROL Heures]

   3. [!UICONTROL Coût estimé des heures]

   4. [!UICONTROL Date d’entrée]

   5. [!UICONTROL Nom du rôle]

   6. [!UICONTROL Nom de la campagne]

   7. [!UICONTROL [!DNL Anaplan]ID d’élément de liste]

  Pour préparer le fichier de rapport de dépenses réelles [!DNL Anaplan] :

   1. Copiez et collez les éléments suivants dans un éditeur de texte ou [!DNL Excel].
   1. Enregistrez le fichier au format CSV.
   1. Chargez le fichier dans [!DNL Anaplan].

      Pour obtenir des instructions, consultez la documentation [!DNL Anaplan] sur l’import de données dans des modules provenant d’un fichier.

   1. Notez le nom que vous avez donné au fichier. Il sera utilisé lors du déploiement du modèle de scénario [!UICONTROL Fusion].

  Exemple de contenu CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* Un processus d’**[!UICONTROL importation des heures effectives du projet]**, préparé pour exécuter l’importation des données fournies dans un chargement de fichier.

Pour obtenir des instructions sur l’une ou l’autre de ces actions, voir la documentation d’[!DNL Anaplan].

## Déploiement sur [!DNL Workfront Fusion]

Procédez comme suit pour déployer ce scénario d’intégration dans votre compte [!DNL Fusion]. Cette opération ne doit être effectuée qu’après avoir procédé à la configuration requise de [!DNL Workfront] et [!DNL Anaplan].

1. Accédez au menu [!UICONTROL Modèles] dans [!DNL Workfront Fusion], puis cliquez sur le modèle de scénario **[!UICONTROL Envoyer les mises à jour des heures effectives Workfront à l’élément de liste [!DNL Anaplan]]**.
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
      <td>Le nom de la liste de votre compte [!DNL Anaplan], ainsi que l’espace de travail et le modèle sélectionnés.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Actual Hours Import]</td> 
      <td> <p>Le nom du fichier qui recevra les données sur les heures réelles du projet.</p> <p> (Exemple : WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Actual Hours Import]</td> 
      <td> <p>Le nom du processus qui exécutera l’import des données d’heures du projet.</p> <p>(Exemple : WF Int - Charger les heures du projet par rôle)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomain]</td> 
      <td>Sous-domaine de votre compte [!DNL Workfront]. Il permet de créer un lien vers votre projet [!DNL Workfront] dans une note qui peut être générée.</td> 
     </tr> 
    </tbody> 
   </table>

   Les détails de la configuration des fichiers et des processus sont fournis dans la documentation de configuration d’[!DNL Anaplan].

1. Sélectionnez ou ajoutez un profil de connexion [!DNL Anaplan].
1. Mettez à jour tous les modules [!DNL Anaplan] restants avec une connexion [!DNL Anaplan], lorsque l’on vous y invite.
1. Sélectionnez ou ajoutez un profil de connexion [!DNL Workfront].
1. Mettez à jour tous les modules [!DNL Workfront] restants avec une connexion [!DNL Workfront] lorsque l’on vous invite à le faire.

## Autres modèles de scénario recommandés

Ce modèle de scénario est complété par les modèles de scénario d’optimisation des dépenses suivants qui peuvent également être déployés :

* [[!UICONTROL Envoyer des mises à jour de projet  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer des dépenses  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Scénarios supplémentaires pour lier les demandes de budget :

* [[!UICONTROL Créer un élément de liste  [!DNL Anaplan]  à partir d’une demande de budget  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Appliquer une allocation de budget  [!DNL Anaplan]  à un projet  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scénarios supplémentaires pour lier des demandes de campagne :

* [[!UICONTROL Créer un élément de liste  [!DNL Anaplan]  à partir d’une demande de campagne  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Appliquer une allocation de budget  [!DNL Anaplan]  à une demande ou un projet de campagne  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
