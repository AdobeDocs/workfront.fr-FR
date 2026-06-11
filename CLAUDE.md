---
source-git-commit: 44629631cd2d99eadbed5fd81cf33458b13702af
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---
# Rechercher des articles candidats avant d’en créer de nouveaux

Lorsque Courtney ajoute du nouveau contenu à incorporer (un document de prise de notes, des commentaires de clients ou de chefs de projet, un collage de Slack/transcriptions, des captures d’écran avec des notes, des questions d’assistance), **ne proposez pas de créer d’abord un nouvel article.** Recherchez les articles existants du référentiel et du candidat de surface où le contenu pourrait s’adapter.

## Workflow requis

1. **Lisez d’abord le nouveau contenu** pour identifier le sujet, l’audience (administrateur ou utilisateur final) et les faits/étapes spécifiques qu’il ajoute.
2. **Rechercher des `help/` pour les candidats** à l’aide de grep et de find. Recherchez les articles qui couvrent déjà la même fonctionnalité, le même domaine ou le même workflow.
3. **Renvoie une liste avec classement** des articles candidats (généralement entre 3 et 7), chacun avec :
   - Chemin d’accès au fichier (chemin du backtick cliquable).
   - Une raison d&#39;une ligne pour laquelle il s&#39;agit d&#39;un candidat (dans quelle section il s&#39;insérerait, ou pourquoi c&#39;est la correspondance la plus proche).
   - Tous les avertissements (par exemple, « inadéquation de l’audience : il s’agit de l’utilisateur final, la réception est orientée administrateur »).
4. **Demandez à Courtney où le placer** avant de le rédiger ou de le modifier. Formulez la question de façon explicite, par exemple : « Dans lequel de ces éléments dois-je rédiger ? » ou « Voulez-vous que je l&#39;adapte à #2, ou pensez-vous qu&#39;il a besoin de son propre article ? »
5. **Ne suggérez qu’un nouvel article** si aucun article existant n’est raisonnablement adapté, et expliquez pourquoi aucun des candidats ne fonctionne.

Même si le contenu appartient « évidemment » à un article connu, faites toujours apparaître 2 à 3 alternatives afin que Courtney puisse confirmer l’emplacement. Cela permet de détecter les quasi-doublons et les endroits où le contenu était déjà partiellement couvert.

---

# Proposer des modifications avant de modifier les articles d&#39;aide

Lorsque vous êtes sur le point de modifier un article d’aide `.md` sous `help/`, **ne modifiez pas encore le fichier**. Tout d’abord, affichez ce que vous prévoyez de modifier et attendez l’approbation explicite.

Pour chaque fichier que vous avez l’intention de toucher :

1. Nommez le fichier (chemin d’accès).
2. Affichez la modification proposée sous la forme d’un diff/fragment de code clôturé (ancien texte et nouveau texte) avec suffisamment de contexte environnant pour être sans ambiguïté.
3. Exposez brièvement la raison (1 phrase).
4. Terminez par une demande explicite, par exemple, « Appliquer ces modifications ? » ou « Voulez-vous que je continue ? »

Seulement après que Courtney a dit oui (ou « go », « apply », « do it », etc.) vous devez appeler les outils d’édition.

Cela s’applique à **chaque** modification d’un article de `.md` d’aide : fautes de frappe, correctifs de liens, permutations d’un seul mot, nettoyages de terminologie, nouvelles sections et réécritures. Pas d&#39;exceptions sauf si Courtney dit explicitement « répare ça » ou « ne demande pas, juste modifie » dans le même tour.

Pour les modifications qui s’étendent sur plusieurs articles : regroupez les diffs proposées par fichier sous une seule réponse. Si la visionneuse est volumineuse, répertoriez d’abord les fichiers concernés avec un résumé d’une ligne chacun, puis affichez les diffs par lots et confirmez avant chaque lot.

Cela ne bloque **pas** la recherche en lecture seule (grep, read) ou la rédaction/exploration dans le chat (aucune écriture de fichier).

---

# Messages de validation Git

Lors de la rédaction ou de la génération d’un message de validation Git, suivez ce format.

## Objet

- Environ **50 caractères ou moins**.
- Résumez le changement d&#39;humeur **impérative** (ex : « Ajouter... », « Corriger... », « Refactoriser... »).

## Corps

- Laissez une ligne vide après le sujet avant le corps.
- Développez des lignes avec environ 72 caractères **.**
- Utilisez **puces** pour l’explication. Chaque puce doit commencer par exactement l’une des valeurs suivantes :
   - **📖** — à utiliser lorsque la modification **ajoute** quelque chose de nouveau : nouveaux fichiers, nouvelles sections, nouvelles fonctionnalités, nouveaux en-têtes, nouvelles lignes ou autre contenu nouveau.
   - **✏️** — utiliser lorsque la modification **modifie** travail existant : modification de lignes existantes, mise à jour de sections existantes, refactorisation ou modification du contenu actuel.

Exemple :

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

---

# Requêtes d’extraction (PR)

## Dérivation du problème Jira

- Dérivez l’identifiant de problème Jira à partir du **nom de branche Git actuel** (par exemple, un segment correspondant à `FFENT-8796`).
- **Si le nom de la branche comprend un ID Jira :** utilisez cet ID dans le titre PR et liez-le dans `# Context` `## Jira` →.
- **Si le nom de la branche ne comprend pas d’ID Jira :** omettez la clé Jira dans le titre PR. Incluez toujours des `## Jira` avec exactement : `No ticket`.

## Titre du PR

**Avec ID Jira :** `{type}/{JIRA-ID}- {short task description}`
Exemple : `feat/FFENT-8001- Add validation for numVariations in OCAPI request`

**Sans ID Jira :** `{type}- {short task description}`
Exemple : `docs- Refresh Object Composite API changelog`

### Types de validation

- **feat** — ajoute une nouvelle fonctionnalité
- **fix** — corrige un bug
- **refactor** — réécrit/restructure le code sans changer son comportement
- **perf** — améliore les performances
- **style** — formatage/espace uniquement ; aucun changement de signification
- **test** — ajoute ou corrige des tests
- **docs** — documentation uniquement, nouveau contenu ajouté
- **build** — outils de build, CI, dépendances, version du projet
- **ops** — infrastructure, déploiement, sauvegarde, récupération
- **corvées** — divers (par exemple, `.gitignore`)

## Corps du PR — sections requises

### `# Summary`
Bref aperçu de ce qui a changé et pourquoi.

### `# Changes`
Organisé par fichier. Pour chaque fichier touché, utilisez un en-tête de niveau 2 avec le chemin en accents graves, puis des puces.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.
```

### `# Context`
Incluez toujours une sous-section `## Jira`.

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Ou si pas de ticket : `No ticket`
