---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Création de modèles dans  [!DNL Adobe Workfront Fusion]
description: Vous pouvez créer de nouveaux modèles de scénario dans  [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: f3f34e807228b299c0570e63bdf329f4e20e0340
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 15%

---

# Créer de nouveaux modèles dans [!DNL Adobe Workfront Fusion]

Vous pouvez créer de nouveaux modèles de scénario dans [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Avant de créer un modèle, vous pouvez vérifier l’onglet [!UICONTROL Modèles publics] pour vous assurer que le modèle que vous souhaitez créer n’est pas déjà disponible.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Créer un modèle

Vous pouvez créer un modèle dans un processus similaire à la création d’un scénario. Les administrateurs de fusion peuvent également créer des modèles à partir de scénarios existants.

* [Créer un modèle](#build-a-template)
* [Création d’un modèle à partir d’un scénario](#create-a-template-from-a-scenario)

### Créer un modèle

1. Cliquez sur **[!UICONTROL Modèles]** ![](assets/fusion-template-icon.png) dans le panneau de navigation de gauche.
1. Cliquez sur **[!UICONTROL Créer un modèle]** dans le coin supérieur droit.
1. (Facultatif) Renommez le modèle en remplaçant le **[!UICONTROL Nouveau nom de modèle]** par défaut dans le coin supérieur gauche.
1. (Facultatif) Pour modifier la langue de votre modèle, cliquez sur **[!UICONTROL Configurer un modèle]** ![](assets/fusion-scenario-settings-icon.png) et sélectionnez la langue dans la liste déroulante Langue .

   >[!IMPORTANT]
   >
   >La sélection Langues correspond aux langues disponibles dans les paramètres du système et ne concerne que le nom du modèle public et sa description. Vous ne pouvez pas modifier la langue d’un modèle une fois le modèle enregistré.

1. (Facultatif) Pour saisir une description du modèle, cliquez sur **[!UICONTROL Configurer un modèle]** ![](assets/fusion-scenario-settings-icon.png) et saisissez la description.
1. Ajoutez des applications, des modules et des outils de la même manière que lors de la création d’un scénario standard.

   Pour ajouter une aide contextuelle aux modules, reportez-vous à la section [Configuration de la fonctionnalité [!UICONTROL Wizard]](#set-up-wizard-functionality) de cet article.

   Pour plus d’informations sur la création d’un scénario, voir [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Si votre modèle comprend des modules qui nécessitent l’ajout de la connexion, des informations d’identification ou d’autres informations sensibles à la confidentialité, ces informations ne sont pas partagées avec les utilisateurs du modèle.

1. (Facultatif) Cliquez sur **[!UICONTROL Exécuter une fois]** pour tester votre modèle.
1. Cliquez sur l&#39;icône **[!UICONTROL Enregistrer]** ![](assets/save-icon.png).

>[!NOTE]
>
>En enregistrant votre modèle, vous le rendez visible pour tous les membres de votre équipe. Si vous souhaitez que votre modèle soit accessible en dehors de votre équipe, vous devez envoyer une demande pour qu’il soit approuvé et publié. La demande est envoyée à Adobe Workfront pour approbation. Une fois validée, le modèle est accessible par d’autres personnes hors de votre équipe.
>
>Pour plus d’informations sur la publication de modèles, voir [Publish and share [!DNL Adobe Workfront Fusion] templates](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

### Création d’un modèle à partir d’un scénario

>[!NOTE]
>
>Pour créer un modèle à partir d’un scénario, vous devez être un administrateur Fusion .

1. Ouvrez la page des détails du scénario à partir de laquelle vous souhaitez créer un scénario.
1. Cliquez sur la liste déroulante **Admin** près du coin supérieur droit de la page.
1. Sélectionnez **Cloner comme modèle**.

   Le scénario est copié dans une page Nouveau modèle.
1. (Facultatif) Renommez le modèle en remplaçant le **[!UICONTROL Nouveau nom de modèle]** par défaut dans le coin supérieur gauche.
1. (Facultatif) Pour modifier la langue de votre modèle, cliquez sur **[!UICONTROL Configurer un modèle]** ![](assets/fusion-scenario-settings-icon.png) et sélectionnez la langue dans la liste déroulante Langue .

   >[!IMPORTANT]
   >
   >La sélection Langues correspond aux langues disponibles dans les paramètres du système et ne concerne que le nom du modèle public et sa description. Vous ne pouvez pas modifier la langue d’un modèle une fois le modèle enregistré.

1. (Facultatif) Pour saisir une description du modèle, cliquez sur **[!UICONTROL Configurer un modèle]** ![](assets/fusion-scenario-settings-icon.png) et saisissez la description.
1. Modifiez les applications, les modules et les outils de la même manière que lors de la modification d’un scénario standard.

   Pour ajouter une aide contextuelle aux modules, reportez-vous à la section [Configuration de la fonctionnalité [!UICONTROL Wizard]](#set-up-wizard-functionality) de cet article.

   >[!NOTE]
   >
   >Si votre modèle comprend des modules qui nécessitent l’ajout de la connexion, des informations d’identification ou d’autres informations sensibles à la confidentialité, ces informations ne sont pas partagées avec les utilisateurs du modèle.

1. (Facultatif) Cliquez sur **[!UICONTROL Exécuter une fois]** pour tester votre modèle.
1. Cliquez sur l&#39;icône **[!UICONTROL Enregistrer]** ![](assets/save-icon.png).

## Configuration de la fonctionnalité [!UICONTROL Wizard] {#set-up-wizard-functionality}

L’ [!DNL Workfront Fusion template] [!UICONTROL assistant] vous permet de fournir aux futurs utilisateurs de votre modèle des instructions ou des informations relatives aux champs spécifiques utilisés dans les modules.

1. Cliquez sur le module ajouté au modèle pour afficher les champs du module.
1. Localisez le champ dans lequel vous souhaitez ajouter des informations [!UICONTROL Wizard] et activez l’option **[!UICONTROL Utiliser dans l’assistant]** pour ce champ.
1. Renseignez les informations que vous souhaitez rendre visibles pour les utilisateurs dans le champ [!UICONTROL Aide] .
1. (Facultatif) Pour permettre aux utilisateurs de voir ce texte lors de l’utilisation du modèle, activez l’option **[!UICONTROL Utiliser comme valeur par défaut]**.
1. Répétez les étapes 2 à 4 pour chaque champ pour lequel vous souhaitez fournir des informations.
1. Cliquez sur **[!UICONTROL OK]** pour enregistrer les modifications et fermer le module.
