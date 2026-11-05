---
mode: agent
description: 'Supprimez le cadrage de la documentation réservée à l’aperçu Workfront pour la GA : prévisualisez les fragments de code standard, class=« preview » HTML et les étapes ou sections parallèles en aperçu par rapport aux étapes ou sections en production.'
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 1%
---

# Supprimer la mise en surbrillance de l’aperçu

Exécuter ce workflow uniquement lorsque je demande de « supprimer la mise en surbrillance de l’aperçu » (ou lorsque la
même intention). Il convertit des instructions/références balisées en prévisualisation et créées par Courtney
rubriques dans le contenu prêt pour la GA.

## Portée

Appliquer uniquement lorsque **tous** sont vrais :

1. J’ai appelé ce workflow.
2. Le chemin d’accès au fichier ne contient **pas** de `product-announcements` (exclure l’ensemble)
arborescence : notes de mise à jour, versions bêta, annonces).
3. Le fichier n’est pas répertorié sous **Chemins exclus** ci-dessous.
4. La ligne de `author:` de première ligne comprend **`Courtney`** (unique ou co-auteur).
5. L’article comporte au moins l’un des éléments suivants :
   - Langage d’aperçu d’environnement dans un corps de texte en prose ou dans des paragraphes de fragment de code réels
     (« informations mises en surbrillance », « Environnement de prévisualisation », « Pas encore en général »
     available », notes de mise à jour rapides) — **pas** une correspondance à partir du texte du lien seul sur un
     page de table des matières/d’index ;
   - Tout élément HTML avec `class="preview"` (`<span>`, `<div>`, `<p>`, `<li>`...) ;
   - Variable de fragment de code de prévisualisation, telle que `{{highlighted-preview}}` ou
     `{{highlighted-preview-article-level}}`.

Si la portée n’est pas claire, confirmez avant de modifier.

**Table des matières/pages d’index — toujours ignorer** lorsque la seule formulation de l’aperçu se trouve dans une
texte affiché du lien markdown pointant vers un autre article, et le fichier n’a pas de
`class="preview"`, aucune variable de fragment de code et aucun modèle d’aperçu en prose
en dehors des liens.

### Chemins exclus

Ne jamais inventorier ou modifier ces éléments, sauf si je les remplace explicitement :

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md`
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md`

## Workflow requis (humain dans la boucle)

Ne pas modifier en masse sans approbation.

1. **Inventaire** — créer une liste triée de chemins d&#39;accès dans la portée (`help/` de recherche). Omettre
   `product-announcements`, chemins exclus et mentions de la table des matières/de l’index uniquement.
2. **Commencer** — demandez s&#39;il faut commencer par le premier article (ou par un chemin que je nomme).
3. **Par article — afficher d&#39;abord, modifier après OK** — lire le fichier, proposer des modifications comme
avant/après des extraits ou une comparaison ciblée, puis attendez une approbation explicite.
4. **Après chaque fichier** — demandez s&#39;il faut passer au suivant (ou arrêter/ignorer).

## Règles de contenu (l’aperçu du contenu devient le document)

Objectif : conserver le comportement documenté pour la Prévisualisation, laisser obsolète « en production »
, puis supprimez les libellés et les wrappers de prévisualisation uniquement.

- **Étapes parallèles** : supprimez l’étape « en production » et conservez l’étape « en aperçu ».
L’étape est essentielle, mais elle doit être reformulée pour ne pas être spécifique à l’aperçu. Correction de la numérotation. si
pas de parallèle clair, s&#39;arrêter et demander quel bloc conserver.
- **Sections parallèles** : supprimez la section environnement de production et remplacez-la
avec le contenu de la section aperçu, puis neutralisez le libellé de l’aperçu et supprimez
  Emballages `class="preview"`.
- **Fragments de code et avis dans la partie supérieure de l’article** : supprimez le standard de prévisualisation uniquement et
les phrases dont le seul objectif est de prévisualiser la disponibilité.
- **`class="preview"`** : supprimez les balises d’ouverture et de fermeture, conservez le contenu interne.
Préserver la structure des listes/tableaux ; corriger les listes rompues ou les espaces blancs errants.
- **Sections commentées (`<!-- … -->`)** : ne pas modifier, sauf si je
dites-le. Si le contenu de l’aperçu n’apparaît que dans les commentaires, appelez-le et demandez.
Par défaut : laissez les commentaires inchangés.

## Ne pas

- S’exécute sur des chemins d’accès `product-announcements` ou des chemins d’accès exclus.
- Modifier automatiquement les blocs commentés.
- Supprimez « Aperçu » lorsqu’il s’agit d’un nom de produit dans un contexte non lié (par exemple, Aperçu).
Environnement sandbox) — demandez si vous n’êtes pas sûr.
- Modifiez le `author:` ou le front-issue sans rapport.
- Ignorer l’étape Afficher → approuver .

## Contrôles qualité avant présentation des modifications

- Aucune `class="preview"` restante dans le périmètre convenu.
- Aucun en-tête en double orphelin ni numéro d’étape rompu.
- L’introduction se lit correctement pour la disponibilité générale (pas de « prévisualisation uniquement » pour les fonctionnalités livrées).
