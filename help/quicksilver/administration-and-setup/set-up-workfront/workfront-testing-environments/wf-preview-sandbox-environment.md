---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 'Environnement de prévisualisation de sandbox  [!DNL Adobe Workfront] '
description: L’environnement de prévisualisation de sandbox est un environnement de test qui sert de réplique à votre environnement réel. Il est actualisé chaque week-end par Workfront. Les données ajoutées à votre environnement réel le vendredi apparaissent dans votre environnement de prévisualisation de sandbox le lundi suivant. Tous les packages d’assistance ont accès à ce sandbox.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 7549c9699a86b6f87e5562efd7e586be282c5619
workflow-type: tm+mt
source-wordcount: '1302'
ht-degree: 93%

---

# Environnement de prévisualisation de sandbox [!DNL Adobe Workfront]

<!-- Audited: 12/2023 -->

Il existe deux environnements de test pour [!DNL Workfront] qui sont des répliques de votre environnement de production [!DNL Workfront] :

* Environnement de prévisualisation de sandbox

  L’environnement de prévisualisation de sandbox est un environnement de test qui sert de réplique à votre environnement réel et qui est actualisé chaque week-end par [!DNL Workfront]. Les données ajoutées à votre environnement réel le vendredi apparaissent dans votre environnement de prévisualisation de sandbox le lundi suivant.

  Tous les packages d’assistance ont accès à l’environnement de prévisualisation de sandbox.

* Environnement de sandbox à actualisation personnalisée

  L’environnement de sandbox à actualisation personnalisée est un environnement de test distinct qui est actualisé manuellement par vos soins. L’obtention du sandbox à actualisation personnalisée entraîne des frais supplémentaires. Pour plus d’informations sur cet environnement, consultez la section [Environnement de sandbox à actualisation personnalisée  [!DNL Adobe Workfront] ](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Package de prise en charge [!UICONTROL Standard]</strong> </p> </th> 
   <th> <p><strong>Packages de prise en charge [!UICONTROL Plus], [!UICONTROL Preferred] et [!UICONTROL Enterprise]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Environnement de prévisualisation de sandbox</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Environnement de sandbox à actualisation personnalisée</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Environnement de prévisualisation de sandbox

L’environnement de prévisualisation de sandbox sert d’environnement dans lequel les utilisateurs et les utilisatrices de votre organisation peuvent tester et travailler en toute sécurité avec les données de l’environnement de production sans affecter ce dernier.

L’environnement de prévisualisation de sandbox contient vos données de production effectives ; cependant, il est actualisé tous les week-ends, de sorte que les données peuvent avoir jusqu’à une semaine de retard par rapport à l’environnement de production. Les éléments créés depuis la dernière actualisation sont dans l’environnement de prévisualisation de sandbox jusqu’à l’actualisation suivante.

Les données circulent de manière unidirectionnelle, de la production à la prévisualisation, et non en sens inverse. Une mise à jour de l’environnement de prévisualisation est toujours prévue par [!DNL Workfront] chaque week-end.

L’environnement de prévisualisation de sandbox permet également à [!DNL Workfront] de déployer de nouvelles fonctionnalités dans un environnement sûr, avant qu’elles ne soient prêtes à être déployées en production. Vous pouvez tester les nouvelles fonctionnalités et donner votre avis sur leur fonctionnement à [!DNL Workfront] en accédant à l’environnement de prévisualisation de sandbox. Ainsi, le code de l’environnement de prévisualisation de sandbox est toujours en avance sur celui de production, même si vos données sont actualisées chaque semaine.

L’environnement de prévisualisation est idéal pour organiser des formations, tester de nouvelles fonctionnalités et déterminer les fonctions de configuration.

>[!NOTE]
>
>Lorsque vous accédez à l’environnement de prévisualisation de sandbox, vous remarquez la bannière bleue en haut de l’écran. La bannière ne peut pas être retirée pendant que vous travaillez dans cet environnement.
>
>Le nom de l’environnement auquel vous accédez (Prévisualisation) et la version de lancement du code s’affichent sur la bannière. Cliquez sur **[!UICONTROL Voir les nouveautés]** pour obtenir des informations sur cette version.
>
>![Bannière d’aperçu](assets/preview-banner-nwe-350x161.png)

## Accéder à l’environnement de prévisualisation de sandbox

Par défaut, en tant qu’administrateur ou administratrice de [!DNL Workfront], vous avez accès à l’environnement de [!UICONTROL prévisualisation] de sandbox. Si vous ne pouvez pas accéder à l’environnement de [!UICONTROL prévisualisation] de sandbox comme décrit dans cette section, contactez votre administrateur ou votre administratrice [!DNL Workfront] ou notre équipe d’assistance clientèle.


### Accéder à l’environnement de prévisualisation de sandbox à partir de l’interface [!DNL Workfront] {#accessing-the-preview-sandbox-from-the-workfront-interface}

En tant que personne membre de l’équipe d’administration [!DNL Workfront], vous pouvez accéder à l’environnement de prévisualisation de sandbox via l’interface [!DNL Workfront].

Pour accéder à l’environnement de prévisualisation de sandbox, procédez comme suit :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Système]** > **[!UICONTROL Préférences]**.

1. Dans la section **[!UICONTROL Environnements de test]**, cliquez sur **[!UICONTROL Prévisualisation de sandbox]**.

1. Connectez-vous avec vos identifiants de prévisualisation.

   Ces identifiants doivent être les mêmes que ceux de production, à moins que vous ne les ayez modifiés dans la production après avoir actualisé la prévisualisation. Les connexions ne sont synchronisées que lorsqu’une actualisation a lieu. Elles ne se synchronisent pas automatiquement.

### Accéder à la prévisualisation de sandbox à l’aide d’une URL {#accessing-the-preview-sandbox-using-a-url}

Vous pouvez accéder à la prévisualisation de sandbox à l’aide d’une URL.

#### Accéder à la prévisualisation de sandbox pour les comptes des clusters 1, 2, 3 et 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

L’URL de la prévisualisation de sandbox est : `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Si vous aviez des signets qui renvoyaient à l’ancienne URL de la prévisualisation Sandbox, veuillez prendre note de ce changement et mettre à jour l’URL dans vos signets.

Pour se connecter à la prévisualisation de sandbox à l’aide d’une URL, procédez comme suit :

1. Accédez à cette URL : `https://companyname.preview.workfront.com/`.

   Si vous êtes client ou cliente EMEA et que votre compte se trouve sur le cluster 4, consultez la section Accès à la prévisualisation de sandbox pour les comptes sur le cluster 4 (comptes EMEA) ci-dessous.

1. Connectez-vous à l’aide de vos identifiants de prévisualisation.

   >[!TIP]
   >
   >Vos identifiants de prévisualisation doivent être les mêmes que vos identifiants de production, à moins que vous ne les ayez modifiés dans la production après l’actualisation de la prévisualisation. Les connexions ne sont synchronisées que lorsqu’une actualisation a lieu. Elles ne se synchronisent pas automatiquement.


#### Accéder à la prévisualisation de sandbox pour les comptes sur le cluster 4 (comptes EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Pour se connecter à la prévisualisation de sandbox à l’aide d’une URL, procédez comme suit :

1. Accédez à cette URL : `https://companyname.preview.workfront.com/`.

   Vous pouvez également accéder à la prévisualisation de sandbox en allant sur [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Connectez-vous à l’aide de vos identifiants de prévisualisation.

   Vos identifiants de prévisualisation doivent être les mêmes que vos identifiants de production, à moins que vous ne les ayez modifiés dans la production après l’actualisation de la prévisualisation. Les connexions ne sont synchronisées que lorsqu’une actualisation a lieu. Elles ne se synchronisent pas automatiquement.

## Recevoir des e-mails à partir de la prévisualisation de sandbox

Workfront désactive toute communication par e-mail à partir de l’environnement de prévisualisation de de sandbox. Si vous souhaitez recevoir des notifications par e-mail à partir de l’environnement de prévisualisation de sandbox, vous devez activer cette fonctionnalité dans vos paramètres d’utilisateur ou d’utilisatrice. Pour plus d’informations sur l’activation des notifications par e-mail dans l’environnement de prévisualisation de sandbox, voir [Activer la diffusion d’e-mails à partir de l’environnement de prévisualisation de sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>La remise de rapports et les notifications push sur l’application mobile sont toujours désactivées dans l’environnement de prévisualisation de sandbox. Ni vous ni l’administrateur ou l’administratrice de [!DNL Workfront] ne pouvez activer la remise de rapports ou les notifications push pour l’application mobile lorsque vous accédez à l’environnement de prévisualisation de sandbox.
>
>Pour plus d’informations sur les remises de rapports pour l’environnement de production, voir [Vue d’ensemble de la remise des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Authentification Single Sign-On (SSO)

Si vous utilisez l’authentification unique, assurez-vous auprès de notre équipe d’assistance à la clientèle qu’elle est correctement configurée, afin que vous puissiez utiliser vos informations d’identification SSO pour vous connecter à la [!UICONTROL prévisualisation] de sandbox. Si votre première connexion échoue, veuillez contacter votre contact d’assistance habituel, ou l’administrateur ou administratrice [!DNL Workfront] pour obtenir de l’aide.

Pour plus d’informations sur l’authentification unique, voir [Vue d’ensemble de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configurer l’authentification unique dans la prévisualisation de sandbox

>[!IMPORTANT]
>
>La procédure décrite sur cette page ne s’applique qu’aux organisations qui n’ont pas encore été intégrées à l’[!DNL Adobe Admin Console]. Si votre organisation a été intégrée à l’[!DNL Adobe Admin Console], aucune action n’est nécessaire.
>
>Pour une liste des procédures qui diffèrent selon que votre organisation a été intégrée ou non à l’[!DNL Adobe Admin Console], voir [Différences d’administration en fonction de la plateforme ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Si vous souhaitez configurer votre prévisualisation de sandbox pour qu’elle fonctionne avec une solution d’authentification unique, vous pouvez le faire en la configurant séparément de votre environnement de production. La configuration SSO dans la prévisualisation de sandbox est indépendante de votre configuration SSO dans l’environnement de production.

Lors de l’actualisation de votre prévisualisation de sandbox (chaque week-end), les informations SSO ne sont pas copiées depuis votre environnement de production pour écraser la configuration de la prévisualisation de sandbox.

Les étapes de la configuration de l’authentification unique dans la prévisualisation de sandbox sont similaires à celles de la configuration dans l’environnement de production.

Pour plus d’informations sur la configuration de [!DNL Workfront] avec l’authentification unique, voir [Vue d’ensemble de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Recalcul automatique des chronologies des projets

Recalculer les chronologies permet aux personnes gestionnaires de voir comment des forces extérieures au projet affectent la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévisionnelles pour le projet.

En tant qu’administrateur ou administratrice Workfront, vous pouvez configurer le moment où Workfront recalcule automatiquement les chronologies de projet. Workfront peut recalculer les chronologies de projet toutes les nuits ou lorsque la portée du projet change, ou les deux.

Pour plus d’informations, voir [Configuration des recalculs de chronologie pour les projets](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Pour l’environnement de Prévisualisation, le recalcul nocturne est désactivé et les chronologies de projet ne sont pas recalculées automatiquement. Vous devez recalculer manuellement la chronologie du projet pour l’environnement de prévisualisation. Pour plus d’informations, voir [Recalculer la chronologie du projet](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Performances et disponibilité de l’environnement de prévisualisation

* Les environnements de prévisualisation [!DNL Workfront] ne sont pas destinés à des tests de performance ou de charge. Utilisez-les plutôt pour valider l’efficacité des fonctionnalités avec les workflows existants de votre entreprise.

* Les workflows impliquant des documents doivent se concentrer sur les processus et non sur les tests de chargement. Les fichiers volumineux ne sont pas pris en charge dans les environnements Sandbox.

* Les environnements de prévisualisation [!DNL Workfront] sont censés être toujours disponibles.

* Toute interruption d’un environnement de prévisualisation [!DNL Workfront] pendant les heures de bureau sera traitée en priorité, immédiatement après que les problèmes de production auront été résolus, le cas échéant.

* Toute interruption de l’environnement de prévisualisation [!DNL Workfront] pendant les week-ends (samedi et dimanche) sera résolue de manière à ce que l’environnement soit opérationnel pendant les heures de bureau le lundi.
