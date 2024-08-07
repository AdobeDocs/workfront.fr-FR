---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Exécuter et diffuser un rapport avec les droits d’accès d’un autre utilisateur ou d’une autre utilisatrice
description: Par défaut, les utilisateurs peuvent uniquement afficher les objets d’un rapport qu’ils sont autorisés à afficher.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 10%

---

# Exécuter et diffuser un rapport avec les droits d’accès d’un autre utilisateur ou d’une autre utilisatrice

Par défaut, les utilisateurs peuvent uniquement afficher les objets d’un rapport qu’ils sont autorisés à afficher.

Vous pouvez permettre à tous les utilisateurs d’afficher les mêmes résultats dans un rapport qu’un autre utilisateur, quel que soit leur niveau d’accès ou d’autorisation sur les objets du rapport.

Si vous exécutez un rapport avec les droits d’accès d’un autre utilisateur disposant d’un accès supérieur (par exemple, les droits d’accès d’un administrateur Adobe Workfront), tous les utilisateurs disposant des droits d’accès pour Afficher le rapport peuvent voir les informations dans le rapport en tant qu’utilisateur spécifié dans le créateur de rapports. Vous pouvez configurer cette option pour les rapports que les utilisateurs trouvent dans l’interface de Workfront ou pour les rapports qui sont remis aux utilisateurs en tant que pièce jointe à un courrier électronique.

>[!TIP]
>
>Vous ne devez remplacer le champ **Exécuter ce rapport par Droits d’accès de :** par un utilisateur actif que si vous souhaitez que le rapport s’affiche avec les droits d’accès de cet utilisateur. Par exemple, un utilisateur de licence de travail peut ne pas disposer des autorisations nécessaires pour voir tous les éléments d’un rapport créé par un utilisateur de licence du forfait ou un administrateur système, sauf si le rapport s’affiche avec les droits d’accès d’un planificateur ou d’un administrateur système.\
>Si le rapport est partagé avec des utilisateurs disposant d’un accès similaire à celui spécifié dans le champ **Exécuter ce rapport avec les droits d’accès de :** , vous pouvez laisser ce champ vide.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations d’un rapport (pour afficher le rapport remis)</p> <p>Gérer les autorisations d’un rapport (pour exécuter le rapport)</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher un rapport avec les droits d&#39;accès d&#39;un autre utilisateur

Si vous renseignez le champ **Exécuter ce rapport avec les droits d’accès de :** , un rapport contient les mêmes données, quel que soit l’utilisateur accédant au rapport. Le rapport s’affiche comme pour l’utilisateur spécifié.

Les utilisateurs accédant au rapport doivent disposer au moins des autorisations Afficher sur celui-ci pour pouvoir le voir. Si l’utilisateur répertorié dans le champ **Exécuter ce rapport avec les droits d’accès de :** est désactivé, le rapport ne s’affiche plus pour les autres utilisateurs avec lesquels le rapport est partagé.

Pour exécuter un rapport avec les droits d&#39;accès d&#39;un autre utilisateur :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis sur **Rapports**.

1. Sélectionnez le rapport à afficher avec les droits d&#39;accès d&#39;un autre utilisateur.
1. Cliquez sur **Actions de rapport**, puis sur **Modifier**.

1. Cliquez sur **Paramètres de rapport**.

1. Dans le champ **Exécuter ce rapport avec les droits d’accès de :** , commencez à saisir le nom de l’utilisateur sous lequel vous souhaitez que le rapport s’affiche, puis sélectionnez-le lorsque vous le verrez dans la liste.\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   >
   >Les utilisateurs disposant d’un niveau d’accès inférieur qui sont autorisés à créer des rapports ne peuvent pas sélectionner un utilisateur autre qu’eux pour le champ **Exécuter ce rapport avec les droits d’accès de :** .

1. Cliquez sur **Terminé**.
1. Cliquez sur **Enregistrer + Fermer**.\
   Le rapport s’affiche désormais pour tous les utilisateurs avec lesquels le rapport est partagé comme s’il avait été affiché par l’utilisateur spécifié dans le champ **Exécuter ce rapport avec les droits d’accès de :** .

>[!IMPORTANT]
>
>La saisie d’un utilisateur autre que l’utilisateur connecté pour le champ **Exécuter ce rapport avec les droits d’accès de :** a un impact sur les informations affichées dans le rapport si ce dernier contient un filtre qui utilise un caractère générique se rapportant à l’utilisateur connecté. Le rapport s’affiche en fonction de la valeur spécifiée dans le champ **Exécuter ce rapport avec les droits d’accès de :** plutôt que selon ce qui est défini dans le filtre de caractères génériques.
>
>Pour plus d’informations sur les caractères génériques pour les champs utilisateur, consultez la section &quot;Variables basées sur l’utilisateur&quot; dans la [présentation des variables de filtre génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Diffuser un rapport avec les droits d&#39;accès d&#39;un autre utilisateur

Vous pouvez configurer des rapports à envoyer en pièce jointe à un email. Vous pouvez configurer ces rapports distribués de sorte qu’ils s’affichent pour les utilisateurs de niveau d’accès supérieur afin que tous les utilisateurs puissent voir les mêmes informations dans les rapports distribués. Les utilisateurs qui verront le rapport remis dans l&#39;email doivent être ajoutés à la liste Envoyer à des destinataires dans la diffusion du rapport. Pour plus d’informations sur la configuration d’un rapport pour la diffusion, consultez l’article [Présentation de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Pour diffuser un rapport avec les droits d&#39;accès d&#39;un autre utilisateur :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis sur **Rapports**.

1. Sélectionnez le rapport à diffuser avec les droits d&#39;accès d&#39;un autre utilisateur.
1. Cliquez sur le nom du rapport pour le sélectionner.
1. Cliquez sur **Actions de rapport**.
1. Cliquez sur **Envoyer le rapport**.

1. Dans le champ **Diffusez ce rapport avec les droits d’accès de :** , commencez à saisir le nom de l’utilisateur que vous souhaitez que le rapport affiche comme lorsqu’il est envoyé par courriel, puis sélectionnez-le lorsque vous le verrez dans la liste. La valeur par défaut est le nom de l’utilisateur qui crée le rapport.\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   >
   >Les utilisateurs disposant d’un niveau d’accès inférieur qui sont autorisés à créer des rapports ne peuvent pas sélectionner un autre utilisateur qu’eux pour le champ **Diffuser ce rapport avec les droits d’accès de :** .

1. Sélectionnez le **format** que le rapport doit afficher dans l&#39;email :

   * HTML
   * PDF
   * MS Excel
   * MS Excel (.xlsx)
   * TSV

1. Cliquez sur **Envoyer maintenant** pour l’envoyer immédiatement.\
   Ou\
   Cliquez sur **Effectuer une diffusion répétée** pour planifier une diffusion récurrente pour le rapport.\
   Pour plus d’informations sur les diffusions de rapports, consultez l’article [Présentation de la diffusion de rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Limites des rapports avec une colonne Source

Les rapports suivants affichent une colonne Source dans laquelle vous pouvez afficher des informations sur l’objet parent :

* Rapports sur les problèmes
* Rapports d’heure
* Rapports sur les documents

Si les utilisateurs ne disposent pas d’autorisations sur l’objet parent d’un problème, d’une heure ou d’un document, la colonne Source du rapport s’affiche vide, même lorsque le rapport est configuré pour s’afficher ou pour être diffusé avec les droits d’accès d’un autre utilisateur.

Pour afficher des informations sur l’objet parent dans le rapport, il est recommandé d’ajouter une colonne pour l’objet parent dans laquelle vous pouvez afficher le nom du parent.

Par exemple, vous pouvez ajouter l’un des éléments suivants à un rapport avec une colonne Source :

* Les colonnes Nom du projet, Nom de la tâche ou Nom de la publication dans un document ou un rapport d’heure.
* Colonnes Nom du projet ou Nom de la tâche pour un rapport de problème.
* Colonne utilisant des expressions du mode texte qui font référence aux trois objets. Voici un exemple de rapport d’une heure :

  `displayname=Custom Source`

  `linkedname=opTask`

  `namekey=view.relatedcolumn`

  `namekeyargkey.0=opTask`

  `namekeyargkey.1=name`

  `textmode=true`

  `valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))`

  `valueformat=HTML`

  Pour plus d’informations sur les vues en mode texte, voir [Modifier une vue à l’aide du mode texte](../text-mode/edit-text-mode-in-view.md).