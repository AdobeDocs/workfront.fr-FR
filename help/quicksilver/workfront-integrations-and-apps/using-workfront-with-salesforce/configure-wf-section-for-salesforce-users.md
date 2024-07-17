---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configuration de la section  [!DNL Adobe Workfront] pour les utilisateurs  [!DNL Salesforce]
description: Après avoir installé  [!DNL Adobe Workfront]  pour Salesforce en tant qu’administrateur  [!DNL Workfront] , vous pouvez le rendre disponible pour vos utilisateurs en l’ajoutant dans une nouvelle section à leurs mises en page d’opportunités et de compte dans Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 5%

---

# Configuration de la section [!DNL Adobe Workfront] pour les utilisateurs [!DNL Salesforce]

Un abonnement [!UICONTROL Pro] [!DNL Workfront] est requis pour utiliser cette fonctionnalité. Pour plus d’informations sur les différents plans disponibles, voir [[!DNL Workfront] Plans.](https://www.workfront.com/plans?lang=fr)

Après avoir installé [!DNL Adobe Workfront] pour [!DNL Salesforce] en tant qu&#39;administrateur [!DNL Workfront], vous pouvez le rendre disponible pour vos utilisateurs en l&#39;ajoutant dans une nouvelle section à leurs [!UICONTROL opportunités] et [!UICONTROL Compte].
dispositions de page dans [!UICONTROL Salesforce].

Pour plus d&#39;informations sur l&#39;installation de [!DNL Workfront for Salesforce], voir [Installation [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Pour que les utilisateurs disposent de [!DNL Workfront] dans les structures [!DNL Classic] et [!DNL Lightning Experience], vous devez ajouter les pages [!DNL WorkfrontOpportunities] et [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] aux mises en page [!UICONTROL Opportunity] et [!UICONTROL Comptes], respectivement.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

* Vous devez disposer d’une instance [!DNL Salesforce] ayant accès à un compte administrateur système.
* Vous devez disposer d’une instance [!DNL Workfront] ayant accès à un compte administrateur système.

## Configuration de la section [!DNL Workfront] dans la structure [!DNL Salesforce Classic]

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur Workfront.
1. Cliquez sur **[!UICONTROL Setup].**
1. Dans la section **[!UICONTROL Build]**, développez **[!UICONTROL Customize].**

1. Développez **[!UICONTROL Opportunités]**, puis cliquez sur **[!UICONTROL Mises en page]** pour ajouter la section [!DNL Workfront] à une Opportunité.

   Ou

   Développez **[!UICONTROL Comptes]**, puis cliquez sur **[!UICONTROL Mises en page]** pour ajouter la section [!DNL Workfront] à un compte.
.

1. Cliquez sur **[!UICONTROL Modifier]** sur une disposition existante.

   Ou

   Cliquez sur **[!UICONTROL Nouveau]** pour ajouter une nouvelle mise en page.

1. (Facultatif) Faites glisser le composant **[!UICONTROL Section]** vers la disposition et déposez-le à l’emplacement de votre choix.\

1. (Facultatif) Attribuez un nom à la nouvelle section.

   Nous vous recommandons de nommer cette section **[!DNL Workfront]**.

1. (Facultatif) Spécifiez la **[!UICONTROL mise en page]** et l’**[!UICONTROL ordre de tabulation]** de votre choix pour la nouvelle section.

   Nous vous recommandons de sélectionner la disposition **[!UICONTROL 1-Column]** pour la section [!DNL Workfront].

1. Cliquez sur **[!UICONTROL OK]**.
1. Dans la zone **[!UICONTROL Disposition]**, cliquez sur **[!UICONTROL Pages Visualforce].**

1. Faites glisser et déposez le composant **[!UICONTROL WorkfrontOpportunities]** dans la nouvelle section de la disposition **[!UICONTROL Opportunités]**.

   Ou

   Faites glisser et déposez le composant **[!UICONTROL WorkfrontComptes]** dans la nouvelle section de la disposition **[!UICONTROL Compte]**.\

1. Cliquez sur l’icône **[!UICONTROL Propriétés]** en haut à droite du nouveau composant ajouté.\

1. Pour obtenir un affichage optimal, spécifiez les propriétés suivantes pour la page [!DNL Workfront Visualforce] :

   * **[!UICONTROL Largeur (en pixels ou %)]** : 100 %
   * **[!UICONTROL Hauteur (en pixels)]** : 600
   * Sélectionnez **[!UICONTROL Afficher les barres de défilement]**.

1. Cliquez sur **[!UICONTROL OK]**.
1. Cliquez sur **[!UICONTROL Enregistrer]** pour enregistrer votre mise en page.

   Tous les utilisateurs auxquels cette disposition est affectée peuvent désormais voir la section [!DNL Workfront] sur leurs objets [!UICONTROL Opportunités] ou [!UICONTROL Comptes] .

   Un écran de connexion [!DNL Workfront] s’affiche dans la section [!DNL Workfront] des utilisateurs. S’ils ne disposent pas d’un compte [!DNL Workfront], ils peuvent réduire la section, mais ne pas la supprimer de leur mise en page.

## Configuration de la section [!DNL Workfront] dans la structure [!DNL Salesforce Lightning Experience]

Vous pouvez ajouter la section [!DNL Workfront] à la disposition d&#39;un [!DNL Salesforce] [!UICONTROL Opportunity] ou d&#39;un compte
dans la structure [!DNL Salesforce Lightning Experience] en accédant à la zone [!UICONTROL Setup] ou à partir d’un compte
ou l’objet [!UICONTROL Opportunity] .

* [Configurez la section  [!DNL Workfront] au niveau de la [!UICONTROL configuration]](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configuration de la section  [!DNL Workfront] au niveau de l’opportunité ou du compte](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configurez la section [!DNL Workfront] au niveau [!UICONTROL Setup] {#configure-the-workfront-section-at-the-setup-level}

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur système.
1. Cliquez sur l&#39;icône **[!UICONTROL Setup]** , puis sur **[!UICONTROL Setup]**.

1. Développez **[!UICONTROL Objet et champs]**, puis cliquez sur **[!UICONTROL Gestionnaire d’objets]**.

1. Cliquez sur **[!UICONTROL Opportunity]** pour personnaliser la disposition d&#39;une opportunité.

   Ou

   Cliquez sur **[!UICONTROL Compte]** pour personnaliser la mise en page d’un compte.

1. Cliquez sur **[!UICONTROL Mise en page de page]**.
1. Cliquez sur le nom d’une mise en page existante pour la modifier.

   Ou

   Cliquez sur **[!UICONTROL Nouveau]** pour créer une mise en page.

1. Passez à la [section [!DNL Workfront] au niveau de l’opportunité ou du compte](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) ci-dessous.

### Configurez la section [!DNL Workfront] au niveau de l&#39;opportunité ou du compte {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur système.
1. Accédez à une **[!UICONTROL opportunité]** ou à un **[!UICONTROL compte]**.

1. Cliquez sur l’icône **[!UICONTROL Setup]** , puis sur **[!UICONTROL Edit Page]**.\

1. Développez la section **[!UICONTROL Custom-Managed]** .
1. Faites glisser et déposez le composant **[!DNL Workfront]** sur votre [!UICONTROL Opportunity] ou votre compte
page.

   Nous vous recommandons d’utiliser la largeur totale de la page pour la section [!DNL Workfront] au lieu de l’une des colonnes de la mise en page.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Tous les utilisateurs auxquels cette disposition est affectée peuvent désormais voir la section [!DNL Workfront] sur leurs objets [!UICONTROL Opportunités] ou [!UICONTROL Comptes] .

   >[!NOTE]
   >
   >Un écran de connexion [!DNL Workfront] s’affiche dans la section [!DNL Workfront] des utilisateurs. S’ils ne disposent pas d’un compte [!DNL Workfront], ils peuvent réduire la section, mais ne pas la supprimer de leur mise en page. Les utilisateurs peuvent se connecter à l’aide de la méthode d’authentification que vous avez activée : Authentification améliorée ou l’URL SAML (Security Assertion Markup Language).

