---
content-type: api
navigation-topic: general-api
title: Champs de texte enrichi dans l’API Adobe Workfront
description: Champs de texte enrichi dans l’API Adobe Workfront
author: John
feature: Workfront API
exl-id: 67fc34dc-0722-4419-8254-0371ad5abfc3
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---


# Champs de texte enrichi dans l’API Adobe Workfront

Certains objets d’Adobe Workfront permettent de stocker du texte avec la mise en forme de texte enrichi. Dans l’API Workfront, le texte enrichi est stocké au format JSON à l’aide du framework open source Draft.js.

## Exemple d’aperçu

Un champ personnalisé avec mise en forme de texte enrichi est appelé **Champ avec du texte enrichi** et peut être associé aux valeurs suivantes :

![](assets/rich-text-example-350x158.png)

**Exemple :** Une requête de GET de base pour récupérer la valeur du champ de formulaire personnalisé **Champ avec du texte enrichi**:

<!-- [Copy](javascript:void(0);) -->
<pre><OBJ Code><OBJ ID><OBJ Code><OBJ ID></pre>

**Exemple :** Cette requête renvoie la valeur de **Champ avec du texte enrichi** dans JSON stocké dans la variable **parameterValue** **DE:champ contenant du texte enrichi**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

**Exemple :** Il s’agit d’une version formatée de la réponse présentée dans la figure directement ci-dessus.

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

## Blocs

Les objets JSON qui stockent le contenu en texte enrichi sont composés de deux parties principales : **blocs** et **entityMaps**.

Un bloc est un objet JSON qui représente une seule ligne de texte formaté. Comme un champ personnalisé unique peut comporter plusieurs lignes de texte, chaque ligne de texte possède son propre bloc et chaque bloc est représenté sous la forme d’un élément dans un tableau parent appelé **blocs**.

**Exemple :** Ici, chaque ligne de texte d’un champ personnalisé est mappée à un élément de bloc dans le tableau de blocs.

![](assets/copy-of-rich-text-mapping-350x159.png)

Chaque élément de bloc étant également un objet JSON, chaque bloc est composé des éléments suivants : **key**, **text**, **type**, **profondeur**, **inlineStyleRanges**, **entityRanges**, et **data**. Chacun de ces éléments fonctionne comme suit :

* **Clé** est l’identifiant unique de ce bloc. La clé est utilisée pour mapper une ligne de texte via entityMaps. Vous trouverez des informations détaillées sur entityMaps dans la section entityMaps de ce document.
* **Texte** est la ligne de contenu texte stockée à partir du champ personnalisé.
* **Type** décrit le type de texte représenté. Par exemple, une ligne de texte stockée dans un bloc peut faire partie d’une liste. Si cette ligne de texte faisait partie d’une liste non ordonnée, son type serait défini comme suit : unordered-list-item.
* Les listes ne sont actuellement pas prises en charge, mais devraient être disponibles prochainement.
* **Profondeur** Ce paramètre définit la profondeur de la ligne lorsque la ligne est une partie imbriquée d’une liste ordonnée ou non ordonnée.
* **inlineStyleRanges** Est un tableau qui décrit le ou les types de formatage appliqués à la ligne de texte représentée par le bloc actuel.

**Exemple :** Voici un tableau inlineStyleRanges qui décrit chaque style au niveau des caractères. Dans ce cas : 9 caractères (longueur : 9) à partir de l’index 0 (décalage : 0) avait le style **Gras** appliqué :

![](assets/copy-of-rich-text-mapping-2-350x136.png)

Si plusieurs types de mise en forme ont été appliqués à une seule ligne, les styles sont mappés à des éléments supplémentaires dans le tableau ** inlineStyleRanges**.

**Exemple :** Voici à quoi ressemblerait un bloc lors du stockage d’une ligne de texte contenant une mise en forme mixte : **Texte en gras et italique**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

>[!NOTE]
>
>Toutes les versions qui suivent la version 20.3 prennent en charge les options de mise en forme gras, italique et souligné.

## entityMaps et entityRanges

Un bloc de données peut potentiellement contenir des entités telles que des liens hypertexte ou d’autres types de mise en forme stylisée qui sont connectés à des sources de données situées en dehors du champ de texte personnalisé.

## Exemples

### Récupération du texte brut à partir de JSON

Lorsqu’un champ personnalisé avec mise en forme de texte enrichi est envoyé, tout le texte est stocké dans le tableau . **blocs**. Cependant, chaque ligne du texte intégral est stockée dans la variable **paramètre text** dans chacun des éléments de bloc distincts qui constituent le tableau parent ; **blocs**. Ainsi, pour récupérer le texte intégral, chaque ligne de texte distincte doit être extraite et découpée en deux. Pour ce faire, effectuez une boucle sur tous les éléments des blocs et concaténez chaque paramètre de texte, avec un délimiteur de ligne (\n).

**Exemple :** Voici à quoi peut ressembler votre JS :

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

### Enregistrement d’une valeur de champ de texte enrichi à l’aide de l’API Workfront

Pour enregistrer les valeurs suivantes d’un champ de texte enrichi à l’aide de l’API Workfront :
<pre>
		Hello <strong>World</strong>!!!
		C'est mon premier <strong>Texte enrichi</strong></pre>

1. Créez un fichier JSON qui représente la valeur du champ de texte enrichi que vous essayez de capturer en organisant chaque ligne de texte dans un élément de bloc, dans le tableau . **blocs**

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Capturez la mise en forme en texte enrichi à l’aide du **inlineStyleRanges** parameter

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Pour capturer la seconde ligne, le texte &quot;Texte enrichi&quot; doit être mis en forme en gras et en italique.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

   >[!NOTE]
   >
   >Bien que la fonctionnalité entityMap ne soit pas prise en charge lors de la version initiale, un champ obligatoire est toujours nécessaire pour transmettre ce JSON dans une requête.

1. Utilisez la variable **stringify** sur le fichier JSON décrit ci-dessus pour effectuer une **PUT** demander et envoyer des mises à jour

   <!-- [Copy](javascript:void(0);) -->
   <pre><OBJ Code><OBJ ID></pre>
