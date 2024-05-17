---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurer l’intégration de JumpSeat
description: Vous pouvez intégrer des [!DNL JumpSeat] avec [!DNL Workfront] pour créer des conseils personnalisés et intégrés au produit.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 12%

---

# Configurer l’intégration de JumpSeat

Vous pouvez intégrer des [!DNL JumpSeat] avec [!DNL Workfront] pour créer des conseils personnalisés et intégrés au produit.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Produit</strong></td> 
   <td>Vous devez disposer d’un [!DNL JumpSeat] planifiez.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p> Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Avant de commencer, vous devez

* Ajouter et activer [!DNL Workfront] comme application dans [!DNL JumpSeat]. Pour plus d’informations, voir [Comment Ajouter Ou Supprimer Une Application](https://support.jumpseat.io/article/how-to-add-an-application/).

## Configurez la variable [!DNL JumpSeat] integration

Nous vous recommandons de configurer une [!DNL JumpSeat] l’intégration dans les environnements de prévisualisation et de production.

>[!TIP]
>
>Vous devez ajouter et activer deux [!DNL Workfront] applications dans [!DNL JumpSeat]: un pour l’aperçu et un pour la production. Voir [Comment Ajouter Ou Supprimer Une Application](https://support.jumpseat.io/article/how-to-add-an-application/) pour plus d’informations.

Pour configurer la variable [!DNL JumpSeat] intégration :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]**.
1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Système]** > **[!UICONTROL [!DNL JumpSeat]Intégration]**.
1. Saisissez votre **[!UICONTROL [!DNL JumpSeat]URL]**, qui se trouve sur l’icône de votre extension dans [!DNL JumpSeat].

   **Exemple :** [!DNL https]:/{mycompanyname}.jumpsièges.io

1. Saisissez le **[!UICONTROL [!DNL JumpSeat]jeton d’intégration]**. Vous pouvez le trouver sur la page **[!UICONTROL Configuration]** page [!DNL JumpSeat].

   **Exemple :** $2 y$10$BevsKeQ8....OYR.LurSg2U64O

1. Cliquez sur **[!UICONTROL Test de la configuration]**.
1. Choisissez si vous souhaitez que l’intégration soit **[!UICONTROL Actif]** ou **[!UICONTROL Inactif]**.

   >[!IMPORTANT]
   >
   >Le test de configuration réalisé à l&#39;étape 5 doit être effectué avec succès afin d&#39;activer l&#39;intégration.

   ![Page d’intégration Saut de siège](assets/jumpseat-integration-page.png)

1. Cliquer sur **[!UICONTROL Enregistrer]**.

>[!TIP]
>
>Pour plus d’informations sur la configuration de [!DNL JumpSeat] intégration, voir [!DNL JumpSeat] documentation pour [SautSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
