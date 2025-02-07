---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurer des préférences pour les mises à jour utilisateur
description: Vous pouvez configurer des préférences qui permettent d’accéder à certaines fonctionnalités lorsque les utilisateurs et les utilisatrices ajoutent des commentaires dans la zone [!UICONTROL Mises à jour] d’un objet.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 91%

---

# Configurer les préférences pour les mises à jour des utilisateurs et utilisatrices

Vous pouvez configurer des préférences permettant aux utilisateurs et aux utilisatrices d’accéder à certaines fonctionnalités lorsqu’ils ajoutent des commentaires dans la zone [!UICONTROL Mises à jour] d’un objet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   Ou
   <p>Actuelle : [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td><p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès [!UICONTROL System Administrator].</p><p>Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Autoriser les utilisateurs et les utilisatrices à ajouter des images dans les mises à jour

Par défaut, les utilisateurs et utilisatrices ne peuvent pas ajouter d’images dans les mises à jour. Lorsque vous activez cette préférence, les utilisateurs et utilisatrices pourront joindre des images dans les mises à jour. La préférence s’applique à toutes les mises à jour dans toutes les zones de votre instance [!DNL Workfront].

>[!NOTE]
>
>* Les images enregistrées dans les mises à jour sont prises en compte dans la limite de stockage des documents. Pour plus d’informations, voir [Vérifier les limites de stockage des documents](../../../documents/managing-documents/check-document-storage.md).
>* Les images sont accessibles via l’onglet [!UICONTROL Mises à jour] d’un objet et sont également disponibles dans la zone [!UICONTROL Documents] sous le [!UICONTROL menu principal].
>

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![Icône des paramètres d’engrenage](assets/gear-icon-settings.png).
1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Interface]** > **[!UICONTROL Mettre à jour les flux]**.
1. Sélectionnez l’onglet **[!UICONTROL Préférences]**.

   ![Préférences utilisateur pour les flux de mise à jour](assets/updatefeeds-preferences-350x137.png)

1. Cochez la case **[!UICONTROL Autoriser les utilisateurs et les utilisatrices à ajouter des images dans les mises à jour]**.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

   Lorsque cette préférence est activée, vous pouvez la désactiver à tout moment. Les images déjà publiées dans les mises à jour resteront dans la zone [!UICONTROL Mises à jour] de l’objet.
