---
name: remove-preview-highlighting
description: ""
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---


# Supprimer la mise en surbrillance de l’aperçu (Workfront)

## Étendue

Appliquer uniquement lorsque **tous** sont vrais :

1. L’utilisateur a appelé ce workflow (par exemple, dit **« supprimer la mise en surbrillance de l’aperçu »** ou clairement dans le même but).
2. Le chemin d’accès au fichier Markdown ne contient **pas** de **`product-announcements`** (excluez l’arborescence entière de dossiers, par exemple les notes de mise à jour, les versions bêta, les annonces sous `help/quicksilver/product-announcements/`).
3. Le fichier Markdown est **non** répertorié sous **[Chemins exclus](#excluded-paths)** ci-dessous.
4. La partie principale du fichier Markdown comprend les **`Courtney`** sur la ligne de `author:` (auteur unique ou co-auteur).
5. L’article contient **au moins l’un** :
   - Aperçu-environnement **langage dans des paragraphes de corps en prose ou de fragments de code** (modèles standard : « informations mises en évidence », « Environnement d’aperçu », « Pas encore disponible pour tous », notes de mise à jour rapide)—**pas** une correspondance provenant de **texte du lien** sur une page de table des matières/d’index (voir ci-dessous) ; ou
   - tout élément HTML avec **`class="preview"`** (par exemple, `<span class="preview">`, `<div class="preview">`) ; ou
   - Extrait de code d’aperçu **variable** tel que **`{{highlighted-preview}}`** ou **`{{highlighted-preview-article-level}}`**.

Si la portée n’est pas claire, confirmez avant de modifier.

**Table des matières / pages d’index — toujours ignorer ce cas :** **Jamais** placez un fichier dans l’inventaire lorsque le **seul** libellé lié à l’aperçu est **à l’intérieur** du texte d’affichage d’un lien Markdown pointant vers **un autre** article (par exemple *Envoyer un rapport dans l’environnement de sandbox de prévisualisation*) et **le fichier a** no **&#x200B;**, `class="preview"`no **variables de fragment de code et** no **plaque de prévisualisation dans** prose en dehors de links **&#x200B;**. Il ne s’agit pas d’une mise en surbrillance de la prévisualisation sur cette page ; il s’agit uniquement d’une mention Table des matières. S’applique à n’importe quel index/table des matières et non à un seul fichier.

### Chemins exclus

Ne les ajoutez jamais à l’inventaire ou ne les modifiez jamais dans ce workflow, sauf si l’utilisateur ou l’utilisatrice les remplace explicitement :

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md` : les limites de prévisualisation et de production parallèles nécessitent une décision éditoriale délibérée en dehors de l’automatisation.
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md` — table des matières des rapports ; le seul signal « preview » est le lien vers l’article de diffusion Aperçu de Sandbox .

## Workflow requis (humain dans la boucle)

Ne modifiez **pas** référentiel en bloc sans approbation.

1. **Inventaire**\
   Créez une liste triée de chemins d’accès qui respectent les règles d’étendue ci-dessus (recherchez le référentiel ; préférez `help/` arborescences). **Omettre** tout chemin sous **`product-announcements`**, tout chemin sous **[Chemins exclus](#excluded-paths)** et toute **Table des matières/index** page correspondant **Table des matières/pages d’index** sous Portée. Si l’utilisateur indique qu’un fichier répertorié ne dispose pas de mise en surbrillance de l’aperçu, supprimez-le de l’exécution et resserrez les critères plutôt que de forcer les modifications.

2. **Début**\
   Demandez-lui s’il faut commencer par le **premier** article de la liste (ou par un chemin d’accès aux noms d’utilisateur).

3. **Par article — afficher d&#39;abord, modifier après OK**
   - Lire le fichier.
   - Proposez des modifications de manière claire : **avant/après les extraits** ou une description de style diff ciblée de ce qui va changer.
   - **Attendez** une approbation explicite (par exemple, « d’accord », « appliquer », « oui ») avant d’écrire le fichier.

4. **Après chaque fichier**\
   Demandez si vous devez passer à l’article **suivant** (ou arrêter/ignorer).

## Règles de contenu (GA : la prévisualisation du contenu devient le document)

Lors de la suppression de la mise en surbrillance de l’aperçu pour **disponibilité générale**, l’objectif est le suivant : **conserver le comportement qui a été documenté pour l’aperçu**, déposer les branches **obsolètes « en production »/ancien processus**, puis **supprimer les libellés et les wrappers de prévisualisation uniquement** afin que la rubrique se lise comme étant à jour pour tous les clients.

### Étapes parallèles

- Si l’article comporte une étape (ou un élément numéroté) **encadrée comme étant « en production »** (ou l’équivalent : production actuelle / comportement de production existant) **et** une étape **parallèle** encadrée comme **« en aperçu »** (ou environnement de prévisualisation) :
   - **Supprimez** l’étape en production (l’ancien chemin).
   - **Conservez** la substance **de l’étape de prévisualisation**, mais **reformulez** afin qu’elle ne soit **pas** spécifique à la prévisualisation (supprimez « en prévisualisation », « Aperçu de l’environnement », etc.). Ajustez la numérotation pour que la liste reste cohérente.

Si la structure est ambiguë (pas de parallèle clair), **arrêtez** et affichez les deux candidats ; demandez à l’utilisateur quel bloc conserver.

### Sections parallèles

- Si une **section** (en-tête + corps) porte sur **dans l’environnement de production»** et qu’il existe une **section parallèle** **sur «dans l’environnement de prévisualisation»** :
   - **Supprimez** la section environnement de production (le contenu remplacé).
   - **Remplacez** par le contenu de la section d’aperçu, puis **supprimez** le libellé preview-environment et les wrappers **`class="preview"`** afin que la section soit neutre (prête pour la mise à disposition générale).

### Fragments de code et avis dans la partie supérieure de l’article

- Supprimez **blocs standard de prévisualisation uniquement** (plages/div ou paragraphes qui expliquent uniquement que le contenu mis en surbrillance est en prévisualisation uniquement, version rapide, sandbox, etc.) une fois la fonctionnalité mise à disposition générale.
- Supprimez les liens ou les phrases dont l’objectif **uniquement** est la disponibilité de l’aperçu, sauf si l’utilisateur ou l’utilisatrice indique de conserver une autre notification.

### `class="preview"` HTML

- Supprimez les **ouverture et fermeture des balises** pour les éléments qui utilisent **`class="preview"`**, **conservation du contenu interne** (markdown/HTML à l’intérieur de la balise).
- Gérez les balises **`<span class="preview">`** et **`<div class="preview">`**, ainsi que le même modèle sur d’autres balises (par exemple, **`<p class="preview">`**, **`<li class="preview">`**) lorsqu’elles apparaissent dans le corps du contenu **visible** (non commenté).
- Conserver la structure des listes/tableaux ; corriger les listes rompues ou les espaces blancs errants après l’encapsulation.

### Sections commentées (commentaires d’HTML)

- **Ne supprimez** ne dépliez ou ne **modifiez** aucun contenu dans **`<!-- … -->`** commentaires HTML **à moins que l’utilisateur n’indique explicitement** que faire (par exemple, supprimer l’ensemble du commentaire, supprimer les classes d’aperçu dans le commentaire uniquement, supprimer les commentaires pour la disponibilité générale).
- Si le contenu ou la **`class="preview"`** liés à la prévisualisation apparaît **uniquement** dans les commentaires, **appelez-le** lors de la révision de l’article : dites ce qui se trouve dans le commentaire et **demandez** que faire. **Par défaut : ne modifiez pas les sections commentées.**

### Que ne pas faire

- N’exécutez pas ce workflow sur les chemins d’accès sous **`product-announcements`** (notes de mise à jour et connexes), car l’inventaire doit les exclure.
- N’inventoriez ou ne modifiez pas les chemins répertoriés sous **[Chemins exclus](#excluded-paths)**, sauf si l’utilisateur demande explicitement à en inclure un.
- **Ne supprimez pas** ne modifiez pas automatiquement les blocs **&#x200B;**) `<!-- … -->` commentés ; suivez **sections commentées** ci-dessus.
- Ne supprimez pas le « Prévisualisation » lorsqu’il n’est **pas** concernant ce modèle de disponibilité des fonctionnalités (par exemple, [Prévisualisation de l’environnement Sandbox] (·) en tant que **nom du produit** dans un contexte non lié) ; faites preuve de jugement et demandez si vous n’êtes pas sûr.
- Ne modifiez pas `author:` ou le frontMATTER sans rapport à moins que l&#39;utilisateur ne le demande.
- N’ignorez pas l’étape **afficher → approuver**.

## Contrôles qualité avant présentation des modifications

- Aucune **`class="preview"`** restante sur la portée convenue du changement.
- Aucun en-tête en double orphelin ni numéro d’étape rompu.
- L’introduction se lit correctement **sans** contredire la disponibilité générale (pas de « prévisualisation uniquement » pour les fonctionnalités fournies).

## Références

- Respectez les conventions de style de documentation et de référentiel **[Workfront &#x200B;](https://experienceleague.adobe.com/?lang=fr)** (règles de validation/RP si l’utilisateur effectue une validation).
