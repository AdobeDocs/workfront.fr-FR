---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Afficher : calculer les différences d''heure et de date'''
description: Découvrez comment calculer les différences d’heure et de date.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 23%

---

# Vue : calculer les différences d’heure et de date

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>Vous ne pouvez pas calculer la différence entre l’heure et la date dans Adobe Workfront entre deux objets différents du même type. Par exemple, vous ne pouvez pas calculer la différence entre l’heure et la date de deux dates sur deux projets, tâches ou problèmes différents.

Vous pouvez calculer la différence entre les éléments suivants :

* Différence entre l’heure et la date entre deux champs de date sur le même objet
* Différence d’heure et de date entre un champ d’un objet et un autre champ de l’objet parent

>[!TIP]
>
>Ces calculs affichent le nombre de jours entre deux dates. Le résultat s’affiche en jours. L’horodatage du champ de date est également pris en compte et le nombre de jours peut être suivi de décimales si les horodatages ne correspondent pas. Si la tâche a été effectuée en retard, le nombre de jours s’affiche sous la forme d’une valeur négative.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : </p><ul><li><p>Contributeur à la modification d’une vue </p></li><li>
   <p>Standard pour modifier un rapport</p></li></ul><p>Ou</p><p>Actuel :</p><ul><li><p>Demander la modification d’une vue </p></li><li>
   <p>Prévoir la modification d’un rapport</p> </li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier une vue</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Calcul de la différence entre l’heure et la date de deux champs de date sur le même objet

Vous pouvez, par exemple, calculer la différence entre la date de fin planifiée et la date de fin réelle d’une tâche.

![](assets/view-planned-actual-completion-dates-datediff-column-new.png)

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter la colonne** et commencez à saisir &quot;Date d’achèvement planifiée&quot; dans le champ **Afficher dans cette colonne** , puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Cliquez sur **Ajouter la colonne** et commencez à saisir &quot;Date d’achèvement réelle&quot; dans le champ **Afficher dans cette colonne** , puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Cliquez sur **Ajouter une colonne**, puis sur **Passer en mode Texte**.

1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :

   ```
    displayname=Planned-Actual Completion Date
    linkedname=direct
    querysort=plannedCompletionDate
    textmode=true
    valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)
    valueformat=HTML
   ```

1. Cliquez sur **Enregistrer**, puis sur **Enregistrer la vue**.

## Calcul de la différence entre l’heure et la date du champ sur un objet et d’un autre champ sur un objet parent

Pour obtenir la liste des objets et de leurs parents, reportez-vous à la section &quot;Présentation de l’interdépendance et de la hiérarchie des objets&quot; dans la section [Présentation des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Vous pouvez, par exemple, calculer la différence entre la date d’achèvement planifié d’une tâche et la date d’achèvement planifié de sa tâche parent, ou du projet sur lequel la tâche est effectuée.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-new.png)

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter la colonne** et commencez à saisir &quot;Date d’achèvement prévue du projet&quot; ou &quot;Date d’achèvement parente&quot; dans le champ **Afficher dans cette colonne** , puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Cliquez sur **Ajouter la colonne** et commencez à saisir &quot;Date d’achèvement planifiée&quot; dans le champ **Afficher dans cette colonne** , puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Cliquez sur **Ajouter une colonne**, puis sur **Passer en mode Texte**.

1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par l’un des codes suivants :

   * Pour afficher la différence entre la date d’achèvement planifiée du projet et celle de la tâche :

     ```
      displayname=Project Planned Completion - Task Planned Completion (Days)
      textmode=true
      valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)
      valueformat=HTML
     ```

   * Pour afficher la différence entre la date d’achèvement planifiée de la tâche parente et celle de la tâche :

     ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)
      textmode=true<br>valueformat=HTML
      displayname=Parent Planned Completion - Planned Completion (Days)
     ```

1. Cliquez sur **Enregistrer**, puis sur **Enregistrer la vue**.
