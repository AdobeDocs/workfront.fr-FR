---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Exécution de rapports dans  [!DNL Workfront Proof]
description: Workfront Proof vous permet d’afficher des rapports afin que vous puissiez suivre l’avancement du travail et l’efficacité de vos équipes.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Exécution de rapports dans [!DNL Workfront Proof]


>[!IMPORTANT]
>
>* <span class="previe">La fonctionnalité de création de rapports n’est plus disponible dans [!DNL Workfront Proof]. L&#39;onglet de rapport s&#39;affiche toujours, mais les données ne sont pas précises.</span>
> 
>* Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Workfront Proof vous permet d’afficher des rapports afin que vous puissiez suivre l’avancement du travail et l’efficacité de vos équipes.

Vous pouvez facilement afficher le nombre de BAT créés dans votre compte [!DNL Workfront Proof], le nombre de versions associées à chaque BAT, la durée de traitement, etc.

## Conditions préalables

La disponibilité des rapports dépend de votre type de compte [!DNL Workfront Proof] et des niveaux d’autorisation des utilisateurs.

* [Conditions préalables du compte](#account-prerequisites)
* [Conditions préalables requises pour l’utilisateur](#user-prerequisites)

### Conditions préalables du compte {#account-prerequisites}

Les informations de création de rapports sont disponibles uniquement avec les plans Premium.

### Conditions préalables requises pour l’utilisateur {#user-prerequisites}

Les informations de création de rapports sont disponibles uniquement pour les utilisateurs disposant d’un accès complet à tous les bons à tirer de votre compte (c’est-à-dire pour les utilisateurs disposant d’ [ profils d’autorisations de BAT dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Dans ce panneau, vous pouvez

* Contrôler la durée des données affichées
* Analyse des modifications apportées aux mesures au fil du temps
* Vérifiez les détails d’un point sélectionné dans le temps en le survolant.
* Vérifiez le nombre total de BAT créés au cours de la période sélectionnée.
* Vérifier le nombre moyen de versions incluses dans les ensembles de BAT terminés

## Affichage des rapports {#viewing-reports}

1. Accédez à la page **[!UICONTROL Tableaux de bord]** .
1. Cliquez sur l’onglet **[!UICONTROL Rapports]** .\
   ![BAT_reports.png](assets/proof-reports-350x193.png)

1. Dans le menu déroulant **[!UICONTROL Période]**, choisissez si vous souhaitez afficher des informations sur les bons à tirer créés au cours des dernières 24 heures, 7 jours, 30 jours, 90 jours ou une période personnalisée.\
   Si vous sélectionnez une période personnalisée, sélectionnez les dates de début et de fin, puis cliquez sur **[!UICONTROL Appliquer]**.\
   Les informations suivantes s’affichent pour la période que vous avez sélectionnée :\
   **BAT créé :** Nombre de BAT créés au cours de la période sélectionnée.\
   **Versions par BAT :** Nombre moyen de versions par BAT pour tous les BAT terminés (Approuvés ou Approuvés avec modifications) au cours de la période sélectionnée.\
   **Durée de rotation :** Durée moyenne entre la création de la première version et le moment où la décision a été prise sur la version finale.\
   **Heure de la première activité :** Durée moyenne entre le moment de la création du BAT et le moment de la première activité sur le BAT.\
   **Bons à tirer en retard :** Pourcentage moyen de bons à tirer terminés (approuvés ou approuvés avec modifications) ayant au moins une version en retard au cours de la période sélectionnée.\
   **Commentaires et réponses :** Nombre moyen de commentaires et de réponses effectués sur tous les bons à tirer au cours de la période sélectionnée.

1. (Facultatif) Sélectionnez ou désélectionnez l’option **[!UICONTROL Afficher la plage min. max.]** pour déterminer si les valeurs minimale et maximale sont affichées dans le graphique.\
   Lorsque cette option est sélectionnée, un ombrage bleu s’affiche entre les valeurs enregistrées minimale et maximale.

1. (Facultatif) Vous pouvez filtrer les données affichées, comme décrit dans la section [Filtrage des rapports](#filtering-reports).

## Filtrage des rapports {#filtering-reports}

Par défaut, les données affichées dans les rapports incluent toutes les informations de votre système [!DNL Workfront Proof]. Vous pouvez utiliser des filtres pour afficher uniquement les informations pertinentes à vos besoins.

Pour filtrer les informations des rapports :

1. Accédez à la page **[!UICONTROL Tableaux de bord]** .
1. Cliquez sur l’onglet **[!UICONTROL Rapports]** .\
   ![BAT_reports.png](assets/proof-reports-350x193.png)

1. Exécutez un rapport, comme décrit dans la section [Affichage des rapports](#viewing-reports).
1. Cliquez sur **[!UICONTROL Filter]**.

1. Sur le côté gauche de la page, sélectionnez l’une des options de filtre suivantes :\
   **[!UICONTROL Type de BAT] :** Sélectionnez le type de BAT que vous souhaitez inclure dans le rapport.\
   **[!UICONTROL Décisions] :** Sélectionnez des options pour déterminer si seuls des bons à tirer contenant certaines décisions ont été pris.\
   **[!UICONTROL Destinataires] :** Sélectionnez des utilisateurs individuels pour afficher les informations relatives aux bons à tirer partagés avec les utilisateurs sélectionnés.\
   **[!UICONTROL Propriétaires de BAT] :** sélectionnez des utilisateurs individuels pour afficher les informations relatives aux BAT appartenant aux utilisateurs sélectionnés.\
   **[!UICONTROL Créateurs de BAT] :** sélectionnez des utilisateurs individuels pour afficher les informations relatives aux BAT créés par les utilisateurs sélectionnés.\
   **[!UICONTROL Comptes] :** Sélectionnez les comptes à inclure dans le rapport.

1. Cliquez sur **[!UICONTROL Appliquer]**.
1. (Facultatif) Sélectionnez ou désélectionnez l’option **[!UICONTROL Afficher la plage min. max.]** pour déterminer si les valeurs minimale et maximale sont affichées dans le graphique.\
   Lorsque cette option est sélectionnée, un ombrage bleu s’affiche entre les valeurs enregistrées minimale et maximale.

## Impression de rapports

1. Accédez à la page **[!UICONTROL Tableaux de bord]** .
1. Cliquez sur l’onglet **[!UICONTROL Rapports]**, puis sur **[!UICONTROL Imprimer]**.\
   ![BAT_reports_print.png](assets/proof-reports-print-350x191.png)

1. Choisissez parmi les différentes options d’impression disponibles.\
   Les options d’impression varient en fonction du navigateur et de la version du navigateur que vous utilisez.
