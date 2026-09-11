---
title: Créer des enregistrements Planning à partir de résumés d'espace d'idéation
description: Grâce à l'Espace d'idéation, une nouvelle fonctionnalité d'Adobe Workfront Planning, vous pouvez transformer des résumés en enregistrements Planning. Les briefs exportés créent de nouveaux enregistrements ou mettent à jour des enregistrements existants. Cet article décrit comment créer ou modifier des enregistrements Planning existants à l'aide de l'espace Idéation.
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 4%

---


# Créer des enregistrements Planning à partir de résumés d&#39;espace d&#39;idées

<!--
Will this release JUST to preview? If not - hide the preview portion below
-->

<!--
I started with this under Records first but what if Ideation will be added to other products and it will generate record types in those products? keep it here so it can be moved, if needed, to a standalone product one day?
-->

<!--
*********************** IMPORTANT ***************
THIS ARTICLE HAS 2 DRAFTS IN 2 SEPARATE AREAS FROM CLAUDE - THEY WERE CREATED AT DIFFERENT TIMES - WHICH ONE WOULD YOU KEEP OR MERGE THEM INTO ONE ARTICLE
-->

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Il est disponible uniquement dans le cadre du programme **Ideation space Beta**. </span>

<span class="preview">Pour plus d’informations, voir [Prise en main de l’espace d’idéation pour Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Grâce à l&#39;Espace d&#39;idéation, une nouvelle fonctionnalité d&#39;Adobe Workfront Planning, vous pouvez transformer des résumés en enregistrements Planning. Les briefs exportés créent de nouveaux enregistrements ou mettent à jour des enregistrements existants.

Cet article décrit comment créer ou modifier des enregistrements Planning existants à l&#39;aide de l&#39;espace Idéation.

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

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
   </td>

<tr> 
   <td role="rowheader"><p>Produits supplémentaires</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence de workflow Adobe</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> 
   <ul>
   <li><p>Vous devez ajouter un workflow et un type de licence Planning au niveau d'accès lorsque vous disposez à la fois d'un workflow et d'un package Planning</p>   </li>
   <li><p>Le paramètre Désactiver l’espace d’idéation de votre niveau d’accès doit être désélectionné</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Autorisations de niveau Contributeur ou supérieur à l’espace de travail et au type d’enregistrement dans lesquels vous souhaitez ajouter des enregistrements </p>
      <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>
      <p>Afficher les autorisations d’accès aux objets Workfront pour les ajouter aux résumés <!--not sure if this is available--></p>
      <p>Autorisations d’éditeur dans l’espace Idéation pour créer des résumés</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Rôles utilisateur Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Tout rôle d’utilisateur GenStudio pour accéder aux campagnes, aux produits et aux rôles</li>
   <li>GenStudio System Manager pour accéder aux activations <!--and Events--></li></ul>
   Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> Rôles utilisateur et autorisations </a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Considérations relatives à l’utilisation de l’Espace d’idéation pour créer des enregistrements

* Vous pouvez uniquement lancer l’espace d’idéation à partir de Workfront Planning au fur et à mesure que vous créez ou modifiez des enregistrements. L’espace Idéation n’existe pas en dehors de Workfront Planning.
* Pour accéder à l’espace Idéation , vous devez disposer d’un espace de travail et d’un type d’enregistrement dans Workfront Planning.
* Les nouveaux enregistrements commencent toujours par le contenu de l’espace réservé, quelle que soit la manière dont vous les créez.
* Lorsque vous supprimez un enregistrement Planning lié à un brief d&#39;idéation, le brief reste dans l&#39;espace Idéation et la zone de travail associée dans l&#39;espace Idéation n&#39;est pas supprimée.
* La synchronisation des informations se produit uniquement de l’espace Idéation vers Workfront Planning. Il n’existe aucune synchronisation inversée ou automatique d’un enregistrement Planning vers le résumé de l’espace d’idéation.
* Les scénarios suivants existent lorsque des champs sont créés, modifiés ou supprimés dans Workfront Planning :

  * De nouveaux champs créés sur les enregistrements liés aux résumés d&#39;idéation sont ajoutés quotidiennement au résumé. Les nouveaux champs apparaissent vides dans le brief de l’idéation.
  * Les champs supprimés restent dans le brief et conservent leurs valeurs antérieures.
  * Les champs renommés mettent à jour leur nom dans le brief.
* Vous pouvez ajouter des documents sous forme de cartes dans l’espace Idéation . Cela inclut également les images.

  Les types de fichiers pris en charge sont les suivants : PDF, Excel, CSV, PNG (et autres formats d’image), Word, PowerPoint. Vidéos non prises en charge.

  Tous les documents chargés sont convertis en PDF sur le serveur principal pour traitement.
* Vous pouvez glisser-déposer des enregistrements directement depuis Workfront Planning dans l&#39;espace et ils s&#39;affichent de la même manière que les fichiers chargés manuellement.

## Créer des enregistrements à l’aide de l’espace d’idéation

1. Dans la page de destination Workfront Planning, cliquez sur la vignette d’un espace de travail que vous pouvez gérer.
1. Cliquez sur la carte d’un type d’enregistrement auquel vous pouvez ajouter des enregistrements.
1. Effectuez l’une des opérations suivantes pour créer un enregistrement :

   * Dans n’importe quel affichage de la page de type d’enregistrement, cliquez sur **Nouvel enregistrement** dans le coin supérieur droit de la page et dans la zone **Choisir une manière d’ajouter vos enregistrements**, cliquez sur **Ouvrir l’espace d’idéation**, puis cliquez sur **Continuer**.
   * Faites défiler jusqu’au bas du tableau des enregistrements et cliquez sur **Nouvelle ligne**, puis sur **Ouvrir l’espace d’idéation**.

     >[!TIP]
     >
     >Sélectionner **Ne pas afficher** ferme définitivement la future invite. Cliquez sur l’icône Fermer **X** pour fermer cette zone, mais elle réapparaîtra la prochaine fois que vous ajouterez un enregistrement intégré.

   ![Nouvelle boîte d’enregistrement avec le bouton Ouvrir l’espace d’idéation](assets/new-record-creation-picker-with-ideation.png)

   L’espace Idéation s’ouvre dans un nouvel onglet avec une invite vide.

   L’enregistrement est immédiatement créé avec le texte d’espace réservé.

1. (Facultatif) Cliquez sur **Utiliser un brief existant** dans la zone d&#39;invite pour parcourir et ajouter un document existant que l&#39;espace Idéation utilisera pour créer le brief et l&#39;enregistrement futur.

   ![Invite vide du résumé de l’idéation](assets/empty-ideation-prompt.png)

1. (Facultatif) Cliquez sur l’icône **Ouvrir les zones de travail précédentes** <!--accurate??--> ![Ouvrir les mémoires existantes](assets/open-existing-briefs-icon.png) dans le coin supérieur droit de la zone d’invite, pour ouvrir les mémoires existantes

1. Dans le **Sur quoi travaillez-vous ?** , décrivez le type d’enregistrement que vous souhaitez créer.

   Plus vous partagez de détails, plus les informations fournies par l&#39;espace d&#39;idéation seront utiles. Par exemple, tapez une description de la campagne que vous prévoyez : « Campagne de rentrée des classes pour une agence marketing ».

1. Cliquez sur **Commencer à idéaliser**.

   L’espace Idéation suit les étapes suivantes pendant la création de votre idée : <!--check some of these in the UI - there might have been UI text changes-->

   1. Comprendre votre objectif et le contexte
   2. Examinez votre espace et les matériaux sélectionnés
   3. Collecter des preuves à partir de documents, de sites web et de données
   4. Synthétiser les résultats dans un résumé de la recherche
   5. Créer et affiner des cartes avec des citations

   Au cours de ce processus, vous verrez l&#39;espace d&#39;idéation rechercher activement des données Workfront Planning connectées ou des informations disponibles sur le web.

   Par exemple, elle peut rechercher des programmes, des produits, des personnages ou des régions existants, ainsi que des concepts similaires disponibles en ligne. <!--check on this with Et-->

   Une fois l’idéation terminée, les éléments suivants sont ajoutés à l’espace d’idéation :

   * Un résumé des résultats de l’IA lié à plusieurs cartes avec des informations détaillées sur les éléments à prendre en compte. Les cartes de détails s’affichent dans une nouvelle section. Un connecteur indique quelle section de carte appartient à quel résumé.

   * Fichier **Brief** dans le coin inférieur gauche de l&#39;espace d&#39;idéation. Le brief est un brouillon du futur enregistrement et s’affiche dans la page Détails d’un enregistrement.

   ![Carte d’idéation avec branches](assets/ideation-card-with-branched-off-additional-cards.png)

1. Continuez à ajouter des informations à l’espace d’idéation pour terminer la création de votre brief.

1. (Conditionnel) Une fois le brief terminé, cliquez sur l’image d’aperçu dans le coin inférieur gauche, puis sur l’une des options suivantes :

   * **Exporter dans un fichier** pour créer un fichier
   * **Exporter vers Workfront Planning** pour créer un enregistrement Planning

   Pour plus d&#39;informations sur l&#39;ajout d&#39;éléments au brief et son exportation, voir [Créer des brief dans l&#39;espace Idéation](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md).

   Cela termine la création de l’enregistrement avec les informations supplémentaires et l’ajoute au type d’enregistrement que vous avez sélectionné à l’origine.

## Modifier les enregistrements existants dans l’espace de destination

Vous pouvez ouvrir l’Espace d’idéation à partir d’enregistrements existants pour les mettre à jour.

Vous ne pouvez pas modifier en masse les enregistrements dans l’espace Idéation .

1. Accédez à un enregistrement existant dans Workfront Planning et ouvrez sa page de détails.

1. Cliquez sur **Ouvrir dans l’espace Idéation**. L’espace Idéation s’ouvre alors dans un nouvel onglet.

   Si une idéation pour l’enregistrement existe déjà, cela ouvre cet espace.

   S&#39;il n&#39;y a pas d&#39;idéation, cela crée un espace d&#39;idéation et un brief.

   >[!TIP]
   >
   >La modification en masse d’enregistrements à l’aide de l’espace de positionnement n’est pas disponible.

   <!-- 
    I don't think these steps are still valid but the environment was not available to test: 
    - If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
    - If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.
    -->

1. Poursuivez la modification du brief comme décrit dans la section [Création d’enregistrements à l’aide de l’espace d’idéation](#create-records-using-the-ideation-space) de cet article.






<!-- this is from Claude, but rephrased and included most of this above: 

## Step 5: Open the Workfront Planning Records panel

To bring real Workfront Planning records into your canvas (rather than just AI-generated ideas), click the **records icon** in the left-hand toolbar (third icon down). This opens the **Workfront Planning Records** panel, listing all **Connected Record types** available in your Planning environment — for example:

- Products
- Regions
- Personas
- Channels
- Activations
- Project
- Test Record
- Experience Manager Assets

## Step 6: Drag real records onto the canvas

Search or browse within a record type (e.g., **Products** or **Personas**), then drag the record you want directly onto the canvas. In the example, an existing **Nike product** record and a **Deep testing** persona record were both dragged in and positioned near the relevant concept cards.

This lets you visually connect your AI-generated ideas to the actual records that already exist in Workfront Planning, grounding the ideation in real data rather than hypothetical entities.


![Dragging a persona record onto the canvas](images/05_drag_persona_record.png)

---

## Step 7: Refine with follow-up prompts

Use the **Ask anything** box in the bottom-right corner at any time to refine the canvas — for example, typing `regenerate` against a specific card to have Catalyze redo that section using updated context. Catalyze will re-run its reasoning steps (searching, synthesizing, citing) and update the affected cards in place.

---

## Step 8: Review the full canvas

Zoom out to see the complete picture: your original campaign goal, all AI-generated concept cards with citations, the real Workfront Planning records you've pulled in (Products, Personas, etc.), and a **Campaign Brief** summary card in the corner pulling it all together.



![Full canvas overview](images/06_full_canvas_overview.png)

---

## Tips

- **Be specific in Step 2** — richer campaign descriptions produce more relevant, better-grounded cards.
- **Check citations** before trusting a generated fact — click **Sources** on any card.
- **Mix AI cards with real records** — dragging in actual Products, Personas, Regions, etc. keeps the canvas tied to your real Planning data, not just AI speculation.
- Responses are AI-generated and may be inaccurate — always verify against the linked sources before finalizing a record.

***************SECOND DRAFT FROM CLAUDE*******************
# Creating and Managing Records with Catalyze Ideation

> This workflow reflects the Closed Beta experience and is expected to evolve before Open Beta and GA. Confirm current behavior before publishing to customers.

This guide explains how to create and ideate on records using Catalyze within Workfront Planning. It covers all entry points, system behavior, data sync rules, and file-upload support.

## Before you start

- You must have access to a record list within Workfront Planning.
- Catalyze always opens in a **new browser tab** — this is consistent across every entry point.
- Any record created through Catalyze starts with **placeholder text** until you begin ideating.

## Option 1: Create a record via the top-level "New Record" button

1. Navigate to your record list in Workfront Planning.
2. Click the **New Record** button at the top of the page.
3. From the dropdown menu, select **Ideate in Catalyze**.
4. A new browser tab opens automatically, launching the Catalyze canvas.
5. A new record is created in Workfront Planning with placeholder text.
6. Begin ideation directly in Catalyze.

**Additional access from the record view:** Open the newly created record and, in its detail modal, click **Ideate in Catalyze**. This opens Catalyze in a new tab (same behavior as above).

## Option 2: Create a record via inline record creation (bottom of table)

1. Scroll to the bottom of the record table.
2. Click **New Record**.
3. The record is created immediately with placeholder text.
4. A pop-up appears with these options:
   - **Open Catalyze** — launches Catalyze in a new browser tab
   - **Don't Show Again** — permanently dismisses the future prompt
   - **X (Close)** — closes the pop-up; it will reappear next time
5. Click **Open Catalyze** to begin ideation.

## Working with existing records

**Contextual actions (bottom selection bar)**
- **Single record selected:** an "Ideate in Canvas" / "Open in Canvas" action appears.
  - If a canvas already exists, it opens that canvas.
  - If no canvas exists, it creates a new one.
- **Multiple records selected:** the Ideate/Open in Canvas action is **not available** — bulk ideation is not supported.

**Record detail panel**
- If no canvas is connected, an **Ideate in Catalyze** button appears in the record header.
- If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
- If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.

**When can you create a canvas for a record?**
A canvas can be created for a record that is in Workfront Planning and still in **draft** state (not yet marked "ready").

## Record deletion behavior

If a Planning record linked to a Catalyze canvas is deleted:
- The canvas remains intact in Catalyze.
- No data is removed from Catalyze.

## Data synchronization rules

**Sync direction:** One-way only, from Catalyze → Workfront Planning. There is no reverse or automatic sync from Planning back to Catalyze.

**Export process:**
1. In Catalyze, click **Export to Planning**.
2. Data is pushed to the connected Workfront Planning record.
3. The export **overwrites all existing field data** in the record.

**Important notes:**
- Changes made directly in Workfront Planning do **not** sync back to Catalyze.
- Data refresh in Workfront Planning is manual only (Beta behavior) — there is no scheduled/automatic sync.
- Schema updates do sync one direction: once connected, Planning schema changes propagate to Catalyze daily — added fields appear empty, removed fields keep their prior values, and renamed fields update in place.

## Uploading documents into the Catalyze canvas

- Files can be added as a "document card" on the canvas — this works the same whether the file is an image or another document type.
- You can drag and drop files directly from Workfront Planning onto the canvas, and they appear the same way as manually uploaded files.
- All uploaded documents are converted to PDF on the backend for processing.
- Supported file types (as of the Aug 2026 beta): **PDF, Excel, CSV, PNG (and likely other image formats), Word, PowerPoint.**
- **Not supported:** video files.
- You can include images directly in a prompt and Catalyze will recognize their content, though small-format legibility is still being refined.

## Key takeaways

- Use **Ideate in Catalyze** to connect records to the AI-assisted ideation workflow.
- Catalyze always launches in a separate browser tab.
- New records always start with placeholder content, regardless of entry point.
- Data flow between Catalyze and Planning is manual and one-directional (Catalyze → Planning).
- Deleting a Planning record does not delete its associated Catalyze canvas.

-->


<!--
Internal info: 

## The Ideation space and Adobe GenStudio

Adobe GenStudio for Performance Marketing is Adobe's end-to-end content supply chain solution, spanning five stages:

1. Strategy and Ideation
2. Workflow and Planning
3. Asset Management
4. Creation and Production
5. Delivery and Activation

The Ideation space fits in the **Strategy and Ideation** stage — the front door of the content supply chain — and is designed to work natively with the rest of GenStudio, so the briefs and strategic direction it generates flow directly into Workfront Planning for execution.
-->


