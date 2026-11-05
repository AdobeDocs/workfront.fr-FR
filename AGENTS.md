---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%
---
# AGENTS.md

Guide de l’agent pour le référentiel **workfront.en** (Adobe Workfront English)
documentation). Ce fichier pointe vers les instructions canoniques afin que tout agent —
quel que soit le fichier de convention qu&#39;il lit — suit les mêmes règles.

## Fichiers d&#39;instructions canoniques

- **Règles à l’échelle du référentiel** : [.github/copilot-instructions.md](.github/copilot-instructions.md)
— formats de recherche d’articles candidats, de proposition avant modification, de validation de message et de RP,
et « combler intelligemment les lacunes ».
- **Écriture de normes** (s’applique automatiquement aux `help/**/*.md`) :
  [.github/instructions/writing-quality.instructions.md](.github/instructions/writing-quality.instructions.md),
avec tous les détails dans
  [.cursor/skills/writing-quality/reference.md](.cursor/skills/writing-quality/reference.md).
- **Notes de mise à jour** (s’applique automatiquement aux `product-announcements/product-releases/**`) :
  [.github/instructions/release-notes-formatter.instructions.md](.github/instructions/release-notes-formatter.instructions.md).
- **Nettoyage de la prévisualisation et de la mise en surbrillance** (workflow à la demande) :
  [.github/prompts/remove-preview-highlighting.prompt.md](.github/prompts/remove-preview-highlighting.prompt.md).

## Comportements non négociables

1. **Rechercher des articles candidats avant d&#39;en créer de nouveaux.** Lorsque du nouveau contenu arrive
dans , recherchez `help/` et faites apparaître une liste classée des articles existants qui pourraient y correspondre,
puis demandez-vous à quoi il appartient avant de rédiger.
2. **Proposez des modifications avant de modifier un article de `.md` d’aide.** Afficher le proposé
diff et attente de l’approbation explicite. La seule exception, c&#39;est quand je dis « juste réparer
il » ou « ne pas demander, juste modifier » dans le même tour. Recherche en lecture seule et en chat
la rédaction est toujours bonne.
3. **Combler intelligemment les lacunes.** Lorsque l’intention est claire, engagez-vous à
bonnes pratiques pour répondre et correspondre aux en-têtes de l’article environnant,
la terminologie et la structure au lieu de présenter les menus d’options.
4. **Appliquez les normes d&#39;écriture de manière proactive** à chaque modification `help/` - n&#39;attendez pas
à rappeler.

## Conventions de validation et de RP

Voir [.github/copilot-instructions.md](.github/copilot-instructions.md) pour plus d’informations
format commit-message (objet impératif ≤ ~50 caractères ; 📖 pour les ajouts, ✏️ pour
modifications) et la structure PR (ID Jira à partir du nom de la branche ; `# Summary`,
`# Changes` par fichier, `# Context` → `## Jira`).
