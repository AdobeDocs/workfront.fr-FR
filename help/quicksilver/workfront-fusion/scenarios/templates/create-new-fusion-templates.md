---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Création de modèles dans [!DNL Adobe Workfront Fusion]
description: Vous pouvez créer de nouveaux modèles de scénario dans [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# Création de modèles dans [!DNL Adobe Workfront Fusion]

Vous pouvez créer de nouveaux modèles de scénario dans [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Avant de créer un modèle, vous pouvez vérifier les [!UICONTROL Modèles publics] pour vous assurer que le modèle que vous souhaitez créer n’est pas déjà disponible.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail, [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Créer un modèle

Vous pouvez créer un modèle dans un processus similaire à la création d’un scénario. Les administrateurs de fusion peuvent également créer des modèles à partir de scénarios existants.

* [Créer un modèle](#build-a-template)
* [Création d’un modèle à partir d’un scénario](#create-a-template-from-a-scenario)

### Créer un modèle

1. Cliquez sur **[!UICONTROL Modèles]** ![](assets/fusion-template-icon.png) dans le panneau de navigation de gauche.
1. Cliquez sur **[!UICONTROL Créer un modèle]** dans le coin supérieur droit.
1. (Facultatif) Renommez le modèle en remplaçant la valeur par défaut. **[!UICONTROL Nouveau nom du modèle]** dans le coin supérieur gauche.
1. (Facultatif) Pour modifier la langue de votre modèle, cliquez sur **[!UICONTROL Configurer un modèle]** ![](assets/fusion-scenario-settings-icon.png) et sélectionnez la langue dans la liste déroulante Langue .

   >[!IMPORTANT]
   >
   >La sélection Langues correspond aux langues disponibles dans les paramètres du système et ne concerne que le nom du modèle public et sa description. Vous ne pouvez pas modifier la langue d’un modèle une fois le modèle enregistré.

1. (Facultatif) Pour saisir une description du modèle, cliquez sur **[!UICONTROL Configurer un modèle]** ![](assets/fusion-scenario-settings-icon.png) et saisissez la description.
1. Ajoutez des applications, des modules et des outils de la même manière que lors de la création d’un scénario standard.

   Pour ajouter une aide contextuelle aux modules, voir [Configuration [!UICONTROL Assistant] fonctionnalité](#set-up-wizard-functionality) dans cet article.

   Pour plus d’informations sur la création d’un scénario, voir [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Si votre modèle comprend des modules qui nécessitent l’ajout de la connexion, des informations d’identification ou d’autres informations sensibles à la confidentialité, ces informations ne sont pas partagées avec les utilisateurs du modèle.

1. (Facultatif) Cliquez sur **[!UICONTROL Exécuter une seule fois]** pour tester votre modèle.
1. Cliquez sur le bouton **[!UICONTROL Enregistrer]** icon ![](assets/save-icon.png).

>[!NOTE]
>
>En enregistrant votre modèle, vous le rendez visible pour tous les membres de votre équipe. Si vous souhaitez que votre modèle soit accessible en dehors de votre équipe, vous devez le publier, puis utiliser un lien partagé, ou demander à votre administrateur d’approuver et de publier le modèle.

### Création d’un modèle à partir d’un scénario

>[!NOTE]
>
>Pour créer un modèle à partir d’un scénario, vous devez être un administrateur Fusion .

1. Ouvrez la page des détails du scénario à partir de laquelle vous souhaitez créer un scénario.
1. Cliquez sur le bouton **Administration** en haut à droite de la page.
1. Sélectionner **Clonage en tant que modèle**.

   Le scénario est copié dans une page Nouveau modèle.
1. (Facultatif) Renommez le modèle en remplaçant la valeur par défaut. **[!UICONTROL Nouveau nom du modèle]** dans le coin supérieur gauche.
1. (Facultatif) Pour modifier la langue de votre modèle, cliquez sur **[!UICONTROL Configurer un modèle]** ![](assets/fusion-scenario-settings-icon.png) et sélectionnez la langue dans la liste déroulante Langue .

   >[!IMPORTANT]
   >
   >La sélection Langues correspond aux langues disponibles dans les paramètres du système et ne concerne que le nom du modèle public et sa description. Vous ne pouvez pas modifier la langue d’un modèle une fois le modèle enregistré.

1. (Facultatif) Pour saisir une description du modèle, cliquez sur **[!UICONTROL Configurer un modèle]** ![](assets/fusion-scenario-settings-icon.png) et saisissez la description.
1. Modifiez les applications, les modules et les outils de la même manière que lors de la modification d’un scénario standard.

   Pour ajouter une aide contextuelle aux modules, voir [Configuration [!UICONTROL Assistant] fonctionnalité](#set-up-wizard-functionality) dans cet article.

   >[!NOTE]
   >
   >Si votre modèle comprend des modules qui nécessitent l’ajout de la connexion, des informations d’identification ou d’autres informations sensibles à la confidentialité, ces informations ne sont pas partagées avec les utilisateurs du modèle.

1. (Facultatif) Cliquez sur **[!UICONTROL Exécuter une seule fois]** pour tester votre modèle.
1. Cliquez sur le bouton **[!UICONTROL Enregistrer]** icon ![](assets/save-icon.png).

## Configuration [!UICONTROL Assistant] fonctionnalité {#set-up-wizard-functionality}

Le [!DNL Workfront Fusion template] [!UICONTROL Assistant] vous permet de fournir aux futurs utilisateurs de votre modèle des instructions ou des informations relatives aux champs spécifiques utilisés dans les modules.

1. Cliquez sur le module ajouté au modèle pour afficher les champs du module.
1. Localisez le champ à ajouter. [!UICONTROL Assistant] et activez **[!UICONTROL Utilisation dans l’assistant]** pour ce champ.
1. Saisissez les informations que vous souhaitez rendre visibles pour les utilisateurs dans la variable [!UICONTROL Aide] champ .
1. (Facultatif) Pour permettre aux utilisateurs de voir ce texte lors de l’utilisation du modèle, activez l’option **[!UICONTROL Utiliser comme valeur par défaut]**.
1. Répétez les étapes 2 à 4 pour chaque champ pour lequel vous souhaitez fournir des informations.
1. Cliquez sur **[!UICONTROL OK]** pour enregistrer les modifications et fermer le module.
