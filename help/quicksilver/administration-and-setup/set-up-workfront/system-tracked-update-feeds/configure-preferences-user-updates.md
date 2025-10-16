---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurer des préférences pour les mises à jour utilisateur
description: Vous pouvez configurer des préférences qui permettent d’accéder à certaines fonctionnalités lorsque les utilisateurs et les utilisatrices ajoutent des commentaires dans la zone [!UICONTROL Mises à jour] d’un objet.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 80%

---

# Configurer les préférences pour les mises à jour des utilisateurs et utilisatrices

<!--Audited: 08/2025-->

Vous pouvez configurer des préférences permettant aux utilisateurs et aux utilisatrices d’accéder à certaines fonctionnalités lorsqu’ils ajoutent des commentaires dans la zone [!UICONTROL Mises à jour] d’un objet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td><p>Administrateur système, pour effectuer ces étapes au niveau du système. </p>
   <p>Planificateur, pour effectuer ces étapes pour un groupe, en plus d’être le responsable de ce groupe.</p></td>
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>To perform these steps at the system level, you need the [!UICONTROL System Administrator] access level.</p><p>To perform them for a group, you must be a manager of that group.</p></td>
  </tr> 
 </tbody> 
</table>-->

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
