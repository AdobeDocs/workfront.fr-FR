---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: L’application XML vous permet d’analyser un texte au format XML via le module XML &gt; Parse XML et de le convertir en un lot afin de rendre les données disponibles pour d’autres modules. Vous pouvez également convertir un lot en texte au format XML via XML &gt; Créer un module XML
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1457'
ht-degree: 9%

---

# XML

L’application [!UICONTROL XML] vous permet d’analyser un texte au format XML via le module [!UICONTROL XML] > [!UICONTROL Parse XML] et de le convertir en lot afin de rendre les données disponibles pour d’autres modules. Vous pouvez également convertir un lot en texte XML via le module [!UICONTROL XML] > [!UICONTROL Créer XML]

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Parse XML]

Le module [!UICONTROL XML] > [!UICONTROL Parse XML] analyse un texte au format XML et génère un seul lot contenant toutes les informations extraites du XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Structure de données]</p> </td> 
   <td> <p>La structure de données décrit la structure du XML pour rendre la sortie du module disponible dans le panneau de mappage pour les modules suivants.</p> <p>Si vous disposez d’un exemple du XML que vous souhaitez analyser, vous pouvez l’utiliser pour générer la structure de données :</p> 
    <ol> 
     <li value="1">Cliquez sur le bouton <strong>[!UICONTROL Ajouter]</strong> .</li> 
     <li value="2">Cliquez sur le bouton <strong>[!UICONTROL Generator]</strong> .</li> 
     <li value="3">Copiez et collez l’exemple XML dans le champ <strong>[!UICONTROL Exemple de données]</strong> .</li> 
     <li value="4">Cliquez sur <strong>[!UICONTROL Enregistrer]</strong>.</li> 
     <li value="5">Vérifiez que la structure de données a bien été générée.</li> 
     <li value="6"> <p>Cliquez sur le bouton <strong>[!UICONTROL Enregistrer]</strong> pour enregistrer la structure de données.</p> <p>Vous pouvez ignorer les étapes 2 à 5 pour fournir une structure de données vide. Si la structure de données est vide, la sortie du module n’est pas disponible dans le panneau de mappage tant que le module n’a pas été exécuté au moins une fois.</p> </li> 
    </ol> <p>Pour plus d’informations, voir <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Structures de données dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conserver les nombres en tant que texte]</td> 
   <td>Activez cette option pour vous assurer que les nombres restent des valeurs de texte (chaîne). Sinon, les nombres sont convertis en valeurs numériques.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>Saisissez ou mappez le texte XML formaté que vous souhaitez analyser.</p> <p>Si vous utilisez une formule, assurez-vous que son type de valeur de résultat est (ou peut être automatiquement contraint) le type de données [!UICONTROL Text]. </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>Si le type de valeur de résultat est [!UICONTROL Buffer] (données binaires), utilisez la fonction <code>toString()</code> pour le convertir en type de données Texte. Pour plus d’informations, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Contrainte de type dans [!DNL Adobe Workfront Fusion]</a> et <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref"> Types de données d’élément dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** Pour télécharger un fichier XML à partir d’une URL et analyser son contenu :
>
>1. Créez un scénario.
>1. Insérez le module [!UICONTROL HTTP] > [!UICONTROL Obtenir un fichier]
>1. Ouvrez la configuration du module et configurez-la comme suit :
>
>   **URL** : URL du fichier XML (par exemple, `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. Cliquez sur **[!UICONTROL OK]** &#x200B; pour enregistrer et fermer la configuration du module.
1. Ajoutez le module [!UICONTROL XML] > [!UICONTROL Parse XML], connectez-le après le module [!UICONTROL HTTP] > [!UICONTROL Obtenir un fichier] et configurez-le comme suit :
>
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL Structure de données]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">Cliquez sur le bouton <strong>[!UICONTROL Ajouter]</strong> .</li> 
&gt;        <li value="2">Cliquez sur le bouton <strong>[!UICONTROL Generator]</strong> .</li> 
&gt;        <li value="3">Dans votre navigateur web, ouvrez un nouvel onglet ou une nouvelle fenêtre.</li> 
&gt;        <li value="4">Insérez l’URL que vous avez utilisée à la troisième étape dans la barre d’adresse et récupérez le fichier XML.</li> 
&gt;        <li value="5">Sélectionnez tout le texte XML et copiez-le dans le Presse-papiers.</li> 
&gt;        <li value="6">Fermez l’onglet ou la fenêtre et revenez à votre scénario.</li> 
&gt;        <li value="7">Collez le texte XML copié dans le champ Exemple de données .</li> 
&gt;        <li value="8">Cliquez sur <strong>[!UICONTROL Enregistrer]</strong>.</li> 
&gt;        <li value="9">Vérifiez que la structure de données a bien été générée.</li> 
&gt;        <li value="10">Cliquez sur <strong>[!UICONTROL Enregistrer]</strong> pour enregistrer la structure de données.</li> 
&gt;       </ol> <p>Vous pouvez ignorer les étapes 2 à 9 pour fournir une structure de données vide. Si la structure de données est vide, la sortie du module n’est pas disponible dans le panneau de mappage tant que le module n’a pas été exécuté au moins une fois.</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL XML]</td> 
&gt;      <td> <p>Faites correspondre l’élément <code>Data </code> de la sortie du module [!UICONTROL HTTP] &gt; [!UICONTROL Obtenir un fichier] dans le champ . Utilisez la fonction <code>toString()</code> pour convertir sa valeur du type de données [!UICONTROL Buffer] (données binaires) en type de données [!UICONTROL Text].</p> <p>Vous pouvez copier et coller le code de la formule dans le champ : <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Pour plus d’informations sur les types de données Buffer et Texte, voir <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Types de données d’élément dans Adobe Workfront Fusion</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>

## [!UICONTROL Analyse des attributs XML]

Par défaut, le module [!UICONTROL XML] > [!UICONTROL Parse XML] place les attributs dans une collection spéciale `_attributes` en tant qu’enfant du noeud qui possède ces attributs. Si le noeud est un noeud de texte et qu’il possède des attributs, deux propriétés spéciales sont ajoutées : `_attributes` pour les attributs et `_value` pour le contenu textuel du noeud.

>[!INFO]
>
**Exemple :** Ce XML :

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

est converti en ce lot :

![](assets/xml-converted-to-bundle.png)

## Créer du XML

Le module [!UICONTROL XML] > [!UICONTROL Créer XML] convertit un lot en texte au format XML.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Structure de données]</p> </td> 
   <td> <p>La structure de données décrit la structure du fichier XML obtenu. Si vous disposez d’un exemple du XML que vous souhaitez créer, vous pouvez l’utiliser pour générer la structure de données :</p> 
    <ol> 
     <li value="1">Cliquez sur le bouton <strong>[!UICONTROL Ajouter]</strong> .</li> 
     <li value="2">Cliquez sur le bouton <strong>[!UICONTROL Generator]</strong> .</li> 
     <li value="3">Copiez et collez l’exemple XML dans le champ Exemple de données .</li> 
     <li value="4">Cliquez sur le bouton <strong>[!UICONTROL Enregistrer]</strong> .</li> 
     <li value="5">Vérifiez que la structure de données a bien été générée.</li> 
     <li value="6">Cliquez sur <strong>[!UICONTROL Enregistrer]</strong> pour enregistrer la structure de données.</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom de l’élément racine]</td> 
   <td>Saisissez le nom de l’élément racine du XML. La valeur par défaut est <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID SYSTÈME Doctype]</td> 
   <td>Saisissez le nom de fichier à utiliser dans la déclaration<code> !DOCTYPE SYSTEM</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype ID PUBLIC]</td> 
   <td>Saisissez le nom de fichier à utiliser dans la déclaration<code> !DOCTYPE PUBLIC</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strip Xml Déclaration]</td> 
   <td>Activez cette option pour supprimer la déclaration XML <code>&lt;?xml ... ?&gt;</code> et <code>&lt;!DOCTYPE ... &gt;</code> et ne laisser que l’élément racine XML et son contenu.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
**Exemple :**
>
Un cas d’utilisation type consiste à transformer les données d’une feuille de calcul [!DNL Google] >en données XML.
>
1. Placez le module [!DNL Google Sheets] > [!UICONTROL Sélectionner les lignes] dans votre scénario pour récupérer les données. Configurez le module pour récupérer les lignes de votre feuille de calcul [!DNL Google]. Définissez la &#x200B;**[!UICONTROL Nombre maximal de lignes renvoyées]** sur un petit nombre, mais plus grand qu’un à des fins de test (par exemple, trois). Exécutez le module [!DNL Google Sheets] en cliquant dessus avec le bouton droit de la souris et en choisissant &quot;**[!UICONTROL Exécuter ce module uniquement]**&quot;. Vérifiez la sortie du module.
1. Connectez le module [!UICONTROL Agrégateur de tableau] après le module [!DNL Google Sheets]. Dans la configuration du module, choisissez le module [!DNL Google Sheets] dans le champ **[!UICONTROL Noeud Source]** . Laissez les autres champs tels quels pour le moment.
1. Connectez le module [!UICONTROL XML] > [!UICONTROL Créer XML] après le module [!UICONTROL Agrégateur de tableau].
>
La configuration du module nécessite une structure de données qui décrit la structure de la sortie XML. Cliquez sur le bouton **[!UICONTROL Ajouter]** pour ouvrir la configuration de la structure de données. La méthode la plus simple pour créer cette structure de données consiste à la générer automatiquement à partir d’un exemple XML.
>
1. Cliquez sur le bouton **[!UICONTROL Generator]** et collez votre exemple XML dans le champ [!UICONTROL Sample data] :
>
![](assets/sample-data-field-350x146.png)
>
1. Cliquer sur **[!UICONTROL Enregistrer]**. Le champ Spécification de la structure de données contient désormais la structure générée.
1. Remplacez le nom de votre structure de données par quelque chose de plus spécifique et cliquez sur **[!UICONTROL Enregistrer]**. Un champ correspondant à l’attribut de tableau racine apparaît comme champ mappable dans la configuration du module JSON.
1. Cliquez sur le bouton **[!UICONTROL Map]** en regard du champ et mappez l’élément `Array[]` de la sortie [!UICONTROL  Array aggator] vers celui-ci :
1. Cliquez sur **[!UICONTROL OK]** pour fermer la configuration du module XML.
1. Ouvrez la configuration du module [!UICONTROL Agrégateur de tableau] . Remplacez la **[!UICONTROL structure cible]** de Personnalisé par le champ d’un module XML correspondant à l’élément XML parent. Faites correspondre les éléments du module [!DNL Google Sheets] aux champs appropriés.
1. Cliquez sur **[!UICONTROL OK]** pour fermer la configuration du module d’agrégation de tableaux.
1. Exécutez le scénario.
>
Le module XML génère le fichier XML correct.
>
1. Ouvrez la configuration du module [!DNL Google Sheets] et augmentez le nombre [!UICONTROL maximal de lignes renvoyées] à un nombre supérieur au nombre de lignes dans votre feuille de calcul pour traiter toutes les données.
>
Le fichier XML obtenu peut être enregistré dans [!DNL Dropbox], envoyé en tant que pièce jointe par courrier électronique, téléchargé via FTP sur un serveur, etc.

## Ajout d’attributs XML

Si vous souhaitez ajouter des attributs à un noeud complexe (un noeud qui contiendra d’autres noeuds), vous devez ajouter une collection portant le nom `_attributes` pour la note complexe dans votre structure de données personnalisée. Cette collection sera mappée aux attributs de noeud. Si vous souhaitez ajouter des attributs à un noeud de texte (par exemple : `<node attr="1">abc</node>`), vous devez ajouter une collection `_attributes` pour les attributs et une propriété de texte `_value` pour la valeur de noeud de ce noeud dans votre structure de données personnalisée.

```
{
   "name": "node",
   "type": "collection",
   "spec": [
      {
         "name": "_attributes",
         "type": "collection"
         "spec": [
            {
               "name": "attr1",
               "type": "text"
            }
         ]
      },
      {
         "name": "_value",
         "type": "text"
      }
   ]
}
```

## Dépannage : impossible de mapper les données du module [!UICONTROL Parse XML]

Assurez-vous que la structure des données est correctement définie. Vous pouvez également utiliser une structure de données vide et exécuter le module au moins une fois pour traiter une entrée XML.
