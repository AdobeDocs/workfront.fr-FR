---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Envoyer un rapport dans l’environnement de prévisualisation de sandbox
description: Les informations contenues dans cette page font référence à des fonctionnalités qui ne sont disponibles que dans les environnements de prévisualisation et de sandbox à actualisation personnalisée. Cette fonctionnalité est désormais disponible dans l’environnement de production.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 394eb1aed6508399b6459430acec7c0729036edc
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 98%

---

# Envoyer un rapport dans l’environnement de prévisualisation de sandbox

<!-- Audited: 11/2024 -->

Les informations contenues dans cette page font référence à des fonctionnalités qui ne sont disponibles que dans les environnements de prévisualisation et de sandbox à actualisation personnalisée. Cette fonctionnalité est désormais disponible dans l’environnement de production.

Vous pouvez définir des options de diffusion de rapports dans n’importe quel environnement de test Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Bien que les environnements de test soient censés fonctionner aussi près que possible de votre environnement de production, certaines fonctionnalités diffèrent de votre environnement de production.

Vous pouvez planifier des rapports dans les environnements de test, mais la manière dont ils sont fournis diffère de celle de l’environnement de production.

Pour plus d’informations sur la planification de la diffusion des rapports dans l’environnement de production, voir [Vue d’ensemble de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Selon l’endroit où vous planifiez les rapports, la fonctionnalité de diffusion diffère entre les environnements de prévisualisation et de sandbox à actualisation personnalisée.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
      <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et regroupements</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Planifier des rapports dans l’environnement de prévisualisation

* [Planifier des rapports dans l’environnement de prévisualisation](#schedule-reports-in-the-preview-environment)

### Planifier des rapports dans l’environnement de prévisualisation

La production ou non d’un rapport dans l’environnement de prévisualisation dépend de l’activation ou non de l’option **Recevoir des e-mails de cet environnement de test**.

Pour plus d’informations sur l’activation des e-mails à partir de l’environnement Sandbox, voir [Activer la diffusion d’e-mails à partir de l’environnement de prévisualisation de sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La planification des rapports pour une diffusion dans l’environnement de prévisualisation est identique à la planification des rapports dans l’environnement de production. Pour plus d’informations sur la planification de la diffusion d’un rapport, voir [Vue d’ensemble de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Lorsque vous planifiez la diffusion d’un rapport dans l’environnement de prévisualisation, les scénarios suivants se présentent :

* Lorsque **Recevoir des e-mails de cet environnement de test** est désactivé pour la personne qui reçoit le rapport, aucun fichier n’est produit lors de la planification de la diffusion du rapport.
* Lorsque **Recevoir des e-mails de cet environnement de test** est activé pour la personne qui reçoit le rapport, le fichier produit lors de la planification de la diffusion du rapport est ajouté dans l’onglet Documents de l’utilisateur ou de l’utilisatrice.

## Planifier des rapports dans l’environnement de sandbox à actualisation personnalisée

La production ou non d’un rapport dans l’environnement de sandbox à actualisation personnalisée dépend de l’activation ou non du paramètre Recevoir des e-mails de cet environnement de test.

Pour plus d’informations sur l’activation des e-mails à partir de l’environnement de prévisualisation, voir la section [Voir et modifier vos paramètres de notification par e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) dans l’article [Modifier vos propres notifications par e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La planification des rapports pour une diffusion dans l’environnement de sandbox à actualisation personnalisée est identique à la planification des rapports dans l’environnement de production. Pour plus d’informations sur la planification de la diffusion d’un rapport, voir [Vue d’ensemble de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Lorsque vous planifiez la diffusion d’un rapport dans l’environnement de sandbox à actualisation personnalisée, les scénarios suivants se présentent :

* Lorsque l’option Recevoir des e-mails de cet environnement de test est désactivée pour la personne qui reçoit le rapport, aucun fichier n’est produit lors de la planification de la diffusion du rapport.
* Lorsque l’option Recevoir des e-mails de cet environnement de test est activée pour la personne qui reçoit le rapport, celui-ci est envoyé sous forme de pièce jointe à l’adresse e-mail associée à l’utilisateur ou à l’utilisatrice.

## Réception des informations par les utilisateurs et utilisatrices externes

Les utilisateurs et utilisatrices externes ne reçoivent pas les rapports envoyés par les environnements de test Workfront, et ne reçoivent pas non plus de notification par e-mail.

Les utilisateurs et utilisatrices externes ne reçoivent des rapports par e-mail que s’ils proviennent d’un environnement de production.
