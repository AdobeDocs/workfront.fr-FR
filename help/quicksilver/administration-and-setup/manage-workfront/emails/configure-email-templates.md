---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: Configurer des modèles de courrier électronique
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer des modèles d’email pour prendre en charge les notifications de rappel.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 8%

---

# Configurer des modèles de courrier électronique

En tant qu’administrateur Adobe Workfront, vous pouvez configurer des modèles d’email pour prendre en charge les notifications de rappel.

Les modèles d’email contiennent le message envoyé aux utilisateurs lorsqu’une notification de rappel est lancée.\
Sans modèle d&#39;email, la notification de rappel sera diffusée en tant que contenu vide dans le corps de l&#39;email.

Les modèles de courrier électronique peuvent être associés à des notifications de rappel pour les problèmes, les tâches, les projets et les feuilles de temps. Lors de la création de modèles de courrier électronique, votre administrateur Workfront peut fournir du contenu pour le courrier électronique et un objet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td><p>Actuelle : formule</p>
   Ou
   <p>Nouvelle : standard</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Administrateur ou administratrice système</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création d’un modèle de courrier électronique {#create-an-email-template}

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Email** > **Notifications**> **Modèles d’e-mail**.

   ![](assets/email-templates-tab-under-setup-email-notifications-area.png)

1. Cliquez sur **Nouveau modèle de courrier électronique**.

1. Dans la zone **Nouveau modèle de courrier électronique**, spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td>Ajoutez un titre pour le modèle d’email. Il s’agit d’un champ obligatoire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type d’objet</td> 
      <td>Indiquez le type d’objet auquel vous souhaitez associer le modèle. Choisissez l’un des objets suivants :
      <ul>
      <li>Projet</li>
      <li>Tâche</li>
      <li>Problème</li>
      <li>Feuille de temps</li> </ul>

   Il s’agit d’un champ obligatoire, défini par défaut sur Projet.</td>
   </tr>
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Ajoutez des informations supplémentaires sur le modèle d’email, son objectif et l’audience prévue.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Objet </td> 
      <td>Ajoutez le texte qui s'affiche dans la ligne Objet de l'email, lors de l'envoi du message électronique généré par le modèle. Il s’agit d’un champ obligatoire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Corps </td> 
      <td> <p>Ajoutez le texte du contenu de l'email.</p> <p>Vous pouvez utiliser la mise en forme des HTMLS pour le contenu de l'email, comme décrit dans la section <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">Ajouter une mise en forme des HTMLS à un modèle d'email</a> de cet article.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

## Ajouter un formatage d’HTML à un modèle d’email {#add-html-formatting-to-an-email-template}

Vous pouvez ajouter des balises d’HTML aux modèles de courrier électronique pour produire des notifications personnalisées.\
Commencez à créer le modèle d’email comme décrit dans [Créer un modèle d’email](#create-a-new-email-template).

La mise en forme des HTMLS peut enrichir vos modèles d&#39;email, comme illustré dans les sections suivantes.

* [Lien vers des objets Workfront](#link-to-workfront-objects)
* [Lien vers des champs personnalisés avec HTML](#link-to-custom-fields-with-html)
* [Exemples d’HTML d’email](#html-email-examples)

### Lien vers des objets Workfront {#link-to-workfront-objects}

Vous pouvez inclure des liens vers les champs Workfront à l’aide du caractère générique `$$` pour indiquer au générateur de messagerie de rechercher des valeurs de la base de données associée à un objet spécifique.

Par exemple, le corps de l’email pour une notification alertant la personne désignée de la tâche sur le point de démarrer peut suivre cette structure :

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

Pour obtenir la valeur &quot;caractère générique&quot; d’un objet, effectuez l’une des opérations suivantes :

* Reportez-vous à l’ explorateur d’API et sélectionnez les noms de vos objets dans l’onglet Champs de n’importe quel objet. Pour plus d’informations sur l’API Explorer, voir [API Explorer](/help/quicksilver/wf-api/general/api-explorer.md).

* Utilisez la valeur `valuefield` que vous trouvez dans une vue en mode texte d’un rapport. Pour plus d’informations sur les valeurs du mode texte, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

La valeur `heading` peut être le nom de l’objet, tel que vous souhaitez qu’il apparaisse dans le corps de l’email.

### Lien vers des champs personnalisés avec HTML {#link-to-custom-fields-with-html}

Vous pouvez inclure des liens vers des utilisateurs et des champs personnalisés à l’aide du caractère générique `$$` pour indiquer au générateur de messagerie de rechercher les valeurs de la base de données associée à l’objet. Ils doivent être présents de chaque côté de la référence d’attribut de la base de données.

Par exemple, l’ajout du texte suivant en tant qu’HTML ajouterait le prénom de l’utilisateur affecté à la notification de rappel associée à une tâche :

`assignedTo:firstName`

Pour ajouter des champs personnalisés utilisant la même mise en forme, vous pouvez ajouter les éléments suivants dans votre notification électronique :

`DE:Custom Field As It Appears in Workfront`

Par exemple, il s’agit d’un modèle d’email qui comprend une référence à un champ personnalisé nommé Date de diffusion et qui suppose que le champ Date de diffusion appartient à une tâche.

Remplacez `<your domain>` par le domaine Workfront de votre entreprise, sans les crochets :

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
>Si le champ appartient à un projet, remplacez la tâche par le projet :
>
>`DE:Project:Delivery Date`

### Exemples d’HTML d’email {#html-email-examples}

* [Notification de rappel de projet tardif (exemple)](#late-project-reminder-notification-example)
* [Rappel Tâche ou problème sur le point de démarrer (exemple)](#task-or-issue-about-to-start-reminder-example)

#### Notification de rappel de projet tardif (exemple) {#late-project-reminder-notification-example}

Pour modifier un modèle d’email en vue d’un rappel de projet tardif, tenez compte de ces informations pour les champs Objet et Contenu .

Remplacez `<your domain>` par le domaine Workfront de votre entreprise, sans les crochets.

**Objet :**

Un Projet Que Vous Gérer Est Devenu En Retard

**Contenu :**

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

Vous obtenez alors un email similaire à ce qui suit :

![](assets/project-became-late-email.png)

#### Rappel Tâche ou problème sur le point de commencer {#task-or-issue-about-to-start-reminder-example}

Vous pouvez également créer une notification de rappel pour une tâche ou un problème à venir.

Le code suivant peut être inclus dans un modèle d’email à utiliser pour les notifications de tâche et de rappel envoyées un nombre indéfini de jours avant la date prévue de début de la tâche ou du problème.

Remplacez `<your domain>` par le domaine Workfront de votre entreprise, sans les crochets.

Pour l’utiliser pour un message électronique de problème, remplacez la valeur `/task/view.` du lien vers l’élément de travail par `/issue/view`.

**Objet :**

`$$name$$ to start on $$plannedStartDate$$`

**Contenu :**

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

Une fois un modèle d’email créé, les utilisateurs peuvent l’associer aux notifications de rappel, comme décrit dans la section [Configuration des notifications de rappel](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
