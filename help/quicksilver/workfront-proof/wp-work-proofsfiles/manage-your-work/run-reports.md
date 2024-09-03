---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Exécuter des rapports dans  [!DNL Workfront Proof]
description: Workfront Proof vous permet d’afficher des rapports afin de suivre la progression du travail et l’efficacité de vos équipes.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 100%

---

# Exécuter des rapports dans [!DNL Workfront Proof]


>[!IMPORTANT]
>
>* <span class="previe">La fonctionnalité de création de rapports n’est plus disponible dans [!DNL Workfront Proof]. L’onglet Rapports apparaît toujours, mais les données ne sont pas exactes.</span>
> 
>* Cet article fait référence aux fonctionnalités du produit [!DNL Workfront Proof] autonome. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Workfront Proof vous permet d’afficher des rapports afin de suivre la progression du travail et l’efficacité de vos équipes.

Vous pouvez facilement consulter le nombre d’épreuves créées dans votre compte [!DNL Workfront Proof], le nombre de versions associées à chaque épreuve, le délai de traitement, etc.

## Conditions préalables

La disponibilité des rapports dépend du type de votre compte [!DNL Workfront Proof] et des niveaux d’autorisation de l’utilisateur ou de l’utilisatrice.

* [Conditions préalables pour le compte](#account-prerequisites)
* [Conditions préalables pour les utilisateurs et utilisatrices](#user-prerequisites)

### Conditions préalables pour le compte {#account-prerequisites}

Les informations de rapport sont disponibles uniquement pour les plans Premium.

### Conditions préalables pour les utilisateurs et utilisatrices {#user-prerequisites}

Les informations de rapport sont disponibles uniquement pour les personnes ayant un accès complet à toutes les épreuves de votre compte (c’est-à-dire les utilisateurs et les utilisatrices qui disposent au moins des [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Dans ce panneau, vous pouvez :

* contrôler la période des données affichées ;
* analyser l’évolution des mesures dans le temps ;
* vérifier les détails d’un point sélectionné dans le temps en le survolant ;
* vérifier le nombre total d’épreuves créées durant la période sélectionnée ;
* vérifier le nombre moyen de versions incluses dans les jeux d’épreuves terminés.

## Afficher les rapports {#viewing-reports}

1. Accédez à la page **[!UICONTROL Tableaux de bord]**.
1. Cliquez sur l’onglet **[!UICONTROL Rapports]**.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Dans le menu déroulant **[!UICONTROL Période]**, choisissez d’afficher les informations sur les épreuves créées au cours des dernières 24 heures, des 7 derniers jours, des 30 derniers jours, des 90 derniers jours ou d’une période personnalisée.\
   Si vous optez pour une période personnalisée, sélectionnez les dates de début et de fin, puis cliquez sur **[!UICONTROL Appliquer]**.\
   Les informations suivantes s’affichent pour la période sélectionnée :\
   **Épreuves créées :** nombre d’épreuves créées au cours de la période sélectionnée.\
   **Versions par épreuve :** nombre moyen de versions par épreuve pour toutes les épreuves terminées (approuvées ou approuvées avec modifications) au cours de la période sélectionnée.\
   **Temps de traitement :** durée moyenne entre la création de la première version et la prise de décision sur la version finale.\
   **Délai de la première activité :** durée moyenne entre la création de l’épreuve et la première activité sur l’épreuve.\
   **Épreuves en retard :** pourcentage moyen d’épreuves terminées (approuvées ou approuvées avec modifications) dont au moins une version était en retard au cours de la période sélectionnée.\
   **Commentaires et réponses :** nombre moyen de commentaires et de réponses apportés à toutes les épreuves au cours de la période sélectionnée.

1. (Facultatif) Sélectionnez ou désélectionnez l’option **[!UICONTROL Afficher la plage min-max]** pour indiquer si les valeurs minimales et maximales doivent être affichées dans le graphique.\
   Lorsque cette option est sélectionnée, un ombrage bleu s’affiche entre les valeurs minimale et maximale enregistrées.

1. (Facultatif) Vous pouvez filtrer les données affichées, comme décrit dans [Filtrage des rapports](#filtering-reports).

## Filtrer les rapports {#filtering-reports}

Par défaut, les données affichées dans les rapports incluent toutes les informations de votre système [!DNL Workfront Proof]. Vous pouvez utiliser des filtres pour n’afficher que les informations dont vous avez besoin.

Pour filtrer les informations des rapports :

1. Accédez à la page **[!UICONTROL Tableaux de bord]**.
1. Cliquez sur l’onglet **[!UICONTROL Rapports]**.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. Exécutez un rapport, comme décrit dans [Affichage des rapports](#viewing-reports).
1. Cliquez sur **[!UICONTROL Filtrer]**.

1. Dans la partie gauche de la page, sélectionnez l’une des options de filtrage suivantes :\
   **[!UICONTROL Type d’épreuve] :** sélectionnez le type d’épreuve que vous souhaitez inclure dans le rapport.\
   **[!UICONTROL Décisions] :** sélectionnez des options pour déterminer si seules des épreuves contenant certaines décisions ont été réalisées.\
   **[!UICONTROL Personnes destinataires] :** sélectionnez des utilisateurs et utilisatrices individuels pour afficher les informations relatives aux épreuves partagées avec les utilisateurs et utilisatrices sélectionnés.\
   **[!UICONTROL Personnes propriétaires d’épreuve] :** sélectionnez des utilisateurs et utilisatrices individuels pour afficher les informations relatives aux épreuves dont ils sont propriétaires.\
   **[!UICONTROL Créateurs et créatrices d’épreuve] :** sélectionnez des utilisateurs et utilisatrices individuels pour afficher les informations relatives aux épreuves créées par les utilisateurs et utilisatrices sélectionnés.\
   **[!UICONTROL Comptes] :** sélectionnez les comptes que vous souhaitez inclure dans le rapport.

1. Cliquez sur **[!UICONTROL Appliquer]**.
1. (Facultatif) Sélectionnez ou désélectionnez l’option **[!UICONTROL Afficher la plage min-max]** pour déterminer si les valeurs minimale et maximale sont affichées dans le graphique.\
   Lorsque cette option est sélectionnée, un ombrage bleu s’affiche entre les valeurs minimale et maximale enregistrées.

## Imprimer des rapports

1. Accédez à la page **[!UICONTROL Tableaux de bord]**.
1. Cliquez sur l’onglet **[!UICONTROL Rapports]**, puis sur **[!UICONTROL Imprimer]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. Sélectionnez l’une des différentes options d’impression disponibles.\
   Les options d’impression varient en fonction du navigateur et de la version du navigateur que vous utilisez.
