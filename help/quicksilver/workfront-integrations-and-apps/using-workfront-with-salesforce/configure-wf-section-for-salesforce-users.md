---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configurez la variable [!DNL Adobe Workfront] section pour [!DNL Salesforce] utilisateurs
description: Après l’installation [!DNL Adobe Workfront] pour Salesforce as a [!DNL Workfront] Pour les administrateurs, vous pouvez les mettre à la disposition de vos utilisateurs en les ajoutant dans une nouvelle section aux mises en page de page Opportunité et Compte dans Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# Configurez la variable [!DNL Adobe Workfront] section pour [!DNL Salesforce] utilisateurs

A [!UICONTROL Pro] [!DNL Workfront] Planifiez l’utilisation de cette fonctionnalité. Pour plus d’informations sur les différents plans disponibles, voir [[!DNL Workfront] Formules.](https://www.workfront.com/plans)

Après l’installation [!DNL Adobe Workfront] pour [!DNL Salesforce] as a [!DNL Workfront] administrateur, vous pouvez le rendre disponible pour vos utilisateurs en l’ajoutant dans une nouvelle section à leur [!UICONTROL Opportunité] et [!UICONTROL Compte]
dispositions de page dans [!UICONTROL Salesforce].

Pour plus d’informations sur l’installation [!DNL Workfront for Salesforce], voir [Installer [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Pour que les utilisateurs puissent [!DNL Workfront] disponibles dans les deux [!DNL Classic] et [!DNL Lightning Experience] frameworks, vous devez ajouter la fonction [!DNL WorkfrontOpportunities] et le [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] à la page [!UICONTROL Opportunité] et [!UICONTROL Comptes] mises en page, respectivement.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

* Vous devez disposer d’un [!DNL Salesforce] avec accès à un compte administrateur système.
* Vous devez disposer d’un [!DNL Workfront] avec accès à un compte administrateur système.

## Configurez la variable [!DNL Workfront] dans la section [!DNL Salesforce Classic] framework

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur Workfront.
1. Cliquez sur **[!UICONTROL Configuration].**
1. Dans le **[!UICONTROL Build]** , développez **[!UICONTROL Personnaliser].**

1. Développer **[!UICONTROL Opportunités]**, puis cliquez sur **[!UICONTROL Disposition de page]** pour ajouter la variable [!DNL Workfront] à une opportunité.

   Ou

   Développer **[!UICONTROL Comptes]**, puis cliquez sur **[!UICONTROL Disposition de page]** pour ajouter la variable [!DNL Workfront] à un compte .

1. Cliquez sur **[!UICONTROL Modifier]** sur une disposition existante.

   Ou

   Cliquez sur **[!UICONTROL Nouveau]** pour ajouter une nouvelle mise en page.

1. (Facultatif) Faites glisser le **[!UICONTROL Section]** à la mise en page et déposez-la à l’emplacement de votre choix.\

1. (Facultatif) Attribuez un nom à la nouvelle section.

   Nous vous recommandons de nommer cette section **[!DNL Workfront]**.

1. (Facultatif) Indiquez le **[!UICONTROL Disposition]** et **[!UICONTROL Ordre de tabulation]** pour la nouvelle section .

   Nous vous recommandons de sélectionner **[!UICONTROL 1 colonne]** de la [!DNL Workfront] .

1. Cliquez sur **[!UICONTROL OK]**.
1. Dans le **[!UICONTROL Disposition]** zone, cliquez sur **[!UICONTROL Pages Visualforce].**

1. Faites glisser et déposez le **[!UICONTROL WorkfrontOpportunities]** à la nouvelle section dans la **[!UICONTROL Opportunités]** Disposition.

   Ou

   Faites glisser et déposez le **[!UICONTROL WorkfrontComptes]** à la nouvelle section dans la  **[!UICONTROL Compte]** Disposition.\

1. Cliquez sur le bouton **[!UICONTROL Propriétés]** en haut à droite du composant nouvellement ajouté.\

1. Pour obtenir un affichage optimal, spécifiez les propriétés suivantes pour la variable [!DNL Workfront Visualforce] page :

   * **[!UICONTROL Largeur (en pixels ou en %)]**: 100 %
   * **[!UICONTROL Hauteur (en pixels)]**: 600
   * Sélectionner **[!UICONTROL Afficher les barres de défilement]**.

1. Cliquez sur **[!UICONTROL OK]**.
1. Cliquez sur **[!UICONTROL Enregistrer]** pour enregistrer votre mise en page.

   Tous les utilisateurs auxquels cette disposition est affectée peuvent désormais voir le [!DNL Workfront] de leur [!UICONTROL Opportunités] ou [!UICONTROL Comptes] objets.

   Les utilisateurs voient une [!DNL Workfront] écran de connexion sur [!DNL Workfront] . S’ils n’ont pas de [!DNL Workfront] , ils peuvent réduire la section, mais pas la supprimer de leur mise en page.

## Configurez la variable [!DNL Workfront] dans la section [!DNL Salesforce Lightning Experience] framework

Vous pouvez ajouter la variable [!DNL Workfront] à la mise en page d’un [!DNL Salesforce] [!UICONTROL Opportunité] ou Compte dans le [!DNL Salesforce Lightning Experience] en accédant à la structure [!UICONTROL Configuration] ou depuis un compte ou [!UICONTROL Opportunité] .

* [Configurez la variable [!DNL Workfront] à l’adresse [!UICONTROL Configuration] level](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configurez la variable [!DNL Workfront] Section au niveau de l’opportunité ou du compte](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configurez la variable [!DNL Workfront] à l’adresse [!UICONTROL Configuration] level {#configure-the-workfront-section-at-the-setup-level}

1. Se connecter [!DNL Salesforce] en tant qu’administrateur système.
1. Cliquez sur le bouton **[!UICONTROL Configuration]** puis cliquez sur **[!UICONTROL Configuration]**.

1. Développer **[!UICONTROL Objet et champs]**, puis cliquez sur **[!UICONTROL Object Manager]**.

1. Cliquez sur **[!UICONTROL Opportunité]** pour personnaliser la disposition d’une opportunité.

   Ou

   Cliquez sur **[!UICONTROL Compte]** pour personnaliser la mise en page d’un compte.

1. Cliquez sur **[!UICONTROL Disposition de page]**.
1. Cliquez sur le nom d’une mise en page existante pour la modifier.

   Ou

   Cliquez sur **[!UICONTROL Nouveau]** pour créer une mise en page.

1. Passez à la [Configurez la variable [!DNL Workfront] Section au niveau de l’opportunité ou du compte](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) ci-dessous.

### Configurez la variable [!DNL Workfront] Section au niveau de l’opportunité ou du compte {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur système.
1. Accédez à un **[!UICONTROL Opportunité]** ou **[!UICONTROL Compte]**.

1. Cliquez sur le bouton **[!UICONTROL Configuration]** puis cliquez sur **[!UICONTROL Modifier la page]**.\

1. Développez l’objet **[!UICONTROL Gestion personnalisée]** .
1. Faites glisser et déposez le **[!DNL Workfront]** sur votre [!UICONTROL Opportunité] ou Page Compte .

   Nous vous recommandons d’utiliser la largeur totale de la page pour la variable [!DNL Workfront] au lieu d’une des colonnes de la mise en page.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Tous les utilisateurs auxquels cette disposition est affectée peuvent désormais voir le [!DNL Workfront] de leur [!UICONTROL Opportunités] ou [!UICONTROL Comptes] objets.

   >[!NOTE]
   >
   >Les utilisateurs voient une [!DNL Workfront] écran de connexion sur [!DNL Workfront] . S’ils n’ont pas de [!DNL Workfront] , ils peuvent réduire la section, mais pas la supprimer de leur mise en page. Les utilisateurs peuvent se connecter à l’aide de la méthode d’authentification que vous avez activée : Amélioration de l’authentification ou de l’URL SAML (Security Assertion Markup Language).

