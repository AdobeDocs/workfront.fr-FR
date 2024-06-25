---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Création et modification de règles de fonctionnement
description: Vous pouvez indiquer si vous souhaitez recevoir de nouvelles fonctionnalités Workfront sur une base mensuelle ou trimestrielle.
author: Lisa
feature: System Setup and Administration
role: Admin
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d96ddcc2f514d9f79e94a3437a3b66e07a270abc
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 4%

---

# Création et modification de règles de fonctionnement

Une règle de fonctionnement vous permet d’appliquer la validation aux objets Workfront et d’empêcher les utilisateurs de créer, modifier ou supprimer un objet lorsque certaines conditions sont remplies. Les règles métier permettent d’améliorer la qualité des données et l’efficacité opérationnelle en empêchant les actions susceptibles de compromettre l’intégrité des données.

Une règle de fonctionnement unique ne peut être affectée qu’à un seul objet. Par exemple, si vous créez une règle de fonctionnement pour ne pas modifier les projets dans certaines conditions, vous ne pouvez pas appliquer la même règle aux tâches. Vous devez créer une règle de fonctionnement distincte avec les mêmes conditions pour les tâches.

Les niveaux d’accès et le partage d’objets ont une priorité plus élevée que les règles métier lorsqu’un utilisateur interagit avec un objet. Par exemple, si un utilisateur dispose d’un niveau d’accès ou d’une autorisation qui ne permet pas de modifier un projet, ceux-ci sont prioritaires sur une règle de fonctionnement qui autorise la modification d’un projet dans certaines conditions.

Il existe également une hiérarchie lorsque plusieurs règles métier sont appliquées à un objet. Par exemple, vous avez deux règles de fonctionnement. L&#39;une restreint la création des dépenses au mois de février. La seconde empêche la modification d’un projet lorsque l’état du projet est Terminé. Si un utilisateur tente d’ajouter une dépense à un projet terminé en juin, la dépense ne peut pas être ajoutée car elle a déclenché la deuxième règle.

Les règles de fonctionnement s’appliquent à la création, la modification et la suppression d’objets via l’API ainsi que dans l’interface de Workfront.

>[!NOTE]
>
>Comme les règles de fonctionnement bloquent certaines actions, vous devez toujours configurer vos règles de fonctionnement d’abord dans un environnement de test ou d’aperçu et les tester minutieusement avant de les activer en production.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Forfait Adobe Workfront</td> 
   <td>Final</td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurations du niveau d’accès</td> 
   <td>Administrateur ou administratrice système</td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Scénarios de règles de fonctionnement

Voici quelques scénarios de règles de fonctionnement simples :

* Les utilisateurs ne peuvent pas ajouter de nouvelles dépenses pendant la dernière semaine de février. Cette formule pourrait être formulée comme suit : `IF(AND(MONTH($$TODAY) = 2, DAYOFMONTH($$TODAY) >= 22), "You cannot add new expenses during the last week of February.")`
* Les utilisateurs ne peuvent pas modifier un projet dont l’état est Terminé. Cette formule pourrait être formulée comme suit : `IF({status} = "CPL", "You cannot edit this project because it is in Complete status.")`

La syntaxe de création d’une règle de fonctionnement est la même que celle de création d’un champ calculé dans un formulaire personnalisé. Pour plus d’informations sur la syntaxe, voir [Ajouter des champs calculés avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Pour plus d’informations sur les instructions IF, voir [Présentation des instructions &quot;IF&quot;](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) et [Opérateurs de condition dans les champs personnalisés calculés](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Pour plus d’informations sur les caractères génériques basés sur l’utilisateur, voir [Utilisation de caractères génériques basés sur l’utilisateur pour généraliser des rapports](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Pour plus d’informations sur les caractères génériques basés sur des dates, voir [Utilisation de caractères génériques basés sur des dates pour généraliser des rapports](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

## Ajouter une nouvelle règle de fonctionnement

{{step-1-to-setup}}

1. Cliquez sur **Règles de fonctionnement** dans le panneau de gauche.
1. Cliquez sur **Nouvelle règle de fonctionnement**.
1. Sélectionnez le type d’objet auquel affecter la règle de fonctionnement, puis cliquez sur **Continuer**.

   ![Sélection d’un objet](assets/object-for-business-rule2.png)

1. Saisissez le **Nom** pour la règle de fonctionnement.
1. Dans le **Est actif** , choisissez si la règle doit être active lors de son enregistrement.

   Si vous sélectionnez **Non**, la règle est enregistrée comme inactive et vous pouvez l’activer ultérieurement.

1. Sélectionnez une **Déclencheur** pour la règle de fonctionnement. Les options sont les suivantes :

   * **A la création de l’objet :** La règle est appliquée lorsqu’un utilisateur tente de créer un objet.
   * **Lors de la modification de l’objet :** La règle est appliquée lorsqu’un utilisateur tente de modifier un objet.
   * **Lors de la suppression d’objet :** La règle est appliquée lorsqu’un utilisateur tente de supprimer un objet.

1. (Facultatif) Saisissez un **Description** de la règle de fonctionnement et ce qui se produit lorsqu’elle est appliquée.
1. Créez la formule dans l’éditeur de formule, au centre de la boîte de dialogue des règles de fonctionnement.

   Le format d’une règle de fonctionnement est &quot;SI la condition définie est remplie, l’utilisateur ne peut pas effectuer d’action sur l’objet et le message s’affiche&quot;.

   Dans la zone de formule, les parties de la règle de fonctionnement que vous créez sont la condition et le message qui s’affiche dans Workfront lorsque la condition est remplie.

   * L’&quot;objet&quot; est le type d’objet sélectionné lors de la création de la règle de fonctionnement. Il s’affiche dans l’en-tête de la boîte de dialogue.
   * L’&quot;action&quot; est le déclencheur que vous avez sélectionné pour la règle : créez, modifiez ou supprimez l’objet.
   * Comme l’objet et l’action sont déjà définis, vous ne les incluez pas dans la formule.
   * Le message d’erreur personnalisé s’affiche pour l’utilisateur lorsqu’il déclenche la règle de fonctionnement. Il doit fournir des instructions claires sur ce qui s’est mal passé et comment corriger le problème.

   ![Boîte de dialogue Ajouter une règle de fonctionnement](assets/add-business-rule-dialog-no-ai-button.png)

   Cet exemple est une règle de fonctionnement pour les dépenses. Si le mois en cours est le mois de juin, les utilisateurs ne sont pas autorisés à créer de nouvelles dépenses et le message l’explique.

   Pour consulter d’autres exemples de règles de fonctionnement, voir [Scénarios de règles de fonctionnement](#scenarios-for-business-rules) dans cet article.

1. (Facultatif) Utilisez la formule **Expressions** et **Champs** dans le panneau de droite pour faciliter la création de la règle.

   Recherchez une expression ou un champ pour restreindre la liste des éléments disponibles.

   La liste des champs disponibles est limitée aux champs liés au type d’objet pour la règle de fonctionnement.

1. Cliquez sur **Enregistrer** lorsque vous avez terminé de créer la règle de fonctionnement.

>[!NOTE]
>
>Après avoir ajouté une règle de fonctionnement, vous devez la tester en ajoutant, modifiant ou supprimant l’objet associé afin de vous assurer que la règle est correctement appliquée.

## Activer une règle de fonctionnement

Lorsqu’une règle de fonctionnement est inactive, le champ Est active de la liste des règles de fonctionnement affiche False. Vous ne pouvez pas mettre à jour l’état de la règle en mode Liste.

Pour activer une règle de fonctionnement :

1. Sélectionnez la règle de fonctionnement dans la liste des règles et cliquez sur l&#39;icône Modifier .
1. Sélectionner **Oui** pour **Est actif** dans la boîte de dialogue des règles de fonctionnement.
1. Cliquer sur **Enregistrer**.
