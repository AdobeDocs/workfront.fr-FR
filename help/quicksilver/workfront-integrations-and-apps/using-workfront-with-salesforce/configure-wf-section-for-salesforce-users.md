---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: 'Configurer la section  [!DNL Adobe Workfront]  pour les utilisateurs et utilisatrices  [!DNL Salesforce] '
description: Après l’installation d’ [!DNL Adobe Workfront]  pour Salesforce en tant qu’administrateur ou administratrice de  [!DNL Workfront] , vous pouvez le mettre à la disposition de vos utilisateurs et utilisatrices en l’ajoutant dans une nouvelle section de leurs dispositions de page Opportunité et Compte dans Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 100%

---

# Configurer la section [!DNL Adobe Workfront] pour les utilisateurs et utilisatrices [!DNL Salesforce]

Un plan [!DNL Workfront] [!UICONTROL Pro] est requis pour l’utilisation de cette fonctionnalité. Pour plus d’informations sur les différents plans disponibles, voir [[!DNL Workfront] Plans](https://business.adobe.com/products/workfront/pricing.html).

Après l’installation d’[!DNL Adobe Workfront] pour [!DNL Salesforce] en tant qu’administrateur ou administratrice de [!DNL Workfront], vous pouvez le mettre à la disposition de vos utilisateurs et utilisatrices en l’ajoutant dans une nouvelle section de leurs dispositions de page [!UICONTROL Opportunité] et [!UICONTROL Compte] dans [!UICONTROL Salesforce].

Pour plus d’informations sur l’installation de [!DNL Workfront for Salesforce], voir [Installer  [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Afin que les utilisateurs et utilisatrices puissent disposer à la fois des frameworks [!DNL Classic] et [!DNL Lightning Experience] de [!DNL Workfront], vous devez ajouter les pages [!DNL WorkfrontOpportunities] et [!UICONTROL Visualforce] [!DNL WorkfrontAccounts] aux dispositions des pages [!UICONTROL Opportunité] et [!UICONTROL Comptes], respectivement.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des accès suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

* Vous devez disposer d’une instance [!DNL Salesforce] offrant l’accès à un compte d’administrateur ou d’administratrice système.
* Vous devez disposer d’une instance [!DNL Workfront] offrant l’accès à un compte d’administrateur ou d’administratrice système.

## Configurer la section [!DNL Workfront] dans le framework [!DNL Salesforce Classic]

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur ou administratrice de Workfront.
1. Cliquez sur **[!UICONTROL Configuration].**
1. Dans la section **[!UICONTROL Version]**, développez **[!UICONTROL Personnaliser].**

1. Développez **[!UICONTROL Opportunités]**, puis cliquez sur **[!UICONTROL Dispositions des pages]** pour ajouter la section [!DNL Workfront] à une opportunité.

   Ou

   Développez **[!UICONTROL Comptes]**, puis cliquez sur **[!UICONTROL Disposition des pages]** pour ajouter la section [!DNL Workfront] à un compte.

1. Cliquez sur **[!UICONTROL Modifier]** sur une disposition existante.

   Ou

   Cliquez sur **[!UICONTROL Nouveau]** pour ajouter une nouvelle disposition.

1. (Facultatif) Faites glisser le composant **[!UICONTROL Section]** dans la disposition et déposez-le à l’emplacement souhaité.

1. (Facultatif) Saisissez un nom pour la nouvelle section.

   Nous vous recommandons de nommer cette section **[!DNL Workfront]**.

1. (Facultatif) Indiquez la **[!UICONTROL disposition]** et l’**[!UICONTROL ordre de touche de tabulation]** souhaités pour la nouvelle section.

   Nous vous recommandons de sélectionner la disposition **[!UICONTROL 1 colonne]** pour la section [!DNL Workfront].

1. Cliquez sur **[!UICONTROL OK]**.
1. Dans la zone **[!UICONTROL Disposition]**, cliquez sur **[!UICONTROL Pages Visualforce].**

1. Faites glisser et déposez le composant **[!UICONTROL WorkfrontOpportunities]** vers la nouvelle section dans la disposition **[!UICONTROL Opportunités]**.

   Ou

   Faites glisser et déposez le composant **[!UICONTROL WorkfrontAccounts]** vers la nouvelle section dans la disposition **[!UICONTROL Compte]**.

1. Cliquez sur l’icône **[!UICONTROL Propriétés]** dans le coin supérieur droit du composant nouvellement ajouté.

1. Pour obtenir un affichage optimal, spécifiez les propriétés suivantes pour la page [!DNL Workfront Visualforce] :

   * **[!UICONTROL Largeur (en pixels ou en %)]** : 100 %
   * **[!UICONTROL Hauteur (en pixels)]** : 600
   * Sélectionnez **[!UICONTROL Afficher les barres de défilement]**.

1. Cliquez sur **[!UICONTROL OK]**.
1. Cliquez sur **[!UICONTROL Enregistrer]** pour enregistrer votre disposition.

   Tous les utilisateurs et utilisatrices auxquels cette disposition est affectée peuvent désormais consulter la section [!DNL Workfront] de leurs objets [!UICONTROL Opportunités] ou [!UICONTROL Comptes].

   Les utilisateurs et utilisatrices voient un écran de connexion [!DNL Workfront] dans la section [!DNL Workfront]. S’ils n’ont pas de compte [!DNL Workfront], ils peuvent réduire la section, mais pas la supprimer de leur disposition.

## Configurer la section [!DNL Workfront] dans le framework [!DNL Salesforce Lightning Experience]

Vous pouvez ajouter la section [!DNL Workfront] à la disposition d’une [!UICONTROL opportunité] ou d’un compte [!DNL Salesforce] dans le framework [!DNL Salesforce Lightning Experience] en accédant à la zone [!UICONTROL Configuration] ou à partir d’un compte ou d’un objet [!UICONTROL Opportunité] .

* [Configurer la section  [!DNL Workfront]  au niveau de la [!UICONTROL configuration]](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configurer la section  [!DNL Workfront]  au niveau de l’opportunité ou du compte](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configurer la section [!DNL Workfront] au niveau de la [!UICONTROL configuration] {#configure-the-workfront-section-at-the-setup-level}

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur ou administratrice système.
1. Cliquez sur l’icône **[!UICONTROL Configuration]**, puis sur **[!UICONTROL Configuration]**.

1. Développer **[!UICONTROL Objet et champs]**, puis cliquez sur **[!UICONTROL Object Manager]**.

1. Cliquez sur **[!UICONTROL Opportunité]** pour personnaliser la disposition d’une opportunité.

   Ou

   Cliquez sur **[!UICONTROL Compte]** pour personnaliser la disposition d’un compte.

1. Cliquez sur **[!UICONTROL Dispositions de page]**.
1. Cliquez sur le nom d’une disposition existante pour la modifier.

   Ou

   Cliquez sur **[!UICONTROL Nouveau]** pour créer une disposition.

1. Passez à [Configurer la section  [!DNL Workfront]  au niveau de l’opportunité ou du compte](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) ci-dessous.

### Configurer la section [!DNL Workfront] au niveau de l’opportunité ou du compte {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Connectez vous à [!DNL Salesforce] en tant que personne responsable de l’administration du système.
1. Accédez à une **[!UICONTROL Opportunité]** ou à un **[!UICONTROL Compte]**.

1. Cliquez sur l’icône **[!UICONTROL Configuration]**, puis sur **[!UICONTROL Modifier la page]**.

1. Développez la section **[!UICONTROL Gestion personnalisée]**.
1. Faites glisser et déposez la composante **[!DNL Workfront]** sur votre page [!UICONTROL Opportunité] ou Compte.

   Nous vous conseillons d’utiliser toute la largeur de la page pour la section [!DNL Workfront] au lieu d’une des colonnes de la disposition.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Désormais, l’ensemble des utilisateurs et des utilisatrices à qui cette disposition est affectée peuvent voir la section [!DNL Workfront] de leurs objets [!UICONTROL Opportunités] ou [!UICONTROL Comptes].

   >[!NOTE]
   >
   >Les utilisateurs et les utilisatrices voient un écran de connexion [!DNL Workfront] sur la section [!DNL Workfront]. S’ils n’ont pas de compte [!DNL Workfront], ils peuvent réduire la section sans pour autant la supprimer de leur disposition. Les utilisateurs et utilisatrices peuvent se connecter à l’aide de la méthode d’authentification que vous avez activée : authentification améliorée ou authentification SAML (Security Assertion Markup Language).

