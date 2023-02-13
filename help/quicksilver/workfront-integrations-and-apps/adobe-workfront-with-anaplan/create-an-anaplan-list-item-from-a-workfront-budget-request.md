---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Créez un [!DNL Anaplan] élément d’une liste à partir d’un [!DNL Adobe Workfront] requête budget
description: Ce scénario d’intégration associe et [!DNL Adobe Workfront] projet (campagne) avec une [!DNL Anaplan] élément de liste des budgets. Pour ce faire, ajoutez une requête de budget à la variable [!DNL Workfront] projet qui doit recevoir un financement. Ce scénario recherche les demandes de budget non traitées, puis exécute un processus pour créer un élément de liste de budget vide dans [!DNL Anaplan] pour lancer les processus d’allocation du budget dans Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 1%

---

# Créez un [!DNL Anaplan] élément d’une liste à partir d’un [!DNL Adobe Workfront] requête budget

Ce scénario d’intégration associe et [!DNL Adobe Workfront] projet (campagne) avec une [!DNL Anaplan] élément de liste des budgets. Pour ce faire, ajoutez une requête de budget à la variable [!DNL Workfront] projet qui doit recevoir un financement. Ce scénario recherche les demandes de budget non traitées, puis exécute un processus pour créer un élément de liste de budget vide dans [!DNL Anaplan] pour lancer les processus d’allocation du budget dans [!DNL Anaplan].

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
   <td role="rowheader" [!DNL>Licence Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL Fusion Workfront pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr>
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

&#42;&#42;Pour plus d’informations sur[!DNL  Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Événement de déclenchement

Ce scénario est planifié pour s’exécuter toutes les 15 minutes.

## Valeur attendue [!DNL Workfront] Configuration

Vous devez avoir les éléments suivants dans [!DNL Workfront] pour utiliser ce scénario :

* Un profil utilisateur dans [!DNL Workfront] named *[!UICONTROL *[!DNL Anaplan] Intégration]**, qui dispose des droits d’administrateur système.

   Pour plus d’informations sur la création d’un utilisateur dans [!DNL Workfront], voir [Ajout d’utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Demande de budget]** formulaire personnalisé joint au [!UICONTROL Requête] .

   Les champs obligatoires suivants doivent être inclus dans le formulaire personnalisé pour faciliter le mappage des données à [!DNL Anaplan]:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>Nom de champ</th> 
     <th>Type de champ</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Type de demande de budget]</td> 
     <td> <p>[!UICONTROL Liste déroulante]</p> <p>Options:</p> 
      <ul> 
       <li> <p>[!UICONTROL Ajustement du financement]</p> </li> 
       <li> <p>[!UICONTROL Financement initial]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Fonds de main-d’oeuvre requis]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Fonds de dépenses demandés]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

   Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Modèles de projet représentant les campagnes et autres projets nécessitant un financement, configurés avec une [!UICONTROL Demande de budget] rubrique de file d’attente. Le [!UICONTROL Demande de budget] la rubrique de file d’attente est affectée à l’utilisation de la variable [!UICONTROL Demande de budget] formulaire personnalisé.
* A **[!UICONTROL résumé de campagne]** formulaire pour l’objet de projet.

   Ce formulaire doit contenir les champs suivants :

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[!UICONTROL Champ de texte enrichi]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Message de clé]</td> 
     <td>[!UICONTROL Champ de texte enrichi]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Audience Target]</td> 
     <td> <p>[!UICONTROL Liste déroulante]</p> <p>Incluez des options qui correspondent à vos processus.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Valeur attendue [!DNL Anaplan] Configuration

Vous devez avoir les éléments suivants dans [!DNL Anaplan] pour utiliser ce scénario :

* Un profil utilisateur dans [!DNL Anaplan] named **[!UICONTROL [!DNL Workfront]Intégration]**, qui dispose des droits d’administrateur système.
* Le [!DNL Anaplan] Modèle que vous souhaitez utiliser pour ce scénario.
* La liste dans la variable [!DNL Anaplan] Modèle qui capture les budgets de campagne.

   Le module de la liste doit prendre en charge la réception des attributs suivants :

   * [!UICONTROL GUID de projet Workfront]
   * [!UICONTROL Nom de la campagne]
   * [!UICONTROL Fonds de main-d&#39;oeuvre requis]
   * [!UICONTROL Fonds de dépenses demandés]
   * [!UICONTROL Type de requête de budget]
   * [!UICONTROL Raison du réglage des fonds]

   Cette liste et ce module doivent stocker les détails supplémentaires nécessaires au bon fonctionnement de la fonction [!DNL Anaplan], y compris la possibilité de définir un budget et de signaler que l’élément de liste des budgets est prêt à être resynchronisé sur [!DNL Workfront].

Pour obtenir des instructions sur l’une de ces actions, voir [!DNL Anaplan] documentation.

## Déploiement sur [!DNL Workfront Fusion]

Procédez comme suit pour déployer ce scénario d’intégration dans votre [!DNL Fusion] compte . Cette opération ne doit être effectuée qu’après avoir terminé les [!DNL Workfront] et [!DNL Anaplan] configuration.

1. Accédez au [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur le bouton **[!UICONTROL Créez un [!DNL Anaplan] élément de liste d’une requête de budget Workfront]** modèle de scénario.
1. Remplacez les valeurs de variable pour les éléments suivants : [!DNL Anaplan] variables :

   | Nom de variable | Remplacer la valeur par |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] ID de l’espace de travail] | L’identifiant d’un espace de travail de votre [!DNL Anaplan] compte . |
   | [!UICONTROL [!DNL Anaplan] ID de modèle] | L’identifiant d’un modèle de votre [!DNL Anaplan] et l’espace de travail sélectionné. |
   | [!UICONTROL [!DNL Anaplan] Nom du module] | Nom du module qui décrit les attributs de campagne dans le [!DNL Anaplan] Liste. |
   | [!UICONTROL Nom de la liste de campagnes] | Le nom de la liste de votre [!DNL Anaplan] et l’espace de travail et le modèle sélectionnés. |

   {style=&quot;table-layout:auto&quot;}

   Vous trouverez des informations détaillées sur la configuration des fichiers et des processus dans la section [!DNL Anaplan] documentation de configuration.

1. Sélectionnez ou ajoutez une [!DNL Anaplan] profil de connexion.
1. Mettre à jour tout le reste [!DNL Anaplan] modules avec un [!DNL Anaplan] connexion, lorsque vous y êtes invité.
1. Sélectionnez ou ajoutez une [!DNL Workfront] profil de connexion.

   Après le déploiement du modèle, il s’agit du module que vous allez mettre à jour pour ajouter ou supprimer des références de champ personnalisées de la valeur de la propriété fields si vous souhaitez modifier les champs mappés par défaut en [!DNL Anaplan].

1. Mettre à jour tout le reste [!DNL Workfront] modules avec un [!DNL Workfront] connexion, lorsque vous y êtes invité.

## Autres modèles de scénario recommandés

Pour terminer le workflow représenté par ce modèle, vous devez également déployer le modèle supplémentaire suivant :

* [[!UICONTROL Appliquez une [!DNL Anaplan] allocation d’un budget à un [!DNL Adobe Workfront] project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Voici d’autres scénarios d’optimisation des dépenses :

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] mises à jour de projet à une [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer [!DNL Adobe Workfront] mises à jour des heures réelles à une [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer [!DNL Adobe Workfront] dépenses d’un [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
