---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Créer un élément de liste  [!DNL Anaplan]  à partir d’une demande de budget  [!DNL Adobe Workfront] '
description: Ce scénario d’intégration associe un projet (campagne)  [!DNL Adobe Workfront]  avec un élément de liste de budget  [!DNL Anaplan] . Pour ce faire, ajoutez une demande de budget au projet  [!DNL Workfront]  qui doit recevoir un financement. Ce scénario recherche les demandes de budget non traitées, puis exécute un processus pour créer un élément de liste de budget vide dans  [!DNL Anaplan]  pour lancer les processus d’attribution de budget dans Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 97%

---

# Créer un élément de liste [!DNL Anaplan] à partir d’une demande de budget [!DNL Adobe Workfront]

Ce scénario d’intégration associe un projet (campagne) [!DNL Adobe Workfront] avec un élément de liste de budget [!DNL Anaplan]. Pour ce faire, ajoutez une demande de budget au projet [!DNL Workfront] qui doit recevoir un financement. Ce scénario recherche les demandes de budget non traitées, puis exécute un processus pour créer un élément de liste de budget vide dans [!DNL Anaplan] pour lancer les processus d’attribution de budget dans [!DNL Anaplan].

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

* Profil d’utilisateur ou d’utilisatrice dans [!DNL Workfront] nommé Intégration **[!DNL Anaplan]**, disposant de droits d’administration système.

  Pour plus d’informations sur la création d’un utilisateur ou d’une utilisatrice dans [!DNL Workfront], voir [Ajouter des utilisateurs et des utilisatrices](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Formulaire personnalisé de **[!UICONTROL demande de budget]** joint à l’objet [!UICONTROL Demande].

  Les champs obligatoires suivants doivent être inclus dans le formulaire personnalisé pour faciliter le mappage des données dans [!DNL Anaplan] :

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>Nom du champ</th> 
     <th>Type de champ</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Budget Request Type]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Options :</p> 
      <ul> 
       <li> <p>[!UICONTROL Adjustment to Funding]</p> </li> 
       <li> <p>[!UICONTROL Initial Funding]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Labor Funds]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Expense Funds]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

  Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Modèles de projet représentant les campagnes et autres projets nécessitant un financement, configurés avec une rubrique de file d’attente [!UICONTROL Demande de budget]. La rubrique de file d’attente [!UICONTROL Demande de budget] est affectée à l’utilisation du formulaire personnalisé [!UICONTROL Demande de budget].
* Formulaire **[!UICONTROL Résumé de campagne]** pour l’objet Projet.

  Ce formulaire doit contenir les champs suivants :

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>Nom du champ</th> 
     <th>Type de champ</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market Start Date]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>[!UICONTROL Rich Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Rich Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Inclut des options qui correspondent à vos processus.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configuration [!DNL Anaplan] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Anaplan] :

* Profil d’utilisateur ou d’utilisatrice dans [!DNL Anaplan] nommé Intégration **[!UICONTROL [!DNL Workfront]]**, disposant de droits d’administration système.
* Modèle [!DNL Anaplan] à utiliser pour ce scénario.
* Liste dans le modèle [!DNL Anaplan] qui capture les budgets de campagne.

  Le module de la liste doit permettre de recevoir les attributs suivants :

   * [!UICONTROL GUID de projet Workfront]
   * [!UICONTROL Nom de la campagne]
   * [!UICONTROL Fonds demandés pour la main-d’œuvre]
   * [!UICONTROL Fonds demandés pour les dépenses]
   * [!UICONTROL Type de demande de budget]
   * [!UICONTROL Raison de l’ajustement des fonds]

  Cette liste et ce module doivent stocker les détails supplémentaires nécessaires au bon fonctionnement d’[!DNL Anaplan], y compris la possibilité de définir un budget et de signaler que l’élément de liste des budgets est prêt à être resynchronisé sur [!DNL Workfront].

Pour obtenir des instructions sur l’une de ces actions, voir la documentation [!DNL Anaplan].

## Déploiement sur [!DNL Workfront Fusion]

Procédez comme suit pour déployer ce scénario d’intégration dans votre compte [!DNL Fusion]. Cette opération ne doit être effectuée qu’après avoir terminé la configuration requise de [!DNL Workfront] et d’[!DNL Anaplan].

1. Accédez au menu [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur le modèle de scénario **[!UICONTROL Créer un élément de liste [!DNL Anaplan] à partir d’une demande de budget Workfront]**.
1. Remplacez les valeurs de variable par les variables [!DNL Anaplan] suivantes :

   | Nom de la variable | Remplacer la valeur par |
   |---|---|
   | ID d’espace de travail [!UICONTROL [!DNL Anaplan]] | ID d’un espace de travail de votre compte [!DNL Anaplan]. |
   | ID de modèle [!UICONTROL [!DNL Anaplan]] | ID d’un modèle de votre compte [!DNL Anaplan] et espace de travail sélectionné. |
   | Nom du module [!UICONTROL [!DNL Anaplan]] | Nom du module qui décrit les attributs de campagne dans la liste [!DNL Anaplan] sélectionnée. |
   | [!UICONTROL Nom de la liste des campagnes] | Nom de la liste de votre compte [!DNL Anaplan] et espace de travail et modèle sélectionnés. |

   {style="table-layout:auto"}

   Vous trouverez des informations détaillées sur la configuration des fichiers et des processus dans la documentation de configuration [!DNL Anaplan].

1. Sélectionnez ou ajoutez un profil de connexion [!DNL Anaplan].
1. Mettez à jour tous les modules [!DNL Anaplan] restants avec une connexion [!DNL Anaplan], lorsque l’on vous y invite.
1. Sélectionnez ou ajoutez un profil de connexion [!DNL Workfront].

   Après le déploiement du modèle, il s’agit du module que vous allez mettre à jour pour ajouter ou supprimer des références de champ personnalisées de la valeur de la propriété fields si vous souhaitez modifier les champs mappés par défaut vers [!DNL Anaplan].

1. Mettez à jour tous les modules [!DNL Workfront] restants avec une connexion [!DNL Workfront], lorsque cela est nécessaire.

## Autres modèles de scénario recommandés

Pour compléter le workflow représenté par ce modèle, vous devez également déployer le modèle supplémentaire suivant :

* [[!UICONTROL Appliquer une attribution de budget  [!DNL Anaplan]  à un projet  [!DNL Adobe Workfront] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Parmi les autres scénarios d’optimisation des dépenses figurent :

* [[!UICONTROL Envoyer des mises à jour de projet  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer des mises à jour des heures effectives  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Envoyer des dépenses  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] &#x200B;]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
