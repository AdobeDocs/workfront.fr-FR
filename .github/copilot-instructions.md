---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 1%
---
# Instructions de pilotage pour workfront.fr

Ce référentiel contient la documentation Adobe Workfront English. Les règles
les éléments ci-dessous s’appliquent à chaque requête dans cet espace de travail. Les normes spécifiques à un sujet sont installées dans
`.github/instructions/*.instructions.md` et chargement automatiques lors de la modification
fichiers correspondants.

## Rechercher des articles candidats avant d’en créer de nouveaux

Lorsque de nouveaux contenus arrivent (un document de prise de vue, des commentaires des clients ou des chefs de projet), un
Collage de Slack/transcription, copies d’écran avec des notes ou questions d’assistance — **pas
proposez d’abord de créer un article.** Rechercher le référentiel et le candidat de surface
des articles existants dans lesquels le contenu peut s’adapter ;

Workflow requis :

1. **Lisez d’abord le nouveau contenu** pour identifier le sujet, l’audience (administration ou fin).
utilisateur), ainsi que les faits ou étapes spécifiques qu’il ajoute.
2. **Rechercher des `help/` pour les candidats** à l’aide de la recherche de grep et de fichiers. Recherchez
articles qui couvrent déjà la même fonctionnalité, la même zone ou le même workflow.
3. **Renvoie une liste avec classement** des articles candidats (généralement entre 3 et 7), chacun avec :
   - Chemin d’accès au fichier (sous forme de lien cliquable).
   - Une raison d’une seule ligne indiquant qu’il s’agit d’un candidat (dans quel article il s’insérerait ou pourquoi)
     c&#39;est la correspondance la plus proche).
   - Tous les avertissements (par exemple, « incohérence d’audience » : il s’agit de l’utilisateur final, l’entrée est
     face à l’administrateur »).
4. **Demandez où le placer** avant de le rédiger ou de le modifier. Formulez la question
explicitement, par exemple : « Dans quel(le) de ces éléments dois-je faire du brouillon ? » ou « Je veux
l&#39;intégrer dans #2, ou pensez-vous qu&#39;il a besoin de son propre article ? »
5. **suggérer uniquement un nouvel article** si aucun article existant n’est raisonnablement adapté, et
expliquez pourquoi aucun des candidats ne fonctionne.

Même si le contenu appartient de manière « évidente » à un article connu, la surface 2-3 est toujours présente
des alternatives afin que le positionnement puisse être confirmé. Cela permet de capturer les quasi-doublons et les
les endroits où le contenu était déjà partiellement couvert.

## Proposer des modifications avant de modifier les articles d&#39;aide

Lorsque vous êtes sur le point de modifier un article d’aide `.md` sous `help/`, **ne modifiez pas le fichier
yet.** Tout d’abord, affichez ce que vous prévoyez de modifier et attendez l’approbation explicite.

Pour chaque fichier que vous avez l’intention de toucher :

1. Nommez le fichier (chemin d’accès).
2. Afficher la modification proposée sous la forme d’une différence/d’un fragment de code clôturé (ancien texte et nouveau texte).
avec suffisamment de contexte environnant pour être sans ambiguïté.
3. Exposez brièvement la raison (une phrase).
4. Terminez par une demande explicite, par exemple : « Appliquer ces modifications ? » ou « Je veux
continuer ? »

Uniquement après approbation explicite (« oui », « aller », « appliquer », « faire », etc.) devriez-vous
appelez les outils d’édition.

Ceci s&#39;applique à **chaque** modification d&#39;un article de `.md` d&#39;aide — fautes de frappe, correctifs de liens,
permutations de mots simples, nettoyage de la terminologie, nouvelles sections et réécritures. Non
exceptions sauf si l’utilisateur dit explicitement « corrigez-le » ou « ne demandez pas, mais
edit » dans le même tour.

Pour les modifications qui s’étendent sur plusieurs articles, regroupez les diffs par fichier proposés sous .
une réponse. Si la visionneuse est volumineuse, répertoriez d’abord les fichiers concernés avec un résumé d’une ligne
chacune d’elles, puis afficher les différences dans les lots et confirmer avant chaque lot.

Cela ne bloque **pas** la recherche en lecture seule (grep, read) ou la rédaction/exploration
dans le chat (aucune écriture de fichier).

## Combler les lacunes intelligemment

Lorsque l’intention est claire dans le contexte, validez la réponse basée sur les bonnes pratiques plutôt que
présentation des menus d&#39;options. Appliquer les normes d&#39;écriture (voir
`.github/instructions/writing-quality.instructions.md`) proactivement — n&#39;attendez pas
qu&#39;on me rappelle de les suivre. Faire correspondre le nouveau texte à celui de l’article environnant
titres, terminologie et structure. Demandez seulement quand une vraie ambiguïté le ferait
modifiez le résultat.

## Messages de validation Git

### Objet

- Environ **50 caractères ou moins**.
- Résumez le changement d&#39;humeur **impérative** (« Ajouter... », « Corriger... », « Refactoriser... »).

### Corps

- Laissez une ligne vide après le sujet avant le corps.
- Développez des lignes avec environ 72 caractères **.**
- Utilisez **puces** pour l’explication. Chaque puce doit commencer par exactement
l’un des éléments suivants :
  - **📖** — lorsque la modification **ajoute** quelque chose de nouveau : nouveaux fichiers, nouvelles sections, nouveau
    fonctionnalités, nouveaux en-têtes, nouvelles lignes ou autre contenu entièrement nouveau.
  - **✏️** — lorsque la modification **modifie** travail existant : modification de lignes existantes,
    mises à jour des sections existantes, refactorisation ou modifications du contenu actuel.

Exemple :

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

## Requêtes de tirage

### Dérivation du problème Jira

- Obtenez l’identifiant de problème Jira à partir du **nom actuel de la branche Git** (par exemple, un
correspondant au segment `FFENT-8796`).
- **Si le nom de la branche comprend un identifiant Jira** utilisez-le dans le titre et le lien de la requête de tirage
dans `# Context` → `## Jira`.
- **Si le nom de la branche ne comprend pas d’ID Jira** omettez la clé Jira de la requête de tirage.
titre. Incluez toujours des `## Jira` avec des `No ticket` exactes.

### Titre du PR

- **Avec ID Jira :** `{type}/{JIRA-ID}- {short task description}`
  - Exemple : `feat/FFENT-8001- Add validation for numVariations in OCAPI request`
- **Sans Jira ID:** `{type}- {short task description}`
  - Exemple : `docs- Refresh Object Composite API changelog`

Types de validation : **feat** (nouvelle fonctionnalité), **fix** (correctif), **refactor** (restructuration)
sans changement de comportement), **perf** (performances), **style** (mise en forme uniquement),
**test** (tests), **docs** (documentation uniquement, nouveau contenu), **build** (build/CI/
dependencies), **ops** (infrastructure/déploiement), **chore** (divers).

### Corps du PR — sections requises

- `# Summary` — bref aperçu de ce qui a changé et pourquoi.
- `# Changes` : organisé par fichier. Pour chaque fichier touché, utilisez un titre de niveau 2
avec le chemin en accents graves, puis les puces.
- `# Context` — toujours inclure une sous-section `## Jira` avec le problème lié, ou
  `No ticket`.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```
