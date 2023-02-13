---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Envoyer [!DNL Adobe Workfront] dépenses d’un [!DNL Anaplan] élément de liste
description: Ce scénario d’intégration partage les détails relatifs aux dépenses d’une [!DNL Adobe Workfront] avec un projet [!DNL Anaplan] élément de liste des budgets. Le partage de ces informations vous permet de tirer le meilleur parti de l’optimisation des dépenses et de l’analyse financière qui permet [!DNL Anaplan] fournit.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# Envoyer [!DNL Adobe Workfront] dépenses d’un [!DNL Anaplan] élément de liste

Ce scénario d’intégration partage les détails relatifs aux dépenses d’une [!DNL Adobe Workfront] avec un projet [!DNL Anaplan] élément de liste des budgets. Le partage de ces informations vous permet de tirer le meilleur parti de l’optimisation des dépenses et de l’analyse financière qui permet [!DNL Anaplan] fournit.

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
   <td> <p>Workfront Fusion pour l’automatisation et l’intégration du travail </p> </td> 
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

* Un profil utilisateur dans [!DNL Workfront] named *[!UICONTROL *[!DNL Anaplan] Intégration]**, qui dispose des droits d’administrateur système.

   Pour plus d’informations sur la création d’un utilisateur dans [!DNL Workfront], voir [Ajout d’utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL résumé de campagne]** formulaire personnalisé associé à l’objet de projet pour stocker les valeurs de données personnalisées que vous choisissez d’envoyer à [!DNL Anaplan].

   Le formulaire doit contenir les champs suivants :

   | Nom de champ | Type de champ |
   |---|---|
   | [!UICONTROL Date de dernière transmission] | Date |
   | [!UICONTROL Notes d’intégration] | Zone de texte |

   Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Valeur attendue [!DNL Anaplan] Configuration

Vous devez avoir les éléments suivants dans [!DNL Anaplan] pour utiliser ce scénario :

* Un profil utilisateur dans [!DNL Anaplan] named **[!UICONTROL [!DNL Workfront ]Intégration]**, qui dispose des droits d’administrateur système.
* Le [!DNL Anaplan] Modèle que vous souhaitez utiliser pour ce scénario.
* La liste dans la variable [!DNL Anaplan] Modèle qui permet de capturer les budgets de campagne.
* Un **[!UICONTROL Importation des dépenses réelles d’un plan]** qui contient les colonnes suivantes, dans cet ordre :

   1. [!UICONTROL [!DNL Workfront] GUID de dépense]

   2. [!UICONTROL [!DNL Workfront] GUID du projet]

   3. [!UICONTROL Montant réel]

   4. [!UICONTROL Description]

   5. [!UICONTROL Type de frais]

   6. [!UICONTROL Date d’entrée en vigueur]

   7. [!UICONTROL Nom de la campagne]

   8. [!UICONTROL [!DNL Anaplan] ID d’élément de liste]
   Pour préparer la [!UICONTROL [!DNL Anaplan] Importation des dépenses réelles] fichier :

   1. Copiez et collez les éléments suivants dans un éditeur de texte ou [!DNL Excel].
   1. Enregistrez le fichier au format CSV.
   1. Chargement du fichier dans [!DNL Anaplan].

      Pour obtenir des instructions, voir [!DNL Anaplan] documentation sur l’importation de données dans des modules à partir d’un fichier.

   1. Notez le nom que vous avez donné au fichier ; il sera utilisé pendant le déploiement de la fonction [!UICONTROL Fusion] modèle de scénario.

   Exemple de contenu CSV

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* Un **[!UICONTROL [!DNL Anaplan]Importation des dépenses planifiée]** qui contient les colonnes suivantes, dans cet ordre :

   1. [!UICONTROL [!DNL Workfront] GUID de dépense]

   2. [!UICONTROL [!DNL Workfront] GUID du projet]

   3. [!UICONTROL Montant réel]

   4. [!UICONTROL Description]

   5. [!UICONTROL Type de frais]

   6. [!UICONTROL Date d’entrée en vigueur]

   7. [!UICONTROL Nom de la campagne]

   8. [!UICONTROL [!DNL Anaplan] ID d’élément de liste]
   Pour préparer la [!UICONTROL [!DNL Anaplan] Importation des dépenses planifiée] fichier :

   1. Copiez et collez les éléments suivants dans un éditeur de texte ou [!DNL Excel]
   1. Enregistrement du fichier au format CSV
   1. Téléchargez le fichier dans Anaplan.

      Pour obtenir des instructions, voir [!DNL Anaplan] documentation sur l’importation de données dans des modules à partir d’un fichier.

   1. Notez le nom que vous avez donné au fichier ; il sera utilisé pendant le déploiement de la fonction [!UICONTROL Fusion] modèle de scénario.

   Exemple de contenu CSV

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>


* A **[!UICONTROL Importation de mise à jour de projet]** processus préparé pour exécuter l’importation des données livrées dans un téléchargement de fichier.

>[!NOTE]
>
>Il existe des fichiers d&#39;import distincts pour les dépenses prévues et réelles afin qu&#39;elles puissent être rapportées indépendamment respectivement au cours des dates prévues et en vigueur.

Pour obtenir des instructions sur l’une de ces actions, voir [!DNL Anaplan] documentation.

## Déploiement sur [!DNL Fusion]

Procédez comme suit pour déployer ce scénario d’intégration dans votre [!DNL Fusion] compte . Cette opération ne doit être effectuée qu’après avoir terminé les [!DNL Workfront] et [!DNL Anaplan] configuration.

1. Accédez au [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur le bouton **[!UICONTROL Envoyer les mises à jour des dépenses Workfront à [!DNL Anaplan] élément de liste]** modèle de scénario.
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
      <td>L’identifiant de l’espace de travail de votre [!DNL Anaplan] compte que vous souhaitez utiliser pour ce scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID de modèle] </td> 
      <td>L’identifiant du modèle de votre [!DNL Anaplan] et l’espace de travail sélectionné que vous souhaitez utiliser pour ce scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Le nom de la liste de votre [!DNL Anaplan] compte et l’espace de travail et le modèle sélectionnés que vous souhaitez utiliser pour ce scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom de fichier [!UICONTROL : Importation des dépenses réelles]</td> 
      <td> <p>Nom du fichier qui recevra les données de dépenses réelles du projet.</p> <p> (Exemple : WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom de fichier [!UICONTROL : Importation des dépenses planifiée]</td> 
      <td> <p>Nom du fichier qui recevra les données de dépenses planifiées du projet.</p> <p> (Exemple : WorkfrontUpdateLinkedProjects_ScheduleExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom du processus [!UICONTROL : Importation de mise à jour de projet]</td> 
      <td> <p>Nom du processus qui exécutera l’importation des données de dépenses du projet.</p> <p>(Exemple : WF Int - Charger les dépenses du projet)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Vous trouverez des informations détaillées sur la configuration des fichiers et des processus dans la section [!DNL Anaplan] documentation de configuration.

1. Sélectionnez ou ajoutez une [!DNL Anaplan] profil de connexion.
1. Mettre à jour tout le reste [!DNL Anaplan] modules avec un [!DNL Anaplan] connexion, lorsque vous y êtes invité.
1. Sélectionnez ou ajoutez une [!DNL Workfront] profil de connexion.
1. Mettre à jour tout le reste [!DNL Workfront] modules avec un [!DNL Workfront] connexion, lorsque vous y êtes invité.
1. Sur le **[!UICONTROL Créer une dépense réelle CSV]** , ajoutez une nouvelle structure de données pour mapper les attributs de projet aux colonnes CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Sur le **[!UICONTROL Créer un fichier CSV de dépenses prévues]** , ajoutez une nouvelle structure de données pour mapper les attributs de projet aux colonnes CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

## Autres modèles de scénario recommandés

Ce modèle de scénario est complété par les modèles de scénario d’optimisation des dépenses suivants qui peuvent également être déployés :

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] mises à jour de projet à une [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer [!DNL Adobe Workfront] mises à jour des heures réelles à une [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Scénarios supplémentaires pour lier les requêtes de budget :

* [[!UICONTROL Créez un [!DNL Anaplan] élément d’une liste à partir d’un [!DNL Adobe Workfront] requête budget]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Appliquez une [!DNL Anaplan] allocation d’un budget à un [!DNL Adobe Workfront] project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scénarios supplémentaires pour lier des requêtes de campagne :

* [[!UICONTROL Créez un [!DNL Anaplan] élément d’une liste à partir d’un [!DNL Adobe Workfront] requête de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Appliquez une [!DNL Anaplan] allocation d’un budget à un [!DNL Adobe Workfront] requête de campagne ou projet de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
