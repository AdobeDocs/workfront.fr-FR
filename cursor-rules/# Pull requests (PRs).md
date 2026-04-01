---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# Requêtes d’extraction (PR)

Lorsque vous rédigez ou révisez le titre ou la description d’une demande d’extraction (par exemple, dans GitHub/GitLab ou lorsque vous y êtes invité dans la conversation de l’agent), suivez ces conventions.

## Dérivation du problème Jira

- **Source de vérité :** dérivez l’ID de problème Jira du **nom de branche Git actuel** (par exemple un segment correspondant au modèle de clé de votre projet, tel que `FFENT-8796`).
- **Si le nom de la branche comprend un ID Jira :** utilisez cet ID dans le titre PR (voir ci-dessous) et liez-le dans `# Context` `## Jira` →.
- **Si le nom de la branche ne comprend pas d’ID Jira** traitez la requête de tirage comme n’étant pas associée à un ticket. **Omettez** la clé Jira du titre PR (n’inventez pas de ticket). Incluez toujours `# Context` → `## Jira`, avec le contenu exact : `No ticket` (aucun lien).

## Titre du PR

**Lorsque le nom de la branche comprend un identifiant de problème Jira**, incluez **les deux** :

1. L’**ID de problème Jira** (par exemple, `FFENT-8001`).
2. Le **type de validation** (voir la liste ci-dessous), utilisant ce modèle :

`{type}/{JIRA-ID}- {short task description}`

Exemple :

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

Utilisez une description concise de style impératif après l’ID. Respectez le modèle d’espacement affiché : type, barre oblique, clé Jira avec trait d’union à la fin, espace, puis la description.

**Lorsque le nom de la branche ne comprend pas d’ID de problème Jira**, omettez le ticket dans le titre et utilisez :

`{type}- {short task description}`

Exemple :

`docs- Refresh Object Composite API changelog`

### Types de validation acceptables (utilisez exactement ces libellés avant `/`)

- **feat** — ajoute une nouvelle fonctionnalité. Lorsqu’un nouvel élément de la table des matières est ajouté ou que le JIRA est connecté à un autre Jira étiqueté `feat`.
- **fix** — corrige un bug
- **refactor** — réécrit/restructure le code sans changer son comportement
- **perf** — améliore les performances (refactorisation spéciale)
- **style** — formatage/espace uniquement ; aucun changement de signification. Seulement les modifications
- **test** — ajoute ou corrige des tests
- **docs** — Nouveau contenu ajouté. documentation uniquement
- **build** — outils de build, CI, dépendances, version du projet, etc.
- **ops** — infrastructure, déploiement, sauvegarde, récupération, etc.
- **corvées** — divers (par exemple, `.gitignore`)

## Corps du PR — sections requises

Utilisez **exactement les sections de niveau supérieur suivantes** (en-têtes Markdown) :

### 1. `# Summary`

Bref aperçu de **ce qui** changé et **pourquoi** (intention commerciale ou technique).

### 2. `# Changes`

Organisez par **fichier**. Pour chaque fichier touché, utilisez un en-tête de niveau 2 avec le chemin en accents graves, puis des puces décrivant les modifications.

Format :

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

Incluez toujours une sous-section **Jira** sous `# Context`.

**Lorsque le nom de la branche comprend un identifiant Jira :** utilisez un lien cliquable vers le problème (dériver la clé du nom de la branche).

Format :

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Remplacez la clé et l’URL par le ticket réel. Si plusieurs tickets s’appliquent, répertoriez-les chacun sur une seule ligne dans la même sous-section.

**Lorsque le nom de la branche ne comprend pas d’ID Jira** conservez le `## Jira` et utilisez exactement :

```markdown
# Context

## Jira
No ticket
```

## Exemple (description PR complète)

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## Exemple (description PR complète, branche sans ID Jira)

**Title:** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```
