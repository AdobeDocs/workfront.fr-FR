---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: Configurer les modèles d’e-mail
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer des modèles d’e-mail pour prendre en charge les notifications de rappel.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 98%

---


# Configurer des modèles d’e-mail

<!--Audited: 10/2024-->


En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer des modèles d’e-mail pour prendre en charge les notifications de rappel.

Les modèles d’e-mail contiennent le message envoyé aux personnes lorsqu’une notification de rappel est initée.\
Sans modèle d’e-mail, la notification de rappel sera délivrée sous la forme d’un contenu vide dans le corps de l’e-mail.

Des modèles d’e-mail peuvent être associés à des notifications de rappel pour les problèmes, les tâches, les projets et les feuilles de temps. Lors de la création de modèles d’e-mail, votre administrateur ou administratrice Workfront peut fournir le contenu de l’e-mail et une ligne d’objet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td><p>Nouveau : Standard</p>
   Ou
   <p>Actuelle : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Administrateur ou administratrice système</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur les conditions d’accès, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un modèle d’e-mail {#create-an-email-template}

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **E-mail** > **Notifications** > **Modèles d’e-mail**.

   ![Onglet Modèles d’e-mail](assets/email-templates-tab-under-setup-email-notifications-area.png)

1. Cliquez sur **Nouveau modèle d’e-mail**.

1. Dans la zone **Nouveau modèle d’e-mail**, spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td>Ajoutez un titre au modèle d’e-mail. Champ obligatoire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type d’objet</td> 
      <td>Spécifiez le type d’objet auquel vous souhaitez associer le modèle. Choisissez parmi les objets suivants :
      <ul>
      <li>Projet</li>
      <li>Tâche</li>
      <li>Problème</li>
      <li>Feuille de temps</li> </ul>

   Il s’agit d’un champ obligatoire et il est défini par défaut sur Projet.</td>
   </tr>
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Ajoutez des informations supplémentaires sur le modèle d’e-mail, son objectif et l’audience visée.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Objet </td> 
      <td>Ajoutez le texte qui s’affiche dans la ligne Objet de l’e-mail, lorsque le message généré par le modèle est envoyé. Champ obligatoire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Corps </td> 
      <td> <p>Ajoutez le texte du contenu du message de l’e-mail.</p> <p>Vous pouvez utiliser le formatage HTML pour le contenu de l’e-mail, comme décrit dans la section <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">Ajouter un formatage HTML à un modèle d’e-mail</a> de cet article.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

## Ajouter un formatage HTML à un modèle d’e-mail {#add-html-formatting-to-an-email-template}

Vous pouvez ajouter des balises HTML aux modèles d’e-mail pour produire des notifications personnalisées.\
Commencez à créer le modèle d’e-mail comme décrit dans [Créer un modèle d’e-mail](#create-a-new-email-template).

Le formatage HTML peut enrichir vos modèles d’e-mail, comme le montrent les sections suivantes.

* [Lier à des objets Workfront](#link-to-workfront-objects)
* [Lier à des champs personnalisés avec HTML](#link-to-custom-fields-with-html)
* [Exemples d’e-mails HTML](#html-email-examples)

### Lier à des objets Workfront {#link-to-workfront-objects}

Vous pouvez inclure des liens vers des champs Workfront en utilisant le caractère générique `$$` pour indiquer au générateur d’e-mails de rechercher les valeurs de la base de données associées à un objet spécifique.

Par exemple, le corps de l’e-mail d’une notification avertissant la personne cessionnaire de la tâche qu’elle est sur le point de commencer peut avoir cette structure :

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b><strong>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td></tr>
</table>
</html>
```

Pour obtenir la valeur « caractère générique » d’un objet, effectuez l’une des opérations suivantes :

* Reportez-vous à l’explorateur d’API et sélectionnez les noms de vos objets dans l’onglet Champs de n’importe quel objet. Pour plus d’informations sur l’explorateur d’API, voir [Explorateur d’API](/help/quicksilver/wf-api/general/api-explorer.md).

* Utilisez la valeur `valuefield` que vous trouvez à l’intérieur de la vue en mode texte d’un rapport. Pour plus d’informations sur les valeurs du mode texte, voir [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

La valeur `heading` peut être le nom de l’objet, tel qu’il doit apparaître dans le corps de l’e-mail.

### Lier à des champs personnalisés avec HTML {#link-to-custom-fields-with-html}

Vous pouvez inclure des liens vers des utilisateurs et utilisatrices et des champs personnalisés en utilisant le caractère générique `$$` pour indiquer au générateur d’e-mails de rechercher des valeurs dans la base de données associée à l’objet. Ils doivent être présents des deux côtés de la référence de l’attribut de la base de données.

Par exemple, en ajoutant le texte suivant en HTML, le prénom de la personne cessionnaire sera ajouté à la notification de rappel associée à une tâche :

`assignedTo:firstName`

Pour ajouter des champs personnalisés en utilisant le même formatage, vous pouvez ajouter ce qui suit dans votre notification par e-mail :

`DE:Custom Field As It Appears in Workfront`

Par exemple, il s’agit d’un modèle d’e-mail qui inclut une référence à un champ personnalisé nommé Date de diffusion et qui suppose que le champ Date de diffusion appartient à une tâche.

Remplacez `<your domain>` par le domaine Workfront de votre entreprise, sans les crochets :

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which has a Delivery Date of $$DE:Task:Delivery Date$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
<tr>
<td><b>Description:</b></td>
<td>$$description$$</td>
<tr>
<td><b>Estimated Effort:</b></td>
<td>$$work$$ hours</td>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
<td><b>Delivery Date:</b></td>
<td>$$DE:Task:Delivery Date$$</td>
</tr>
</table>
</html>
```

>[!NOTE]
>
>Si le champ appartient à un projet, remplacez tâche par projet :
>
>`DE:Project:Delivery Date`

### Exemples d’e-mails HTML {#html-email-examples}

* [Notification de rappel de projet en retard (exemple)](#late-project-reminder-notification-example)
* [Rappel de tâche ou problème sur le point de commencer (exemple)](#task-or-issue-about-to-start-reminder-example)

#### Notification de rappel de projet en retard (exemple) {#late-project-reminder-notification-example}

Pour modifier un modèle d’e-mail pour un rappel de projet en retard, tenez compte de ces informations pour les champs Objet et Contenu.

Remplacez `<your domain>` par le domaine Workfront de votre entreprise, sans les crochets.

**Objet :**

Un projet que vous gérez a pris du retard.

**Contenu :**

```html
<html>
<p>The <b><a href="https://<your domain>.my.workfront.com/project/view?ID=$$ID$$">$$name$$</a></b> project you are assigned as the owner of just became late.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
</tr>
</table>
<p>Please review the task plan and bring it up to date to reflect the progress made so far. If it is necessary to update the plan to bring it reflect reality going forward, be sure to speak to $$sponsor:name$$ for approval before make these changes to the work breakdown structure.</p>
</html>
```

Cela produit un e-mail similaire à ce qui suit :

![Le projet est devenu un e-mail en retard](assets/project-became-late-email.png)

#### Rappel de tâche ou problème sur le point de commencer {#task-or-issue-about-to-start-reminder-example}

Vous pouvez également créer une notification de rappel pour une tâche ou un problème à venir.

Le code suivant peut être inclus dans un modèle d’e-mail à utiliser pour les notifications de rappel de tâches et de problèmes qui sont envoyées un nombre quelconque de jours avant la date de début prévue de la tâche ou du problème.

Remplacez `<your domain>` par le domaine Workfront de votre entreprise, sans les crochets.

Pour l’utiliser pour un e-mail concernant un problème, remplacez la valeur `/task/view.` dans le lien vers l’élément de travail par `/issue/view`.

**Objet :**

`$$name$$ to start on $$plannedStartDate$$`

**Contenu :**

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><ahref=https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<tablewidth=350"style=font-size:12px;">
<tr>
<td><b>Task Name:</b></td>
<td>$$name$$</td>
</tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<td><b>Created on:</b></td>
<td>$$entryDate$$</td>
</tr>
<tr>
<td><b>Project Manager:</b></td>
<td>$$project:owner:name$$</td>
<tr>
<td><b>Priority:</b></td>
<td>$$priority$$</td>
</tr>
<tr>
<td><b>Who is assigned to:</b></td>
<td>$$assignedTo:name$$</td>
</tr>
<tr>
<td><b>When it's due:</b></td>
<td>$$estCompletionDate$$</td>
</tr>
</table>
</html>
```

![email_template_delivered.png](assets/email-template-delivered.png)

Après avoir créé un modèle d’e-mail, les utilisateurs et utilisatrices peuvent l’associer à des notifications de rappel, comme décrit dans [Configurer les notifications de rappel](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
