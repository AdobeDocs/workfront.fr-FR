---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Message d’erreur : Paramètre non valide : Valeur de conversion"
description: '"Vous recevez le message d’erreur suivant lorsque vous tentez de modifier le format d’un champ personnalisé sur un formulaire personnalisé existant : "Paramètre non valide : valeur de conversion `&lt;..&gt;`"'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 14%

---

# Message d’erreur : Paramètre non valide : valeur de conversion

## Problème

Vous recevez le message d’erreur suivant lorsque vous tentez de modifier le format d’un champ personnalisé sur un formulaire personnalisé existant : &quot;Paramètre non valide : valeur de conversion &quot;&lt;...>&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Cause

Ce message se produit dans le scénario suivant :

Par exemple, vous avez un champ personnalisé au format Texte.  Maintenant, vous souhaitez modifier le format du champ personnalisé en devise. Quelque part dans votre instance Adobe Workfront, ce champ est déjà attaché à un objet et contient des informations déjà spécifiées. Les informations existantes dans au moins un de ces champs sont déjà au format Texte. Par conséquent, le format du champ ne peut pas être modifié en devise.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>
   <p>Nouvelle : standard</p>
   <p>ou</p>
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès à :</p> 
    <ul> 
     <li> <p>Création de rapports, de tableaux de bord et de calendriers</p> </li> 
     <li> <p>Création de filtres, d’affichages et de groupes</p> </li> 
    </ul>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

Procédez comme suit :

1. Créez des rapports pour tous les objets auxquels ce champ peut être associé à leur Forms personnalisée.\
   Pour plus d&#39;informations sur la création d&#39;un rapport, voir [Création d&#39;un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Insérez le champ personnalisé que vous essayez de modifier dans la vue du rapport afin de voir quel objet ce champ est renseigné par une valeur de texte.
1. Corrigez les valeurs des champs personnalisés des objets qui s’affichent au format texte et attribuez-leur une valeur au format Devise, puis tentez à nouveau de modifier le champ Format du formulaire personnalisé.\
   Ou\
   Si trop de valeurs de champ sont déjà renseignées avec des informations au format texte, pensez à ajouter un nouveau champ personnalisé à votre formulaire personnalisé et à le formater en tant que devise.
