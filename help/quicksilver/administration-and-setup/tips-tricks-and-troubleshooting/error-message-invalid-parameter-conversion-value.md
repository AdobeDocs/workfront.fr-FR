---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Message d’erreur : Paramètre non valide : valeur de conversion'
description: '"Vous recevez le message d’erreur suivant lorsque vous tentez de modifier le format d’un champ personnalisé sur un formulaire personnalisé existant : "Paramètre non valide : valeur de conversion `&lt;..&gt;`"'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 14%

---

# Message d’erreur : Paramètre non valide : valeur de conversion

## Problème

Vous recevez le message d’erreur suivant lorsque vous tentez de modifier le format d’un champ personnalisé sur un formulaire personnalisé existant : &quot;Paramètre non valide : valeur de conversion &quot;&lt;...>&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Cause

Ce message se produit dans le scénario suivant :

Par exemple, vous avez un champ personnalisé au format Texte.  Maintenant, vous souhaitez modifier le format du champ personnalisé en devise. Quelque part dans votre instance Adobe Workfront, ce champ est déjà attaché à un objet et contient des informations déjà spécifiées. Les informations existantes dans au moins un de ces champs sont déjà au format Texte. Par conséquent, le format du champ ne peut pas être modifié en devise.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans?lang=fr" target="_blank">Plan Workfront</a>*</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences</a>*</p> </td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Niveau d’accès*</strong> </td> 
   <td> <p>Modifier l’accès à :</p> 
    <ul> 
     <li> <p>Création de rapports, de tableaux de bord et de calendriers</p> </li> 
     <li> <p>Création de filtres, d’affichages et de groupes</p> </li> 
    </ul> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

Procédez comme suit :

1. Créez des rapports pour tous les objets auxquels ce champ peut être associé à leur Forms personnalisée.\
   Pour plus d&#39;informations sur la création d&#39;un rapport, voir [Création d&#39;un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Insérez le champ personnalisé que vous essayez de modifier dans la vue du rapport afin de voir quel objet ce champ est renseigné par une valeur de texte.
1. Corrigez les valeurs des champs personnalisés des objets qui s’affichent au format texte et attribuez-leur une valeur au format Devise, puis tentez à nouveau de modifier le champ Format du formulaire personnalisé.\
   Ou\
   Si trop de valeurs de champ sont déjà renseignées avec des informations au format texte, pensez à ajouter un nouveau champ personnalisé à votre formulaire personnalisé et à le formater en tant que devise.
