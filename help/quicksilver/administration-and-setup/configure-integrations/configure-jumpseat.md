---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurer l’intégration de JumpSeat
description: Vous pouvez intégrer  [!DNL JumpSeat] à  [!DNL Workfront] pour créer des conseils personnalisés et intégrés au produit.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 24%

---

# Configurer l’intégration de JumpSeat

Vous pouvez intégrer [!DNL JumpSeat] à [!DNL Workfront] pour créer des conseils personnalisés et intégrés au produit.

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
   <td>Vous devez avoir un plan [!DNL JumpSeat] actif.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p> Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et les administratrices [!DNL Workfront], voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à un utilisateur ou à une utilisatrice un accès administratif complet</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Avant de commencer, vous devez

* Ajoutez et activez [!DNL Workfront] en tant qu&#39;application dans [!DNL JumpSeat]. Pour Plus D’Informations, Voir [Comment Ajouter Ou Supprimer Une Application](https://support.jumpseat.io/article/how-to-add-an-application/).

## Configuration de l’intégration [!DNL JumpSeat]

Nous vous recommandons de configurer une intégration [!DNL JumpSeat] dans vos environnements Aperçu et Production.

>[!TIP]
>
>Vous devez ajouter et activer deux applications [!DNL Workfront] distinctes dans [!DNL JumpSeat] : une pour l’aperçu et une pour la production. Pour plus d’informations, voir [Comment Ajouter Ou Supprimer Une Application](https://support.jumpseat.io/article/how-to-add-an-application/) .

Pour configurer l’intégration [!DNL JumpSeat] :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]**.
1. Dans le panneau de gauche, cliquez sur **[!UICONTROL System]** > **[!UICONTROL [!DNL JumpSeat]Integration]**.
1. Saisissez votre **[!UICONTROL [!DNL JumpSeat]URL]**, qui se trouve sur l’icône de votre extension dans [!DNL JumpSeat].

   **Exemple :** [!DNL https]://{mycompanyname}.jumpsièges.io

1. Saisissez le jeton d’intégration **[!UICONTROL [!DNL JumpSeat]]**. Vous pouvez le trouver sur la page **[!UICONTROL Configuration]** dans [!DNL JumpSeat].

   **Exemple :** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. Cliquez sur **[!UICONTROL Test de la configuration]**.
1. Choisissez si vous souhaitez que l’intégration soit **[!UICONTROL Active]** ou **[!UICONTROL Inactive]**.

   >[!IMPORTANT]
   >
   >Le test de configuration réalisé à l&#39;étape 5 doit être effectué avec succès afin d&#39;activer l&#39;intégration.

   ![}Page d’intégration JumpSeat](assets/jumpseat-integration-page.png)

1. Cliquer sur **[!UICONTROL Enregistrer]**.

>[!TIP]
>
>Pour plus d’informations sur la configuration de votre intégration [!DNL JumpSeat], consultez la documentation [!DNL JumpSeat] pour [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
