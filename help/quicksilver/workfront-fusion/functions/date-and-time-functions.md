---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Fonctions de date et d’heure dans Adobe Workfront Fusion
description: Les fonctions de date et d’heure suivantes sont disponibles dans le panneau de mappage d’Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 76c63afc-4bb6-4895-9bba-6b3913ecbcf6
source-git-commit: 6374a1a0ca49507872c71eaebd5227e88e3225b7
workflow-type: tm+mt
source-wordcount: '1958'
ht-degree: 98%

---

# Fonctions de date et d’heure dans [!DNL Adobe Workfront Fusion]

## Conditions d’accès



Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :



<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>N’importe quelle</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licence</td>  
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td>  
   <td> 
   <p>Actuel : aucune exigence de licence [!DNL Workfront Fusion].</p> 
   <p>Ou</p> 
   <p>Hérité : Tout </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produit</td>  
   <td> 
   <p>Nouveau :</p> <ul><li>Formule [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>Plan [!UICONTROL Ultimate] [!DNL Workfront] : [!DNL Workfront Fusion] est inclus.</li></ul> 
   <p>Ou</p> 
   <p>Actuel : votre organisation doit acheter [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Variables

### now

### timestamp

## Fonctions

### [!UICONTROL addSeconds (date ; nombre)]

Renvoie une nouvelle date suite à l’ajout d’un nombre donné de secondes à une date. Pour soustraire les secondes, saisissez un nombre négatif.

>[!INFO]
>
>**Exemples :**
>
>* `addSeconds(2016-12-08T15:55:57.536Z;2)`
>
>   Renvoie 2016-12-08T15:55:59.536Z
>
>* `addSeconds(2016-12-08T15:55:57.536Z;-2)`
>
>   Renvoie 2016-12-08T15:55:55.536Z

### [!UICONTROL addMinutes (date ; nombre)] {#addminutes-date-number}

Renvoie une nouvelle date suite à l’ajout d’un nombre donné de minutes à une date. Pour soustraire les minutes, saisissez un nombre négatif.

>[!INFO]
>
>**Exemples :**
>
>* `addMinutes(2016-12-08T15:55:57.536Z;2)`
>
>    Renvoie 2016-12-08T15:57:57.536Z
>
>* `addMinutes(2016-12-08T15:55:57.536Z;-2)`
>
>    Renvoie 2016-12-08T15:53:57.536Z

### [!UICONTROL addHours (date ; nombre)] {#addhours-date-number}

Renvoie une nouvelle date suite à l’ajout d’un nombre d’heures donné à une date. Pour soustraire les heures, saisissez un nombre négatif.

>[!INFO]
>
>**Exemples :**
>
>* `addHours(2016-12-08T15:55:57.536Z; 2)`
>
>    Renvoie 2016-12-08T17:55:57.536Z
>
>* `addHours(2016-12-08T15:55:57.536Z;-2)`
>
>    Renvoie 2016-12-08T13:55:57.536Z

### [!UICONTROL addDays (date ; nombre)] {#adddays-date-number}

Renvoie une nouvelle date suite à l’ajout d’un nombre donné de jours à une date. Pour soustraire les jours, saisissez un nombre négatif.

>[!INFO]
>
>**Exemples :**
>
>* `addDays(2016-12-08T15:55:57.536Z;2)`
>
>    Renvoie 2016-12-10T15:55:57.536Z
>
>* `addDays(2016-12-08T15:55:57.536Z;-2)`
>
>    Renvoie 2016-12-6T15:55:57.536Z

### [!UICONTROL addMonths (date ; nombre)]

Renvoie une nouvelle date suite à l’ajout d’un nombre donné de mois à une date. Pour soustraire les mois, saisissez un nombre négatif.

>[!INFO]
>
>**Exemples :**
>
>* `addMonths(2016-08-08T15:55:57.536Z;2)`
>
>    Renvoie 2016-10-08T15:55:57.536Z
>
>* `addMonths(2016-08-08T15:55:57.536Z;-2)`
>
>    Renvoie 2016-06-08T15:55:57.536Z

### [!UICONTROL addYears (date ; nombre)]

Renvoie une nouvelle date suite à l’ajout d’un nombre d’années donné à une date. Pour soustraire les années, saisissez un nombre négatif.

>[!INFO]
>
>**Exemples :**
>
>* `addYears(2016-08-08T15:55:57.536Z;2)`
>
>    Renvoie 2018-08-08T15:55:57.536Z
>
>* `addYears(2016-12-08T15:55:57.536Z; -2)`
>
>    Renvoie 2014-08-08T15:55:57.536Z

### [!UICONTROL setSecond (date ; nombre)]

Cette fonction renvoie une nouvelle date avec les secondes spécifiées dans les paramètres.

Indiquez un nombre compris entre 0 et 59. Si le nombre se trouve en dehors de cette plage, la fonction renvoie une seconde à partir de la minute précédente (pour un nombre négatif) ou de la minute suivante (pour un nombre positif).

Si vous devez indiquer un nombre en dehors de la plage, nous vous recommandons d’utiliser [!UICONTROL addSeconds], comme décrit ci-dessus dans la section [addSeconds (date ; nombre)](#addseconds-date-number).

>[!INFO]
>
>**Exemples :**
>
>* `setSecond(2015-10-07T11:36:39.138Z;10)`
>
>    Renvoie 2015-10-07T11:36:10.138Z
>
>* `setSecond(2015-10-07T11:36:39.138Z; 6)`
>
>    Renvoie 2015-10-07T11:37:01.138Z

### [!UICONTROL setMinute (date ; nombre)]

Cette fonction renvoie une nouvelle date avec les minutes spécifiées dans les paramètres.

Indiquez un nombre compris entre 0 et 59. Si le nombre se trouve en dehors de cette plage, la fonction renvoie une seconde à partir de l’heure précédente (pour un nombre négatif) ou de l’heure suivante (pour un nombre positif).

Si vous devez spécifier un nombre en dehors de la plage, nous vous recommandons d’utiliser addMinutes, comme décrit ci-dessus dans la section [addMinutes (date ; nombre)](#addminutes-date-number).

>[!INFO]
>
>**Exemples :**
>
>* `setMinute(2015-10-07T11:36:39.138Z;10)`
>
>    Renvoie 2015-10-07T11:10:39.138Z
>
>* `setMinute(2015-10-07T11:36:39.138Z;61)`
>
>    Renvoie 2015-10-07T12:01:39.138Z

### [!UICONTROL setHour (date; nombre)]

Cette fonction renvoie une nouvelle date avec l’heure spécifiée dans les paramètres.

Indiquez un nombre compris entre 0 et 23. Si le nombre se trouve en dehors de cette plage, la fonction renvoie une heure à partir du jour précédent (pour un nombre négatif) ou du jour suivant (pour un nombre positif).

Si vous devez spécifier un nombre en dehors de la plage, nous vous recommandons d’utiliser addHours, comme décrit ci-dessus dans la section [addHours (date ; nombre)](#addhours-date-number).

>[!INFO]
>
>**Exemples :**
>
>* `setHour(2015-08-07T11:36:39.138Z;6)`
>
>   Renvoie 2015-08-07T06:36:39.138Z
>
>* `setHour(2015-08-07T11:36:39.138;-6)`
>
>    Renvoie 2015-08-06T18:36:39.138Z

### [!UICONTROL setDay (date ; nombre/nom du jour en anglais)]

Cette fonction renvoie une nouvelle date avec le jour spécifié dans les paramètres.

Vous pouvez utiliser cette fonction pour définir le jour de la semaine, avec le dimanche comme 1 et le samedi comme 7. Si vous indiquez un nombre compris entre 1 et 7, la date obtenue est comprise dans la semaine en cours (du dimanche au samedi). Si le nombre ne figure pas dans cette plage, la fonction renvoie un jour de la semaine précédente (pour un nombre négatif) ou de la semaine suivante (pour un nombre positif).

Si vous devez spécifier un nombre en dehors de la plage, nous vous recommandons d’utiliser addDays, comme décrit ci-dessus dans la section [addDays (date ; nombre)](#adddays-date-number).

>[!INFO]
>
>**Exemples :**
>
>* `setDay(2018-06-27T11:36:39.138Z;Monday)`
>
>   Renvoie 2018-06-25T11:36:39.138Z
>
>* `setDay(2018-06-27T11:36:39.138Z;1)`
>
>   Renvoie 2018-06-24T11:36:39.138Z
>
>* `setDay(2018-06-27T11:36:39.138Z;7)`
>
>   Renvoie 2018-06-30T11:36:39.138Z

### [!UICONTROL setDate (date ; nombre)]

Cette fonction renvoie une nouvelle date avec le jour du mois spécifié dans les paramètres.

Indiquez un nombre compris entre 1 et 31. Si le nombre se trouve en dehors de cette plage, la fonction renvoie un jour à partir du mois précédent (pour un nombre négatif) ou du mois suivant (pour un nombre positif).

>[!INFO]
>
>**Exemples :**
>
>* `setDate(2015-08-07T11:36:39.138Z;5)`
>
>   Renvoie 2015-08-05T11:36:39.138Z
>
>* `setDate(2015-08-07T11:36:39.138Z;32)`
>
>   Renvoie 2015-09-01T11:36:39.138Z

### [!UICONTROL setMonth (date ; nombre/nom du mois en anglais)]

Cette fonction renvoie une nouvelle date avec le mois spécifié dans les paramètres.

Indiquez un nombre compris entre 1 et 12. Si le nombre ne figure pas dans cette plage, la fonction renvoie le mois de l’année précédente (pour un nombre négatif) ou de l’année suivante (pour un nombre positif).

>[!INFO]
>
>**Exemples :**
>
>* `setMonth(2015-08-07T11:36:39.138Z;5)`
>
>   Renvoie 2015-05-07T11:36:39.138Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;17)`
>
>   Renvoie 2016-05-07T11:36:39.138Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;january)`
>
>   Renvoie 2015-01-07T12:36:39.138Z

### [!UICONTROL setYear (date ; nombre)]

Renvoie une nouvelle date avec l’année spécifiée dans les paramètres.

>[!INFO]
>
>**Exemple :**
>
>* `setYear(2015-08-07T11:36:39.138Z;2017)`
>
>   Renvoie 2017-08-07T11:36:39.138Z

### [!UICONTROL formatDate (date, format, [fuseau horaire])]

Utilisez cette fonction lorsque vous disposez d’une valeur Date, telle que `12-10-2021 20:30`, que vous souhaitez mettre en forme en tant que valeur Texte, par exemple `Dec 10, 2021 8:30 PM`.

Cela s’avère utile, par exemple, lorsque vous devez remplacer le format de date d’une application ou d’un service web par celui d’une application ou d’un service web connecté dans le même scénario.

Pour plus d’informations, consultez les sections [Date](../../workfront-fusion/mapping/item-data-types.md#date) et [Texte](../../workfront-fusion/mapping/item-data-types.md#text) dans l’article [Types de données d’élément dans Adobe Workfront Fusion](../../workfront-fusion/mapping/item-data-types.md).

#### Paramètres

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Paramètre</th> 
   <th>Type de données attendu* </th> 
   <th>Rôle</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL date] </td> 
   <td>Date </td> 
   <td> <p>Convertit une valeur Date en valeur Texte. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL format] </td> 
   <td>Texte </td> 
   <td> <p>Permet de définir un format à l’aide de jetons de mise en forme de date/heure. Pour plus d’informations, consultez la section <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">Jetons pour le formatage de la date et de l’heure dans [!DNL Adobe Workfront Fusion]</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL timezone] </td> 
   <td>Texte </td> 
   <td> <p>(Facultatif) Permet de spécifier le fuseau horaire utilisé pour la conversion. </p> <p>Pour obtenir la liste des fuseaux horaires reconnus, consultez la colonne « Nom de la base de données des fuseaux horaires » dans Wikipédia <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">Liste des fuseaux horaires de la base de donnée des fuseaux horaires</a>. Seules les valeurs répertoriées dans cette colonne sont reconnues par la fonction comme un fuseau horaire valide. Toute autre valeur est ignorée et le fuseau horaire des scénarios spécifié dans votre profil est utilisé à la place. Pour plus d’informations, consultez l’article <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Modifier les paramètres de profil dans [!DNL Adobe Workfront Fusion]</a>.</p> <p>Si vous omettez ce paramètre, le fuseau horaire Scénarios spécifié dans vos paramètres de profil est appliqué. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

Si un autre type est fourni, la coercition de type est appliquée. Pour plus d’informations, consultez la section [Coercition de type dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

#### Valeur et type de renvoi

La fonction `formatDate` renvoie une représentation textuelle de la valeur Date donnée en fonction du format et du fuseau horaire spécifiés. Le type de données est Texte.

>[!INFO]
>
>**Exemples :** le scénario et le fuseau horaire web ont tous deux été définis sur `Europe/Prague` dans ces exemples.
>
>![](assets/date&time-functions-examples-350x61.png)
>
>* `formatDate(1. Date created;MM/DD/YYYY)`
>
>    Renvoie 10/01/2018
>
>* `formatDate(1. Date created; YYYY-MM-DD hh:mm A)`
>
>   Renvoie 2018-10-01 09:32 AM
>
>* `formatDate(1. Date created;DD.MM.YYYY HH:mm;UTC)`
>
>    Renvoie 01.10.2018 07:32
>
>* `formatDate(now;DD.MM.YYYY HH:mm)`
>
>    Renvoie 19.03.2019 15:30

### [!UICONTROL parseDate (text; format; [timezone])]

Utilisez cette fonction lorsque vous disposez d’une valeur Texte représentant une date (telle que `12-10-2019 20:30` ou `Aug 18, 2019 10:00 AM`) et que vous souhaitez convertir (analyser) en une valeur Date (représentation lisible par un ordinateur binaire). Pour plus d’informations, voir [Date](../../workfront-fusion/mapping/item-data-types.md#date) et [Texte](../../workfront-fusion/mapping/item-data-types.md#text) dans l’article [Types de données d’élément dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

#### Paramètres

La seconde colonne indique le type attendu. Si un autre type est fourni, la coercition de type est appliquée. Pour plus d’informations, voir [Coercition de type dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Paramètre</th> 
   <th>Type de données attendu* </th> 
   <th>Rôle</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL text] </td> 
   <td>Texte </td> 
   <td> <p>Convertit une valeur Date en valeur Texte. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL format] </td> 
   <td>Texte </td> 
   <td> <p>Permet de définir un format à l’aide de jetons de mise en forme de date/heure. Pour plus d’informations, voir <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">Jetons de mise en forme de la date et de l’heure dans Adobe Workfront Fusion</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL timezone] </td> 
   <td>Texte </td> 
   <td> <p>(Facultatif) Permet de spécifier le fuseau horaire utilisé pour la conversion. </p> <p>Pour obtenir la liste des fuseaux horaires reconnus, consultez la colonne « Nom de la base de données des fuseaux horaires » dans Wikipédia <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">Liste des fuseaux horaires de la base de donnée des fuseaux horaires</a>. Seules les valeurs répertoriées dans cette colonne sont reconnues par la fonction comme un fuseau horaire valide. Toute autre valeur est ignorée et le fuseau horaire des scénarios spécifié dans votre profil est utilisé à la place. Pour plus d’informations, voir l’article <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Modifier des paramètres de profil dans Adobe Workfront Fusion</a>.</p> <p>Si vous omettez ce paramètre, le fuseau horaire Scénarios spécifié dans vos paramètres de profil est appliqué.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

Si un autre type est fourni, la coercition de type est appliquée. Pour plus d’informations, consultez la section [Coercition de type dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

#### Valeur et type de renvoi

Cette fonction convertit une chaîne de texte en date, selon le format et le fuseau horaire spécifiés. Le type de données de la valeur est Date.

>[!INFO]
>
>**Exemples :** dans les exemples suivants, la valeur Date renvoyée est exprimée selon la norme ISO 8601, mais le type de données du résultat est Date.
>
>* `parseDate(2016-12-28;YYYY-MM-DD)`
>
>    Renvoie 2016-12-28T00:00:00.000Z
>
>* `parseDate(2016-12-28 16:03;YYYY-MM-DD HH:mm)`
>
>    Renvoie 2016-12-28T16:03:00.000Z
>
>* `parseDate(2016-12-28 04:03 pm; YYYY-MM-DD hh:mm a)`
>
>    Renvoie 2016-12-28T16:03:06.000Z
>
>* `parseDate(1482940986;X)`
>
>   Renvoie 2016-12-28T16:03:06.000Z

### [!UICONTROL dateDifference (Date1 ; Date2 ; Unité)]

Renvoie un nombre représentant la différence entre deux dates, exprimée dans l’unité spécifiée.

Date2 est soustraite de Date1.

Utilisez l’une des valeurs d’heure suivantes pour le paramètre `unit` :

* millisecondes
* secondes
* minutes
* heures
* jours
* semaines
* mois

Si aucune unité n’est spécifiée, la fonction renvoie la différence en millisecondes.

>[!INFO]
>
>**Exemples :**
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z)`
>
>    Renvoie `600,000`
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;hours)`
>
>    Renvoie `4`
>
>* `dateDifference2021-06-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;months)`
>
>    Renvoie `1`

### Exemples supplémentaires

#### Calculer le n-ième jour de la semaine dans le mois

Cette section est adaptée à [!DNL Workfront Fusion] de la page web [!DNL Exceljet] qui explique comment obtenir le n-ième jour de la semaine dans un mois.

Si vous devez calculer une date correspondant au n-ième jour de la semaine dans un mois (par exemple, premier mardi, troisième vendredi, etc.), vous pouvez utiliser la formule suivante :

![](assets/date&time-functions-calc-nth-day-350x31.png)

```
{{addDays(setDate(1.date; 1); 1.n * 7 - formatDate(addDays(setDate(1.date; 1); "-" + 1.dow); "E"))}}
```

La formule contient les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>1.n</code> </td> 
   <td> <p> N-ième jour :</p> 
    <ul> 
     <li><code>1</code> pour le 1er mardi</li> 
     <li><code>2</code> pour le 2e mardi</li> 
     <li><code>3</code> pour le 3e mardi, etc.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>2.dow</code> </td> 
   <td> <p> jour de la semaine :</p> 
    <ul> 
     <li><code>1</code> pour lundi</li> 
     <li><code>2</code> pour mardi</li> 
     <li><code>3</code> pour mercredi</li> 
     <li><code>4</code> pour jeudi</li> 
     <li><code>5</code> pour vendredi</li> 
     <li><code>6</code> pour samedi</li> 
     <li><code>7</code> pour dimanche</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>1.date</code> </td> 
   <td> <p> La date détermine le mois. Pour calculer le n ième de la semaine du mois en cours, utilisez la variable <code>now</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Si vous ne souhaitez calculer qu’un seul cas spécifique, par exemple un mercredi sur deux, vous pouvez remplacer les éléments `1.n` et `2.dow` dans la formule avec les nombres correspondants. Pour le deuxième mercredi du mois en cours, vous utiliserez les valeurs suivantes :

* `1.n` = `2`
* `1.dow` = `3`
* `1.date` = `now`

![](assets/nth-day-variable-value-350x33.png)

#### Explication :

* `setDate(now;1)` renvoie le premier du mois en cours
* `formatDate(....;E)` renvoie jour de la semaine (1, 2, ... 6)

### Calculer les jours entre les dates

Une possibilité consiste à utiliser l’expression suivante :

![](assets/calculate-days-between-dates-350x68.png)

```
{{round((2.value - 1.value) / 1000 / 60 / 60 / 24)}}
```

>[!NOTE]
>
>* Les valeurs de `D1` et `D2` doivent être des valeurs de type Date. S’il s’agit de valeurs de type Chaîne (par exemple, 20.10.2018), utilisez la fonction `parseDate()` pour les convertir en valeurs de type Date.
>
>* La fonction `round()` est utilisée dans les cas où l’une des dates tombe dans la période d’heure d’été et pas l’autre. Dans ce cas, la différence en heures est d’une heure de moins ou de plus. Vous pouvez la diviser par 24 pour un résultat non entier. Vous perdez une heure d’heure d’été. L’arrondi l’aplanit de sorte que vous n’ayez pas de pourcentage.

#### Calculer le dernier jour ou la dernière milliseconde du mois

Lorsque vous indiquez une pédiode, par exemple dans un module de recherche, si la période s’étend sur tout le mois précédent sous la forme d’un intervalle fermé (l’intervalle qui inclut les deux points limites), vous devez calculer le dernier jour du mois.

2019-09-01 ≤ D ≤ 2019-09-30

La formule ci-dessous présente une méthode de calcul du dernier jour du mois précédent :

![](assets/last-day-prev-month.png)

```
{{addDays(setDate(now; 1); -1)}}
```

Dans certains cas, vous devez calculer non seulement le dernier jour du mois, mais littéralement sa dernière milliseconde :

2019-09-01T00:00:00.000Z ≤ D ≤ 2019-09-30T23:59:59,999Z

Cette formule présente un moyen de calculer la dernière milliseconde du mois précédent :

![](assets/last-millisecond-prev-month-350x45.png)

```
{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD"; "UTC") - 1; "x")}}
```

Si vous avez besoin que le résultat utilise votre paramètre de fuseau horaire, omettez l’argument UTC :

![](assets/omit-utc-argument-350x45.png)

`{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD") - 1; "x")}}`

Cependant, il est préférable d’utiliser l’intervalle à demi-ouverture à la place (l’intervalle qui exclut l’un de ses points limites), en précisant plutôt le premier jour du mois suivant et en remplaçant l’opérateur « inférieur ou égal » à par « inférieur à » comme suit :

`2019-09-01 ≤ D < 2019-10-01`

`2019-09-01T00:00:00.000Z ≤ D < 2019-10-01T00:00:00.000Z`
