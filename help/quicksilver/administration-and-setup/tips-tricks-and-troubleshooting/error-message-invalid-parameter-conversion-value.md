---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Message D’Erreur : Paramètre Non Valide : Valeur De Conversion'
description: 'Vous recevez le message d’erreur suivant lorsque vous tentez de modifier le format d’un champ personnalisé sur un formulaire personnalisé existant : « Paramètre non valide : valeur de conversion &grave;&lt;..&gt; »'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 88%

---

# Message d’erreur : paramètre non valide : valeur de conversion

## Problème

Vous recevez le message d’erreur suivant lorsque vous tentez de modifier le format d’un champ personnalisé dans un formulaire personnalisé existant : « Paramètre non valide : valeur de conversion &quot;&lt;...>&quot; ».\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Cause

Ce message s’affiche dans le cas suivant :

Par exemple, vous avez un champ personnalisé formaté en tant que texte.  Vous voulez maintenant changer le format du champ personnalisé en devise. Quelque part dans votre instance Adobe Workfront, ce champ est déjà lié à un objet et des informations y sont déjà spécifiées. Les informations existantes dans au moins l’un de ces champs sont déjà formatées en tant que texte. Par conséquent, le format du champ ne peut être modifié en devise.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux éléments suivants :</p> 
    <ul> 
     <li> <p>Créer des rapports, des tableaux de bord et des calendriers</p> </li> 
     <li> <p>Créer des filtres, des vues et des regroupements</p> </li> 
    </ul>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

Procédez comme suit :

1. Créez des rapports pour tous les objets dont le champ est susceptible d’être associé à leurs formulaires personnalisés.\
   Pour plus d’informations sur la création d’un rapport, consultez la section [Créer un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Incluez le champ personnalisé que vous essayez de modifier dans la vue du rapport afin de voir les objets dont ledit champ contient une valeur de texte.
1. Corrigez les valeurs du champ personnalisé des objets qui s’affichent au format texte et donnez-leur une valeur formatée en tant que devise. Ensuite, essayez à nouveau de modifier le champ Format du formulaire personnalisé.\
   Ou\
   Si vous avez trop de valeurs de champ déjà remplies avec des informations au format texte, envisagez d’ajouter un nouveau champ personnalisé à votre formulaire personnalisé et de le formater en tant que devise.
