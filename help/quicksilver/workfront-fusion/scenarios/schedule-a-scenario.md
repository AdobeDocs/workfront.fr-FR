---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Planification d’un scénario dans Adobe Workfront Fusion
description: Par défaut, un scénario s’exécute toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant le moment et la fréquence d’exécution d’un scénario activé.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# Planification d’un scénario dans [!DNL Adobe Workfront Fusion]

Par défaut, un scénario s’exécute toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant le moment et la fréquence d’exécution d’un scénario activé.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">   
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p><p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail] </p>  </td>    </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Planification d’un scénario

1. Dans le coin supérieur droit de la page Détails du scénario, cliquez sur **[!UICONTROL Options]** > **[!UICONTROL Planification]**

   Ou

   Cliquez sur le bouton **[!UICONTROL Planification]** icône (horloge) sur le module déclencheur du scénario.

1. Renseignez les champs suivants :

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Exécuter le scénario]</td> 
      <td> <p>Sélectionnez la fréquence d'exécution du scénario, puis sélectionnez l'intervalle.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL À intervalles réguliers]</strong> </p> <p>Saisissez le nombre de minutes entre les exécutions. La valeur par défaut est de 15 minutes.</p> </li> 
        <li> <p><strong>[!UICONTROL Une fois]</strong> </p> <p>Saisissez la date et l’heure d’exécution du scénario. Utiliser le format <code>MM/DD/YYYY h:mm A</code>. Exemple: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Chaque jour]</strong> </p> <p>Saisissez l’heure à laquelle vous souhaitez que le scénario s’exécute. Utiliser le format <code>h:mm A</code>. Exemple: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Jours de la semaine]</strong> </p> <p>Jours : Sélectionnez les jours de la semaine où vous souhaitez que le scénario s’exécute. Vous pouvez sélectionner un ou plusieurs jours.</p> <p>Heure : Saisissez l’heure à laquelle vous souhaitez que le scénario s’exécute les jours sélectionnés. Utiliser le format <code>h:mm A</code>. Exemple: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Jours du mois]</strong> </p> <p>Jours : Sélectionnez les jours du mois pendant lesquels vous souhaitez que le scénario s’exécute. Vous pouvez sélectionner un ou plusieurs jours.</p> <p>Heure : Saisissez l’heure à laquelle vous souhaitez que le scénario s’exécute les jours sélectionnés. Utiliser le format <code>h:mm A</code>. Exemple: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Dates spécifiées]</strong> </p> <p>Mois : Sélectionnez les mois pendant lesquels vous souhaitez exécuter le scénario. Vous pouvez sélectionner un ou plusieurs mois.</p> <p>Jours : Sélectionnez les jours du mois pendant lesquels vous souhaitez que le scénario s’exécute. Vous pouvez sélectionner un ou plusieurs jours.</p> <p>Heure : Saisissez l’heure à laquelle vous souhaitez que le scénario s’exécute les jours sélectionnés. Utiliser le format <code>h:mm A</code>. Exemple: <code>11:00 PM</code></p> </li> 
       </ul> <p>Remarque : Une date doit exister pour qu’un scénario s’exécute à cette date. Par exemple, un scénario planifié uniquement pour le 31 du mois ne s’exécutera pas en février, avril, juin, septembre ou novembre, car ces mois n’ont pas de 31e jour.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Planification avancée]</td> 
      <td>Vous pouvez définir des intervalles de temps spécifiques pendant lesquels votre scénario doit s’exécuter. Vous pouvez spécifier des intervalles de la journée, des jours de semaine ou des mois. Pour chaque intervalle, cliquez sur <strong>[!UICONTROL Ajouter]</strong> et renseignez les champs comme décrit dans le champ [!UICONTROL Exécuter le scénario] .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Saisissez la date et l’heure après lesquelles vous souhaitez que le scénario s’exécute. Utiliser le format <code>MM/DD/YYYY h:mm A</code>. Exemple: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>Saisissez la date et l’heure auxquelles vous souhaitez que le scénario s’exécute. Utiliser le format <code>MM/DD/YYYY h:mm A</code>. Exemple: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL OK]** pour enregistrer les paramètres de planification et revenir au scénario.
