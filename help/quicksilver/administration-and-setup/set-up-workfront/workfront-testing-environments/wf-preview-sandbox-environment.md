---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Environnement de test d’aperçu  [!DNL Adobe Workfront]
description: L’environnement de test Aperçu Sandbox est un environnement de test qui sert de réplique à votre environnement en ligne. Il est actualisé chaque week-end par Workfront. Les données ajoutées à votre environnement de production le vendredi s’affichent dans votre sandbox d’aperçu le lundi suivant. Tous les modules d’assistance ont accès à cet environnement de test.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 8%

---

# Environnement de test d’aperçu [!DNL Adobe Workfront]

<!-- Audited: 12/2023 -->

Il existe deux environnements de test pour [!DNL Workfront] qui sont des répliques de votre environnement de production [!DNL Workfront] :

* Aperçu d’un environnement de test

  L’environnement de test Aperçu Sandbox est un environnement de test qui sert de réplique de votre environnement en ligne et qui est actualisé chaque week-end par [!DNL Workfront]. Les données ajoutées à votre environnement de production le vendredi s’affichent dans votre sandbox d’aperçu le lundi suivant.

  Tous les modules de prise en charge ont accès à l’environnement de test de prévisualisation.

* Environnement de test d’actualisation personnalisé

  L’environnement de test d’actualisation personnalisée est un environnement de test distinct que vous actualisez manuellement. L’obtention de l’environnement de test d’actualisation personnalisée entraîne des frais supplémentaires. Pour plus d’informations sur cet environnement, voir [L’ [!DNL Adobe Workfront] environnement Sandbox d’actualisation personnalisée](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard] Package de support </strong> </p> </th> 
   <th> <p><strong> Packages d’assistance [!UICONTROL Plus], [!UICONTROL Preferred] et [!UICONTROL Enterprise] </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Aperçu d’un environnement de test</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Sandbox d’actualisation personnalisée</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aperçu d’un environnement de test

L’environnement de test Aperçu sert d’environnement dans lequel les utilisateurs de votre entreprise peuvent tester et utiliser en toute sécurité les données de l’environnement de production sans affecter l’environnement de production.

L’environnement de test Aperçu contient vos données de production réelles. Cependant, il s’actualise chaque week-end afin que les données puissent se trouver jusqu’à une semaine après l’environnement de production. Les éléments créés depuis la dernière actualisation sont placés dans l’environnement Aperçu de l’environnement de test jusqu’à l’actualisation suivante.

Les flux de données sont unidirectionnels, de la production à la prévisualisation, et non inversés. Une actualisation de l’environnement de prévisualisation est toujours planifiée par [!DNL Workfront] chaque week-end.

Preview Sandbox permet également à [!DNL Workfront] de déployer de nouvelles fonctionnalités dans un environnement sécurisé, avant qu’elles ne soient prêtes à être déployées en production. Vous pouvez tester les nouvelles fonctionnalités et donner des commentaires [!DNL Workfront] sur celles-ci en accédant à l’environnement de test de prévisualisation. C’est pourquoi le code de l’environnement de test de prévisualisation est toujours en avance sur le code de production, bien que vos données soient actualisées chaque semaine.

L’environnement d’aperçu est idéal pour exécuter des formations, tester de nouvelles fonctionnalités et déterminer les fonctionnalités de configuration.

>[!NOTE]
>
>Lorsque vous accédez à l’environnement de test Aperçu, remarquez la bannière bleue en haut de l’écran. La bannière ne peut pas être supprimée lorsque vous travaillez dans cet environnement.
>
>Le nom de l’environnement auquel vous accédez (Aperçu) et la version de publication du code s’affichent sur la bannière. Cliquez sur **[!UICONTROL Voir les nouveautés]** pour plus d’informations sur cette version.
>
>![](assets/preview-banner-nwe-350x161.png)

## Accès à l’environnement de test d’aperçu

Par défaut, en tant qu’administrateur [!DNL Workfront], vous avez accès à l’environnement Sandbox [!UICONTROL Preview]. Si vous ne pouvez pas accéder à l’environnement sandbox [!UICONTROL Preview] comme décrit dans cette section, contactez votre administrateur [!DNL Workfront] ou notre équipe d’assistance clientèle.


### Accès à l’environnement de test d’aperçu à partir de l’interface [!DNL Workfront] {#accessing-the-preview-sandbox-from-the-workfront-interface}

En tant qu’administrateur [!DNL Workfront], vous pouvez accéder à l’environnement de test de prévisualisation via l’interface [!DNL Workfront].

Pour accéder à l’environnement de test d’aperçu :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Système]** > **[!UICONTROL Préférences]**.

1. Dans la section **[!UICONTROL Test Environments]**, cliquez sur **[!UICONTROL Sandbox Preview]**.

1. Connectez-vous à l’aide de vos informations d’identification d’aperçu.

   Elles doivent être identiques à vos informations d’identification de production, sauf si vous les avez modifiées dans Production après l’actualisation de l’aperçu. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

### Accès à l’environnement de test d’aperçu à l’aide d’une URL {#accessing-the-preview-sandbox-using-a-url}

Vous pouvez accéder à l’onglet Aperçu de l’environnement de test à l’aide d’une URL.

#### Accès à l’aperçu de l’environnement de test pour les comptes sur une grappe 1, 2, 3 et 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

L’URL de l’environnement de test de prévisualisation est : `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Si des signets pointaient vers l’ancienne URL de l’environnement de test d’aperçu, veuillez prendre note de cette modification et mettre à jour l’URL dans vos signets.

Pour vous connecter à l’environnement de test d’aperçu à l’aide d’une URL :

1. Accédez à cette URL : `https://companyname.preview.workfront.com/`.

   Si vous êtes un client EMEA et que votre compte se trouve sur une grappe 4, reportez-vous à la section Accès à l’aperçu sandbox pour les comptes sur une grappe 4 (comptes EMEA) ci-dessous.

1. Connectez-vous à l’aide de vos informations d’identification de prévisualisation.

   >[!TIP]
   >
   >Vos informations d’identification de prévisualisation doivent être identiques à celles de votre production, sauf si vous les avez modifiées dans Production après l’actualisation de prévisualisation. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.


#### Accès à l’environnement de test d’aperçu pour les comptes d’une grappe 4 (comptes EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Pour vous connecter à l’environnement de test d’aperçu à l’aide d’une URL :

1. Accédez à cette URL : `https://companyname.preview.workfront.com/`.

   Vous pouvez également accéder à l’environnement de test de prévisualisation en accédant à [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Connectez-vous à l’aide de vos informations d’identification de prévisualisation.

   Vos informations d’identification de prévisualisation doivent être identiques à celles de votre production, sauf si vous les avez modifiées dans Production après l’actualisation de prévisualisation. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

## Réception d’emails à partir de l’environnement de test de prévisualisation

Workfront désactive toutes les communications par courrier électronique à partir de l’environnement Preview Sandbox. Si vous souhaitez recevoir des notifications par courrier électronique de l’environnement de prévisualisation Sandbox, vous devez activer cette fonctionnalité dans vos paramètres utilisateur. Pour plus d’informations sur l’activation des notifications par courrier électronique dans l’environnement de prévisualisation Sandbox, voir [Activation de la diffusion des emails à partir de l’environnement de prévisualisation Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>La remise des rapports et les notifications push sur l’application mobile sont toujours désactivées pour l’environnement de prévisualisation Sandbox. Ni vous, ni l’administrateur [!DNL Workfront] ne pouvez activer la remise de rapports ou les notifications push pour l’application mobile lorsque vous accédez à l’environnement Preview Sandbox.
>
>Pour plus d’informations sur les diffusions de rapports pour l’environnement de production, voir [Présentation de la diffusion de rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Authentification Single Sign-On (SSO)

Si vous utilisez la connexion unique, travaillez avec notre équipe du service clientèle pour vous assurer qu’elle est correctement configurée afin que vous puissiez utiliser vos informations d’identification SSO pour vous connecter au sandbox [!UICONTROL Preview]. Si votre connexion initiale échoue, contactez votre contact d&#39;assistance classique ou votre administrateur [!DNL Workfront] pour obtenir de l&#39;aide.

Pour plus d’informations sur l’authentification unique, voir [Présentation de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configuration de l’authentification unique dans l’environnement de test de prévisualisation

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées à [!DNL Adobe Admin Console]. Si votre organisation a été intégrée à [!DNL Adobe Admin Console], aucune action n’est nécessaire.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à [!DNL Adobe Admin Console], voir [Différences d’administration basées sur les plateformes ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Si vous souhaitez configurer votre environnement de test de prévisualisation pour qu’il fonctionne avec une solution de connexion unique, vous pouvez le faire en le configurant séparément de votre environnement de production. La configuration SSO dans l’environnement de test de prévisualisation est indépendante de la configuration SSO dans l’environnement de production.

Lorsque votre environnement de test d’aperçu est actualisé (chaque week-end), les informations d’authentification unique ne sont pas copiées à partir de votre environnement de production pour remplacer la configuration de l’environnement de test d’aperçu.

Les étapes de configuration de l’authentification unique dans l’environnement de test de prévisualisation sont similaires à celles de configuration dans l’environnement de production.

Pour plus d’informations sur la configuration de [!DNL Workfront] avec l’authentification unique, voir [Vue d’ensemble de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Prévisualiser les performances et la disponibilité de l’environnement

[!DNL Workfront] Les environnements d’aperçu ne sont pas destinés aux tests de performance ou de chargement. Utilisez plutôt ces environnements pour valider la fonctionnalité avec les workflows existants de votre organisation.

[!DNL Workfront] Les environnements d’aperçu sont conçus pour être toujours disponibles.

Toute panne d’un environnement de prévisualisation [!DNL Workfront] pendant les heures ouvrées normales sera une priorité absolue immédiatement après que tous les problèmes de production seront résolus, le cas échéant.

Toute panne d’un environnement de prévisualisation [!DNL Workfront] le week-end (le samedi et le dimanche) sera corrigée afin que l’environnement soit en cours d’exécution pendant les heures ouvrables le lundi.
