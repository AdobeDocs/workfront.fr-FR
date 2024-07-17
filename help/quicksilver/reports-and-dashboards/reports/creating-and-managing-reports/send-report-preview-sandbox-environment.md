---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Envoyer un rapport dans l’environnement de prévisualisation de sandbox
description: Les informations de cette page font référence à des fonctionnalités disponibles uniquement dans les environnements Sandbox Aperçu et Actualisation personnalisée. Cette fonctionnalité n’est pas disponible dans l’environnement de production.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 17%

---

# Envoyer un rapport dans l’environnement de prévisualisation de sandbox

Les informations de cette page font référence à des fonctionnalités disponibles uniquement dans les environnements Sandbox Aperçu et Actualisation personnalisée. Cette fonctionnalité n’est pas disponible dans l’environnement de production.

Vous pouvez configurer des options de remise de rapport dans n’importe quel environnement de test Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Bien que les environnements de test soient destinés à fonctionner aussi près que possible de votre environnement de production, certaines fonctionnalités diffèrent de votre environnement de production.

Vous pouvez planifier des rapports dans les environnements de test, mais leur diffusion diffère de celle de l’environnement de production.

Pour plus d’informations sur la planification des rapports pour la diffusion dans l’environnement de production, voir [Présentation de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Selon l’emplacement où vous planifiez les rapports, la fonctionnalité de diffusion diffère entre les environnements de test Aperçu et Actualisation personnalisée .

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Planification de rapports dans l’environnement Aperçu

* [Planification de rapports dans l’environnement Aperçu](#schedule-reports-in-the-preview-environment)

### Planification de rapports dans l’environnement Aperçu

La génération ou non d’un rapport livré dans l’environnement Aperçu dépend de l’activation ou non de la fonction **Recevoir les emails de cet environnement de test**.

Pour plus d’informations sur l’activation des emails à partir de l’environnement Sandbox, voir [Activation de la diffusion des emails à partir de l’environnement Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La planification des rapports à diffuser dans l’environnement Aperçu est identique à la planification des rapports dans l’environnement Production. Pour plus d’informations sur la planification de la remise d’un rapport, voir [Présentation de la remise d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Lorsque vous planifiez la remise d&#39;un rapport dans l&#39;environnement Aperçu , les scénarios suivants se présentent :

* Lorsque **Recevoir des emails de cet environnement de test** est désactivé pour l’utilisateur qui reçoit le rapport, aucun fichier n’est généré lors de la planification de la remise du rapport.
* Lorsque l’option **Recevoir les emails de cet environnement de test** est activée pour l’utilisateur qui reçoit le rapport, le fichier généré lors de la planification de la remise du rapport est ajouté à l’onglet Documents de l’utilisateur.

## Planification de rapports dans l’environnement Sandbox d’actualisation personnalisée

La génération ou non d’un rapport livré dans le sandbox d’actualisation personnalisée dépend de l’activation ou non du paramètre Recevoir des emails de cet environnement de test.

Pour plus d’informations sur l’activation des emails à partir de l’environnement de prévisualisation, reportez-vous à la section [Affichage et modification des paramètres de votre notification électronique](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) de l’article [Modifier vos propres notifications électroniques](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La planification de la remise de rapports dans l’environnement Sandbox d’actualisation personnalisée est identique à la planification de rapports dans l’environnement de production. Pour plus d’informations sur la planification de la remise d’un rapport, voir [Présentation de la remise d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Lorsque vous planifiez la remise d’un rapport dans l’environnement Sandbox d’actualisation personnalisée, les scénarios suivants se présentent :

* Lorsque l’option Recevoir les emails de cet environnement de test est désactivée pour l’utilisateur qui reçoit le rapport, aucun fichier n’est généré lors de la planification de la remise du rapport.
* Lorsque l’option Recevoir les emails de cet environnement de test est activée pour l’utilisateur qui reçoit le rapport, le rapport est envoyé par courriel en pièce jointe de l’adresse électronique associée à l’utilisateur.

## Comment les utilisateurs externes sont avertis

Les utilisateurs externes ne reçoivent pas de rapports envoyés depuis les environnements de test de Workfront et ne reçoivent pas de notification par e-mail.

Les utilisateurs externes ne reçoivent des rapports par courrier électronique que s’ils sont envoyés depuis un environnement de production.
