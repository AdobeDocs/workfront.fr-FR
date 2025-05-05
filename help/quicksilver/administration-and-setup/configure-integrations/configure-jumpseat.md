---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurer l’intégration de JumpSeat
description: Vous pouvez intégrer  [!DNL JumpSeat]  à  [!DNL Workfront]  pour créer des conseils personnalisés sur le produit.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Nolan, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 01b7eb79028eb3fe47f988a31cb62ace31bba3f1
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 93%

---

# Configurer l’intégration de JumpSeat

Vous pouvez intégrer [!DNL JumpSeat] à [!DNL Workfront] pour créer des conseils personnalisés sur le produit.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez avoir un plan [!DNL JumpSeat] actif.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p> Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et les administratrices [!DNL Workfront], voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à un utilisateur ou à une utilisatrice un accès administratif complet</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

+++

## Conditions préalables

Avant de commencer, vous devez

* Ajoutez et activez [!DNL Workfront] en tant qu’application dans [!DNL JumpSeat]. Pour plus d’informations, voir [Comment ajouter ou supprimer une application](https://support.jumpseat.io/article/how-to-add-an-application/).

>[!IMPORTANT]
>
>Si vous utilisez l’expérience unifiée Adobe, vous devez utiliser l’URL d’application suivante : `.workfront.adobe.com`.



## Configurer l’intégration de [!DNL JumpSeat]

Nous vous recommandons de configurer une intégration de [!DNL JumpSeat] dans vos environnements de prévisualisation et de production.

>[!TIP]
>
>Vous devez ajouter et activer deux applications [!DNL Workfront] distinctes dans [!DNL JumpSeat] - une pour la prévisualisation et une pour la production. Pour plus d’informations, voir [Comment ajouter ou supprimer une application](https://support.jumpseat.io/article/how-to-add-an-application/).

Pour configurer l’intégration de [!DNL JumpSeat] :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Système]** > **[!UICONTROL [!DNL JumpSeat]Intégration]**.
1. Saisissez votre URL **[!UICONTROL [!DNL JumpSeat]]** qui se trouve sur l’icône de votre extension dans [!DNL JumpSeat].

>[!BEGINSHADEBOX]

**Exemple :**

https://{mycompanyname}.jumpsièges.io

&#x200B;>>

>[!ENDSHADEBOX]

1. Saisissez le jeton de l’intégration **[!UICONTROL [!DNL JumpSeat]]**. Vous pouvez le trouver sur la page **[!UICONTROL Configuration]** dans [!DNL JumpSeat].

   **Exemple :** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. Cliquez sur **[!UICONTROL Tester la configuration]**.
1. Choisissez si vous souhaitez que l’intégration soit **[!UICONTROL Active]** ou **[!UICONTROL Inactive]**.

   >[!IMPORTANT]
   >
   >Le test de configuration effectué à l’étape 5 doit être réussi pour que l’intégration soit activée.

   ![Page d’intégration de JumpSeat](assets/jumpseat-integration-page.png)

1. Cliquer sur **[!UICONTROL Enregistrer]**.

>[!TIP]
>
>Pour plus d’informations sur la configuration de votre intégration [!DNL JumpSeat], voir la [!DNL JumpSeat]documentation de [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
