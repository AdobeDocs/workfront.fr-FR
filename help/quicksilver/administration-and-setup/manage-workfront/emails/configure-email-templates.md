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
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 1%

---

# Configurer des modèles de courrier électronique

En tant qu’administrateur Adobe Workfront, vous pouvez configurer des modèles d’email pour prendre en charge les notifications de rappel.

Les modèles d’email contiennent le message envoyé aux utilisateurs lorsqu’une notification de rappel est lancée.\
Sans modèle d&#39;email, la notification de rappel sera diffusée en tant que contenu vide dans le corps de l&#39;email.

Les modèles de courrier électronique peuvent être associés à des notifications de rappel pour les problèmes, les tâches, les projets et les feuilles de temps. Lors de la création de modèles de courrier électronique, votre administrateur Workfront peut fournir du contenu pour le courrier électronique et un objet.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Administrateur système</p> </td> 
  </tr> 
 </tbody> 
</table>

## Créer un modèle de courrier électronique {#create-a-new-email-template}

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Email** > **Notifications**.

1. Cliquez sur le bouton **Modèles de courrier électronique** , puis cliquez sur **Nouveau modèle de courrier électronique**.

1. Dans le **Nouveau modèle de courrier électronique** qui s’affiche, indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Modèle de courrier électronique</td> 
      <td>Titre du modèle d’email (obligatoire).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Description du modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type d’objet</td> 
      <td>Indiquez le type d’objet avec lequel vous souhaitez associer le modèle (obligatoire, il sera défini par défaut sur "Problème").</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Objet </td> 
      <td>Objet affiché lors de l’envoi du message électronique (obligatoire).</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> <p>Contenu affiché lors de l’envoi du message électronique.</p> <p>Vous pouvez utiliser la mise en forme par HTML pour le contenu de l’email, comme décrit dans la section <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">Ajouter un formatage de HTML à un modèle de courrier électronique</a> dans cet article.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

## Ajouter un formatage de HTML à un modèle de courrier électronique {#add-html-formatting-to-an-email-template}

Vous pouvez ajouter des balises de HTML aux modèles de courrier électronique pour produire des notifications personnalisées.\
Commencez à créer le modèle d’email comme décrit dans la section [Créer un modèle de courrier électronique](#create-a-new-email-template).

La mise en forme des HTMLs peut enrichir vos modèles d&#39;email, comme illustré dans les sections suivantes.

* [Lien vers des objets Workfront](#link-to-workfront-objects)
* [Lien vers des champs personnalisés avec HTML](#link-to-custom-fields-with-html)
* [Exemples de courriers électroniques de HTML](#html-email-examples)

### Lien vers des objets Workfront {#link-to-workfront-objects}

Vous pouvez inclure des liens vers les champs Workfront à l’aide du `$$` caractère générique indiquant au générateur de messagerie de rechercher les valeurs de la base de données associées à un objet spécifique.

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

<!-- Refer to the API Explorer and select the names of your objects from the Fields tab of any object. For more information about the API Explorer, see [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

* Utilisez la valeur &quot;valueField&quot; que vous trouvez dans une vue en mode texte d’un rapport. Pour plus d’informations sur les valeurs du mode texte, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   La valeur &quot;titre&quot; peut être le nom de l’objet, car vous souhaitez qu’il apparaisse dans le corps de l’email.

### Lien vers des champs personnalisés avec HTML {#link-to-custom-fields-with-html}

Vous pouvez inclure des liens vers des utilisateurs et des champs personnalisés à l’aide de la variable **$$** caractère générique indiquant au générateur de messagerie de rechercher les valeurs de la base de données associée à l’objet. Ils doivent être présents de chaque côté de la référence d’attribut de la base de données.

Par exemple, l’ajout du texte suivant en tant que HTML ajouterait le prénom de l’utilisateur affecté à la notification de rappel associée à une tâche :

`assignedTo:firstName`

Pour ajouter des champs personnalisés utilisant la même mise en forme, vous pouvez ajouter les éléments suivants dans votre notification électronique :

`DE:Custom Field As It Appears in Workfront`

Par exemple, il s’agit d’un modèle d’email qui comprend une référence à un champ personnalisé nommé Date de diffusion et qui suppose que le champ Date de diffusion appartient à une tâche.

Remplacer `<your domain>` avec le domaine Workfront de votre entreprise, sans les crochets :

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

### Exemples de courriers électroniques de HTML {#html-email-examples}

* [Notification de rappel de projet tardif (exemple)](#late-project-reminder-notification-example)
* [Rappel Tâche ou problème sur le point de démarrer (exemple)](#task-or-issue-about-to-start-reminder-example)

#### Notification de rappel de projet tardif (exemple) {#late-project-reminder-notification-example}

Pour modifier un modèle d’email en vue d’un rappel de projet tardif, tenez compte de ces informations pour les champs Objet et Contenu .

Remplacer `<your domain>` avec le domaine Workfront de votre entreprise, sans les crochets.

**Objet:**

Un Projet Que Vous Gérez Est Devenu En Retard

**Contenu:**

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

![](assets/screen-shot-2016-09-16-at-3.52.54-pm-350x103.png)

#### Rappel Tâche ou problème sur le point de commencer {#task-or-issue-about-to-start-reminder-example}

Vous pouvez également créer une notification de rappel pour une tâche ou un problème à venir.

Le code suivant peut être inclus dans un modèle d’email à utiliser pour les notifications de tâche et de rappel envoyées un nombre indéfini de jours avant la date prévue de début de la tâche ou du problème.

Remplacer `<your domain>` avec le domaine Workfront de votre entreprise, sans les crochets.

Pour l’utiliser pour un message électronique de problème, modifiez la variable `/task/view.` dans le lien de l’élément de travail vers `/issue/view`.

**Objet:**

`$$name$$ to start on $$plannedStartDate$$`

**Contenu:**

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
