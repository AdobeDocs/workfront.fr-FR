---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Exécuter et remettre un rapport avec les droits d’accès d’une autre personne
description: Par défaut, les utilisateurs et utilisatrices ne peuvent voir que les objets d’un rapport qu’ils ont le droit d’afficher.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 96%

---

# Exécuter et remettre un rapport avec les droits d’accès d’une autre personne

<!-- Audited: 11/2024 -->

Par défaut, les utilisateurs et utilisatrices ne peuvent voir que les objets d’un rapport qu’ils ont le droit d’afficher.

Vous pouvez permettre à tous les utilisateurs et utilisatrices de voir les mêmes résultats dans un rapport qu’une autre personne, quel que soit leur niveau d’accès ou d’autorisation sur les objets contenus dans le rapport.

Si vous exécutez un rapport avec les droits d’accès d’un autre utilisateur ou d’une autre utilisatrice disposant d’un accès supérieur (par exemple, les droits d’accès d’un administrateur ou d’une administratrice Adobe Workfront), tous les utilisateurs et utilisatrices autorisés à consulter le rapport peuvent voir les informations contenues dans le rapport en tant que personne spécifiée dans le report builder. Vous pouvez configurer cela pour les rapports que les utilisateurs et utilisatrices trouvent dans l’interface Workfront, ou pour les rapports qui sont envoyés aux utilisateurs et utilisatrices en tant que pièce jointe à un e-mail.

>[!TIP]
>
>Vous ne devez remplacer le champ **Exécuter ce rapport avec les droits d’accès suivants :** par une personne active que si vous souhaitez que le rapport s’affiche avec les droits d’accès de cette personne.Par exemple, un utilisateur ou utilisatrice avec une licence de travail peut ne pas avoir le droit de voir tous les éléments d’un rapport créé par une personne avec une licence de plan ou par un administrateur ou une administratrice système, à moins que le rapport ne s’affiche avec les droits d’accès d’une personne responsable de la planification ou d’un administrateur ou d’une adminsitratrice système.\
>Si le rapport est partagé avec des utilisateurs et utilisatrices disposant d’un accès similaire à celui de la personne spécifiée dans le champ **Exécuter ce rapport avec les droits d’accès suivants :**, vous pouvez laisser ce champ vide.

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
   <td> <p>Autorisations Afficher pour un rapport (pour afficher le rapport remis)</p><p>Autorisations Gérer pour un rapport (pour exécuter le rapport)</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher un rapport avec les droits d’accès d’une autre personne

Le remplissage du champ **Exécuter ce rapport avec les droits daccès suivants :** permet de s’assurer que le rapport contient les mêmes données, peu importe la personne qui accède au rapport. Le rapport s’affiche de la même façon que pour la personne spécifiée.

Les utilisateurs et utilisatrices qui accèdent au rapport doivent avoir au moins les autorisations Afficher pour le rapport pour pouvoir le voir. Si la personne mentionnée dans le champ **Exécuter ce rapport avec les droits daccès suivants :** est désactivée, le rapport ne s’affiche plus pour les autres personnes avec lesquelles le rapport est partagé.

Pour exécuter un rapport avec les droits d’accès d’une autre personne, procédez comme suit :

1. Cliquez sur l’icône de **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône de **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Rapports]**.

1. Sélectionnez le rapport que vous souhaitez afficher avec les droits d’accès d’une autre personne.
1. Cliquez sur **Actions de rapport**, puis sur **Modifier**.

1. Cliquez sur **Paramètres du rapport**.

1. Dans le champ **Exécuter ce rapport avec les droits d’accès suivants :**, commencez à saisir le nom de la personne pour laquelle vous souhaitez que le rapport s’affiche, puis sélectionnez-le lorsqu’il apparaît dans la liste.\
   ![Exécuter avec les droits d’accès de ](assets/unshimmed-access-rights-of.png)

   >[!NOTE]
   >
   >Les utilisateurs et utilisatrices ayant un niveau d’accès inférieur qui sont autorisés à créer des rapports n’ont pas la possibilité de sélectionner une autre personne qu’eux-mêmes pour le champ **Exécuter ce rapport avec les droits d’accès suivants :**.

1. Cliquez sur **Terminé**.
1. Cliquez sur **Enregistrer + Fermer**.\
   Le rapport s’affiche désormais pour tous les utilisateurs et utilisatrices avec lesquels il est partagé comme s’il était affiché par la personne spécifiée dans le champ **Exécuter ce rapport avec les droits d’accès suivants :**.

>[!IMPORTANT]
>
>La saisie d’une personne autre que la personne connectée pour le champ **Exécuter ce rapport avec les droits d’accès suivants :** a une incidence sur les informations affichées dans le rapport si celui-ci contient un filtre qui utilise un caractère générique faisant référence à la personne connectée. Le rapport s’affiche en fonction de la valeur spécifiée dans le champ **Exécuter ce rapport avec les droits d’accès suivants :** plutôt qu’en fonction de la valeur définie dans le filtre de caractères génériques.
>
>Pour plus d’informations sur les caractères génériques pour les champs utilisateur ou utilisatrice, voir la section « Variables basées sur l’utilisateur ou l’utilisatrice » dans [Vue d’ensemble des variables de filtre de caractères génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Envoyer un rapport avec les droits d’accès d’une autre personne

Vous pouvez configurer les rapports pour qu’ils soient envoyés en tant que pièce jointe à un e-mail. Vous pouvez configurer ces rapports remis pour qu’ils s’affichent de la même manière que pour les utilisateurs et utilisatrices ayant un niveau d’accès supérieur, afin que tous les utilisateurs et utilisatrices puissent voir les mêmes informations dans les rapports remis. Les utilisateurs et utilisatrices qui verront le rapport remis dans l’e-mail doivent être ajoutés à la liste des personnes destinataires de l’envoi du rapport. Pour plus d’informations sur le paramétrage d’un rapport en vue de sa remise, voir l’article [Vue d’ensemble de la remise des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Pour remettre un rapport avec les droits d’accès d’une autre personne, procédez comme suit :

1. Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **Rapports**.

1. Sélectionnez le rapport que vous souhaitez diffuser avec les droits d’accès d’une autre personne.
1. Cliquez sur le nom du rapport pour le sélectionner.
1. Cliquez sur **Actions de rapport**.
1. Cliquez sur **Envoyer le rapport**.

1. Dans le champ **Diffuser ce rapport avec les droits d’accès de :**, commencez à taper le nom de la personne sous lequelle vous souhaitez que le rapport s’affiche lorsqu’il est envoyé par e-mail, puis sélectionnez-le lorsqu’il apparaît dans la liste. La valeur par défaut est le nom de la personne qui crée le rapport.\
   ![Rapport envoyé avec droits d’accès de ](assets/unshimmed-send-report-access-rights-of.png)

   >[!NOTE]
   >
   >Les personnes ayant un niveau d’accès inférieur qui sont autorisées à créer des rapports n’ont pas la possibilité de sélectionner une autre personne qu’elles-mêmes pour le champ **Diffuser ce rapport avec les droits d’accès de :**.

1. Sélectionnez le **format** dans lequel vous souhaitez que le rapport s’affiche dans l’e-mail :

   * HTML
   * PDF
   * Excel
   * Excel (.xlsx)
   * TSV

1. Cliquez sur **Envoyer maintenant** pour l’envoyer immédiatement.\
   Ou\
   Cliquez sur **Effectuer une diffusion répétée** pour planifier une diffusion récurrente du rapport.\
   Pour plus d’informations sur les diffusions des rapports, voir l’article [Vue d’ensemble de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Limitations pour les rapports avec une colonne Source

Les rapports suivants affichent une colonne Source dans laquelle vous pouvez afficher des informations sur l’objet parent :

* Rapports sur les événements
* Rapports sur les heures
* Rapports sur les documents

Si les personnes ne disposent pas d’autorisations sur l’objet parent d’un problème, d’une heure ou d’un document, la colonne Source du rapport s’affiche vide, même lorsque le rapport est configuré pour s’afficher ou pour être diffusé avec les droits d’accès d’une autre personne.

Pour afficher des informations sur l’objet parent dans le rapport, il est recommandé d’ajouter une colonne pour l’objet parent dans laquelle vous pouvez afficher le nom du parent.

Par exemple, vous pouvez ajouter l’un des éléments suivants à un rapport avec une colonne Source :

* Les colonnes Nom du projet, Nom de la tâche ou Nom du problème dans un rapport sur les documents ou les heures.
* Colonnes Nom du projet ou Nom de la tâche pour un rapport sur les problèmes.
* Une colonne utilisant des expressions en mode texte qui fait référence aux trois objets. Voici un exemple de rapport sur les heures :

  ```
  displayname=Custom Source
  
  linkedname=opTask
  
  namekey=view.relatedcolumn
  
  namekeyargkey.0=opTask
  
  namekeyargkey.1=name
  
  textmode=true
  
  valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))
  
  valueformat=HTML
  ```

  Pour plus d’informations sur les vues en mode texte, voir [Modifier une vue en mode texte](../text-mode/edit-text-mode-in-view.md).