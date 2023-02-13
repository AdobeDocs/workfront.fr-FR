---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Créez un [!DNL Anaplan] élément d’une liste à partir d’un [!DNL Adobe Workfront] requête de campagne
description: Ce scénario d’intégration associe et [!DNL Adobe Workfront] avec un projet [!DNL Anaplan] élément de liste des budgets.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 2%

---

# Créez un [!DNL Anaplan] élément d’une liste à partir d’un [!DNL Adobe Workfront] requête de campagne

Ce scénario d’intégration associe et [!DNL Adobe Workfront] avec un projet [!DNL Anaplan] élément de liste des budgets.

Ce scénario recherche de nouvelles requêtes de campagne ajoutées à une file d’attente de requêtes. Dès qu’une requête de campagne est enregistrée, une ligne de budget est ajoutée dans la variable [!DNL Anaplan] lancer le processus de financement.

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
   <td role="rowheader">Formule [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> </td> 
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

* A **[!UICONTROL résumé de campagne]** formulaire personnalisé joint au [!UICONTROL Requête] .

   Les champs obligatoires suivants doivent être inclus dans le formulaire personnalisé pour faciliter le mappage des données vers Anaplan :

   | Nom de champ | Type de champ |
   |---|---|
   | [!UICONTROL Total des fonds demandés] |  |
   | [!UICONTROL Fonds de main-d&#39;oeuvre requis] |  |
   | [!UICONTROL Fonds de dépenses demandés] |  |
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

   Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Un projet configuré en tant que file d’attente de requêtes pour capturer de nouvelles requêtes de campagne. Le [!UICONTROL résumé de campagne] Un formulaire doit être joint à ces demandes.

## Valeur attendue [!DNL Anaplan] Configuration

Vous devez avoir les éléments suivants dans [!DNL Anaplan] pour utiliser ce scénario :

* Un profil utilisateur dans [!DNL Anaplan] named **[!UICONTROL [!DNL Workfront]Intégration]**, qui dispose des droits d’administrateur système.
* Le [!DNL Anaplan] Modèle que vous souhaitez utiliser pour ce scénario.
* La liste dans la variable [!DNL Anaplan] Modèle qui capture les budgets de campagne.

   Le module de la liste doit prendre en charge la réception des attributs suivants :

   * [!UICONTROL [!DNL Workfront] GUID de requête]
   * [!UICONTROL [!DNL Workfront] GUID du projet]
   * [!UICONTROL Nom de la campagne]
   * [!UICONTROL Fonds de main-d&#39;oeuvre requis]
   * [!UICONTROL Fonds de dépenses demandés]
   * [!UICONTROL Type de requête de budget]

   Cette liste et ce module doivent stocker les détails supplémentaires nécessaires au bon fonctionnement de la fonction [!DNL Anaplan], y compris la possibilité de définir un budget et de signaler que l’élément de liste des budgets est prêt à être resynchronisé sur [!DNL Workfront].

Pour obtenir des instructions sur l’une de ces actions, voir [!DNL Anaplan] documentation.

## Déploiement sur [!DNL Workfront Fusion]

Procédez comme suit pour déployer ce scénario d’intégration dans votre [!DNL Fusion] compte . Cette opération ne doit être effectuée qu’après avoir terminé les [!DNL Workfront] et [!DNL Anaplan] configuration.

1. Accédez au [!UICONTROL Modèles] dans [!DNL Workfront Fusion] et cliquez sur le bouton **[!UICONTROL Créez un [!DNL Anaplan] élément de liste d’une requête de campagne Workfront]** modèle de scénario.
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

* [[!UICONTROL Appliquez une [!DNL Anaplan] allocation d’un budget à un [!DNL Adobe Workfront] requête de campagne ou projet de campagne]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

Voici d’autres scénarios d’optimisation des dépenses :

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] mises à jour de projet à une [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] mises à jour des heures réelles à une [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Envoyer [!DNL Adobe Workfront] dépenses d’un [!DNL Anaplan] élément de liste]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
