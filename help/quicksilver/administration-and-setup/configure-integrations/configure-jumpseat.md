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
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 91%

---

# Configurer l’intégration de JumpSeat

Vous pouvez intégrer [!DNL JumpSeat] à [!DNL Workfront] pour créer des conseils personnalisés sur le produit.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table>
  <tr>
   <td>Package Adobe Workfront
   </td>
    <p>Workflow Ultimate</p>
   <td> <p>Prime ou Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Licences Adobe Workfront
   </td>
   <td>Standard
   <p>Plan</p>
   </td>
  </tr>
  </tr>
  <tr>
   <td>Produit
   </td>
   <td>Vous devez avoir un plan [!DNL JumpSeat] actif.
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td>Vous devez être administrateur ou administratrice [!DNL Workfront].
   </td>
  </tr>
</table>

Pour plus d’informations sur ce tableau, voir la section [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

https://{mycompanyname}.jumpseat.io

>>

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
