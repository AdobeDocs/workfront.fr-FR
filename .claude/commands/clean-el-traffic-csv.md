---
name: clean-el-traffic-csv
description: Nettoie une exportation CSV de trafic Experience League/Adobe Analytics brut vers des pages uniquement Workfront, triées par Pages vues. À utiliser lorsque l’utilisateur fournit un fichier CSV de trafic de pages Experience League (colonnes telles que « URL de page générique », « Visiteurs uniques », « Visites », « Pages vues ») et demande à le nettoyer, à le filtrer ou à le traiter, ou mentionne les feuilles de calcul « suivi de la documentation » / « articles les plus consultés ».
source-git-commit: 3c5f28f5656fec574cb1ca9d3853703b6b900fdb
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---


# Nettoyer le trafic Experience League au format CSV

Transforme une exportation brute de trafic de page Experience League sous forme de tableau à structure libre Adobe Analytics en un fichier CSV dédupliqué, propre et uniquement Workfront, trié par pages vues, en remplaçant le fichier d’origine.

## Formes d&#39;entrée

L’entrée peut prendre deux formes :

1. **Exportation brute** : commence par des lignes de commentaires de métadonnées (`#===`, `# Freeform`, `# Report suite: ...`, `"# Date: <range>"`, etc.), suivies d’un tableau de répartition hiérarchique (par exemple `Solution (v2)` → `workfront` → `Page URL Generic (v33)` → lignes d’URL individuelles). La `Page URL Generic (v33)` de cellule littérale (ou un libellé de `Page URL Generic ...` similaire) apparaît à mi-chemin vers le bas, dans la deuxième colonne.
2. **CSV déjà nettoyé** : la première ligne est déjà un en-tête brut comme `Page URL Generic (v33),Unique Visitors,Visits,Page Views`, sans lignes de métadonnées ni colonnes de début supplémentaires.

Détectez la forme que vous avez avant de commencer : si la ligne 1 est une ligne d’en-tête simple correspondant à la forme 2, passez directement à l’étape 2 (aucune période ne sera disponible, donc passez également à l’étape 7, sauf si l’utilisateur fournit une période séparément).

## Workflow

### Étape 0 : capturer la période (exportation brute uniquement, avant de supprimer quoi que ce soit)

Recherchez la ligne de métadonnées près du `# Date: <range>` correspondant supérieur (par exemple, `"# Date: Jul 1, 2026 - Jul 31, 2026"`). Enregistrez les `<range>` (par exemple, `Jul 1, 2026 - Jul 31, 2026`) - cela sera nécessaire ultérieurement à l’étape 7. Effectuez cette opération avant la suppression des lignes.

### Étape 1 : réduire l&#39;exportation brute à un tableau brut (exportation brute uniquement)

1. Recherchez la ligne contenant la `Page URL Generic (...)` de cellule (elle se trouve dans la deuxième colonne de l&#39;exportation standard).
2. Supprimez chaque ligne au-dessus de cette ligne, y compris les lignes de commentaires des métadonnées et les lignes de sous-total `Solution (v2)`/`workfront`.
3. Supprimez chaque colonne à gauche de la cellule de `Page URL Generic` (dans l’exportation standard, il s’agit uniquement de la colonne A).
4. Sur cette même ligne (à présent la ligne d’en-tête), remplacez les valeurs de sous-total numériques à droite de `Page URL Generic (...)` par les en-têtes littéraux, dans l’ordre : `Unique Visitors`, `Visits`, `Page Views`. Ne modifiez pas la cellule `Page URL Generic (...)`.

Résultat : un fichier CSV brut avec un `Page URL Generic (v33),Unique Visitors,Visits,Page Views` d’en-tête suivi d’une ligne par URL.

### Étape 2 : conserver uniquement les lignes Workfront

Pour chaque ligne de données, vérifiez si l’URL contient la sous-chaîne littérale `/workfront/` (barre oblique des deux côtés). Le préfixe des paramètres régionaux n’a pas d’importance (`/en/`, `/zh-hans/`, etc. - tous restent tant que le segment de produit correspond).

- Supprimez la ligne si l’URL ne contient **pas** de `/workfront/` comme segment de chemin d’accès. Cette action supprime d’autres produits tels que `workfront-fusion`, `workfront-learn`, `proofhqpapi`, etc. (une sous-chaîne telle que `tutorials-workfront` ne compte **pas** ; la correspondance doit être la `/workfront/` exacte du segment).
- Conserver la ligne autrement.

### Étape 3 : supprimer l’URL

Pour chaque ligne restante, recherchez des `/using` dans l’URL et conservez uniquement la partie provenant de (et comprenant) la `/` qui suit, en ignorant tout ce qui se trouve avant et y compris les `/using`.

Exemple : `https://experienceleague.adobe.com/en/docs/workfront/using/home` → `/home`

Si `/using` n’est pas trouvée dans l’URL d’une ligne de Workfront, laissez cette URL inchangée et marquez-la pour l’utilisateur ou l’utilisatrice plutôt que de faire des suppositions.

### Étape 4 : supprimer les suffixes de fragment/requête

Si l’URL tronquée contient un `#` ou un `?`, supprimez ce caractère et tout ce qui suit.

Exemple : `/manage-scenarios/restore-a-scenario-version#compare-scenario-versions` → `/manage-scenarios/restore-a-scenario-version`

### Étape 5 : fusion des doublons

Après la réduction, plusieurs lignes peuvent désormais partager la même URL (par exemple, deux lignes de paramètres régionaux différentes qui se réduisent au même chemin d’accès). Combinez toutes les lignes avec une URL identique dans une ligne, en additionnant `Unique Visitors`, `Visits` et `Page Views` indépendamment.

Exemple : `/home,2,2,3` et `/home,5,6,7` → `/home,7,8,10`

### Étape 6 : trier par vues de page

Triez toutes les lignes de données par `Page Views` décroissant (les plus grandes en premier). La ligne d’en-tête reste fixe en haut, au-dessus des données triées.

### Étape 7 : ajoutez la ligne de période (exportation brute uniquement, si elle est capturée à l’étape 0).

Avant de l’insérer, supprimez toutes les virgules de la période capturée (par exemple, `Jul 1, 2026 - Jul 31, 2026` → `Jul 1 2026 - Jul 31 2026`) : la période brute comporte des virgules qui seraient autrement lues comme des séparateurs de colonnes CSV sur cette ligne.

Insérez une nouvelle ligne tout en haut, au-dessus de la ligne d’en-tête, contenant uniquement la période séparée par des virgules.

Ordre des lignes finales : ligne de période → ligne d’en-tête → lignes de données triées.

### Étape 8 : enregistrer

Remplacez le fichier d’entrée d’origine avec le résultat nettoyé.

## Hors de portée

L’envoi ou le partage du fichier CSV nettoyé (par exemple vers Slack) est une étape distincte, non encore définie. N’essayez pas de joindre ou de charger le fichier où que ce soit dans le cadre de cette compétence.

## Implémentation (exportation brute)

Pour une exportation brute, exécutez les étapes 0 à 8 avec ce script PowerShell testé plutôt que de modifier les lignes manuellement. Il est plus rapide et moins sujet aux erreurs pour les fichiers comportant des centaines de lignes. Remplacez `$path` par le chemin d’accès réel au fichier.

Avant l&#39;exécution, vérifiez si le fichier est verrouillé (par exemple, ouvert dans Excel) — si `Set-Content` échoue avec « en cours d&#39;utilisation par un autre processus », demandez à l&#39;utilisateur de le fermer, puis relancez l&#39;exécution.

```powershell
$path = "<full path to the CSV>"
$lines = Get-Content -Path $path -Encoding UTF8

# Step 0: capture the date range
$dateLine = $lines | Where-Object { $_ -match '# Date:\s*(.+?)"?\s*$' } | Select-Object -First 1
$null = $dateLine -match '# Date:\s*(.+?)"?\s*$'
$dateRange = $matches[1].Trim('"').Trim()

# Step 1: find the "Page URL Generic" row and strip everything above/left of it
$headerIdx = -1
for ($i = 0; $i -lt $lines.Count; $i++) {
    if ($lines[$i] -match 'Page URL Generic') { $headerIdx = $i; break }
}
$headerParts = $lines[$headerIdx].Split(',')
$urlHeaderLabel = $headerParts[1]
$newHeader = "$urlHeaderLabel,Unique Visitors,Visits,Page Views"

$dataLines = $lines[($headerIdx + 1)..($lines.Count - 1)] | Where-Object { $_.Trim() -ne '' }

$rows = @()
foreach ($line in $dataLines) {
    $comma1 = $line.IndexOf(',')
    $rest = $line.Substring($comma1 + 1)   # drop column(s) left of the URL
    $parts = $rest.Split(',')
    if ($parts.Count -ne 4) { continue }
    $url = $parts[0]
    $uv = [int]$parts[1]
    $vi = [int]$parts[2]
    $pv = [int]$parts[3]

    # Step 2: keep only /workfront/ rows
    if ($url -notmatch '/workfront/') { continue }

    # Step 3: trim to from "/using" onward
    $usingIdx = $url.IndexOf('/using')
    if ($usingIdx -lt 0) { continue }   # flag/report these separately if any occur
    $trimmed = $url.Substring($usingIdx + 6)   # 6 = length of "/using"

    # Step 4: strip # or ? suffix
    $hashIdx = $trimmed.IndexOfAny(@('#', '?'))
    if ($hashIdx -ge 0) { $trimmed = $trimmed.Substring(0, $hashIdx) }

    $rows += [PSCustomObject]@{ URL = $trimmed; UV = $uv; Visits = $vi; PV = $pv }
}

# Step 5: merge duplicates
$grouped = $rows | Group-Object URL | ForEach-Object {
    [PSCustomObject]@{
        URL    = $_.Name
        UV     = ($_.Group | Measure-Object UV -Sum).Sum
        Visits = ($_.Group | Measure-Object Visits -Sum).Sum
        PV     = ($_.Group | Measure-Object PV -Sum).Sum
    }
}

# Step 6: sort by Page Views descending
$sorted = $grouped | Sort-Object -Property PV -Descending

# Step 7 + 8: prepend date range (commas stripped) + header, then save
$dateRangeNoCommas = $dateRange -replace ',', ''
$outLines = @()
$outLines += $dateRangeNoCommas
$outLines += $newHeader
$outLines += $sorted | ForEach-Object { "$($_.URL),$($_.UV),$($_.Visits),$($_.PV)" }

Set-Content -Path $path -Value $outLines -Encoding UTF8
```

Pour un fichier CSV déjà nettoyé (forme d’entrée 2), ignorez la logique de déplacement de l’en-tête et de période ; exécutez simplement les étapes 2 à 6 et 8 sur l’en-tête/les lignes existants en l’état.
