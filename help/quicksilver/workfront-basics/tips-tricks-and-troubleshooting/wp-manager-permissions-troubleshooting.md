---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Dépannage pour les autorisations de gestionnaire d’épreuve Workfront
description: Les profils d’autorisation disponibles dans  [!DNL Adobe] Workfront pour les utilisateurs de la vérification sont Administrateur, Superviseur et Gestionnaire.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---

# Résolution des problèmes d’autorisations [!UICONTROL [!DNL Workfront] du Gestionnaire de BAT]

Vous trouverez ci-dessous les profils d’autorisation disponibles dans [!DNL Adobe Workfront] pour les utilisateurs de la vérification :

* [!UICONTROL Administrateur]
* [!UICONTROL Superviseur]
* [!UICONTROL Manager]

<!--For detailed information about these options and how to configure them, see .-->

Lors de l’octroi d’autorisations [!UICONTROL Manager] à un utilisateur, les informations de dépannage suivantes sont disponibles :

* **PROBLÈME :** Les utilisateurs disposant des autorisations [!UICONTROL Manager] ne peuvent pas afficher les bons à tirer créés par d’autres utilisateurs. À la place, ils voient l’écran [!UICONTROL Accès refusé].

  ![](assets/access-denied-350x161.png)

  **SOLUTION :** Les utilisateurs disposant des autorisations [!UICONTROL Manager] doivent être explicitement ajoutés aux bons à tirer. Les bons à tirer doivent toujours être créés à partir de la fenêtre [!UICONTROL Options de vérification avancées] et les utilisateurs doivent toujours être ajoutés à partir de cette option.

* **PROBLÈME :** Les utilisateurs disposant des autorisations [!UICONTROL Manager] ne peuvent pas ajouter de versions de BAT aux bons à tirer créés par d’autres utilisateurs (ils peuvent éventuellement envoyer un BAT dans l’ensemble de documents, mais les versions ne seraient PAS connectées à l’ensemble d’origine créé par un autre utilisateur).\
   **SOLUTION :** Les utilisateurs disposant d’autorisations [!UICONTROL Manager] peuvent envoyer les versions au BAT d’un autre utilisateur uniquement si l’utilisateur disposant d’autorisations [!UICONTROL Manager] lorsque les deux conditions suivantes sont réunies :

   * Explicitement ajouté aux bons à tirer
   * Défini comme [!UICONTROL Auteurs] (rôle de BAT) sur les bons à tirer

* **PROBLÈME :** Les utilisateurs disposant des autorisations [!UICONTROL Manager] ne peuvent pas modifier les commentaires d’autres utilisateurs sur un BAT qu’ils ne détiennent pas ou qu’ils n’ont pas créé.\
   **SOLUTION :** Si les utilisateurs disposant des autorisations [!UICONTROL Manager] ne possèdent pas les bons à tirer, mais doivent pouvoir modifier les commentaires, ajoutez-les en tant que [!UICONTROL Auteurs] (ou [!UICONTROL Modérateurs]).\
   Ces trois types d’autorisations sont disponibles dans [!DNL Workfront] pour les licences de type [!UICONTROL Planner], [!UICONTROL Worker], [!UICONTROL Requester], [!UICONTROL Reviewer]. L’administrateur système ou l’administrateur utilisateur de [!DNL Workfront] peut modifier les profils des utilisateurs et y ajuster les autorisations [!DNL Workfront Proof].
