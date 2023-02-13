---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Le [!DNL Adobe Workfront] Aperçu de l’environnement de test
description: L’environnement de test Aperçu est un environnement de test qui sert de réplique à votre environnement en ligne. Il est actualisé chaque week-end par Workfront. Les données ajoutées à votre environnement de production le vendredi s’affichent dans votre sandbox d’aperçu le lundi suivant. Tous les modules d’assistance ont accès à cet environnement de test.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 0%

---

# Le [!DNL Adobe Workfront] Aperçu de l’environnement de test

Il existe deux environnements de test pour [!DNL Workfront] qui sont des répliques de votre [!DNL Workfront] environnement de production :

* Aperçu d’un environnement de test

   L’environnement de test Aperçu est un environnement de test qui sert de réplique à votre environnement en ligne et qui est actualisé chaque week-end par [!DNL Workfront]. Les données ajoutées à votre environnement de production le vendredi s’affichent dans votre sandbox d’aperçu le lundi suivant.

   Tous les modules de prise en charge ont accès à l’environnement de test de prévisualisation.

* Environnement de test d’actualisation personnalisé

   L’environnement de test d’actualisation personnalisée est un environnement de test distinct que vous actualisez manuellement. L’obtention de l’environnement de test d’actualisation personnalisée entraîne des frais supplémentaires. Pour plus d’informations sur cet environnement, voir [Le [!DNL Adobe Workfront] Environnement Sandbox d’actualisation personnalisée](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Package de prise en charge [!UICONTROL Standard]</strong> </p> </th> 
   <th> <p><strong>Packages d’assistance [!UICONTROL Plus], [!UICONTROL Préférés] et [!UICONTROL Enterprise]</strong> </p> </th> 
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

L’environnement de test d’aperçu contient vos données de production réelles. toutefois, il s’actualise chaque week-end afin que les données puissent se trouver jusqu’à une semaine après l’environnement de production. Les éléments créés depuis la dernière actualisation sont placés dans l’environnement Aperçu de l’environnement de test jusqu’à l’actualisation suivante.

Les flux de données sont unidirectionnels, de la production à la prévisualisation, et non inversés. Une actualisation de l’environnement de prévisualisation est toujours planifiée par [!DNL Workfront] chaque week-end. Pour plus d’informations sur le jour et l’heure spécifiques de l’actualisation, accédez à [status.adobe.com](https://status.adobe.com/fr/).

L’aperçu de l’environnement de test permet également [!DNL Workfront] pour déployer de nouvelles fonctionnalités dans un environnement sécurisé, avant qu’elles ne soient prêtes à être déployées en production. Vous pouvez tester les nouvelles fonctionnalités et leur donner [!DNL Workfront] commentaires sur leurs fonctionnalités en accédant à Preview Sandbox. C’est pourquoi le code de l’environnement de test de prévisualisation est toujours en avance sur le code de production, bien que vos données soient actualisées chaque semaine.

L’environnement d’aperçu est idéal pour exécuter des formations, tester de nouvelles fonctionnalités et déterminer les fonctionnalités de configuration.

>[!NOTE]
>
>Lorsque vous accédez à l’environnement de test Aperçu, remarquez la bannière bleue en haut de l’écran. La bannière ne peut pas être supprimée lorsque vous travaillez dans cet environnement.
>
>Le nom de l’environnement auquel vous accédez (Aperçu) et la version de publication du code s’affichent sur la bannière. Cliquez sur **[!UICONTROL Découvrez les nouveautés]** pour plus d’informations sur cette version.
>
>![](assets/preview-banner-nwe-350x161.png)

## Accès à l’environnement de test d’aperçu

Par défaut, sous la forme [!DNL Workfront] administrateur, vous avez accès au [!UICONTROL Aperçu] Environnement Sandbox. Si vous ne pouvez pas accéder au [!UICONTROL Aperçu] Environnement Sandbox comme décrit dans cette section, contactez votre [!DNL Workfront] ou de notre équipe du service clientèle.

* [Accès à l’environnement de test d’aperçu à partir du [!DNL Workfront] Interface](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [Accès à l’environnement de test d’aperçu à l’aide d’une URL](#accessing-the-preview-sandbox-using-a-url)

### Accès à l’environnement de test d’aperçu à partir du [!DNL Workfront] Interface {#accessing-the-preview-sandbox-from-the-workfront-interface}

Comme [!DNL Workfront] administrateur, vous pouvez accéder à l’environnement de test d’aperçu via le [!DNL Workfront] .

Pour accéder à l’environnement de test d’aperçu :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Système]** > **[!UICONTROL Préférences]**.

1. Dans le **[!UICONTROL Environnements de test]** , cliquez sur **[!UICONTROL Aperçu des environnements de test]**.

1. Connectez-vous à l’aide de vos informations d’identification d’aperçu.

   Elles doivent être identiques à vos informations d’identification de production, sauf si vous les avez modifiées dans Production après l’actualisation de l’aperçu. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

### Accès à l’environnement de test d’aperçu à l’aide d’une URL {#accessing-the-preview-sandbox-using-a-url}

* [Accès à l’aperçu de l’environnement de test pour les comptes sur une grappe 1, 2, 3 et 5](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [Accès à l’environnement de test d’aperçu pour les comptes d’une grappe 4 (comptes EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### Accès à l’aperçu de l’environnement de test pour les comptes sur une grappe 1, 2, 3 et 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

Historiquement, vous avez accédé à l’environnement de test de prévisualisation en accédant à [https://companyname.attasksandbox.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.attasksandbox.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNGTfPKCDnAylzkclNwdSuEXksLFRg).

Cette URL n’est plus prise en charge et n’a pas été redirigée vers notre nouvelle URL pour l’environnement de prévisualisation Sandbox. La nouvelle URL correcte de l’environnement de test d’aperçu est la suivante : [https://companyname.preview.workfront.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.preview.workfront.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNFZQYw9VWjr2tuvQLfSJHneqJj_PQ).

>[!NOTE]
>
>Si des signets pointaient vers l’ancienne URL de l’environnement de test d’aperçu, veuillez prendre note de cette modification et mettre à jour l’URL dans vos signets.

Pour vous connecter à l’environnement de test d’aperçu à l’aide d’une URL :

1. Accédez à cette URL : [[!DNL https]: //companyname.preview.workfront.com/](https://companyname.preview.workfront.com/)

   Si vous êtes un client EMEA et que votre compte se trouve sur une grappe 4, reportez-vous à la section [Accès à l’environnement de test d’aperçu pour les comptes d’une grappe 4 (comptes EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) dans cet article.

1. Connectez-vous à l’aide de vos informations d’identification de prévisualisation.

   Vos informations d’identification de prévisualisation doivent être identiques à celles de votre production, sauf si vous les avez modifiées dans Production après l’actualisation de prévisualisation. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

#### Accès à l’environnement de test d’aperçu pour les comptes d’une grappe 4 (comptes EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Pour vous connecter à l’environnement de test d’aperçu à l’aide d’une URL :

1. Accédez à cette URL : `https://companyname.preview.workfront.com/`.

   Vous pouvez également accéder à l’environnement de test d’aperçu en accédant à [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Connectez-vous à l’aide de vos informations d’identification de prévisualisation.

   Vos informations d’identification de prévisualisation doivent être identiques à celles de votre production, sauf si vous les avez modifiées dans Production après l’actualisation de prévisualisation. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.

## Réception d’emails à partir de l’environnement de test de prévisualisation

Workfront désactive toutes les communications par courrier électronique à partir de l’environnement Preview Sandbox. Si vous souhaitez recevoir des notifications par courrier électronique de l’environnement de prévisualisation Sandbox, vous devez activer cette fonctionnalité dans vos paramètres utilisateur. Pour plus d’informations sur l’activation des notifications par courrier électronique dans l’environnement de prévisualisation Sandbox, voir [Activation de la diffusion des emails à partir de l’environnement Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>La remise des rapports et les notifications push sur l’application mobile sont toujours désactivées pour l’environnement de prévisualisation Sandbox. Ni vous ni le [!DNL Workfront] Lorsque vous accédez à l’environnement Preview Sandbox, l’administrateur peut activer la remise de rapports ou les notifications push pour l’application mobile.
>
>Pour plus d’informations sur les diffusions de rapports pour l’environnement de production, voir [Présentation de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Authentification Single Sign-On (SSO)

Si vous utilisez l’authentification unique, travaillez avec notre équipe du service clientèle pour vous assurer qu’elle est correctement configurée afin que vous puissiez utiliser vos informations d’identification SSO pour vous connecter à [!UICONTROL Aperçu] Environnement de test. Si votre connexion initiale échoue, contactez votre contact d’assistance classique ou [!DNL Workfront] pour obtenir de l’aide.

Pour plus d’informations sur l’authentification unique, voir [Présentation de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configuration de l’authentification unique dans l’environnement de test de prévisualisation

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées au [!DNL Adobe Admin Console]. Si votre entreprise a été intégrée à la variable [!DNL Adobe Admin Console], aucune action n’est nécessaire.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à la variable [!DNL Adobe Admin Console], voir [Différences d’administration basées sur les plateformes ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Si vous souhaitez configurer votre environnement de test de prévisualisation pour qu’il fonctionne avec une solution de connexion unique, vous pouvez le faire en le configurant séparément de votre environnement de production. La configuration SSO dans l’environnement de test de prévisualisation est indépendante de la configuration SSO dans l’environnement de production.

Lorsque votre environnement de test d’aperçu est actualisé (chaque week-end), les informations d’authentification unique ne sont pas copiées à partir de votre environnement de production pour remplacer la configuration de l’environnement de test d’aperçu.

Les étapes de configuration de l’authentification unique dans l’environnement de test de prévisualisation sont similaires à celles de configuration dans l’environnement de production.

Pour plus d’informations sur la configuration [!DNL Workfront] avec SSO, voir [Présentation de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Prévisualiser les performances et la disponibilité de l’environnement

[!DNL Workfront] Les environnements d’aperçu ne sont pas destinés à des tests de performance ou de chargement. Utilisez plutôt ces environnements pour valider la fonctionnalité avec les workflows existants de votre entreprise.

[!DNL Workfront] Les environnements d’aperçu sont conçus pour être toujours disponibles.

Toute panne à un [!DNL Workfront] L’environnement de prévisualisation pendant les heures de bureau normales sera une priorité absolue immédiatement après la résolution de problèmes de production, le cas échéant.

Toute panne à un [!DNL Workfront] L’environnement d’aperçu le week-end (le samedi et le dimanche) est abordé afin que l’environnement soit exécuté pendant les heures d’ouverture le lundi.
