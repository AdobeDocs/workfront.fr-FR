---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Envoyer [!DNL Adobe Workfront] mises à jour de projet à une [!DNL Anaplan] élément de liste
description: Ce scénario d’intégration partage la progression, l’état et les détails de planification clés d’une [!DNL Adobe Workfront] avec un projet [!DNL Anaplan] élément de liste des budgets. Le partage de ces informations vous permet de tirer le meilleur parti de l’optimisation des dépenses et de l’analyse financière qui permet [!DNL Anaplan] fournit.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 2%

---

# Envoyer [!DNL Adobe Workfront] mises à jour de projet à une [!DNL Anaplan] élément de liste

Ce scénario d’intégration partage la progression, l’état et les détails de planification clés d’une [!DNL Adobe Workfront] avec un projet [!DNL Anaplan] élément de liste des budgets. Le partage de ces informations vous permet de tirer le meilleur parti de l’optimisation des dépenses et de l’analyse financière qui permet [!DNL Anaplan] fournit.

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

* Un profil utilisateur dans [!DNL Workfront] named **[!UICONTROL [!DNL Anaplan]Intégration]**, qui dispose des droits d’administrateur système.

   Pour plus d’informations sur la création d’un utilisateur dans [!DNL Workfront], voir [Ajout d’utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL résumé de campagne]** formulaire personnalisé joint à l’objet de projet pour stocker les valeurs de données personnalisées que vous choisissez d’envoyer à Anaplan.

   Les champs suivants représentent des exemples de champs qui peuvent être inclus dans le formulaire personnalisé pour faciliter le mappage des données vers Anaplan, mais ils ne sont pas nécessaires pour ce scénario d’intégration :

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Nom de champ</th> 
     <th>Type de champ</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL À La Date De Début Du Marché]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL À La Date De Fin Du Marché]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Présentation de Campaign]</td> 
     <td>[!UICONTROL Champ de texte de paragraphe]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Message de clé]</td> 
     <td>[!UICONTROL Champ de texte de paragraphe]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Audience Target]</td> 
     <td> <p>[!UICONTROL Liste déroulante]</p> <p>Incluez des options qui correspondent à vos processus.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Valeur attendue [!DNL Anaplan] Configuration

Vous devez avoir les éléments suivants dans [!DNL Anaplan] pour utiliser ce scénario :

* Un profil utilisateur dans [!DNL Anaplan] named **[!UICONTROL [!DNL Workfront]Intégration]**, qui dispose des droits d’administrateur système.
* Le [!DNL Anaplan] Modèle que vous souhaitez utiliser pour ce scénario.
* La liste dans la variable [!DNL Anaplan] Modèle que vous souhaitez utiliser pour ce scénario.
* A **[!UICONTROL Importation de mise à jour de projet]** qui contient les colonnes suivantes, dans cet ordre :

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] GUID du projet]

3. [!UICONTROL Nom de la campagne]

4. [!UICONTROL Pourcentage d&#39;achèvement]

5. [!UICONTROL Date de début prévue]

6. [!UICONTROL Date d&#39;achèvement prévue]

7. [!UICONTROL Heures prévues]

8. [!UICONTROL Coûts prévus]

9. [!UICONTROL Montant de charge prévu]

10. [!UICONTROL Coût réel de main-d&#39;œuvre]

11. [!UICONTROL Coût prévu de la main-d&#39;œuvre]

12. [!UICONTROL Statut]

Pour préparer la [!UICONTROL [!DNL Anaplan] Importation des dépenses planifiée] fichier :

1. Copiez et collez les éléments suivants dans un éditeur de texte ou [!DNL Excel]
1. Enregistrement du fichier au format CSV
1. Téléchargez le fichier dans Anaplan.

   Pour obtenir des instructions, voir [!DNL Anaplan] documentation sur l’importation de données dans des modules à partir d’un fichier.

1. Notez le nom que vous avez donné au fichier ; il sera utilisé pendant le déploiement de la fonction [!UICONTROL Fusion] modèle de scénario.

Exemple de contenu CSV

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

1. [!UICONTROL Présentation de la campagne]

2. [!UICONTROL Message clé]

3. [!UICONTROL Date de début du marché]

4. [!UICONTROL Date de fin du marché]

5. [!UICONTROL Public cible]

Incluez également tous les autres champs que vous souhaitez définir dans le mappage.

* A **[!UICONTROL Importation de mise à jour de projet]** processus préparé pour exécuter l’importation des données livrées dans un téléchargement de fichier.

Pour obtenir des instructions sur l’une de ces actions, voir [!DNL Anaplan] documentation.

## Déploiement sur [!DNL Workfront Fusion]

Effectuez les étapes suivantes pour déployer ce scénario d’intégration sur votre compte Fusion. Cette opération ne doit être effectuée qu’après avoir terminé les [!DNL Workfront] et [!DNL Anaplan] configuration.

1. Accédez au [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur le bouton **[!UICONTROL Envoi des mises à jour de projet Workfront à [!DNL Anaplan] élément de liste]** modèle de scénario.
1. Remplacez les valeurs de variable pour les éléments suivants : [!DNL Anaplan] variables :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
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
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>Le nom de la liste de votre [!DNL Anaplan] et l’espace de travail et le modèle sélectionnés.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom de fichier [!UICONTROL : Importation de mise à jour de projet]</td> 
      <td>Nom du fichier qui recevra les données de mise à jour du projet.<p>(Exemple : WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom du processus [!UICONTROL : Importation de mise à jour de projet]</td> 
      <td> <p>Nom du processus qui exécutera l’importation des données du projet.</p> <p>(Exemple : WF Int - Mettre à jour les détails d’une campagne)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomain]</td> 
      <td>Le sous-domaine de votre [!DNL Workfront] compte . Elle sert à créer un lien vers votre [!DNL Workfront] dans une note qui peut être générée.</td> 
     </tr> 
    </tbody> 
   </table>

   Vous trouverez des informations détaillées sur la configuration des fichiers et des processus dans la section [!DNL Anaplan] documentation de configuration.

1. Sélectionnez ou ajoutez une [!DNL Anaplan] profil de connexion.
1. Mettre à jour tout le reste [!DNL Anaplan] modules avec un [!DNL Anaplan] connexion, lorsque vous y êtes invité.
1. Sélectionnez ou ajoutez une [!DNL Workfront] profil de connexion.

   Le filtre est configuré pour extraire tous les projets liés incomplets et ceux qui ont été terminés au cours des 29 dernières minutes. Si vous modifiez la fréquence de la variable [!DNL Fusion] vous souhaitez mettre à jour cette valeur une fois que le modèle de scénario a été déployé.

1. Sur le **[!UICONTROL Création de projets Mise à jour de CSV]** , ajoutez une nouvelle structure de données pour mapper les attributs de projet aux colonnes CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Mettre à jour tout le reste [!DNL Workfront] modules avec un [!DNL Workfront] connexion, lorsque vous y êtes invité.

## Autres modèles de scénario recommandés

Ce modèle de scénario est complété par les modèles de scénario d’optimisation des dépenses suivants qui peuvent également être déployés :

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] mises à jour des heures réelles à une [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer [!DNL Adobe Workfront] dépenses d’un [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Scénarios supplémentaires pour lier les requêtes de budget :

* [[!UICONTROL Créez un [!DNL Anaplan] élément d’une liste à partir d’un [!DNL Adobe Workfront] requête budget]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Appliquez une [!DNL Anaplan] allocation d’un budget à un [!DNL Adobe Workfront] project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Scénarios supplémentaires pour lier des requêtes de campagne :

* [[!UICONTROL Créez un [!DNL Anaplan] élément d’une liste à partir d’un [!DNL Adobe Workfront] requête de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Appliquez une [!DNL Anaplan] allocation d’un budget à un [!DNL Adobe Workfront] requête de campagne ou projet de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
