---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurer les préférences pour les mises à jour des utilisateurs et utilisatrices
description: Vous pouvez configurer des préférences qui permettent d’accéder à certaines fonctionnalités lorsque les utilisateurs et les utilisatrices ajoutent des commentaires dans la zone [!UICONTROL Mises à jour] d’un objet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: fd876089c964d57224452023b4656cd6df40b5a3
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 100%

---

# Configurer les préférences pour les mises à jour des utilisateurs et utilisatrices

Vous pouvez configurer des préférences permettant aux utilisateurs et aux utilisatrices d’accéder à certaines fonctionnalités lorsqu’ils ajoutent des commentaires dans la zone [!UICONTROL Mises à jour] d’un objet.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès [!UICONTROL System Administrator].</p><p>Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas accès, demandez à la personne administratrice [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour plus d’informations sur la manière dont un un administrateur ou une administratrice de [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Autoriser les utilisateurs et les utilisatrices à ajouter des images dans les mises à jour

Par défaut, les utilisateurs et utilisatrices ne peuvent pas ajouter d’images dans les mises à jour. Lorsque vous activez cette préférence, les utilisateurs et utilisatrices pourront joindre des images dans les mises à jour. La préférence s’applique à toutes les mises à jour dans toutes les zones de votre instance [!DNL Workfront].

>[!NOTE]
>
>* Les images enregistrées dans les mises à jour sont prises en compte dans la limite de stockage des documents. Pour plus d’informations, voir [Vérifier les limites de stockage des documents](../../../documents/managing-documents/check-document-storage.md).
>* Les images sont accessibles via l’onglet [!UICONTROL Mises à jour] d’un objet et sont également disponibles dans la zone [!UICONTROL Documents] sous le [!UICONTROL menu principal].
>

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).
1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Interface]** > **[!UICONTROL Mettre à jour les flux]**.
1. Sélectionnez l’onglet **[!UICONTROL Préférences]**.

   ![Préférences utilisateur pour les flux de mise à jour](assets/updatefeeds-preferences-350x137.png)

1. Cochez la case **[!UICONTROL Autoriser les utilisateurs et les utilisatrices à ajouter des images dans les mises à jour]**.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

   Lorsque cette préférence est activée, vous pouvez la désactiver à tout moment. Les images déjà publiées dans les mises à jour resteront dans la zone [!UICONTROL Mises à jour] de l’objet.
