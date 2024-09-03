---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Planifier un scénario dans Adobe Workfront Fusion
description: Par défaut, un scénario s’exécute toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant le moment et la fréquence d’exécution d’un scénario activé.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: f5549be5951a2648d6a77d25bebbd4141f18d36c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 100%

---

# Planifier un scénario dans [!DNL Adobe Workfront Fusion]

Par défaut, un scénario s’exécute toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant le moment et la fréquence d’exécution d’un scénario activé. Vous pouvez planifier les scénarios Fusion pour qu’ils s’exécutent toutes les 5 minutes.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">   
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Planifier un scénario

1. Dans le coin supérieur droit de la page Détails du scénario, cliquez sur **[!UICONTROL Options]** > **[!UICONTROL Planification]**

   Ou

   Cliquez sur l’icône **[!UICONTROL Planification]** (horloge) sur le module de déclenchement du scénario.

1. Renseignez les champs suivants :

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Run scenario]</td> 
      <td> <p>Sélectionnez la fréquence, puis l’intervalle d’exécution du scénario.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL At regular intervals]</strong> </p> <p>Saisissez le nombre de minutes entre les exécutions. La valeur par défaut est de 15 minutes.</p> </li> 
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>Saisissez la date et l’heure d’exécution du scénario. Utilisez le format <code>MM/DD/YYYY h:mm A</code>. Exemple : <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Every day]</strong> </p> <p>Saisissez l’heure à laquelle vous souhaitez que le scénario s’exécute. Utilisez le format <code>h:mm A</code>. Exemple : <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Days of the week]</strong> </p> <p>Jours : sélectionnez les jours de la semaine pendant lesquels le scénario doit s’exécuter. Vous pouvez sélectionner un ou plusieurs jours.</p> <p>Heure : saisissez l’heure à laquelle le scénario doit s’exécuter les jours sélectionnés. Utilisez le format <code>h:mm A</code>. Exemple : <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Days of the month]</strong> </p> <p>Jours : sélectionnez les jours du mois pendant lesquels le scénario doit s’exécuter. Vous pouvez sélectionner un ou plusieurs jours.</p> <p>Heure : saisissez l’heure à laquelle le scénario doit s’exécuter les jours sélectionnés. Utilisez le format <code>h:mm A</code>. Exemple : <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Specified dates]</strong> </p> <p>Mois : sélectionnez les mois pendant lesquels le scénario doit s’exécuter. Vous pouvez sélectionner un ou plusieurs mois.</p> <p>Jours : sélectionnez les jours du mois pendant lesquels le scénario doit s’exécuter. Vous pouvez sélectionner un ou plusieurs jours.</p> <p>Heure : saisissez l’heure à laquelle le scénario doit s’exécuter les jours sélectionnés. Utilisez le format <code>h:mm A</code>. Exemple : <code>11:00 PM</code></p> </li> 
       </ul> <p>Remarque : pour qu’un scénario s’exécute à une date, celle-ci doit exister. Par exemple, un scénario planifié uniquement pour le 31 du mois ne s’exécutera pas en février, avril, juin, septembre ou novembre, car ces mois n’ont pas de 31e jour.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Advanced scheduling]</td> 
      <td>Vous pouvez définir des intervalles de temps spécifiques pendant lesquels votre scénario doit s’exécuter. Vous pouvez spécifier des intervalles en heures de la journée, en jours de semaine ou en mois. Pour chaque intervalle, cliquez sur <strong>[!UICONTROL Add]</strong> et renseignez les champs comme décrit dans le champ [!UICONTROL Run scenario].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Saisissez la date et l’heure après lesquelles vous souhaitez que le scénario s’exécute. Utilisez le format <code>MM/DD/YYYY h:mm A</code>. Exemple : <code>06/25/2019 11:00 PM</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>Saisissez la date et l’heure auxquelles vous souhaitez que le scénario s’exécute. Utilisez le format <code>MM/DD/YYYY h:mm A</code>. Exemple : <code>06/25/2019 11:00 PM</code></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL OK]** pour enregistrer les paramètres de planning et revenir au scénario.
