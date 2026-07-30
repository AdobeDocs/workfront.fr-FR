---
name: release-notes-formatter
description: Formatez et validez les notes de mise à jour de Workfront pour garantir la cohérence, la structure correcte et des liens appropriés. À utiliser uniquement pour les fichiers de notes de mise à jour dans les répertoires de versions de produits ou lorsque l’utilisateur mentionne des notes de mise à jour, des versions de produit ou des versions trimestrielles. Ne s’applique pas aux articles de procédure ni à la documentation générale.
source-git-commit: fa39320af72acf6d2ceaf201480baf78a07ae76e
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 3%

---


# Formateur de notes de mise à jour

Formater et valider les notes de mise à jour d’Adobe Workfront dans le répertoire `help/quicksilver/product-announcements/product-releases/`.

## Types de page

Identifiez le type de page à partir du chemin d’accès au fichier et du contenu :

| Type de page | Modèle de fichier | Modèle |
|-----------|-------------|----------|
| **Vue d’ensemble** | `{YY}-q{N}-release-overview.md` | Voir .#overview-page-template |
| **Zone du produit** | `{YY}-q{N}-{area}.md` | Voir .#product-area-page-template |
| **Planification** | `planning-release-activity-{YY}-q{N}.md` | Similaire à la zone de produit |
| **Apparence** | `look-and-feel-updates-{YY}-q{N}.md` | Voir .#look-and-feel-page-template |

## Étape 0 : déterminer le trimestre (faire ceci avant toute autre chose)

>[!IMPORTANT]
>
>N&#39;affectez jamais une fonction à un document-trimestre à l&#39;aide des mathématiques de trimestre calendaire à sa date d&#39;aperçu ou de production. Doc-quarter est basé sur la **version mensuelle** la fonctionnalité est livrée, par regroupement interne release-calendar de Workfront, qui est décalé par rapport au trimestre calendaire (voir le tableau [Calendrier des versions 2026](#2026-release-calendar) près de la fin de ce fichier). Par exemple, une fonctionnalité dont la date de production est le 13 août 2026 appartient au trimestre doc `26-q4`, et non au trimestre `26-q3`, car la version mensuelle d’août est mappée à `26-q4`.
>
>Le tableau « Mappage des trimestres » plus bas (Formulaire écrit / Mois) sert à écrire les noms des trimestres dans les titres (par exemple, « Troisième trimestre » pour le T3) — il n&#39;est **pas** suffisant à lui seul pour décider dans quels fichiers de trimestre une fonctionnalité appartient. Effectuez toujours une vérification croisée par rapport au tableau Calendrier des versions avant de créer ou de modifier un fichier.
>
>Si la date de production d’une fonctionnalité n’apparaît pas dans le tableau Calendrier des versions (par exemple, elle se situe au-delà de la période du tableau), demandez à l’utilisateur de mettre à jour le calendrier plutôt que de faire des suppositions.

## Workflow de formatage

### Étape 1 : valider FrontMATTER

Champs obligatoires pour toutes les pages de notes de mise à jour :

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

Règles :
- `feature` doit être exactement `Product Announcements`
- `recommendations` doit être exactement `noDisplay, noCatalog`
- N’inventez jamais une `exl-id`, incluez-la uniquement si elle existe déjà
- Ne pas ajouter de `draft: Probably` sur les pages réelles (modèles uniquement)

### Étape 2 : valider la structure par type de page

#### Pages de la zone de produit

1. **H1** : `{Written Quarter} {Area} enhancements`
   - Exemple : `# Second Quarter 2026 Administrator enhancements`
   - Le trimestre doit être écrit : « Premier trimestre », « Deuxième trimestre », « Troisième trimestre », « Quatrième trimestre »

2. **Paragraphe d’introduction** : décrit la zone et les liens vers la présentation.
   - Doit être lié au fichier de vue d’ensemble **trimestre correct**
   - Bogue courant : liaison au trimestre précédent (par exemple, `26-q1` au lieu de `26-q2`)

3. **H2 par fonctionnalité** : titre de la fonctionnalité comme en-tête
   - **Fonctionnalités les plus récentes en premier** — la note de mise à jour la plus récente doit apparaître comme le premier H2 après le paragraphe d&#39;introduction
   - Les anciennes fonctionnalités suivent dans l’ordre chronologique inverse

4. **Bloc de légende de date** après chaque point H2 :

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

5. **Corps** : description des fonctionnalités, puis lien vers la documentation d’aide.

#### Pages de présentation

1. **H1** : `{Written Quarter} release overview`

2. **Paragraphe d’introduction** avec le mois de publication prévu

3. **`>[!IMPORTANT]`bloc** avec le tableau de calendrier des versions

4. `Adobe Workfront enhancements`**** H2 avec liste à puces des liens d’ancrage :

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

5. **H3 par zone de produit** avec le tableau des fonctionnalités HTML (voir .claude/commands/_release-notes-formatter-reference.md#overview-feature-table)
   - Dans chaque tableau, **les fonctionnalités les plus récentes en premier** — la ligne la plus récente apparaît en haut du tableau (après la ligne d’en-tête)

6. **Sections de fin** (H2) : notes de mise à jour pour d’autres zones, mises à jour des visionneuses de vérification pour bureau, annonces, version de l’API, mises à jour de maintenance, mises à jour de formation

### Étape 3 : valider les liens

- **Lien d’aperçu dans les pages de la zone produit** : doit pointer vers le même trimestre
  - Correct : `26-q2-release-activity/26-q2-release-overview.md`
  - Erreur : `26-q1-release-activity/26-q1-release-overview.md`
- **Liens d’ancrage dans la vue d’ensemble** : doivent correspondre aux identifiants H3 (minuscules, tirets).
- **Liens des fonctionnalités dans les tableaux de présentation** : vous devez utiliser `class="MCXref xref" xrefformat="{para}"`
- **Liens vers les documents d’aide** : doit commencer par `/help/quicksilver/`

### Étape 4 : valider les dates

- Format : `{Month} {Day}, {Year}` (par exemple, « 12 mars 2026 »)
- Utiliser des `TBD` pour les dates inconnues
- Les dates du bloc de `>[!NOTE]` de la page de la zone produit doivent correspondre à la ligne correspondante du tableau d’aperçu
- Les dates de prévisualisation doivent précéder les dates de production.

### Étape 5 : correctifs courants

Appliquez ces correctifs lors du formatage :

| Problème | Corriger |
|-------|-----|
| Mauvais trimestre du lien d’aperçu | Mettre à jour pour correspondre au propre trimestre du fichier |
| Bloc de date de `>[!NOTE]` manquant | Ajouter un bloc après l’en-tête de fonctionnalité H2 |
| Format de date incohérent | Normaliser pour `Month Day, Year` |
| Ligne vide manquante avant `>[!NOTE]` | Ajouter une ligne vide |
| Espaces supplémentaires dans les lignes de légende | Rogner l’espace de fin |
| HTML dans les pages de zone de produit | Conserver en tant que markdown (HTML est réservé aux tableaux de présentation uniquement) |
| `exl-id` manquant | Ne le faites pas — n&#39;en générez pas |

### Étape 6 : mettre à jour la table des matières

Chaque fois que vous créez une **nouvelle** page de notes de mise à jour (présentation ou zone produit), ajoutez-la à `help/quicksilver/TOC.md` dans la même modification. Une page qui ne figure pas dans la table des matières n’apparaît pas dans la navigation publiée, même si des liens dans le tableau d’aperçu pointent vers elle.

Où l’ajouter :

- La table des matières comporte une section par trimestre sous un en-tête tel que `* 2026 Q3 Release {#release-26-q3}`. Si l’en-tête du trimestre n’existe pas encore (première page d’un nouveau trimestre), ajoutez-le au-dessus du trimestre précédent afin que le dernier trimestre se trouve en haut.
- Sous cet en-tête de trimestre, répertoriez les pages dans cet ordre :
  1. **Présentation** en premier (`Third Quarter 2026 release overview`).
  2. **Pages de zone de produit** classées par ordre alphabétique par nom de zone (administrateur, documents, opérations d’entreprise, projets, compte rendu des performances, demande).
  3. **Autres améliorations** la dernière (toujours après les zones de produit alphabétiques).

Chaque entrée de la table des matières est un lien Markdown utilisant le titre de la page et le chemin d’accès absolu au référentiel :

```markdown
      * [Third Quarter 2026 Documents enhancements](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-documents.md)
```

Associez la mise en retrait (six espaces) aux entrées environnantes. Utilisez la page H1 mot à mot comme texte du lien, par exemple `Documents enhancements`, `Requesting enhancements` (pas `Requests`), de sorte que les libellés de la table des matières correspondent aux trimestres précédents.

Erreurs courantes à éviter :

- Création d’une page de zone produit sans l’ajouter à la table des matières.
- Création d’un lien vers la présentation d’un autre trimestre à partir de la nouvelle page produit (étape 3).
- Insérer les pages d&#39;un nouveau trimestre sous l&#39;en-tête du trimestre précédent.

### Étape 7 : mettre à jour la page d’accueil

Chaque fois que vous créez une **page d’aperçu du nouveau trimestre** (c’est-à-dire qu’il s’agit de la première page d’un nouveau trimestre, et pas seulement d’une nouvelle page de zone produit ajoutée à un trimestre existant), mettez à jour les `help/quicksilver/home.md` dans la même modification :

- Dans la section `>[!TAB Latest release]` , remplacez le lien de présentation de la version par le lien de présentation du nouveau trimestre.
- Toujours dans cette section, mettez à jour le lien de l’activité de publication Adobe Workfront Planning afin qu’il pointe vers le fichier de planification du nouveau trimestre (`planning-release-activity-{YY}-q{N}.md`), le cas échéant.
- Dans l’onglet `>[!TAB {YYYY} releases]` de l’année en cours, ajoutez le lien de présentation du nouveau trimestre en haut de la liste, au-dessus de l’entrée du trimestre précédent.

Ne `home.md` touchez pas lorsque vous ajoutez uniquement une page de zone produit à un trimestre qui contient déjà une page d’aperçu.

Erreurs courantes à éviter :

- Création d&#39;une page d&#39;aperçu d&#39;un nouveau trimestre sans mise à jour de l&#39;onglet « Dernière version » de `home.md` (il continuera à pointer vers l&#39;ancien trimestre).
- Oubliez également d’ajouter le nouveau trimestre à la liste d’onglets de l’année en cours.

## Conventions de dénomination des fichiers

| Type | Motif | Exemple |
|------|---------|---------|
| Vue d’ensemble | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| Zone du produit | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| Répertoire | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

Limaces de zone standard : `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## Mappage du trimestre

>[!NOTE]
>
>Ce tableau permet d&#39;écrire les noms de trimestre (par exemple, dans un H1 ou un titre). Il ne détermine PAS les fichiers du trimestre auxquels appartient une fonctionnalité : utilisez pour cela le tableau [Calendrier des versions 2026](#2026-release-calendar) ci-dessous, car doc-quarter est décalé par rapport au trimestre calendaire.

| Trimestre | Formulaire Écrit | Mois |
|---------|-------------|--------|
| T1 | Premier Trimestre | Jan-Mar |
| T2 | Deuxième Trimestre | Avr-Juin |
| T3 | Troisième trimestre | Juillet-Septembre |
| T4 | Quatrième trimestre | Oct-Déc |

**Important — trimestre de document utilisé dans les noms de fichier (`26-q3`, `26-q4`, etc.) est décalé d’un mois par rapport à ce mappage de calendrier.** Elle suit plutôt le regroupement calendrier de publication interne de Workfront, où chaque trimestre de document = les deux versions mensuelles précédentes + le mois de publication trimestriel. Par exemple, le trimestre doc `26-q3` couvre les versions mensuelles de mai/juin/juillet 2026 (`2026.07` de mise à jour trimestrielle) et le trimestre doc `26-q4` couvre les versions mensuelles d’août/septembre/octobre 2026 (`2026.10` de mise à jour trimestrielle). Vérifiez toujours le calendrier des versions ci-dessous (ou demandez-en un mis à jour) avant de supposer que le trimestre d’un fichier est basé sur le tableau calendrier-trimestre ci-dessus.

## Calendrier Des Versions 2026

Source : « Calendrier de publication mensuel 2026 » (wiki Adobe corp, espace AWF — `wiki.corp.adobe.com`, clé d’espace AWF, titre « Calendrier de publication mensuel 2026 »). WebFetch ne peut pas atteindre cette page (nécessite l’authentification unique Adobe) ; demandez à l’utilisateur de coller un PDF/tableau mis à jour lorsque des dates sont nécessaires au-delà de ce qui est capturé ici.

| Mois de publication | Aperçu final | Production | Version mensuelle | Publication Trimestrielle | Trimestre doc |
|---|---|---|---|---|---|
| Novembre 2025 | 30 Octobre 2025 | 13 Novembre 2025 | 2025.11 | 2026.01 | 26-t1 |
| Déc 2025 | 27 Novembre 2025 | 11-Déc-2025 | 2025.12 | 2026.01 | 26-t1 |
| Janvier 2026 | 23 Déc. 2025 | 15 Janvier 2026 | 2026.01 | 2026.01 | 26-t1 |
| Février 2026 | 29 Janvier 2026 | 12 Février 2026 | 2026.02 | 2026.04 | 26-t2 |
| Mars 2026 | 26 Février 2026 | 12 Mars 2026 | 2026.03 | 2026.04 | 26-t2 |
| Avril 2026 | 2 Avril 2026 | 16-Avr-2026 | 2026.04 | 2026.04 | 26-t2 |
| Mai 2026 | 30-Avr-2026 | 14 Mai 2026 | 2026.05 | 2026.07 | 26-t3 |
| Juin 2026 | 28 Mai 2026 | 11 Juin 2026 | 2026.06 | 2026.07 | 26-t3 |
| Juillet 2026 | 7 Juillet 2026 | 16 Juillet 2026 | 2026.07 | 2026.07 | 26-t3 |
| Août 2026 | 30 Juillet 2026 | 13-Août-2026 | 2026.08 | 2026.10 | 26-t4 |
| Sep 2026 | 3 Septembre 2026 | 17 Septembre 2026 | 2026.09 | 2026.10 | 26-t4 |
| Oct 2026 | 01-Oct-2026 | 15-Oct-2026 | 2026.10 | 2026.10 | 26-t4 |
| Novembre 2026 | 29 Octobre 2026 | 12 Novembre 2026 | 2026.11 | 2027.01 | 27-t1 |
| Déc 2026 | 26 Novembre 2026 | 10-Déc-2026 | 2026.12 | 2027.01 | 27-t1 |
| Janvier 2027 | 5 Janvier 2027 | 14-Jan-2027 | 2027.01 | 2027.01 | 27-t1 |

Remarques sur l&#39;utilisation de ce tableau :

- **Aperçu final** est la dernière date à laquelle les fonctionnalités peuvent apparaître dans l’aperçu de cette version mensuelle. Utilisez-la pour la puce « dernière date à laquelle les fonctionnalités peuvent apparaître dans l’environnement d’aperçu » de la page d’aperçu (mois de fin de trimestre uniquement).
- **Production** est la date de production officielle pour tous de cette version mensuelle.
- Pour le mois de fin de trimestre (celui correspondant à la colonne Version trimestrielle), le tableau du planning de la page Aperçu répertorie la version de ce mois **deux fois** : une fois dans la colonne « Version mensuelle » datée du **un jour avant** la date de production (date de version rapide), et une fois dans la colonne « Version trimestrielle » datée de la date de production réelle. Les mois non finaux d’un trimestre utilisent la même date de production dans la liste mensuelle et dans toutes les références de « version rapide ». Aucun ajustement n’est nécessaire.
- Ce tableau ne date que de janvier 2027. Si des dates ultérieures sont nécessaires, demandez à l’utilisateur ou à l’utilisatrice un calendrier mis à jour plutôt que de faire des suppositions.

La mise à jour trimestrielle de la production arrive généralement le jeudi de la deuxième semaine complète du dernier mois du trimestre.

## Liste de contrôle de validation

Lors de l’examen d’un fichier de notes de mise à jour, vérifiez les points suivants :

- [ ] FrontMATTER contient tous les champs obligatoires avec des valeurs correctes
- [ ] H1 correspond au format du type de page
- [ ] lien Aperçu pointe vers le trimestre correct
- [ ] Chaque fonctionnalité comporte un bloc de date `>[!NOTE]` (pages de zone de produit)
- [ ] format de date est cohérent (`Month Day, Year`)
- [ ] lignes du tableau des fonctionnalités de l’aperçu correspondent au contenu de la page de la zone produit
- [ ] Aucun lien interne rompu
- [ ] liens d’ancrage dans la vue d’ensemble correspondent aux ID de section H3
- [ Les fonctionnalités ] sont classées en commençant par la plus récente (pages de zone de produit et tableaux de présentation)
- [ ] Les nouvelles pages de notes de mise à jour sont répertoriées dans `help/quicksilver/TOC.md` sous le trimestre approprié, avec la présentation en premier et les zones de produits dans l’ordre alphabétique (Autre dernière)
- [ ] Si une nouvelle page d’aperçu du trimestre a été créée, `help/quicksilver/home.md`’onglet « Dernière version » et l’onglet de l’année en cours y pointent

## Ressources supplémentaires

- Pour obtenir des modèles et des exemples HTML complets, voir .claude/commands/_release-notes-formatter-reference.md
