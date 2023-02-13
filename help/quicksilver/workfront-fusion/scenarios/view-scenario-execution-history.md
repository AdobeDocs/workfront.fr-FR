---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Affichage de l’historique d’exécution d’un scénario dans Adobe Workfront Fusion
description: Vous pouvez afficher des informations sur toutes les exécutions d’un scénario ou rechercher des données spécifiques dans toutes les exécutions du scénario.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# Afficher l’historique d’exécution d’un scénario dans [!DNL Adobe Workfront Fusion]

Vous pouvez afficher des informations sur toutes les exécutions d’un scénario ou rechercher des données spécifiques dans toutes les exécutions du scénario.

L’historique d’exécution d’un scénario affiche toutes les exécutions d’un scénario pour les 30 derniers jours.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p><p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Afficher toutes les exécutions d’un scénario

### Afficher l’historique d’exécution du scénario sur la page [!UICONTROL Détails du scénario] page

1. Cliquez sur le bouton **[!UICONTROL Scénario]** dans le panneau de gauche, puis cliquez sur le scénario.

   Ou

   Si vous travaillez sur le scénario dans l’éditeur de scénario, cliquez sur la flèche vers la gauche. ![](assets/exit-editing-arrow.png) près du coin supérieur gauche de la fenêtre.

1. Affichez les informations dans la liste de droite.

   ![](assets/open-history-tab-350x202.png)

   C

   Vous pouvez également cliquer sur pour afficher une page entière de ces informations. La vue de page entière vous permet de filtrer l’historique pour afficher des exécutions spécifiques.

   Les détails suivants sont répertoriés pour chaque exécution du scénario :

   * Date à laquelle l’exécution a été effectuée **[!UICONTROL Démarré]**
   * **[!UICONTROL État]** (succès ou échec)
   * Exécuter **[!UICONTROL Durée]**
   * Nombre **[!UICONTROL Opérations]**
   * Taille de **[!UICONTROL Transfert de données]**
   * Lier à **[!UICONTROL Détails]**

### Afficher l’historique d’exécution du scénario sur la page [!UICONTROL Histoire] tab

Le [!UICONTROL Histoire] affiche plus de détails que ce qui est disponible dans la [!UICONTROL Détails du scénario] page. Vous pouvez également filtrer et trier les exécutions sur le [!UICONTROL Histoire] .

1. Cliquez sur le bouton **[!UICONTROL Scénario]** dans le panneau de gauche, puis cliquez sur le scénario.

   Ou

   Si vous travaillez sur le scénario dans l’éditeur de scénario, cliquez sur la flèche vers la gauche. ![](assets/exit-editing-arrow.png) près du coin supérieur gauche de la fenêtre.

1. Cliquez sur le bouton **[!UICONTROL Histoire]** dans le coin supérieur gauche de la page.
1. (Facultatif) Pour plus d’informations sur une exécution de scénario sélectionnée, y compris les lots qui ont été traités, cliquez sur le bouton **[!UICONTROL Détails]** lien.

   Pour plus d’informations sur les lots de traitement, voir [Flux d’exécution du scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >Le [!UICONTROL détails] n’est visible que si les détails de l’exécution sont disponibles.

## Filtrage de l&#39;historique d&#39;exécution du scénario

Vous pouvez filtrer l’historique de l’exécution pour n’afficher que les exécutions avec les valeurs spécifiées.

1. Ouvrez l’historique de la page entière pour un scénario, comme décrit dans la section [Afficher l’historique d’exécution du scénario sur la page [!UICONTROL Histoire] tab](#view-scenario-execution-history-on-the-history-tab) dans cet article.
1. Cliquez sur le bouton [!UICONTROL filter] icon ![](assets/fusion-scenario-filter-icon.png) dans l’en-tête de la colonne que vous souhaitez filtrer.
1. Dans le [!UICONTROL filter] , saisissez les valeurs à utiliser pour filtrer les données.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

L’icône de filtre est orange dans les colonnes avec un filtre actuellement principal.

## Tri de l&#39;historique d&#39;exécution du scénario

Vous pouvez trier l&#39;historique d&#39;exécution du scénario.

1. Ouvrez l’historique de la page entière pour un scénario, comme décrit dans la section [Afficher l’historique d’exécution du scénario sur la page [!UICONTROL Histoire] tab](#view-scenario-execution-history-on-the-history-tab) dans cet article.
1. Cliquez sur le bouton [!UICONTROL Tri] dans l’en-tête de la colonne sur laquelle vous souhaitez filtrer les données.
1. Facultatif : Pour inverser l’ordre du tri, cliquez sur le bouton [!UICONTROL Tri] à nouveau.

## Recherche de toutes les exécutions d’un scénario

1. Cliquez sur le bouton **[!UICONTROL Scénario]** icon ![](assets/scenarios-icon.png) dans le panneau de gauche, puis cliquez sur le scénario.

   Ou

   Si vous travaillez sur le scénario dans l’éditeur de scénario, cliquez sur la flèche vers la gauche. ![](assets/exit-editing-arrow.png) près du coin supérieur gauche de la fenêtre.

1. Cliquez sur le bouton **[!UICONTROL Histoire]** dans le coin supérieur gauche de l’écran.
1. Cliquez sur **[!UICONTROL Recherche de texte intégral]** en haut de la liste des exécutions.

   Ou

   Type **Ctrl+Maj+F** (Windows) ou **Cmd+Maj+F** (Mac) La variable [!UICONTROL Recherche dans l’historique] s’ouvre.

1. (Facultatif) Pour rechercher des exécutions qui contiennent du texte spécifique, saisissez le texte dans la barre de recherche du champ **[!UICONTROL Recherche dans l’historique]** fenêtre.

   Pour rechercher du texte exact, entourez le texte de guillemets doubles (&quot;exemple&quot;).

   >[!INFO]
   >
   >**Exemple :** Si vous souhaitez trouver l’exécution qui a créé un projet spécifique, saisissez l’ID de projet dans la variable [!UICONTROL Recherche de texte intégral] de la barre
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (Facultatif) Pour limiter votre recherche par période, sélectionnez les dates de début et de fin de votre recherche dans la [!UICONTROL Par période] zone.

   >[!NOTE]
   >
   >* Les exécutions ne sont disponibles que pendant les 30 jours précédents.
   >
   >* [!DNL Workfront Fusion] stocke les charges utiles webhook pendant 30 jours. L’accès à une payload webhook plus de 30 jours après sa création entraîne l’erreur &quot;[!UICONTROL Échec de la lecture du fichier à partir du stockage.]&quot;



1. (Facultatif) Pour limiter votre recherche par état, sélectionnez l’état de votre choix dans le **[!UICONTROL Par statut]** menu déroulant.


   Les états disponibles sont les suivants :

   * [!UICONTROL Tout]

   * [!UICONTROL Erreur]

   * [!UICONTROL Avertissement]

   * [!UICONTROL Succès]

1. (Facultatif) Modifiez l’ordre dans lequel les résultats s’affichent dans la variable **[!UICONTROL Tri par date]** menu déroulant.

1. (Facultatif) Pour copier un ID d’exécution de scénario, cliquez sur le bouton **[!UICONTROL Copie de l’ID d’exécution]** icon <img src="assets/copy-fusion-execution-id-icon.png"> dans la ligne de l’exécution souhaitée ;

1. (Facultatif) Cliquez sur un résultat de la variable [!UICONTROL Recherche de texte intégral] pour examiner le lot de sortie du module scénario qui contient les informations.
