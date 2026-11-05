---
description: Normes d’écriture techniques de Workfront pour les articles d’aide. Applique le Guide de style de la documentation de Workfront et les principes de développement d’informations techniques de qualité (DQTI).
applyTo: "help/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%
---

# Qualité d’écriture

Appliquez ces normes lors de la modification, de la révision ou de la rédaction d’un article d’aide.
Conservez l’intention de l’auteur et l’exactitude technique. Pour le complet
ponctuation, terminologie, majuscules et référence de procédure, lire
[.cursor/skills/writing-quality/reference.md](../../.cursor/skills/writing-quality/reference.md).

N’appliquez **ces règles** notes de mise à jour sous .
`help/quicksilver/product-announcements/product-releases/` — utiliser
instructions de formatage des notes de mise à jour à la place.

## Voix et point de vue

- Utiliser **deuxième personne** (« Vous pouvez... ») en s’adressant au lecteur.
- Utilisez des contractions pour une tonalité de conversation (ne pas, ne peut pas, c&#39;est, ils sont).
- Utilisez « Nous vous recommandons » pour les bonnes pratiques, et non « Il est recommandé » ou « Vous devriez ».
- Lorsque vous écrivez pour un groupe d’utilisateurs, référencez d’autres rôles à la troisième personne.
- N&#39;utilisez jamais de pronoms sexospécifiques — restructurez la phrase ou utilisez « they ».
- Pas de barre oblique pour les choix — utilisez « ou » (« lui ou elle » et non « il ou elle »).

## Clarté (DQTI)

- Une idée par phrase ; conservez les phrases en dessous de 25 mots dans la mesure du possible.
- Diriger avec l’action ou le résultat, et non le contexte d’arrière-plan.
- Utilisez le mot le plus simple (« use » non « use », « start » non « initiate »).
- Évitez les nominalisations (« créer » et non « la création de »).
- Utilisez un langage spécifique et concret — évitez les termes vagues (« plusieurs », « divers »).
- Évitez les doubles négatifs.

## Concretence et orientation des tâches (DQTI)

- Utilisez des exemples spécifiques avec des valeurs réalistes ; nommez les éléments et les champs exacts de l’IU.
- Concentrez-vous sur ce que l’utilisateur peut *faire*, et non sur ce qu’*le système*.
- Procédures de lead avec des verbes impératifs (« Créer une tâche », « Configurer des notifications »).
- Fournissez suffisamment de contexte pour agir, mais pas plus.
- Insérez un lien vers une aide détaillée (« Pour plus d’informations, voir [article]. »).

## Majuscules

- **En-têtes** : casse de phrase toujours (« Créer une tâche », pas « Créer une tâche »).
- **Termes Workfront** : saisissez uniquement en majuscules lorsque vous référencez directement un élément de l’interface utilisateur.
  - Direct : « Remplissez le champ Date d’achèvement prévue ».
  - Indirect : « Chaque tâche doit avoir une date d’achèvement planifiée. »
  - Conseil : si vous pouvez mettre « le » ou « a » devant le terme, il est généralement en minuscules.
- **Boutons** : suivez la casse de l’interface utilisateur ; les boutons Tout en majuscules deviennent la casse de la phrase.
- **Rôles** : « Administrateur système » pour le rôle dans l’interface utilisateur ; « Workfront »
« administrateur » pour la personne.

## Titres

- Commande impérative en phrase, basée sur une tâche (« Configurer les niveaux d&#39;accès »).
- Les articles de présentation se terminent par « présentation » (présentation des projets ).
- Divisez de longues sections en plusieurs en-têtes avec des sous-objectifs clairs.

## Renvois et liens

| Situation | Format |
|-----------|--------|
| Lien après avoir donné des informations | « Pour plus d’informations, voir [Nom de l’article]. » |
| Lien sans information préalable | « Pour plus d’informations, voir [Nom de l’article]. » |
| Lien vers une section d’un autre article | « Pour plus d’informations, voir [Nom de la section] dans [Nom de l’article]. » |
| Lien vers une section du même article | « Pour plus d’informations, voir [Nom de la section] dans cet article. » |

- Dans un paragraphe : en ligne. Dans une étape de procédure : sur une nouvelle ligne après l’étape.
- Liens multiples : utilisez une liste à puces.
- Utilisez « coin supérieur droit »/« coin supérieur gauche » pour les positions à l’écran.

## Gras et italique

- **Gras** actions cliquables et éléments d’interface utilisateur **dans les étapes de la procédure uniquement**.
- Ne mettez pas en gras les éléments de l’interface utilisateur, les noms des boîtes de dialogue, des pages, des icônes ou des menus
noms en dehors des étapes de la procédure.
- Utilisez *italique* pour le texte que l’utilisateur doit saisir (« Type *my.workfront.com*... »).
- N&#39;utilisez jamais l&#39;italique pour mettre l&#39;accent — restructurez plutôt la phrase.

## Notes, conseils et avertissements

Utilisez avec parcimonie ; une utilisation excessive les rend invisibles.

- Une note/conseil/avertissement maximum par section ; ne les empilez jamais.
- Combinez des notes connexes dans une note avec une liste à puces.
- N’utilisez pas de notes pour annoncer une nouvelle fonctionnalité : relisez plutôt le texte de l’article.

| Type | Rôle |
|------|---------|
| `>[!NOTE]` | Informations ne correspondant pas au paragraphe ; contrôle de version/compatibilité |
| `>[!TIP]` | Des suggestions intéressantes qui facilitent la vie de l’utilisateur |
| `>[!IMPORTANT]` | Informations vitales pour l’étape ou la procédure |
| `>[!WARNING]` | Alerter l’utilisateur d’une perte de données potentielle |

## Procédures

- Utilisez des en-têtes de commande impératifs ; présentations uniquement lorsque cela est nécessaire.
- Format d’introduction préféré : expression infinie + deux-points (« Pour créer un temporaire
mot de passe : »).
- Les procédures en une seule étape utilisent toujours une liste numérotée.
- Utilisez « type » ou « select » — évitez les mots vagues comme « set » ou « specifier ».
- Étapes conditionnelles : « (Conditionnel) Si vous êtes membre de plusieurs équipes,
sélectionnez... ». Étapes facultatives : « (Facultatif) Pour ajouter un émoticône, cliquez sur... ».
- Décrivez la réponse du système avant qu’elle ne se produise ou immédiatement après.
- Plusieurs méthodes : commencez par documenter la méthode la plus simple, puis utilisez « Ou ».
- Navigation par menu/onglet : « Cliquez **E-mail** > **Notifications** » (mettez les noms en gras, pas
les crochets ; espaces autour des crochets). Ne pas utiliser de crochets pour le menu principal
navigation : utilisez le fragment de code du menu principal.

## Référence rapide de ponctuation

| Règle | Exemple |
|------|---------|
| Virgule d&#39;Oxford toujours | « motif, moyens et opportunité » |
| Virgule avant « then » dans les procédures | « Cliquez sur Configuration, puis sur Interface. » |
| Virgule après l’année dans une date au milieu de la phrase | « Le numéro du 2 janvier 2016 de... » |
| Pas de virgule avec le mois-année uniquement | « Janvier 2016 » |
| Deux-points avant une liste, minuscules après | « Sélectionnez l’une des options suivantes : option A » |
| Pas de signe deux-points après les en-têtes de procédure | « Créer une tâche » |
| Aem tirets avec parcimonie | Restructurer la phrase si possible |
| Points dans les extensions de fichier | « Charger un fichier .pdf » |

## Organisation (DQTI)

- Structure logique avec divulgation progressive (présentation → détails → référence).
- Une rubrique par section ; utilisez des listes pour 3 éléments parallèles ou plus.
- Gardez les éléments de liste et leur introduction grammaticalement parallèles.
- Utilisez des tableaux pour les comparaisons structurées ou les descriptions de champs.
- Évitez les paragraphes de texte accrochés aux murs — divisez-les en blocs digestibles.

## Liste de contrôle de validation

- [ ] Deuxième personne tout au long, les contractions utilisées.
- [ ] le cas de phrase sur tous les en-têtes.
- [ ] termes de Workfront ont été correctement mis en majuscules (référence directe ou indirecte).
- [ ] Gras uniquement sur les actions cliquables dans les étapes de la procédure.
- [ ] références croisées utilisent le format standard.
- [ ] notes/conseils/avertissements non empilés, un maximum par section.
- [ ] virgule d’Oxford utilisée de manière cohérente.
- [ Les étapes de la procédure ] utilisent des verbes spécifiques (saisissez, sélectionnez, cliquez).
- [ ] Étapes conditionnelles/facultatives correctement libellées.
- [ ] Aucun pronom de genre.
- [ ] Les phrases sont claires, concrètes et axées sur la tâche ; la structure parallèle tient.
