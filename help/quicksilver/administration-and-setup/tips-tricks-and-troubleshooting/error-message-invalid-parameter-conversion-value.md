---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Message d''erreur : Paramètre non valide : valeur de conversion'''
description: "Vous recevez le message d’erreur suivant lorsque vous tentez de modifier le format d’un champ personnalisé sur un formulaire personnalisé existant : 'Invalid Parameter: valeur de conversion `&lt;...&gt;`"
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 1%

---

# Message d’erreur : Paramètre non valide : valeur de conversion

## Problème

Vous recevez le message d’erreur suivant lorsque vous tentez de modifier le format d’un champ personnalisé sur un formulaire personnalisé existant : &quot;Invalid Parameter : valeur de conversion &quot;&lt;...>&quot;\
![custom_field_format_incorrect_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Cause

Ce message se produit dans le scénario suivant :

Par exemple, vous avez un champ personnalisé au format Texte.  Maintenant, vous souhaitez modifier le format du champ personnalisé en devise. Quelque part dans votre [!DNL Adobe Workfront] , ce champ est déjà attaché à un objet et contient des informations déjà spécifiées. Les informations existantes dans au moins un de ces champs sont déjà au format Texte. Par conséquent, le format du champ ne peut pas être modifié en devise.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">[!DNL Workfront] plan</a>*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] Présentation des licences</a>*</p> </td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Niveau d’accès*</strong> </td> 
   <td> <p>Modifier l’accès à :</p> 
    <ul> 
     <li> <p>Création de rapports, de tableaux de bord et de calendriers</p> </li> 
     <li> <p>Création de filtres, d’affichages et de groupes</p> </li> 
    </ul> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

Procédez comme suit :

1. Créez des rapports pour tous les objets auxquels ce champ peut être associé à leur Forms personnalisée.\
   Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Insérez le champ personnalisé que vous essayez de modifier dans la vue du rapport afin de voir quel objet ce champ est renseigné par une valeur de texte.
1. Corrigez les valeurs des champs personnalisés des objets qui s’affichent au format texte et attribuez-leur une valeur au format Devise ; Essayez de modifier à nouveau le champ Format du formulaire personnalisé.\
   Ou\
   Si trop de valeurs de champ sont déjà renseignées avec des informations au format texte, pensez à ajouter un nouveau champ personnalisé à votre formulaire personnalisé et à le formater en tant que devise.
