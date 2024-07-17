---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Créer un élément de liste  [!DNL Anaplan]  à partir d’une demande de campagne  [!DNL Adobe Workfront]
description: Ce scénario d’intégration associe un projet  [!DNL Adobe Workfront] à un élément de liste  [!DNL Anaplan] budget.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 9%

---

# Créer un élément de liste [!DNL Anaplan] à partir d’une requête de campagne [!DNL Adobe Workfront]

Ce scénario d’intégration associe un projet [!DNL Adobe Workfront] à un élément de liste budgétaire [!DNL Anaplan].

Ce scénario recherche de nouvelles requêtes de campagne ajoutées à une file d’attente de requêtes. Dès qu’une demande de campagne est enregistrée, une ligne de budget est ajoutée dans [!DNL Anaplan] pour démarrer le processus de financement.

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
   <td role="rowheader">Formule [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> </td> 
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

* Un profil utilisateur dans [!DNL Workfront] nommé **[!UICONTROL [!DNL Anaplan]Integration]**, disposant des droits d’administrateur système.

  Pour plus d&#39;informations sur la création d&#39;un utilisateur dans [!DNL Workfront], voir [Ajout d&#39;utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Un formulaire personnalisé **[!UICONTROL résumé de campagne]** joint à l’objet [!UICONTROL Request].

  Les champs obligatoires suivants doivent être inclus dans le formulaire personnalisé pour faciliter le mappage des données vers Anaplan :

  | Nom de champ | Type de champ |
  |---|---|
  | [!UICONTROL Total des fonds demandés] |   |
  | [!UICONTROL Fonds de main-d’oeuvre requis] |   |
  | [!UICONTROL Fonds de dépenses requis] |   |
  | [!UICONTROL Envoyé à [!DNL Anaplan]] | Case à cocher |

  Les champs facultatifs suivants peuvent être présents sur le formulaire. Ce scénario mappe uniquement les champs ci-dessus, mais tous les champs supplémentaires du dossier de campagne peuvent être mappés.

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
     <td>Date </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL À La Date De Fin Du Marché]</td> 
     <td>Date</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Présentation de Campaign]</td> 
     <td>Zone de texte</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Message de clé]</td> 
     <td>Zone de texte</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Audience Target]</td> 
     <td> <p>Menu déroulant</p> <p>Incluez des options qui correspondent à vos processus.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer ou modifier un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Un projet configuré en tant que file d’attente de requêtes pour capturer de nouvelles requêtes de campagne. Le formulaire [!UICONTROL résumé de campagne] doit être joint à ces demandes.

## Configuration [!DNL Anaplan] attendue

Pour utiliser ce scénario, vous devez disposer des éléments suivants dans [!DNL Anaplan] :

* Un profil utilisateur dans [!DNL Anaplan] nommé **[!UICONTROL [!DNL Workfront]Integration]**, disposant des droits d’administrateur système.
* Le modèle [!DNL Anaplan] que vous souhaitez utiliser pour ce scénario.
* Liste du modèle [!DNL Anaplan] qui capture les budgets de campagne.

  Le module de la liste doit prendre en charge la réception des attributs suivants :

   * [!UICONTROL [!DNL Workfront] Request GUID]
   * [!UICONTROL [!DNL Workfront] GUID de projet ]
   * [!UICONTROL Nom de la campagne]
   * [!UICONTROL Fonds de main-d’oeuvre requis]
   * [!UICONTROL Fonds de dépenses requis]
   * [!UICONTROL Type de requête de budget]

  Cette liste et ce module doivent stocker les détails supplémentaires nécessaires à la fonctionnalité normale de [!DNL Anaplan], y compris la possibilité de définir un budget et de signaler que l&#39;élément de liste de budget est prêt à être resynchronisé sur [!DNL Workfront].

Pour obtenir des instructions sur l’une de ces actions, consultez la documentation [!DNL Anaplan].

## Déploiement sur [!DNL Workfront Fusion]

Effectuez les étapes suivantes pour déployer ce scénario d’intégration sur votre compte [!DNL Fusion]. Cette opération ne doit être effectuée qu’après avoir terminé la configuration [!DNL Workfront] et [!DNL Anaplan] requise.

1. Accédez au menu [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur l’élément de liste **[!UICONTROL [!DNL Anaplan] d’un modèle de requête de campagne Workfront]** .
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

* [[!UICONTROL  Appliquez une  [!DNL Anaplan]  allocation budgétaire à une  [!DNL Adobe Workfront] requête de campagne ou projet de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

Voici d’autres scénarios d’optimisation des dépenses :

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] des mises à jour de projet à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] des mises à jour en heures réelles à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyez [!DNL Adobe Workfront] des dépenses à un  [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
