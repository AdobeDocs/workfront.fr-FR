---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Outils
description: Le [!DNL Adobe Workfront Fusion Tools] comprend plusieurs modules utiles qui peuvent améliorer votre scénario.
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2290'
ht-degree: 0%

---

# [!UICONTROL Outils]

Le [!DNL Adobe Workfront Fusion Tools] comprend plusieurs modules utiles qui peuvent améliorer votre scénario.

[!UICONTROL Outils] Les modules sont disponibles à partir de la liste des applications ou de la [!UICONTROL Outils] icon ![](assets/tools-icon-small.png) au bas de l’écran.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Outils] et leurs champs

* [Triggers](#triggers)
* [Actions](#actions)
* [Agrégateurs](#aggregators)
* [Transformers](#transformers)

### Triggers

#### [!UICONTROL déclencheur de base]

Ce module vous permet de créer un déclencheur personnalisé et de définir ses lots d’entrée.

Vous pouvez utiliser ce module, par exemple, pour les contacts ou toute autre liste programmée pour l’envoi à une adresse email spécifique (telle que [!UICONTROL Email] >[!UICONTROL Envoyer un courrier électronique]ou [!DNL Gmail] >[!UICONTROL Envoyer un courrier électronique] ) ou comme simple rappel à déclencher lorsque vous le souhaitez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bundle]</td> 
   <td> <p>Créez des lots personnalisés en ajoutant des éléments de tableau. Le tableau est constitué des paires nom-valeur.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Obtention de plusieurs variables]](#get-multiple-variables)
* [[!UICONTROL Get Variable]](#get-variable)
* [[!UICONTROL Incrémenter, fonction]](#increment-function)
* [[!UICONTROL Définition de plusieurs variables]](#set-multiple-variables)
* [[!UICONTROL Définir la variable]](#set-variable)
* [[!UICONTROL Dormir]](#sleep)

#### [!UICONTROL Obtention de plusieurs variables]

Ce module récupère les valeurs qui ont été créées précédemment par la fonction [!UICONTROL Définir la variable] ou [!UICONTROL Définition de plusieurs variables] module .

Ce module peut lire les variables qui ont été définies n’importe où dans le scénario, même si la variable a été définie sur un itinéraire différent de celui où la variable [!UICONTROL Obtention de plusieurs variables] se trouve. La seule condition requise est que la variable [!UICONTROL Outils] > [!UICONTROL Définir la variable] ou [!UICONTROL Outils] > [!UICONTROL Définir plusieurs variables] est exécuté avant l’exécution du module [!UICONTROL Outils] > [!UICONTROL Obtention de plusieurs variables] module . Pour plus d’informations sur l’ordre d’exécution des modules, voir [Module de routeur dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variables]</td>
        <td>Ajoutez les variables que vous souhaitez que le module récupère.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Nom de variable]</td>
        <td>Pour chaque variable que vous ajoutez, mappez le nom de la variable que vous souhaitez obtenir.</td>
    </tr>
</table>

>[!INFO]
>
>**Exemples :**  Vous trouverez ci-dessous des utilisations possibles de la fonction [!UICONTROL Définir]/[!UICONTROL Obtenir (plusieurs) variable(s)] modules :
>
>* Pour stocker une valeur calculée en vue d’une utilisation ultérieure, même sur un autre itinéraire. Cela s’avère utile lorsque la valeur est utilisée dans plusieurs modules et que la formule de calcul de la valeur est trop complexe.
>* Pour déboguer une formule. Si une formule utilisée dans un module ne semble pas donner un résultat correct, copiez-la et collez-la dans un [!UICONTROL Définir la variable] que vous insérez avant le module correspondant. Déconnectez le ou les modules après la [!UICONTROL Définir la variable] et exécutez le scénario. Vérifiez les [!UICONTROL Définir la variable] sortie du module, ajustez ou simplifiez la formule, exécutez à nouveau le scénario, puis continuez jusqu’à ce que le problème soit résolu.


#### [!UICONTROL Get Variable]

Ce module récupère une valeur qui a été créée précédemment par la fonction [!UICONTROL Définir la variable] ou [!UICONTROL Définition de plusieurs variables] module .

Ce module peut lire les variables qui ont été définies n’importe où dans le scénario, même si la variable a été définie sur un itinéraire différent de celui où la variable [!UICONTROL Get Variable] se trouve. La seule condition requise est que la variable [!UICONTROL Outils] > [!UICONTROL Définir la variable] ou [!UICONTROL Outils] > [!UICONTROL Définition de plusieurs variables] est exécuté avant l’exécution du module [!UICONTROL Outils] > [!UICONTROL Get Variable] module . Pour plus d’informations sur l’ordre d’exécution des modules, voir [Module de routeur dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom de variable]</td> 
   <td> <p>Faites correspondre le nom de la variable que vous souhaitez que le module obtienne.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Incrémenter, fonction]

Ce module renvoie une valeur incrémentée de 1 après l’opération de chaque module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Réinitialiser une valeur]</td> 
   <td> <p>Sélectionnez cette option lorsque vous souhaitez que le module incrémente la valeur. </p> 
    <ul> 
     <li>[!UICONTROL Après un cycle]</li> 
     <li>[!UICONTROL Après l’exécution d’un scénario]</li> 
     <li>[!UICONTROL Jamais]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple:**
>
>L’une des utilisations du module est de mettre en oeuvre une affectation &quot;à tour de rôle&quot; de tâches, de pistes, d’emails, etc., à des utilisateurs d’un groupe. L’algorithme choisit les personnes désignées d’un groupe dans un ordre rationnel, allant généralement du haut vers le bas d’une liste. Lorsque l’algorithme atteint la fin de la liste, il attribue alors l’attribution suivante à l’utilisateur en haut de la liste et continue à effectuer des affectations vers le bas de la liste.
>
>Le scénario suivant envoie un email au premier destinataire après chaque exécution d’un scénario à numéro impair, et au deuxième destinataire après chaque exécution d’un scénario à numéro pair.
>
>![](assets/example-email-350x246.gif)
>
>1. Pour créer ce scénario :
>1. Définissez la variable **[!UICONTROL Réinitialiser une valeur]** sur Jamais.
>1. Définissez l’itinéraire des valeurs impaires. Définissez le filtre pour cet itinéraire à l’aide de la fonction mathématique modulaire qui est égale à `1`:
>
>   ![](assets/odd-350x459.png)
>
>  **Remarque**: N’oubliez pas de modifier la variable [!UICONTROL Égal à] à partir de la valeur par défaut [!UICONTROL Texte] à l’opérateur [!UICONTROL Numérique] de l’opérateur.
>
>1. Définissez l’itinéraire des valeurs pair à l’aide de la fonction mathématique modulaire qui est égale à `0`:
>
>La fonction d’incrément en ajoute une chaque fois que le scénario s’exécute. Les filtres vérifient l’incrément et agissent sur sa valeur, en s’assurant que les emails sont répartis de manière égale.

#### [!UICONTROL Définition de plusieurs variables]

Ce module crée des variables qui peuvent être mappées par d’autres modules de l’itinéraire. La variable peut également être mappée à la variable [!UICONTROL Get Variable] ou [!UICONTROL Obtention de plusieurs variables] modules pour tout itinéraire dans le scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variables]</td> 
   <td>Ajoutez les variables que le module doit définir.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom de variable] </td> 
   <td>Pour chaque variable, saisissez le nom de la variable. Ce nom s’affiche lors du mappage de la variable dans d’autres modules. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valeur de variable] </td> 
   <td>Pour chaque variable, saisissez la valeur de la variable. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durée de vie de la variable] </td> 
   <td> <p>Sélectionnez la durée de validité des variables (conserver la même valeur).</p> 
    <ul> 
     <li><strong>[!UICONTROL Un cycle]</strong>: La variable est valide pour un cycle. Utile lorsque plusieurs webhooks dans un scénario d’exécution sont reçus (plus de webhooks = plus de cycles). </li> 
     <li><strong>[!UICONTROL Une exécution]</strong>: La variable est valide pour une exécution de scénario. Une exécution peut contenir un ou plusieurs cycles.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Définir la variable]

Ce module crée une variable qui peut être mappée par d’autres modules de l’itinéraire. La variable peut également être mappée à la variable [!UICONTROL Get Variable] ou [!UICONTROL Obtention de plusieurs variables] modules pour tout itinéraire dans le scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nom de variable] </td> 
   <td>Saisissez le nom de la variable. Ce nom s’affiche lors du mappage de la variable dans d’autres modules. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durée de vie de la variable] </td> 
   <td> <p>Sélectionnez la durée de validité des variables (conserver la même valeur).</p> 
    <ul> 
     <li><strong>[!UICONTROL Un cycle]</strong>: La variable est valide pour un cycle. Utile lorsque plusieurs webhooks dans un scénario d’exécution sont reçus (plus de webhooks = plus de cycles). </li> 
     <li><strong>[!UICONTROL Une exécution]</strong>: La variable est valide pour une exécution de scénario. Une exécution peut contenir un ou plusieurs cycles.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valeur de variable] </td> 
   <td>Saisissez ou mappez la valeur de la variable. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dormir]

Ce module vous permet de retarder le flux du scénario jusqu’à 300 secondes (5 minutes).

Cette fonction peut s’avérer utile, par exemple, si vous souhaitez réduire la valeur [!DNL target] chargement du serveur de service ou pour imiter le comportement humain lors de l’envoi de SMS ou d’emails en masse.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Délai]</p> </td> 
   <td> <p>Saisissez le nombre de secondes pendant lesquelles le scénario sera suspendu.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Si vous souhaitez suspendre le flux pendant de plus longues périodes, nous vous suggérons de diviser votre scénario en deux scénarios :
>
>* Le premier scénario contiendrait la partie avant la pause.
>* Le deuxième scénario contiendrait la partie après.
>
>Le premier scénario consiste à stocker toutes les informations nécessaires dans un entrepôt de données, ainsi que l’horodatage actuel. Le deuxième scénario recherche périodiquement dans l’entrepôt de données des enregistrements dont l’horodatage est antérieur au délai prévu, récupère les enregistrements, finalise le traitement des données et supprime les enregistrements de l’entrepôt de données.
>
>Pour plus d’informations sur les entrepôts de données, voir [Entrepôts de données dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>Pour plus d’informations sur des modules d’entrepôt de données spécifiques, voir [[!UICONTROL Entrepôt de données] modules](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### Agrégateurs

* [[!UICONTROL Agrégateur numérique]](#numeric-aggregator)
* [[!UICONTROL Agrégateur de tableau]](#table-aggregator)
* [[!UICONTROL Agrégateur de texte]](#text-aggregator)

#### [!UICONTROL Agrégateur numérique]

Ce module permet de récupérer des valeurs numériques, puis d&#39;appliquer l&#39;une des fonctions sélectionnées (SUM, AVG, COUNT, MAX, MIN), et de renvoyer le résultat dans un seul lot.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Module source]</p> </td> 
   <td> <p>Sélectionnez le module à partir duquel vous souhaitez agréger les champs.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL, fonction d’agrégat]</p> </td> 
   <td> <p>Sélectionnez la fonction à utiliser pour agréger les valeurs.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Groupe [!UICONTROL par]</p> </td> 
   <td> <p>Définissez une expression selon laquelle vous souhaitez regrouper la sortie agrégée. Cette expression peut contenir un ou plusieurs éléments mappés. Les données agrégées sont ensuite séparées en groupes à l’aide de la valeur de cette expression. Chaque groupe génère un lot distinct avec une clé (l’expression évaluée) et une valeur (la valeur agrégée). Vous pouvez utiliser la clé comme filtre dans les modules suivants.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arrêter le traitement après une agrégation vide]</td> 
   <td>Activez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Value]</p> </td> 
   <td> <p>Saisissez ou mappez la valeur que vous souhaitez agréger.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agrégateur de tableau]

Ce module fusionne les valeurs des champs sélectionnés des lots reçus en un seul lot à l’aide d’un séparateur de colonne et de ligne spécifié (ce qui vous permet de créer un tableau).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Module source]</p> </td> 
   <td> <p>Sélectionnez le module à partir duquel vous souhaitez agréger les champs.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Champs agrégés]</td> 
   <td> <p> Sélectionnez dans le module sélectionné ci-dessus les champs contenant les valeurs que vous souhaitez agréger dans le seul lot.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Séparateur de colonnes]</p> </td> 
   <td> <p>Sélectionnez ou saisissez le type de séparateur qui séparera les colonnes de valeurs de champ dans le lot obtenu. Si vous sélectionnez [!UICONTROL Autre], saisissez le caractère à utiliser pour séparer les valeurs dans le champ du séparateur.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Séparateur de lignes]</p> </td> 
   <td> <p>Sélectionnez ou saisissez le type de séparateur qui séparera les lignes de valeur de champ dans le lot obtenu. Si vous sélectionnez [!UICONTROL Autre], saisissez le caractère à utiliser pour séparer les valeurs dans le champ du séparateur.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Groupe [!UICONTROL par]</p> </td> 
   <td> <p>Définissez une expression selon laquelle vous souhaitez regrouper la sortie agrégée. Cette expression peut contenir un ou plusieurs éléments mappés. Les données agrégées seront ensuite séparées en groupes à l’aide de la valeur de cette expression. Chaque groupe génère un lot distinct avec une clé (l’expression évaluée) et une valeur (la valeur agrégée). Vous pouvez utiliser la clé comme filtre dans les modules suivants.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arrêter le traitement après une agrégation vide]</td> 
   <td>Sélectionnez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agrégateur de texte]

Ce module fusionne les valeurs des champs sélectionnés des lots reçus en un seul lot.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Module source]</p> </td> 
   <td> <p>Sélectionnez le module à partir duquel vous souhaitez agréger les champs.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Séparateur de lignes]</p> </td> 
   <td> <p>Sélectionnez ou saisissez le type de séparateur qui séparera les lignes de valeur de champ dans le lot obtenu. Si vous sélectionnez [!UICONTROL Autre], saisissez le caractère à utiliser pour séparer les valeurs dans le champ du séparateur.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Groupe [!UICONTROL par]</p> </td> 
   <td> <p>Définissez une expression contenant un ou plusieurs éléments mappés. Les données agrégées sont séparées sous Groupes avec la même valeur d’expression. Chaque groupe génère en tant que lot distinct contenant une clé avec l’expression évaluée et le texte agrégé. Vous pouvez ainsi utiliser la clé comme filtre dans les modules suivants.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texte]</td> 
   <td> <p> Saisissez ou mappez le texte que vous souhaitez que le module agrège.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arrêter le traitement après une agrégation vide]</td> 
   <td>Sélectionnez cette option pour arrêter le scénario lorsqu’il n’y a aucun résultat.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** Vous pouvez utiliser l’agrégateur de texte pour insérer d’autres valeurs (par exemple, les noms de client ou les notes) dans un seul lot et envoyer un email contenant toutes les valeurs du corps du message ou de l’objet du message.

### Transformers

* [[!UICONTROL Composer une chaîne]](#compose-a-string)
* [[!UICONTROL Convertir le codage du texte]](#convert-the-encoding-of-the-text)
* [[!UICONTROL Basculer]](#switch)

#### [!UICONTROL Composer une chaîne]

Convertit n’importe quelle valeur en type de données string (texte). Cela facilite le mappage lors du mappage, par exemple, de données binaires.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texte]</td> 
   <td> <p>Saisissez ou mappez les données que vous souhaitez convertir en texte.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convertir le codage du texte]

Convertit le texte d’entrée saisi (ou les données binaires) en codage sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input data]</p> </td> 
   <td> <p>Saisissez ou mappez le contenu à convertir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Page de code des données d’entrée]</td> 
   <td> <p>Sélectionnez le type de codage des données d’entrée. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Page de code de données de sortie]</p> </td> 
   <td> <p>Sélectionnez le type d'encodage de vos données cible (sortie).</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Basculer]

Vérifie la valeur d’entrée pour une correspondance avec la liste de valeurs fournie. Renvoie une sortie basée sur le résultat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input]</p> </td> 
   <td> <p>Saisissez l’expression que vous souhaitez évaluer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utiliser des expressions régulières pour faire correspondre]</td> 
   <td> <p>Activez cette option pour utiliser des expressions régulières. Le module détermine les cas en fonction de l’expression régulière, plutôt qu’en fonction d’une correspondance exacte.</p> 
    <div> 
     <p>Une expression régulière est une séquence de caractères dans laquelle chaque caractère est soit un métacaractère, ayant une signification spéciale, soit un caractère normal ayant une signification littérale. Ces caractères et métacaractères identifient un modèle qui peut être utilisé pour rechercher du texte. Par exemple, si vous souhaitez rechercher des noms, vous pouvez configurer une expression régulière pour rechercher un modèle constitué de deux mots consécutifs commençant par des majuscules. Les expressions régulières sont un puissant outil de recherche et de manipulation de texte.</p> 
     <p>Le présent article ne vise pas à aborder la question des expressions régulières. Nous vous recommandons les ressources suivantes :</p> 
     <ul> 
      <li>Pour obtenir la liste complète des métacaractères, voir <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">Expressions régulières</a> dans la documentation web MDN.</li> 
      <li>Pour un tutoriel sur la création d’expressions régulières, nous vous recommandons de <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>Pour expérimenter des expressions régulières, nous vous recommandons le <a href="https://regex101.com/">Expressions régulières 101</a> site web. Sélectionnez l’INDICATEUR ECMAScript (JavaScript) dans le panneau de gauche.</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cas] </td> 
   <td> <p>Si l’entrée contient une valeur saisie dans le champ [!UICONTROL Pattern], la valeur saisie dans le champ [!UICONTROL Output] est renvoyée.</p> <p>Si l’entrée ne correspond à aucune des valeurs que vous avez définies dans un champ [!UICONTROL Modèle], l’une des actions suivantes se produit :</p> 
    <ul> 
     <li>La valeur du champ [!UICONTROL Sinon] est renvoyée.</li> 
     <li>Si aucune valeur n’est renseignée dans le champ [!UICONTROL Sinon], aucune sortie n’est renvoyée.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>Saisissez la valeur renvoyée lorsque les critères définis dans le champ Cas ne sont pas remplis. </p> </td> 
  </tr> 
 </tbody> 
</table>
