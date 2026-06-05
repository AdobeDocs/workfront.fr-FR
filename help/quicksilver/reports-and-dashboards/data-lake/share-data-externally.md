---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Établir une connexion à Workfront Data Connect
description: Workfront Data Connect vous permet d’utiliser les données Workfront de votre organisation avec des outils de Business Intelligence ou de les stocker dans un entrepôt de données externe.
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/pPk3qt9-o3QhAajyI4eGhwe0J2tRphXDstrJxmdW8Ww
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1489
ht-degree: 4%

---

# Établir une connexion à Workfront Data Connect

Workfront Data Connect vous permet d’utiliser les données Workfront de votre organisation avec des outils de Business Intelligence ou de les stocker dans un entrepôt de données externe.

Pour connecter votre lac de données Data Connect à un produit externe, vous devez d’abord créer une connexion comme décrit dans la section [Création d’un compte de lecteur ou d’une connexion pour Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Vous devez ensuite ajouter les adresses IP requises à la place sur la liste autorisée de données, comme décrit dans la section [Ajouter des adresses IP à la liste autorisée ](#add-ips-to-the-allowlist) ci-dessous.

La plupart des produits nécessitent les informations suivantes sur votre lac de données pour établir une connexion :

| Nom du champ | Valeur |
|---------------|-------------|
| Serveur | URL de la connexion, sans la partie `https://` (sur la page **Data Connect** dans Workfront*) |
| Port | `443` |
| Base de données | `WORKFRONT` |
| Entrepôt de données | `READER_WH` |
| Schéma | `WF` |
| Rôle | `READER_ROLE` |
| Nom d’utilisateur ou d’utilisatrice | Nom d’utilisateur choisi lors de la création de la connexion (sur la page **Data Connect** de Workfront*) |
| Mot de passe | Mot de passe choisi lors de la première connexion à Snowflake* |

*Pour plus d’informations sur l’emplacement de la page **Data Connect** contenant vos connexions, voir [Création d’un compte de lecteur ou d’une connexion pour Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Une fois qu’une entrée est ajoutée à la place sur la liste autorisée IP, toutes les autres adresses IP ne sont plus autorisées. Assurez-vous d’avoir saisi toutes les adresses IP requises (pour les expériences de création et de lecture de votre outil de visualisation) avant d’essayer d’utiliser l’outil. Si ce n’est pas le cas, vous pouvez rencontrer une erreur concernant des informations d’identification non valides.
>
>Si aucune adresse IP n’est incluse dans votre liste autorisée, mais que vous rencontrez toujours des problèmes pour vous connecter à un outil BI, vérifiez la configuration du serveur proxy de l’outil BI.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter des adresses IP à la place sur la liste autorisée

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Connexion aux données**.

1. Cliquez sur l’onglet **Adresses IP autorisées**, puis sur le bouton **Ajouter une adresse IP à votre**.

1. Saisissez le nom de l’adresse IP dans **Description de l’adresse IP** et saisissez l’adresse IP (ou le bloc CIDR) de l’outil que vous souhaitez utiliser dans **Adresse IP**, puis cliquez sur **Ajouter une adresse IP pour Placer sur la liste autorisée**.

   ![Ajouter une adresse IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Recherche de plages d’adresses IP Azure pour Microsoft Power BI

Le trafic de Microsoft Power BI vers Data Connect ne provient pas d’une seule adresse fixe. Microsoft publie les plages d’adresses IP en tant que blocs CIDR dans un fichier JSON volumineux. Cette section explique comment trouver les blocs pour les régions que vous utilisez réellement.

### Source Microsoft officielle pour les plages d’adresses IP et les balises de service Azure

Microsoft publie la liste sur la page de téléchargement [Plages d’adresses IP et balises de service Azure - Cloud public](https://www.microsoft.com/en-us/download/details.aspx?id=56519). Téléchargez le fichier JSON actif (le nom de fichier est généralement similaire à `ServiceTags_Public_YYYYMMDD.json`). Actualisez la liste autorisée lorsque Microsoft met à jour ce fichier ou lorsque des problèmes de connectivité apparaissent après une modification de Microsoft.

>[!NOTE]
>
>Le fichier JSON est très volumineux, souvent bien au-delà de 100 000 lignes. C&#39;est ce qui est attendu. Les sections dont vous avez besoin sont petites ; vous n&#39;avez pas besoin de lire le fichier entier à la main.

### Power BI et Power Query Online

Les clients signalent parfois « Power BI » lorsque le trafic provient en fait des composants Power Query que Microsoft traite comme un service Azure distinct dans la liste des balises de service.

| Si vos utilisateurs... | Recherchez cette balise de service dans le fichier JSON |
|----------------|---------------------------------------|
| Utilisez le service Power BI, les jeux de données hébergés dans Azure ou les passerelles dans le contexte cloud | `PowerBI` (entrées globales ou régionales telles que `PowerBI.EastUS`) |
| Utilisez Power Query Online, les flux de données cloud et des expériences similaires | `PowerQueryOnline` (entrées globales ou régionales telles que `PowerQueryOnline.EastUS`) |

Si votre organisation utilise les deux expériences, ajoutez des blocs CIDR provenant des deux `PowerBI` et `PowerQueryOnline` pour les mêmes régions. Si vous n’en ajoutez qu’un seul, certains utilisateurs peuvent toujours être bloqués tandis que d’autres réussissent.

### Choisissez les balises régionales, et non l’agrégat global.

Le fichier JSON contient une seule entrée toutes les régions pour `PowerBI` (et de même pour `PowerQueryOnline`) qui agrège de nombreuses régions et peut contenir des centaines de blocs CIDR, ainsi que de nombreuses entrées régionales plus petites telles que `PowerBI.WestUS`, `PowerBI.WestUS2` et `PowerBI.WestUS3`. Chaque objet régional répertorie uniquement les préfixes de cette zone géographique, généralement des dizaines de lignes au maximum. Nous vous recommandons de ne pas ajouter l’entrée globale, sauf si vous avez une exigence documentée pour autoriser chaque région Azure. Pour la plupart des clients Data Connect, les entrées régionales sont les valeurs par défaut appropriées. Ajoutez les régions dans lesquelles vos clients et utilisateurs Power BI s’exécutent réellement, ainsi qu’une petite mémoire tampon pour la redondance (par exemple, une région secondaire de reprise après sinistre utilisée par votre société).

### Choisissez vos régions

Les noms des zones géographiques de Microsoft dans le fichier ressemblent à `EastUS`, `WestEurope`, `GermanyWestCentral`, etc. Utilisez les régions où votre capacité Power BI et les utilisateurs sont hébergés, et non celles où se trouve votre bureau, bien qu’elles soient souvent alignées.

| Scénario | Éléments à ajouter en premier |
|----------|-------------------|
| Utilisation aux États-Unis | Commencez par les régions des États-Unis que vous connaissez et que votre client utilise (exemples : `EastUS`, `EastUS2`, `WestUS`, `WestUS2`, `WestUS3`, `CentralUS`, `SouthCentralUS`). Vous n’avez pas besoin de toutes les régions des États-Unis, sauf si votre administrateur Microsoft confirme l’hébergement multi-région. |
| Utilisation dans l’Union européenne ou au Royaume-Uni | Commencez par les régions utilisées par votre client (exemples : `WestEurope`, `NorthEurope`, `FranceCentral`, `GermanyWestCentral`, `SwedenCentral`, `UKSouth`). Ajoutez-en davantage uniquement si les utilisateurs et utilisatrices couvrent d’autres régions Microsoft. |
| Utilisation en Asie-Pacifique | Ajoutez les régions confirmées par votre administrateur Power BI ou Azure (exemples : `SoutheastAsia`, `EastAsia`, `AustraliaEast`). |
| Zones géographiques multiples | Ajoutez les deux ensembles de balises régionales (par exemple, UE et US) pour chaque service (`PowerBI` et `PowerQueryOnline` si les deux sont utilisés). |
| Région inconnue | Demandez à votre administrateur Microsoft 365 ou Power BI quelles régions Azure hébergent vos ressources Power BI, ou consultez les paramètres de votre client Administrateur Power BI. Si vous devez débloquer rapidement pour les tests, ajoutez une paire de zones géographiques connue (par exemple, `EastUS` et `WestUS`) et surveillez, puis réduisez la liste une fois que vous avez confirmé. |

### Recherchez des plages d’adresses IP et ajoutez-les à la liste autorisée .

Pour collecter des plages d’adresses IP à partir de Microsoft et les ajouter à votre Workfront, procédez comme suit :

1. Ouvrez la page de téléchargement [Plages d’adresses IP et balises de service Azure - Cloud public](https://www.microsoft.com/en-us/download/details.aspx?id=56519), téléchargez le fichier JSON des balises de service et enregistrez-le localement (par exemple, `Downloads\ServiceTags_Public_YYYYMMDD.json`).

1. Ouvrez le fichier dans un éditeur qui gère correctement les fichiers JSON volumineux, tel que Visual Studio Code.

1. Utilisez la fonction Rechercher de votre éditeur (`Ctrl+F` sous Windows ou `Cmd+F` sous macOS) pour localiser les objets JSON dont le champ `"name"` est égal à une balise de service telle que `PowerBI.EastUS` ou `PowerQueryOnline.WestEurope`. Recherches utiles :

   * `"name": "PowerBI.WestUS"` — sautez vers West US Power BI.
   * `"name": "PowerQueryOnline.WestUS"` — accéder à West US Power Query Online.
   * `PowerBI.` : répertoriez toutes les balises régionales Power BI, puis affinez-les en fonction de votre nom de région.

1. Sous chaque objet correspondant, recherchez le tableau nommé `addressPrefixes`. Chaque chaîne de ce tableau est un bloc CIDR (par exemple, `20.59.79.96/27` ou un préfixe IPv6). Il s’agit des valeurs que vous ajouterez à votre Workfront placer sur la liste autorisée.

1. Ajoutez chaque CIDR à la Workfront placer sur la liste autorisée, comme décrit dans la section [Ajout d’adresses IP à la place sur la liste autorisée ](#add-ips-to-the-allowlist) dans cet article. Patientez quelques minutes pour la propagation des politiques si votre environnement met les règles en cache.

1. À partir de Power BI ou de Power Query Online, exécutez une petite requête de test sur Data Connect pour valider la connexion. En cas d’échec, capturez l’heure approximative et demandez à votre équipe réseau si les refus s’alignent sur les plages manquantes. Vérifiez à nouveau si vous avez manqué `PowerQueryOnline` lorsque seul le `PowerBI` a été ajouté, ce qui est un écart courant.

Par exemple, si votre administrateur Microsoft confirme que vos charges de travail Power BI utilisent Ouest des États-Unis, Ouest des États-Unis 2 et Ouest des États-Unis 3, et que vos utilisateurs utilisent à la fois Power BI et Power Query Online, vous devez ouvrir six objets : `PowerBI.WestUS`, `PowerBI.WestUS2`, `PowerBI.WestUS3` et le `PowerQueryOnline.<Region>` correspondant pour chacun, puis copier le `addressPrefixes` des six.

### Référence de structure JSON

D’un point de vue conceptuel, chaque bloc de balise de service se présente comme suit. Les fichiers réels contiennent davantage de métadonnées.

```json
{
  "name": "PowerBI.WestUS2",
  "id": "PowerBI.WestUS2",
  "properties": {
    "region": "westus2",
    "systemService": "PowerBI",
    "addressPrefixes": [
      "203.0.113.0/24",
      "2001:db8::/32"
    ],
    "networkFeatures": ["API", "NSG", "UDR", "FW"]
  }
}
```

Le tableau `addressPrefixes` contient les blocs CIDR que vous ajouterez à Workfront. Les autres champs concernent les scénarios de mise en réseau Azure et ne s’appliquent pas ici.

### Conserver la place sur la liste autorisée

* Microsoft modifie les plages d’adresses IP au fil du temps. Lorsque Microsoft publie un fichier JSON mis à jour, actualisez ou comparez votre liste autorisée régulièrement, en particulier après un incident de connectivité.
* Si votre environnement prend en charge IPv6 vers Snowflake et que Microsoft répertorie les préfixes IPv6, incluez-les si votre politique de sécurité autorise IPv6. Sinon, assurez la coordination avec votre équipe réseau.

## Supprimer une adresse IP de la place sur la liste autorisée

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Connexion aux données**.

1. Cliquez sur l’onglet **Adresses IP autorisées**, puis sur l’icône de corbeille ![icône de suppression](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à droite de l’adresse IP que vous souhaitez supprimer.

1. Dans la fenêtre qui s&#39;affiche, cochez la case pour confirmer, puis cliquez sur **Supprimer**.

## Partage de données avec des outils de Business Intelligence

Vous trouverez ci-dessous un certain nombre d’outils courants de Business Intelligence. Consultez leurs sites de documentation pour en savoir plus sur la connexion à votre lac de données.

* Tableau
* Power BI
* Domo
* SAP HANA

## Stocker les données dans un entrepôt de données externe

Vous trouverez ci-dessous un certain nombre d’entrepôts de données courants ; consultez leurs sites de documentation pour en savoir plus sur la connexion à votre lac de données.

* Databricks
* AWS Redshift
