---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Afficher l’historique d’exécution d’un scénario dans Adobe Workfront Fusion
description: Vous pouvez afficher des informations sur toutes les exécutions d’un scénario ou rechercher des données spécifiques dans toutes les exécutions du scénario.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: ae57c38149bf6db3bbbb471fad8f3567b7d712a7
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 100%

---

# Afficher l’historique d’exécution d’un scénario dans [!DNL Adobe Workfront Fusion]

Vous pouvez afficher des informations sur toutes les exécutions d’un scénario ou rechercher des données spécifiques dans toutes les exécutions du scénario.

L’historique d’exécution d’un scénario affiche toutes les exécutions d’un scénario pour les 30 derniers jours.

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
   </td>  
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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Afficher toutes les exécutions d’un scénario

### Afficher l’historique d’exécution du scénario sur la page [!UICONTROL Détails du scénario]

1. Cliquez sur l’onglet **[!UICONTROL Scénario]** dans le panneau de gauche, puis cliquez sur le scénario.

   Ou

   Si vous travaillez sur le scénario dans l’éditeur de scénario, cliquez sur la flèche vers la gauche ![](assets/exit-editing-arrow.png) près du coin supérieur gauche de la fenêtre.

1. Affichez les informations dans la liste de droite.

   ![](assets/open-history-tab-350x202.png)

   Vous pouvez également cliquer pour afficher une page entière de ces informations. La vue de page entière vous permet de filtrer l’historique pour afficher des exécutions spécifiques.

   Les détails suivants sont répertoriés pour chaque exécution du scénario :

   * Date à laquelle l’exécution a **[!UICONTROL démarré]**
   * **[!UICONTROL Statut]** (succès ou échec)
   * **[!UICONTROL Durée]** de l’exécution
   * Nombre d’**[!UICONTROL opérations]**
   * Taille du **[!UICONTROL transfert de données]**
   * Lier à **[!UICONTROL Détails]**

>[!NOTE]
>
>L’historique des scénarios affiche un badge de **traitement** en regard des scénarios récemment exécutés, tandis que les détails de l’exécution sont écrits dans le stockage. Le traitement se produit immédiatement après l’exécution du scénario et ne doit pas durer plus de quelques minutes. Les détails de l’exécution du scénario peuvent ne pas être visibles pendant le traitement de l’exécution.

### Afficher l’historique d’exécution du scénario sur l’onglet [!UICONTROL Historique]

L’onglet [!UICONTROL Historique] affiche plus de détails que ce qui est disponible dans la page [!UICONTROL Détails du scénario]. Vous pouvez également filtrer et trier les exécutions sur l’onglet [!UICONTROL Historique].

1. Cliquez sur l’onglet **[!UICONTROL Scénario]** dans le panneau de gauche, puis cliquez sur le scénario.

   Ou

   Si vous travaillez sur le scénario dans l’éditeur de scénario, cliquez sur la flèche gauche ![](assets/exit-editing-arrow.png) près du coin supérieur gauche de la fenêtre.

1. Cliquez sur l’onglet **[!UICONTROL Historique]** dans le coin supérieur gauche de la page.
1. (Facultatif) Pour plus d’informations sur une exécution de scénario sélectionnée, y compris les lots qui ont été traités, cliquez sur le lien **[!UICONTROL Détails]**.

   Pour plus d’informations sur les lots de traitement, voir [Flux d’exécution du scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >* Le lien [!UICONTROL détails] n’est visible que si les détails de l’exécution sont disponibles.
   >
   >* L’historique des scénarios affiche un badge **Historique de traitement** en regard des scénarios récemment exécutés, tandis que les détails de l’exécution sont écrits dans le stockage. Le traitement se produit immédiatement après l’exécution du scénario et ne doit pas durer plus de quelques minutes. Les détails de l’exécution du scénario peuvent ne pas être visibles pendant le traitement de l’exécution.

## Filtrer l’historique d’exécution d’un scénario

Vous pouvez filtrer l’historique d’exécution pour n’afficher que les exécutions contenant les valeurs spécifiées.

1. Ouvrez l’historique d’un scénario en mode pleine page, comme décrit dans la section [Afficher l’historique d’exécution d’un scénario dans l’onglet [!UICONTROL Historique]](#view-scenario-execution-history-on-the-history-tab) de cet article.
1. Cliquez sur l’icône [!UICONTROL filtrer] ![](assets/fusion-scenario-filter-icon.png) dans l’en-tête de la colonne que vous souhaitez filtrer.
1. Dans la boîte de dialogue [!UICONTROL filtrer], saisissez les valeurs à utiliser pour filtrer les données.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

L’icône de filtre est orange dans les colonnes avec un filtre actif.

## Trier l’historique d’exécution d’un scénario

Vous pouvez trier l’historique d’exécution d’un scénario.

1. Ouvrez l’historique d’un scénario en mode pleine page, comme décrit dans la section [Afficher l’historique d’exécution d’un scénario dans l’onglet [!UICONTROL Historique]](#view-scenario-execution-history-on-the-history-tab) de cet article.
1. Cliquez sur l’icône [!UICONTROL Trier] dans l’en-tête de la colonne sur laquelle vous souhaitez filtrer les données.
1. Facultatif : pour inverser l’ordre de tri, cliquez à nouveau sur l’icône [!UICONTROL Trier].

## Rechercher toutes les exécutions d’un scénario

1. Cliquez sur l’icône **[!UICONTROL Scénario]** ![](assets/scenarios-icon.png) dans le panneau de gauche, puis sélectionnez le scénario.

   Ou

   Si vous travaillez sur le scénario dans l’éditeur de scénario, cliquez sur la flèche vers la gauche ![](assets/exit-editing-arrow.png) près du coin supérieur gauche de la fenêtre.

1. Sélectionnez l’onglet **[!UICONTROL Historique]** dans le coin supérieur gauche de l’écran.
1. Cliquez sur **[!UICONTROL Recherche de texte intégral]** en haut de la liste des exécutions.

   Ou

   Effectuez les raccourcis clavier **Ctrl+Maj+F** (Windows) ou **Cmd+Maj+F** (Mac). La fenêtre [!UICONTROL Rechercher dans l’historique] s’affiche.

1. (Facultatif) Pour rechercher des exécutions qui contiennent du texte spécifique, saisissez le texte dans la barre de recherche de la fenêtre **[!UICONTROL Rechercher dans l’historique]**.

   Pour rechercher une correspondance exacte, entourez le texte de guillemets doubles (« exemple »).

   >[!INFO]
   >
   >**Exemple :** si vous souhaitez trouver l’exécution qui a créé un projet spécifique, saisissez l’ID de projet dans la barre de [!UICONTROL Recherche de texte intégral].
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (Facultatif) Pour limiter votre recherche à une période spécifique, sélectionnez les dates de début et de fin de votre recherche dans la zone [!UICONTROL Par période].

   >[!NOTE]
   >
   >* Les exécutions ne sont disponibles que pour les 30 jours précédents.
   >
   >* [!DNL Workfront Fusion] stocke les payloads de webhook pendant 30 jours. L’accès à une payload de webhook plus de 30 jours après sa création entraîne l’erreur « [!UICONTROL Échec de la lecture du fichier à partir du stockage] ».


1. (Facultatif) Pour limiter votre recherche à un statut spécifique, sélectionnez le statut de votre choix dans le menu déroulant **[!UICONTROL Par statut]**.


   Les statuts disponibles sont les suivants :

   * [!UICONTROL Tous]

   * [!UICONTROL Erreur]

   * [!UICONTROL Avertissement]

   * [!UICONTROL Succès]

1. (Facultatif) Modifiez l’ordre dans lequel les résultats s’affichent dans le menu déroulant **[!UICONTROL Trier par date]**.

1. (Facultatif) Pour copier un ID d’exécution de scénario, cliquez sur l’icône **[!UICONTROL Copier l’ID d’exécution]**. <img src="assets/copy-fusion-execution-id-icon.png"> dans la ligne de l’exécution souhaitée

1. (Facultatif) Cliquez sur un résultat de la [!UICONTROL Recherche de texte intégral] pour examiner le lot de sortie du module de scénario qui contient les informations.
