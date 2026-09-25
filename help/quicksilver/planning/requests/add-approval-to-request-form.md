---
title: Ajout d’une approbation à un formulaire de demande dans Adobe Workfront Planning
description: Vous pouvez ajouter un processus d’approbation à un formulaire de demande Adobe Workfront Planning, afin de lancer une approbation pour chaque demande soumise, avant la création d’un enregistrement.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/E9LEGJ8T822JuvIO3s8nn6UkLbX-j4ffwaKSviKxl0o
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 3b3d455ded251b06084249cf9df12c1f112f05e9
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 5%
---
# Ajouter une approbation à un formulaire de demande dans Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->


<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Vous pouvez ajouter un processus d’approbation à un formulaire de demande Adobe Workfront Planning, afin de lancer une approbation pour chaque demande soumise, avant la création d’un enregistrement.

<!--<span class="preview">Multiple stages are supported in the approval process. When all required decisions in a stage are made, the next stage begins and the new stage's approvers receive an email notification.</span>-->

Cet article décrit comment un responsable d’espace de travail peut ajouter une approbation à un formulaire de demande associé à un type d’enregistrement.

Pour plus d’informations sur la création d’un formulaire de demande dans Workfront Planning, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Pour plus d’informations sur la soumission d’une demande à un type d’enregistrement pour créer un enregistrement, voir [ Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Tout Workfront ou workflow avec un package Planning</p></li>
Ou
<li><p>Tout package Planning lorsqu’il est acheté en tant que produit autonome</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Norme de workflow</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Norme de planification</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Vous devez ajouter un workflow et un type de licence Planning au niveau d'accès lorsque vous disposez à la fois d'un workflow et d'un package Planning</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérez les autorisations d’un espace de travail et d’un type d’enregistrement</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à l’ajout d’approbations à un formulaire de demande

* Vous pouvez ajouter un ou plusieurs approbateurs (utilisateurs ou équipes) à un formulaire de demande ou à une règle d’approbation.
* Les règles d’approbation acheminent les demandes en fonction des valeurs de champ de la demande soumise (par exemple, différents approbateurs pour différentes valeurs d’un champ « Type de campagne »).
* Vous pouvez afficher les informations d&#39;approbation sur l&#39;enregistrement créé à partir des champs Date d&#39;approbation par et Date d&#39;approbation . Voir Création de champs.
* Si tous les approbateurs approuvent, un enregistrement est créé pour le type d&#39;enregistrement associé au formulaire de demande.
* Si au moins un approbateur rejette la demande, aucun enregistrement n’est créé pour le type d’enregistrement ; la demande reste/se trouve à la place dans la zone des Demandes de Workfront. (Ce point est apparu dans les deux sections avec un libellé légèrement différent — fusionné ici en une seule déclaration.)
* Lorsque plusieurs approbateurs sont requis, ils doivent tous prendre une décision avant que la demande ne soit approuvée ou rejetée, sauf si l’option Une seule décision est requise est activée.
* Si une équipe est définie comme approbateur, une seule décision est nécessaire de la part d&#39;un membre de cette équipe.
* Les approbations sont facultatives : si aucune approbation n&#39;est jointe à un formulaire de demande, Workfront Planning crée l&#39;enregistrement immédiatement après l&#39;envoi.
* <span class="preview">Vous pouvez ajouter une ou plusieurs étapes aux approbations.</span>

## Ajouter des règles d’approbation à un formulaire de demande

Les règles d’approbation définissent le processus d’approbation en fonction des valeurs de champ dans les demandes envoyées.

Par exemple, si un formulaire de demande comporte le champ « Type de campagne », il est possible de créer une règle qui envoie la demande à une personne lorsque le champ comporte la valeur « Numérique » et à une autre personne lorsqu’il comporte la valeur « Imprimer ».

Pour définir des règles d&#39;approbation pour un formulaire de demande :

1. Commencez à créer un formulaire de demande pour un type d’enregistrement, comme décrit dans l’article [Créer et gérer un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Lorsque le formulaire s’ouvre, cliquez sur **Paramètres**.

   L’onglet **Paramètres** s’ouvre.

1. Pour commencer à configurer les règles d’approbation, cliquez sur **Approbations** ![Icône Validations](assets/approvals-icon-on-form.png) dans le panneau de gauche.

1. (Facultatif) Si vous souhaitez définir un processus d&#39;approbation par défaut, ajoutez au moins un utilisateur ou une équipe au champ **Approbateurs** de la zone **Règle d&#39;approbation par défaut**, puis cochez la case **Une seule décision est requise** si vous souhaitez que l&#39;enregistrement soit créé après son approbation par l&#39;un des approbateurs par défaut.

   ![Zone de règle d&#39;approbation par défaut](assets/default-approvers.png)

1. (Facultatif) Commencez à ajouter des règles d’approbation. Pour chaque règle d’approbation personnalisée, procédez comme suit :

   1. Cliquez sur **Ajouter une règle d’approbation**.
   1. Cliquez sur le titre de l’espace réservé **Règle d’approbation sans titre** et saisissez un nom pour la règle d’approbation.
   1. Cliquez sur **Sélectionner un champ** et sélectionnez le champ qui active la règle.
   1. Sélectionnez l’opérateur de la règle. Les opérateurs varient en fonction du type de champ.
   1. Si l’opérateur sélectionné requiert une valeur, cliquez sur l’icône plus et ajoutez une ou plusieurs valeurs.
   1. (Facultatif) Cliquez sur **Ajouter une condition** pour ajouter d’autres conditions et les connecter par des instructions **Et** ou **Ou** en configurant les conditions supplémentaires comme indiqué dans les étapes C-E.
   1. Dans la zone **Actions** de la règle d&#39;approbation, dans le champ **Approbateurs**, ajoutez au moins un utilisateur ou une équipe à définir comme approbateur lorsque la condition est remplie.
   1. (Conditionnel et facultatif) Si vous souhaitez que l&#39;enregistrement soit créé après son approbation par l&#39;un des approbateurs, cochez la case **Une seule décision est requise**. Dans le cas contraire, tous les approbateurs doivent décider de l&#39;approbation avant que la demande ne soit acceptée ou rejetée.

   >[!NOTE]
   >
   >   Tenez compte des points suivants lors de l’ajout de règles d’approbation :
   >
   >   * Si seule une règle par défaut est configurée, elle s’applique à chaque demande soumise.
   >   * Si une règle personnalisée est respectée, la valeur par défaut n’est pas appliquée au workflow d’approbation de la demande. Seules les règles personnalisées correspondantes s’appliquent pour les approbations et la règle par défaut est ignorée.
   >   * Si plusieurs règles personnalisées sont respectées, la première de l’ordre s’applique. Dans ce cas, l’approbation par défaut ne s’applique pas, le cas échéant.

1. <span class="preview">(Facultatif) Cliquez sur **Ajouter une étape** pour ajouter une autre étape à l’approbation.</span>

1. Cliquez sur **Enregistrer** pour enregistrer les règles d’approbation.

1. <span class="preview">(Facultatif) Pour ajouter d’autres étapes à l’approbation, procédez comme suit :</span>

   1. <span class="preview">Cliquez sur **Ajouter une étape**.</span>

      <span class="preview">La zone **Validation en plusieurs étapes** s’affiche. Si vous avez déjà créé une action d’approbation par défaut, ces approbateurs sont automatiquement ajoutés à l’étape 1.</span>

   1. <span class="preview">Dans le champ **Ajouter des personnes ou des équipes**, ajoutez au moins un utilisateur ou une équipe à définir comme approbateur pour l’étape.</span>
   1. <span class="preview">(Conditionnel et facultatif) Si vous souhaitez que l&#39;enregistrement passe à l&#39;étape suivante après son approbation par l&#39;un des approbateurs, cochez la case **Une seule décision est requise**. Dans le cas contraire, tous les approbateurs doivent décider de l’approbation avant que la demande ne passe à l’étape suivante.</span>
   1. <span class="preview">Cliquez sur **Ajouter une étape** et répétez l’étape B pour ajouter d’autres étapes à l’approbation.</span>

      <span class="preview">Lorsqu’il existe plusieurs étapes, vous pouvez cliquer sur l’icône **Glisser** ![Icône Glisser](assets/drag-icon.png) pour les faire glisser et les déposer dans l’ordre.</span>

      <span class="preview">Cliquez sur **Supprimer cette étape** pour supprimer une étape de l’approbation, ou cliquez sur l’icône **Supprimer** ![icône Supprimer](assets/delete.png) à côté d’un approbateur ou d’une approbatrice pour supprimer l’utilisateur ou l’équipe de la liste des approbateurs dans une étape.</span>

      ![Zone de validation en plusieurs étapes](assets/planning-request-multi-stage-approval-box.png)

   1. <span class="preview">Lorsque vous avez terminé de créer le workflow d’approbation, cliquez sur **Enregistrer**.</span>

      <span class="preview">Vous pouvez modifier ou supprimer l’approbation multi-étape à partir de la page Approbations </span>.

1. (Facultatif) Cliquez sur **Publier** si vous n’avez jamais partagé le formulaire de demande auparavant.



<!--

## Add an approval to a request form in the Production environment

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 
1. (Optional and conditional) If you have set more than one approver, and only need one approver to make a decision, enable the **Only one decision is required** option.

    (****most of the Note below is duplicated in the Create a request form article***)

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Requests area of Workfront.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before.

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers.

   For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).

-->