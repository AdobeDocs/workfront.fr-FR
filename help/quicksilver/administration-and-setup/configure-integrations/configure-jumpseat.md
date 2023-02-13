---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configuration de l’intégration JumpSeat
description: Vous pouvez intégrer des [!DNL JumpSeat] avec [!DNL Workfront] pour créer des conseils personnalisés et intégrés au produit.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# Configuration de l’intégration JumpSeat

Vous pouvez intégrer des [!DNL JumpSeat] avec [!DNL Workfront] pour créer des conseils personnalisés et intégrés au produit.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Produit</strong></td> 
   <td>Vous devez avoir une principale [!DNL JumpSeat] planifiez.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p> Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Avant de commencer, vous devez

* Ajouter et activer [!DNL Workfront] en tant qu’application dans [!DNL JumpSeat]. Pour plus d’informations, voir [Comment Ajouter Ou Supprimer Une Application](https://support.jumpseat.io/article/how-to-add-an-application/).

## Configurez la variable [!DNL JumpSeat] integration

Nous vous recommandons de configurer une [!DNL JumpSeat] l’intégration dans les environnements de prévisualisation et de production.

>[!TIP]
>
>Vous devez ajouter et activer deux [!DNL Workfront] applications dans [!DNL JumpSeat]: un pour l’aperçu et un pour la production. Voir [Comment Ajouter Ou Supprimer Une Application](https://support.jumpseat.io/article/how-to-add-an-application/) pour plus d’informations.

Pour configurer la variable [!DNL JumpSeat] intégration :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]**.
1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Système]** > **[!UICONTROL [!DNL JumpSeat]Intégration]**.
1. Saisissez votre **[!UICONTROL [!DNL JumpSeat]URL]**.

   **Exemple :** [!DNL https]://{mycompanyname}.jumpsièges.io

1. Saisissez le **[!UICONTROL [!DNL JumpSeat]jeton d’intégration]**. Vous pouvez le trouver sur la page **[!UICONTROL Configuration]** page [!DNL JumpSeat].

   **Exemple :** $2 y$10$BevsKeQ8...OYR.LurSg2U64O

1. Cliquez sur **[!UICONTROL Configuration du test]**.
1. Choisissez si vous souhaitez que l’intégration soit **[!UICONTROL Principal]** ou **[!UICONTROL Inactif]**.

   >[!IMPORTANT]
   >
   >Le test de configuration réalisé à l&#39;étape 5 doit être effectué avec succès afin d&#39;activer l&#39;intégration.

   ![Page d’intégration Saut de siège](assets/jumpseat-integration-page.png)

1. Cliquer sur **[!UICONTROL Enregistrer]**.
