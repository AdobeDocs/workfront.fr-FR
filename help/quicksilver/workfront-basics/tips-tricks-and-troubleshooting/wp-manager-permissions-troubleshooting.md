---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Résolution des problèmes d’autorisations de gestion Workfront Proof
description: Les profils d’autorisation disponibles dans  [!DNL Adobe]  Workfront pour les utilisateurs et utilisatrices de la relecture Workfront sont Administration, Supervision et Gestion.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 100%

---

# Résolutions des problèmes d’autorisations de gestion [!UICONTROL [!DNL Workfront] Proof]

Vous trouverez ci-dessous les profils d’autorisation disponibles dans [!DNL Adobe Workfront] pour les utilisateurs et utilisatrices de la relecture :

* [!UICONTROL Administration]
* [!UICONTROL Superviseur ou superviseuse]
* [!UICONTROL Gestion]

<!--For detailed information about these options and how to configure them, see .-->

Lorsqu’un utilisateur ou une utilisatrice reçoit les autorisations de [!UICONTROL gestion], les informations de dépannage suivantes sont disponibles :

* **PROBLÈME :** les utilisateurs et utilisatrices avec des autorisations de [!UICONTROL gestion] ne peuvent pas afficher les épreuves créées par d’autres personnes. Au lieu de cela, ils voient l’écran [!UICONTROL Accès refusé].

  ![](assets/access-denied-350x161.png)

  **SOLUTION :** les utilisateurs et utilisatrices avec des autorisations de [!UICONTROL gestion] doivent être explicitement ajoutés aux épreuves. Les épreuves doivent toujours être créées à partir des [!UICONTROL Options de relecture avancée] et les utilisateurs et utilisatrices doivent toujours être ajoutés via cette option.

* **PROBLÈME :** les utilisateurs et utilisatrices avec des autorisations de [!UICONTROL gestion] ne peuvent pas ajouter de versions aux épreuves créées par d’autres personnes (ils peuvent éventuellement envoyer une épreuve dans l’ensemble de documents, mais les versions ne seraient PAS connectées à l’ensemble d’origine créé par une autre personne).\
   **SOLUTION :** les personnes avec des autorisations de [!UICONTROL gestion] ne peuvent envoyer les versions à l’épreuve d’une autre personne que si les personnes disposant des autorisations de [!UICONTROL gestion] remplissent les deux conditions suivantes :

   * Elles ont été explicitement ajoutées aux épreuves.
   * Elles ont été définies comme [!UICONTROL Auteurs et autrices] (rôle d’épreuve) sur les épreuves.

* **PROBLÈME :** les utilisateurs et utilisatrices avec des autorisations de [!UICONTROL gestion] ne peuvent pas modifier les commentaires d’autres personnes sur une épreuve qu’ils ne possèdent pas ou qu’ils n’ont pas créée.\
   **SOLUTION :** si les utilisateurs et utilisatrices disposant d’autorisations de [!UICONTROL gestion] ne sont pas propriétaires des épreuves, mais qu’ils doivent pouvoir modifier les commentaires, ajoutez-les en tant qu’[!UICONTROL Auteurs et autrices] (ou [!UICONTROL Modérateurs et modératrices]).\
   Ces trois types d’autorisations sont disponibles dans [!DNL Workfront] pour les types de licences [!UICONTROL Planification], [!UICONTROL Personne employée], [!UICONTROL Demande], [!UICONTROL Révision]. Les administrateurs et administratrices système ou des utilisateurs et utilisatrices dans [!DNL Workfront] peuvent modifier les profils des utilisateurs et utilisatrices et ajuster les autorisations [!DNL Workfront Proof] à partir des profils.
