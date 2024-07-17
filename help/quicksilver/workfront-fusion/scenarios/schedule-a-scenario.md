---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Planifier un scénario dans Adobe Workfront Fusion
description: Par défaut, un scénario s’exécute toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant le moment et la fréquence d’exécution d’un scénario activé.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: f5549be5951a2648d6a77d25bebbd4141f18d36c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 23%

---

# Planification d’un scénario dans [!DNL Adobe Workfront Fusion]

Par défaut, un scénario s’exécute toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant le moment et la fréquence d’exécution d’un scénario activé. Les scénarios de fusion peuvent être planifiés pour s’exécuter aussi souvent que toutes les 5 minutes.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">   
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Planification d’un scénario

1. Dans le coin supérieur droit de la page de détails du scénario, cliquez sur **[!UICONTROL Options]** > **[!UICONTROL Planification]**

   Ou

   Cliquez sur l’icône **[!UICONTROL Planification]** (horloge) sur le module de déclenchement du scénario.

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
        <li> <p><strong>[!UICONTROL Une fois]</strong> </p> <p>Saisissez la date et l’heure d’exécution du scénario. Utilisez le format <code>MM/DD/YYYY h:mm A</code>. Exemple : <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Chaque jour]</strong> </p> <p>Saisissez l’heure à laquelle vous souhaitez que le scénario s’exécute. Utilisez le format <code>h:mm A</code>. Exemple : <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Jours de la semaine]</strong> </p> <p>Jours : sélectionnez les jours de la semaine pendant lesquels le scénario doit s’exécuter. Vous pouvez sélectionner un ou plusieurs jours.</p> <p>Heure : saisissez l’heure à laquelle le scénario doit s’exécuter sur les jours sélectionnés. Utilisez le format <code>h:mm A</code>. Exemple : <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Jours du mois]</strong> </p> <p>Jours : sélectionnez les jours du mois pendant lesquels le scénario doit s’exécuter. Vous pouvez sélectionner un ou plusieurs jours.</p> <p>Heure : saisissez l’heure à laquelle le scénario doit s’exécuter sur les jours sélectionnés. Utilisez le format <code>h:mm A</code>. Exemple : <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Dates spécifiées]</strong> </p> <p>Mois : sélectionnez les mois pendant lesquels vous souhaitez exécuter le scénario. Vous pouvez sélectionner un ou plusieurs mois.</p> <p>Jours : sélectionnez les jours du mois pendant lesquels le scénario doit s’exécuter. Vous pouvez sélectionner un ou plusieurs jours.</p> <p>Heure : saisissez l’heure à laquelle le scénario doit s’exécuter sur les jours sélectionnés. Utilisez le format <code>h:mm A</code>. Exemple : <code>11:00 PM</code></p> </li> 
       </ul> <p>Remarque : une date doit exister pour qu’un scénario s’exécute à cette date. Par exemple, un scénario planifié uniquement pour le 31 du mois ne s’exécutera pas en février, avril, juin, septembre ou novembre, car ces mois n’ont pas de 31e jour.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Planification avancée]</td> 
      <td>Vous pouvez définir des intervalles de temps spécifiques pendant lesquels votre scénario doit s’exécuter. Vous pouvez spécifier des intervalles de la journée, des jours de semaine ou des mois. Pour chaque intervalle, cliquez sur <strong>[!UICONTROL Ajouter]</strong> et renseignez les champs comme décrit dans le champ [!UICONTROL Exécuter le scénario] .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Saisissez la date et l’heure après lesquelles vous souhaitez que le scénario s’exécute. Utilisez le format <code>MM/DD/YYYY h:mm A</code>. Exemple : <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>Saisissez la date et l’heure auxquelles vous souhaitez que le scénario s’exécute. Utilisez le format <code>MM/DD/YYYY h:mm A</code>. Exemple : <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL OK]** pour enregistrer les paramètres de planification et revenir au scénario.
