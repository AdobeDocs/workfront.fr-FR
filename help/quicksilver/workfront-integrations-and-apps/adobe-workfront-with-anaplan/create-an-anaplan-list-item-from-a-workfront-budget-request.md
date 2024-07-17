---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Créer un élément de liste  [!DNL Anaplan]  à partir d’une demande de budget  [!DNL Adobe Workfront]
description: Ce scénario d’intégration associe un projet  [!DNL Adobe Workfront] (campagne) à un élément  [!DNL Anaplan] de liste de budgets. Pour ce faire, ajoutez une requête de budget au projet  [!DNL Workfront] qui doit recevoir un financement. Ce scénario recherche les demandes de budget non traitées, puis exécute un processus pour créer un élément de liste de budget vide dans  [!DNL Anaplan] afin de lancer les processus d’allocation de budget dans Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 6%

---

# Créer un élément de liste [!DNL Anaplan] à partir d’une requête de budget [!DNL Adobe Workfront]

Ce scénario d’intégration associe un projet [!DNL Adobe Workfront] (campagne) à un élément de liste budgétaire [!DNL Anaplan]. Pour ce faire, ajoutez une demande de budget au projet [!DNL Workfront] qui doit recevoir un financement. Ce scénario recherche les demandes de budget non traitées, puis exécute un processus pour créer un élément de liste de budget vide dans [!DNL Anaplan] afin de lancer les processus d&#39;allocation de budget dans [!DNL Anaplan].

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
   <td role="rowheader" [!DNL>Licence Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL Fusion Workfront pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr>
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

&#42;&#42; Pour plus d’informations sur les [!DNL  Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Événement de déclenchement

Ce scénario est planifié pour s’exécuter toutes les 15 minutes.

## Configuration [!DNL Workfront] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Workfront] :

* Un profil utilisateur de [!DNL Workfront] nommé *[!UICONTROL *[!DNL Anaplan] Integration]**, disposant des droits d’administrateur système.

  Pour plus d&#39;informations sur la création d&#39;un utilisateur dans [!DNL Workfront], voir [Ajout d&#39;utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Un formulaire personnalisé **[!UICONTROL Demande de budget]** joint à l’objet [!UICONTROL Demande].

  Les champs obligatoires suivants doivent être inclus dans le formulaire personnalisé pour faciliter le mappage des données vers [!DNL Anaplan] :

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
     <td> <p>[!UICONTROL Liste déroulante]</p> <p>Options :</p> 
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

  Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer ou modifier un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Modèles de projet représentant les campagnes et autres projets nécessitant un financement, configurés avec une rubrique de file d’attente [!UICONTROL Demande de budget]. La rubrique de file d’attente [!UICONTROL Requête budgétaire] est affectée à l’utilisation du formulaire personnalisé [!UICONTROL Requête budgétaire].
* Formulaire **[!UICONTROL résumé de campagne]** pour l’objet de projet.

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

  Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer ou modifier un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Configuration [!DNL Anaplan] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Anaplan] :

* Un profil utilisateur dans [!DNL Anaplan] nommé **[!UICONTROL [!DNL Workfront]Integration]**, disposant des droits d’administrateur système.
* Le modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* Liste du modèle [!DNL Anaplan] qui capture les budgets de campagne.

  Le module de la liste doit prendre en charge la réception des attributs suivants :

   * [!UICONTROL GUID de projet Workfront]
   * [!UICONTROL Nom de la campagne]
   * [!UICONTROL Fonds de main-d’oeuvre requis]
   * [!UICONTROL Fonds de dépenses requis]
   * [!UICONTROL Type de requête de budget]
   * [!UICONTROL Raison de l’ajustement du financement]

  Cette liste et ce module doivent stocker les détails supplémentaires nécessaires à la fonctionnalité normale de [!DNL Anaplan], y compris la possibilité de définir un budget et de signaler que l&#39;élément de liste de budget est prêt à être resynchronisé sur [!DNL Workfront].

Pour obtenir des instructions sur l’une de ces actions, consultez la documentation [!DNL Anaplan].

## Déploiement sur [!DNL Workfront Fusion]

Effectuez les étapes suivantes pour déployer ce scénario d’intégration sur votre compte [!DNL Fusion]. Cette opération ne doit être effectuée qu’après avoir terminé la configuration [!DNL Workfront] et [!DNL Anaplan] requise.

1. Accédez au menu [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur l’élément de liste **[!UICONTROL [!DNL Anaplan] d’un modèle de requête de budget Workfront]** .
1. Remplacez les valeurs de variable pour les variables [!DNL Anaplan] suivantes :

   | Nom de variable | Remplacer la valeur par |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | L’identifiant d’un espace de travail de votre compte [!DNL Anaplan]. |
   | [!UICONTROL [!DNL Anaplan] ID de modèle] | L’identifiant d’un modèle de votre compte [!DNL Anaplan] et l’espace de travail sélectionné. |
   | [!UICONTROL [!DNL Anaplan] Nom du module ] | Nom du module qui décrit les attributs de campagne dans la liste sélectionnée [!DNL Anaplan]. |
   | [!UICONTROL Nom de liste de campagnes] | Nom de la liste de votre compte [!DNL Anaplan] et de l’espace de travail et du modèle sélectionnés. |

   {style="table-layout:auto"}

   Vous trouverez des détails sur la configuration des fichiers et des processus dans la documentation de configuration de [!DNL Anaplan].

1. Sélectionnez ou ajoutez un profil de connexion [!DNL Anaplan].
1. Mettez à jour tous les modules [!DNL Anaplan] restants avec une connexion [!DNL Anaplan] lorsque vous y êtes invité.
1. Sélectionnez ou ajoutez un profil de connexion [!DNL Workfront].

   Après le déploiement du modèle, il s’agit du module que vous allez mettre à jour pour ajouter ou supprimer des références de champ personnalisées de la valeur de la propriété fields si vous souhaitez modifier les champs mappés par défaut sur [!DNL Anaplan].

1. Mettez à jour tous les modules [!DNL Workfront] restants avec une connexion [!DNL Workfront] lorsque vous y êtes invité.

## Autres modèles de scénario recommandés

Pour terminer le workflow représenté par ce modèle, vous devez également déployer le modèle supplémentaire suivant :

* [[!UICONTROL  Appliquez une  [!DNL Anaplan] allocation budgétaire à un [!DNL Adobe Workfront] projet]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Voici d’autres scénarios d’optimisation des dépenses :

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] des mises à jour de projet à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer [!DNL Adobe Workfront] des mises à jour en heures réelles à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyez [!DNL Adobe Workfront] des dépenses à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
