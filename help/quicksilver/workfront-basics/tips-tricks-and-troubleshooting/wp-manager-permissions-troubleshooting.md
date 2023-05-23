---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Résolution des problèmes d’autorisations de Workfront BAT Manager
description: Les profils d’autorisation disponibles dans [!DNL Adobe] Les utilisateurs de la vérification Workfront sont administrateurs, superviseurs et gestionnaires.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] Gestionnaire de BAT] dépannage des autorisations

Vous trouverez ci-dessous les profils d’autorisation disponibles dans [!DNL Adobe Workfront] pour les utilisateurs de la vérification :

* [!UICONTROL Administrateur]
* [!UICONTROL Superviseur]
* [!UICONTROL Gestionnaire]

<!--For detailed information about these options and how to configure them, see .-->

Lors de l’octroi d’un utilisateur [!UICONTROL Manager] autorisations, les informations de dépannage suivantes sont disponibles :

* **PROBLÈME :** Utilisateurs avec [!UICONTROL Manager] les autorisations ne peuvent pas afficher les bons à tirer créés par d’autres utilisateurs. Au lieu de cela, ils voient le [!UICONTROL Accès refusé] écran.

   ![](assets/access-denied-350x161.png)

   **SOLUTION :** Utilisateurs avec [!UICONTROL Manager] les autorisations doivent être explicitement ajoutées aux bons à tirer. Les BAT doivent toujours être créés à partir du [!UICONTROL Options de vérification avancées] et les utilisateurs doivent toujours être ajoutés via cette option.

* **PROBLÈME :** Utilisateurs avec [!UICONTROL Manager] les autorisations ne peuvent pas ajouter de versions de BAT aux BAT créés par d’autres utilisateurs (ils peuvent éventuellement envoyer un BAT dans l’ensemble de documents, mais les versions ne seraient PAS connectées à l’ensemble d’origine créé par un autre utilisateur).\
   **SOLUTION :** Utilisateurs avec [!UICONTROL Manager] les autorisations ne peuvent envoyer les versions au BAT d’un autre utilisateur que si l’utilisateur dispose de [!UICONTROL Manager] les autorisations lorsque les deux éléments suivants :

   * Explicitement ajouté aux bons à tirer
   * Définissez comme [!UICONTROL Auteurs] (rôle de BAT) sur les BAT

* **PROBLÈME :** Utilisateurs avec [!UICONTROL Manager] les autorisations ne peuvent pas modifier les commentaires d’autres utilisateurs sur un BAT qu’ils ne possèdent pas ou qu’ils n’ont pas créé.\
   **SOLUTION :** Si les utilisateurs utilisent [!UICONTROL Manager] les autorisations ne sont pas propriétaires des bons à tirer, mais elles doivent pouvoir modifier les commentaires, les ajouter en tant que [!UICONTROL Auteurs] (ou [!UICONTROL Modérateurs]).\
   Ces trois types d’autorisations sont disponibles dans la section [!DNL Workfront] pour [!UICONTROL Planificateur], [!UICONTROL Worker], [!UICONTROL Demandeur], [!UICONTROL Réviseur] de type licences. Administrateur système ou administrateur utilisateur dans [!DNL Workfront] peut modifier les profils des utilisateurs et ajuster les [!DNL Workfront Proof] autorisations de là-bas.
