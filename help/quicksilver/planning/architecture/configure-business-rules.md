---
title: Configurer les règles métier de type d’enregistrement
description: Vous pouvez configurer des règles métier de type enregistrement qui peuvent appliquer certaines actions sur les enregistrements en fonction des valeurs de champ.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6f64c3e6ebb8407c38ad3a1d46b2fc63b534879e
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 4%

---


# Configurer des règles métier de type enregistrement

{{planning-important-intro}}

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Vous pouvez configurer des règles métier pour les types d’enregistrements Adobe Workfront Planning afin d’indiquer que certains champs sont requis avant qu’une action sur un enregistrement de ce type soit autorisée ou empêchée.

Selon la formulation de la règle, vous pouvez autoriser les actions suivantes sur les enregistrements si les règles métier définies sont respectées :

* Modifier ou ne pas modifier un enregistrement
* Supprimer ou ne pas supprimer un enregistrement

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès afin d’effectuer les étapes de cet article :  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
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
   <td>   <p>Gérer les autorisations sur un espace de travail et sur un type d’enregistrement</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant la configuration des règles métier

* Les règles métier joignent une condition à une modification de champ ou à une suppression d’enregistrement. La règle n’entre en jeu qu’à un seul moment précis et délibéré : lorsqu’un champ est sur le point de devenir une valeur de champ que vous configurez dans la règle.

* Voici à quoi ressemble une règle en langage clair : « Avant de pouvoir modifier cet enregistrement, le champ Résumé de la campagne doit avoir une valeur ».

  Si le champ est vide, la modification de l’enregistrement est bloquée et l’utilisateur reçoit un message clair expliquant ce qu’il doit faire avant de continuer. Une fois qu’il a mis à jour le champ obligatoire et réessayé, la modification est autorisée.

* Les règles ne bloquent pas la création d’enregistrements. Les utilisateurs peuvent toujours créer des enregistrements, mais ils doivent s’assurer que les champs obligatoires ne sont pas vides ou ne contiennent pas la valeur spécifiée.
* Les règles ne modifient ou ne suppriment pas automatiquement les enregistrements. La modification doit être délibérée et déclenchée par un utilisateur.
* Les règles ne sont pas appliquées rétroactivement : les anciens enregistrements ne sont pas affectés. La vérification des règles ne s’exécute que la prochaine fois qu’une personne tente de modifier ou de supprimer un enregistrement.
* Vous ne pouvez pas ajouter de règles métier aux types d’enregistrements globaux dans leurs espaces de travail principaux ou secondaires.
* Vous pouvez créer une condition pour votre règle métier qui fait référence à tous les types de champ, à l’exception des suivants :
  * Champs de formule
  * Champs de recherche
  * Champs de référence
* Les règles s’appliquent à toutes les personnes autorisées à modifier ou supprimer des enregistrements.
* Vous pouvez avoir plusieurs règles métier pour un type d’enregistrement.  <!--Syuzanna is checking this because it should be just ONE rule per action: one per edit and one per delete - see this: https://workfront.slack.com/archives/C0BHWEUSJCU/p1788281638322049?thread_ts=1787924876.280359&cid=C0BHWEUSJCU; I also logged a bug for this because it released with more than one per action - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/6a99add600001e9aa90435ec181dec3e/overview-->

  Toutes les règles sont vérifiées ensemble au même moment et le message d’erreur affiche tous les champs manquants dans une instruction.

## Configuration des règles métier

1. Accédez à une page de type d’enregistrement.
1. Depuis n’importe quel affichage, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Règles métier**.

   La page du tableau Règles métier s’ouvre.
1. Cliquez sur **Nouvelle règle métier**.
1. Dans la zone **Nouvelle règle métier**, ajoutez un nom pour la règle métier dans le premier champ disponible. Il s’agit d’un champ obligatoire.
1. (Facultatif) Ajoutez une description pour définir la règle métier, puis cliquez sur **Enregistrer**.

   Le formulaire de configuration des règles métier s’ouvre.

   ![Formulaire de configuration des règles métier](assets/business-rule-setup-form.png)

1. Dans la section **Si** du formulaire de configuration des règles métier, sélectionnez les actions que vous souhaitez restreindre ou autoriser en fonction d&#39;une règle spécifique. Choisissez parmi les options suivantes : <!--check UI text-->
   * **Modification de l&#39;enregistrement** : les utilisateurs seront autorisés à modifier ou non l&#39;enregistrement, si la condition définie dans cette règle est remplie.
   * **Suppression de l&#39;enregistrement** : les utilisateurs seront autorisés à supprimer ou non l&#39;enregistrement, si la condition définie dans cette règle est remplie.
     <!--add screen shot when UI text is final-->
1. Dans le champ **Formule**, ajoutez la règle métier. Choisissez un opérateur pour votre règle dans la section **Expressions de formule** du panneau de droite.

   Par exemple, vous pouvez choisir **IF** dans la section **Autres** champs, ou commencer à taper « IF », puis cliquer dessus lorsqu&#39;il s&#39;affiche dans la liste de suggestions.

   >[!TIP]
   >
   >Il est recommandé de sélectionner les champs et les opérateurs dans la liste de suggestions afin de conserver la syntaxe correcte de la règle.
1. Sélectionnez et le champ à rendre obligatoire pour permettre la modification ou la suppression des enregistrements de ce type d&#39;enregistrement.

   Par exemple, vous pouvez saisir l’instruction suivante pour que le champ **Résumé de la campagne** soit obligatoire :

   ```
      IF(ISBLANK({Campaign summary}),"Campaign summary is a required field. You cannot edit this record without a value for the Campaign summary field.")
   ```

   >[!IMPORTANT]
   >
   >Nous vous recommandons vivement d’inclure dans la formule de règle les informations suivantes afin de faciliter la compréhension des utilisateurs et des utilisatrices lorsqu’une action qu’ils ou elles tentent d’effectuer sur un enregistrement n’est pas autorisée :
   >
   >* Champs exacts pour lesquels la règle est configurée.
   >* Conséquence exacte en cas de non-respect de la règle.

   Le champ **Formule** contient des indicateurs lorsqu’un champ ou une expression est erroné.  <!--add screen shot?-->

   Dans la section **Alors** de la règle métier, vous pouvez voir une explication de la fonction de la règle.

1. Cliquez sur **Activer** pour rendre la règle active pour ce type d’enregistrement, puis sur **Enregistrer**.

   Les règles sont appliquées immédiatement après leur activation et tous les utilisateurs et utilisatrices autorisés à modifier ou supprimer des enregistrements dans le type d’enregistrement sélectionné doivent les suivre.
1. (Facultatif et recommandé) Cliquez sur la flèche vers l&#39;arrière à gauche de l&#39;en-tête de la page **Règles métier** pour afficher la page de type d&#39;enregistrement et accéder à une vue de tableau ou ouvrir la page d&#39;un enregistrement, puis essayez de modifier ou de supprimer un enregistrement afin de tester la règle que vous venez de créer.

## Gestion des règles métier

Vous pouvez modifier, supprimer ou désactiver des règles métier existantes.

La modification d’une règle existante ne modifie pas les enregistrements existants. La règle modifiée s&#39;applique uniquement aux enregistrements existants lorsqu&#39;une personne tente de les modifier ou de les supprimer.

1. Revenez à la page de table **Règles métier** pour le type d’enregistrement.
1. Recherchez la règle que vous souhaitez modifier.
1. Pointez sur le nom de la règle, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur l’une des options suivantes :

   * **Modifier** : ouvre la page de configuration des règles métier et vous pouvez modifier les informations relatives à la règle métier.
   * **Désactiver** : <!--check this in the UI: right now, it says Disable--> permet d’empêcher le déclenchement de la règle, mais en la préservant pour le futur, si nécessaire.
   * **Supprimer** : toutes les informations relatives à la règle sont supprimées. Les règles supprimées ne peuvent pas être récupérées.

   Les règles modifiées ou désactivées ne s’appliquent qu’aux enregistrements futurs et ne sont pas appliquées rétroactivement.

   <!--add NEW screen shot below if UI is fixed with Deactivate at release; it was fixed in devTest-->

   <!--![Business rule more menu expanded](assets/business-rule-more-menu-in-table-expanded.png)-->

<!--

***********FROM CLAUDE - BELOW - MUST EDIT*******************


### What business rules actually do

Business rules attach a condition to a **status change**. Instead of enforcing complete data the moment someone creates a record (which would slow everyone down), the rule only kicks in at one specific, deliberate moment: when a status is about to change to a status you've configured.

A rule looks like this in plain language:

> "Before a record can move to **Ready for Execution**, the field **Brand** must have a value."

If the field is empty, the status change is blocked and the person gets a clear message telling them what to fix. Once they fill it in and try again, the change goes through.

A few important things this is *not*:

* **It doesn't block record creation.** People can still create a new record instantly and fill it in over time, exactly like today. 
* **It doesn't auto-fill anything or auto-change statuses.** A person always has to make the status change themselves.
* **It doesn't retroactively flag old records.** Records that are already sitting in the target status aren't affected — the check only runs the next time someone tries to move a record *into* that status.

### Step 1: Open the business rules configuration area

Business rules live alongside your other admin setup — you won't need to hunt for a separate "Planning" panel. From your workflow setup area:

1. Go to the main **workflow setup / admin configuration** area for your workspace.
2. Look for the **business rules** section for the record type you want to configure (for example, "Materials" or "Campaigns").


### Step 2: Choose the record type

Rules are configured per record type, so pick the one you want to add a rule to. For example, if you want to make sure every Materials record has key fields filled in before execution, select **Materials**.

### Step 3: Create a new rule

For each rule, you'll specify three things:

| What you set | Example |
|---|---|
| **Record type** | Materials |
| **Target status** | Ready for Execution |
| **Required field** | Brand |

In other words: "When a Materials record's status is changed to **Ready for Execution**, the field **Brand** must have a value."

You can add more than one rule for the same status. For example, you might require Brand, Therapeutic Area, Indication, and Estimated Launch Date all to be filled in before a record can move to "Ready for Execution" — each is its own rule, and all of them are checked together.

**What fields can you require?**

* Connected record fields (e.g., a linked Brand or Indication record) — the rule passes as soon as at least one record is linked.
* Standard text fields (single-line or paragraph) — the rule passes once there's any value.
* Date fields — the rule passes once a date is set.

**What you can't use yet:** formula fields and lookup fields aren't supported as rule targets in this release, since they're calculated in the background rather than filled in directly by a person.

### Step 4: Write the message people will see

When you create a rule, you'll also provide the message that shows up if someone tries to make the change without the field filled in. Keep it specific and actionable — something like:

> "Brand is required."

You don't need to worry about formatting a whole error banner — the system handles combining messages if multiple rules are violated at once (see below).

### Step 5: Save the rule

Once saved, the rule takes effect **immediately** for everyone in the workspace — no need to log out, refresh, or wait for a deployment. The very next time anyone tries to move a record into that status, the rule is checked.

### What your team will actually experience

Here's what changes for the people using Planning day to day, once a rule is live.

#### If a required field is empty

1. A planner opens a record and changes the status to the gated status (say, "Ready for Execution").
2. The system checks all rules tied to that status.
3. If a required field is empty, the change is **rejected** — the status reverts back to what it was.
4. A toast message appears, naming exactly which field(s) are missing:
   > *"Status change blocked: 'Brand' and 'Estimated Launch Date' must be populated before moving to 'Ready for Execution.'"*
5. The planner fills in the missing field(s) and tries the status change again.
6. This time, the rule passes, and the status updates normally.

#### If everything is already filled in

Nothing changes. The status updates instantly, with no extra steps or popups. Business rules are invisible until they're actually needed.

#### If several fields are missing at once

All the violated rules are checked together, and the message lists every missing field in one go — planners don't have to fix one field, try again, get told about the next one, and repeat.

### Step 6: Edit or remove a rule later

Rules aren't set in stone. To make changes:

1. Go back to the business rules configuration area for the record type.
2. Find the rule you want to change.
3. Edit the required field, target status, or message — or delete the rule entirely.
4. Save. The change applies immediately to future status changes.

Keep in mind: editing or deleting a rule **only affects transitions going forward.** Records that already made it into the target status before the change aren't reevaluated.
3## A few things worth knowing

* **This is separate from locking records after a status change.** Business rules (as described here) only check field completeness *before* a status change goes through. A different, related feature governs whether a record becomes fully locked from edits/deletion once it reaches a certain status — that's not what's covered here.
* **Bulk status changes** (changing status on many records at once) aren't fully defined yet for how they interact with business rules — if your team relies heavily on bulk actions, check with your Adobe contact on current behavior.
* **If a rule can't be evaluated** due to a system error, the transition is blocked rather than silently allowed through — you'll never end up with an incomplete record slipping past a rule because of a backend hiccup.
* **Turning the feature off** doesn't delete your configured rules — they're just paused. Turning it back on restores them exactly as they were, no reconfiguration needed.

### Quick reference: setting up your first rule

1. Confirm the feature is enabled for your tenant.
2. Go to workflow setup → business rules for your record type.
3. Choose the record type (e.g., Materials).
4. Create a rule: target status + required field.
5. Write a clear, specific error message.
6. Save — it's live immediately.
7. Repeat for each field you want to require.
8. Test it yourself: try changing a record's status with the field empty, confirm you see the expected message, fill in the field, and confirm the status change now goes through.

That's it — from here on, anyone converting a record forward will get a clear nudge if something's missing, instead of a downstream project quietly showing up incomplete.

-->