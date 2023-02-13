---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Envoi d’un rapport dans l’environnement Aperçu d’un environnement Sandbox
description: Les informations de cette page font référence à des fonctionnalités disponibles uniquement dans les environnements Sandbox Aperçu et Actualisation personnalisée. Cette fonctionnalité n’est pas disponible dans l’environnement de production.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Envoi d’un rapport dans l’environnement Aperçu d’un environnement Sandbox

Les informations de cette page font référence à des fonctionnalités disponibles uniquement dans les environnements Sandbox Aperçu et Actualisation personnalisée. Cette fonctionnalité n’est pas disponible dans l’environnement de production.

Vous pouvez configurer des options de remise de rapport dans n’importe quel environnement de test Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Bien que les environnements de test soient destinés à fonctionner aussi près que possible de votre environnement de production, certaines fonctionnalités diffèrent de votre environnement de production.

Vous pouvez planifier des rapports dans les environnements de test, mais leur diffusion diffère de celle de l’environnement de production.

Pour plus d’informations sur la planification des rapports pour la diffusion dans l’environnement de production, voir [Présentation de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Selon l’emplacement où vous planifiez les rapports, la fonctionnalité de diffusion diffère entre les environnements de test Aperçu et Actualisation personnalisée .

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Planification de rapports dans l’environnement Aperçu

* [Planification de rapports dans l’environnement Aperçu](#schedule-reports-in-the-preview-environment)

### Planification de rapports dans l’environnement Aperçu

La génération ou non d’un rapport diffusé dans l’environnement Aperçu dépend de **Réception d’emails à partir de cet environnement de test** est activé ou non.

Pour plus d’informations sur l’activation des courriers électroniques à partir de l’environnement Sandbox, voir [Activation de la diffusion des emails à partir de l’environnement Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La planification des rapports à diffuser dans l’environnement Aperçu est identique à la planification des rapports dans l’environnement Production. Pour plus d’informations sur la planification de la remise d’un rapport, voir [Présentation de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Lorsque vous planifiez la remise d&#39;un rapport dans l&#39;environnement Aperçu , les scénarios suivants se présentent :

* When **Réception d’emails à partir de cet environnement de test** est désactivé pour l’utilisateur qui reçoit le rapport. Aucun fichier n’est généré lors de la planification de la remise du rapport.
* When **Réception d’emails à partir de cet environnement de test** est activée pour l’utilisateur qui reçoit le rapport. Le fichier généré lors de la planification de l’envoi du rapport est ajouté dans l’onglet Documents de l’utilisateur.

## Planification de rapports dans l’environnement Sandbox d’actualisation personnalisée

La génération ou non d’un rapport livré dans le sandbox d’actualisation personnalisée dépend de l’activation ou non du paramètre Recevoir des emails de cet environnement de test.

Pour plus d’informations sur l’activation des emails à partir de l’environnement de prévisualisation, voir la section [Afficher et modifier vos paramètres de notification électronique](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) dans l’article [Activation ou désactivation de vos propres notifications d’événement](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La planification de la remise de rapports dans l’environnement Sandbox d’actualisation personnalisée est identique à la planification de rapports dans l’environnement de production. Pour plus d’informations sur la planification de la remise d’un rapport, voir [Présentation de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Lorsque vous planifiez la remise d’un rapport dans l’environnement Sandbox d’actualisation personnalisée, les scénarios suivants se présentent :

* Lorsque l’option Recevoir les emails de cet environnement de test est désactivée pour l’utilisateur qui reçoit le rapport, aucun fichier n’est généré lors de la planification de la remise du rapport.
* Lorsque l’option Recevoir les emails de cet environnement de test est activée pour l’utilisateur qui reçoit le rapport, le rapport est envoyé par courriel en pièce jointe de l’adresse électronique associée à l’utilisateur.

## Comment les utilisateurs externes sont avertis

Les utilisateurs externes ne reçoivent pas de rapports envoyés depuis les environnements de test de Workfront et ne reçoivent pas de notification par e-mail.

Les utilisateurs externes ne reçoivent des rapports par courrier électronique que s’ils sont diffusés à partir d’un environnement de production.
