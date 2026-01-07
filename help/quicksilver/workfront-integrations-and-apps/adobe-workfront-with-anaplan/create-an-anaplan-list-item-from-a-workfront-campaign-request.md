---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Créer un élément de liste  [!DNL Anaplan]  à partir d’une requête de campagne  [!DNL Adobe Workfront] '
description: Ce scénario d’intégration relie un projet  [!DNL Adobe Workfront]  à un élément de la liste budgétaire  [!DNL Anaplan] .
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 98%

---

# Créer un élément de liste [!DNL Anaplan] à partir d’une requête de campagne [!DNL Adobe Workfront]

Ce scénario d’intégration relie un projet [!DNL Adobe Workfront] à un élément de liste budgétaire [!DNL Anaplan].

Ce scénario surveille les nouvelles requêtes de campagne ajoutées à une file d’attente des requêtes. Dès qu’une requête de campagne est enregistrée, un élément de la liste budgétaire est ajouté sur [!DNL Anaplan] pour lancer le processus de financement.

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

* Profil d’utilisateur ou d’utilisatrice dans [!DNL Workfront] nommé Intégration **[!UICONTROL [!DNL Anaplan]]**, disposant de droits d’administration système.

  Pour plus d’informations sur la création d’un utilisateur ou d’une utilisatrice dans [!DNL Workfront], voir [Ajouter des utilisateurs et des utilisatrices](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Un formulaire personnalisé **[!UICONTROL Résumé de campagne]** attaché à l’objet [!UICONTROL Requête].

  Les champs obligatoires suivants doivent être inclus dans le formulaire personnalisé afin de faciliter le mappage des données avec Anaplan :

  | Nom du champ | Type de champ |
  |---|---|
  | [!UICONTROL Total des fonds demandés] |   |
  | [!UICONTROL Fonds demandés pour la la main-d’œuvre] |   |
  | [!UICONTROL Fonds demandés pour les dépenses] |   |
  | [!UICONTROL Envoyé à [!DNL Anaplan]] | Case à cocher |

  Les champs facultatifs suivants peuvent être présents dans le formulaire. Ce scénario ne met en correspondance que les champs ci-dessus, mais tous les champs supplémentaires du résumé de campagne peuvent être mappés.

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Nom du champ</th> 
     <th>Type de champ</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market Start Date]</td> 
     <td>Date </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>Date</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>Zone de texte</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>Zone de texte</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>Menu déroulant</p> <p>Inclut des options qui correspondent à vos processus.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Un projet configuré comme une file d’attente des demandes pour capturer les nouvelles demandes de campagne. Le formulaire [!UICONTROL Résumé de campagne] doit être joint à ces requêtes.

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
   * [!UICONTROL Fonds demandés pour les dépenses]
   * [!UICONTROL Type de requête de budget]

  Cette liste et ce module doivent stocker les détails supplémentaires nécessaires au fonctionnement normal d’[!DNL Anaplan], notamment la possibilité de définir un budget et de communiquer que l’élément de la liste budgétaire est prêt à être synchronisé avec [!DNL Workfront].

Pour obtenir des instructions sur l’une de ces actions, voir la documentation [!DNL Anaplan].

## Déploiement sur [!DNL Workfront Fusion]

Procédez comme suit pour déployer ce scénario d’intégration dans votre compte [!DNL Fusion]. Cette opération ne doit être effectuée qu’après avoir procédé à la configuration obligatoire de [!DNL Workfront] et [!DNL Anaplan].

1. Accédez au menu [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur **[!UICONTROL Créer un élément de liste [!DNL Anaplan] à partir d’un modèle de scénario de requête de campagne Workfront]**.
1. Remplacez les valeurs des variables [!DNL Anaplan] suivantes :

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

* [[!UICONTROL Appliquer une allocation de budget  [!DNL Anaplan]  à une requête de campagne  [!DNL Adobe Workfront]  ou à un projet de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

Parmi les autres scénarios d’optimisation des dépenses figurent :

* [[!UICONTROL Envoyer des mises à jour de projet  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] ]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyer des mises à jour des heures effectives  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] ]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyer des dépenses  [!DNL Adobe Workfront]  à un élément de liste  [!DNL Anaplan] ]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
