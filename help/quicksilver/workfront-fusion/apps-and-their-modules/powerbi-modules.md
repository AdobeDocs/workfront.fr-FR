---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Power BI
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2493'
ht-degree: 95%

---

# Modules [!DNL Power BI]

[!DNL Power BI] est une application qui vous permet de visualiser et de présenter des données à vos parties prenantes. Elle peut utiliser des données provenant de diverses sources.

>[!NOTE]
>
>[!DNL Workfront Fusion] n’est pas une source de données. Bien que [!DNL Workfront Fusion] puisse créer et utiliser des sources de données, il ne stocke pas vos données.


## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigence des produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez l’administration [!DNL Workfront].

&#42;&#42;Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Informations sur l’API Microsoft Power BI

Le connecteur Microsoft Power BI utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td> https://api.powerbi.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Version de l’API</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.0.2</td> 
  </tr>
 </tbody> 
 </table>

## Modules [!DNL Power BI] et leurs domaines

Lorsque vous configurez [!DNL Power BI], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de cela, des champs supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Tableaux de bord](#dashboards)
* [Rapports](#reports)
* [Jeu de données](#dataset)
* [Applications](#apps)
* [Autre](#other)

### Tableaux de bord

* [Création d’un tableau de bord](#create-a-dashboard)
* [Obtention d’un tableau de bord](#get-a-dashboard)
* [Obtention d’une mosaïque de tableau de bord](#get-a-dashboard-tile)
* [Mosaïques du tableau de bord de liste](#list-dashboard-tiles)
* [Tableaux de bord de liste](#list-dashboards)

#### [!UICONTROL Créer un tableau de bord]

Ce module d’action crée un nouveau tableau de bord.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Saisissez ou mappez un nom pour le tableau de bord.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe qui sera propriétaire du nouveau tableau de bord.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtenir un tableau de bord]

Ce module d’action permet de récupérer les métadonnées d’un tableau de bord spécifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
      <td>
        <p>Sélectionnez ou mappez l’option pour choisir le tableau de bord pour lequel vous souhaitez récupérer des métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du tableau de bord pour lequel vous souhaitez récupérer des métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire des tableaux de bord dont vous souhaitez récupérer les métadonnées.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtenir une tuile de tableau de bord]

Ce module d’action récupère les métadonnées d’une tuile de tableau de bord spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
      <td>
        <p>Sélectionnez ou affichez l’option pour choisir les détails du tableau de bord que vous souhaitez récupérer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du tableau de bord dont vous souhaitez récupérer les détails.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tile ID]</td>
      <td>Saisissez ou mappez l’identifiant de la tuile [!DNL Power BI] dont vous souhaitez récupérer les détails.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire de la tuile que vous souhaitez récupérer.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Répertorier des tuiles du tableau de bord]

Ce module de recherche permet de récupérer une liste de tuiles de tableau de bord.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
    <td>
      <p>Sélectionnez ou affichez l’option pour choisir le tableau de bord dont vous voulez répertorier les tuiles.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Dashboard ID]</td>
    <td>
      <p>Saisissez ou mappez l’identifiant du tableau de bord qui contient les tuiles que vous souhaitez répertorier.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Group ID]  </td>
    <td>Sélectionnez ou mappez l’identifiant du groupe qui possède les tableaux de bord contenant les tuiles que vous souhaitez répertorier.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]  </td>
    <td>
      <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Répertorier des tableaux de bord]

Ce module de recherche permet d’obtenir une liste de tableaux de bord.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Sélectionnez ou mappez l’identifiant du groupe propriétaire des tableaux de bord que vous souhaitez répertorier.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

### Rapports

* [Copier un rapport](#copy-a-report)
* [Suppression d’un rapport](#delete-a-report)
* [Obtention d’un rapport](#get-a-report)
* [Rapports de liste](#list-reports)

#### [!UICONTROL Copier un rapport]

Ce module d’action copie un rapport existant.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Sélectionnez ou affichez l’option pour choisir le rapport que vous souhaitez copier.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du rapport que vous souhaitez copier.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du rapport que vous souhaitez copier.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL New Copied Report Name]</td>
      <td>Saisissez ou mappez un nom pour le nouveau rapport.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Supprimer un rapport]

Ce module d’action supprime un rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Sélectionnez ou affichez l’option pour choisir le rapport que vous souhaitez supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du rapport que vous souhaitez supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du rapport que vous souhaitez supprimer.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtenir un rapport]

Ce module d’action permet de récupérer les métadonnées d’un rapport spécifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Sélectionnez ou mappez l’option pour choisir le rapport pour lequel vous souhaitez récupérer des métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du rapport pour lequel vous souhaitez récupérer des métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du rapport dont vous souhaitez récupérer les métadonnées.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Répertorier des rapports]

Ce module de recherche permet d’obtenir une liste de rapports.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>Sélectionnez ou mappez l’identifiant du groupe propriétaire des rapports que vous souhaitez répertorier.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p>
      </td>
    </tr>
  </tbody>
</table>


### Jeu de données

* [Ajout/suppression de lignes dans un tableau de jeu de données](#add-or-delete-rows-in-a-dataset-table)
* [Création d’un jeu de données](#create-a-dataset)
* [Suppression d’un jeu de données](#delete-a-dataset)
* [Obtention d’un jeu de données](#get-a-dataset)
* [Jeux de données de liste](#list-datasets)
* [Actualisation d’un jeu de données](#refresh-a-dataset)

#### [!UICONTROL Ajouter ou supprimer des lignes dans un tableau de jeu de données]

Ce module d’action ajoute ou supprime des lignes d’un tableau de jeu de données push spécifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a table]</td>
      <td>Sélectionnez ou mappez l’option pour sélectionner le jeu de données qui contient le tableau que vous souhaitez ajuster.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dataset ID]</td>
      <td>Saisissez ou mappez l’identifiant du jeu de données qui contient les lignes que vous souhaitez ajouter ou supprimer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Saisissez ou mappez le nom du tableau qui contient les lignes que vous souhaitez ajouter ou supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Saisissez ou mappez l’identifiant du groupe propriétaire du jeu de données.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Select the Action]</td>
      <td>
        <p>Sélectionnez ou mappez l’action que vous souhaitez effectuer.</p>
        <ul>
          <li>
            <p>[!UICONTROL Add rows]</p>
          </li>
          <li>
            <p>[!UICONTROL Delete All Rows]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>
        <p>Ajoutez les champs de la ligne.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Key]</b>
            </p>
            <p>Saisissez ou mappez le nom de la clé.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Field Type]</b>
            </p>
            <p>Sélectionnez ou mappez le type de champ :</p>
            <ul>
              <li>
                <p>Booléen</p>
              </li>
              <li>
                <p>Date</p>
              </li>
              <li>
                <p>Texte</p>
              </li>
              <li>
                <p>Nombre</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[!UICONTROL Value]</p>
            <p>Saisissez ou mappez la valeur de la clé.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Créér un jeu de données]

Ce module d’action crée un nouveau jeu de données.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Saisissez ou mappez un nom pour le jeu de données.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe qui sera propriétaire du nouveau jeu de données.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default Mode]</td>
      <td>
        <p>Sélectionnez ou mappez le mode par défaut pour le jeu de données :</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b> : jeu de données avec une connexion en direct à [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As on Prem]</b> : jeu de données avec une connexion en direct au service [!DNL On-premise Analysis].</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: jeu de données qui permet un accès programmatique pour l’introduction de données dans le système de gestion des données. [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: jeu de données qui prend en charge la diffusion de données en continu et permet un accès programmatique pour l’introduction de données dans le système. [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: jeu de données qui prend en charge la diffusion de données en continu.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tables]</td>
      <td>Ajoutez des tableaux au jeu de données. Pour les champs, voir <a href="#Table" class="MCXref_0">Champs de tableau</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>Ajoutez les sources de données. Pour les champs, voir <a href="#Data" class="MCXref_0">Champs des sources de données</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>Sélectionnez ou mappez la politique intentionnelle pour le jeu de données :</p>
        <ul>
          <li>
            <p>[!UICONTROL None]</p>
          </li>
          <li>
            <p>[!UICONTROL Basic FIFO]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Champs du tableau

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>  Saisissez ou mappez un nom pour le tableau.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Columns]</td>
      <td>
        <p>Ajoutez les colonnes :</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Saisissez (mappez) un nom de colonne.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Data Type]</b>
            </p>
            <p>Sélectionnez ou mappez le type de données :</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL Date Time]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Format String]</b>
            </p>
            <p>Saisissez (mappez) la chaîne de format.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>Saisissez ou mappez les détails des lignes.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Measures]</td>
      <td>Ajoutez la mesure pour les tableaux.</td>
    </tr>
  </tbody>
</table>

##### Champs des sources de données

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Database]  </td>
      <td>
        <p>Saisissez ou mappez la base de données que vous souhaitez utiliser.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Server]  </td>
      <td>
        <p>Saisissez ou mappez le nom du serveur que vous souhaitez utiliser.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>Saisissez ou mappez l’URL que vous souhaitez utiliser.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data source ID]</td>
      <td>
        <p>  Saisissez ou mappez l’identifiant de la source de données.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data source Type]  </td>
      <td>
        <p>Sélectionnez ou mappez le type de source de données. Exemple : SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gateway ID]  </td>
      <td>Saisissez ou mappez l’identifiant de la passerelle que vous souhaitez utiliser.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Supprimer un jeu de données]

Ce module d’action supprime un jeu de données.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Sélectionnez ou affichez l’option pour choisir le jeu de données que vous souhaitez supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du jeu de données que vous souhaitez supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du jeu de données que vous souhaitez supprimer.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtenir un jeu de données]

Ce module d’action permet de récupérer les métadonnées d’un jeu de données spécifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>Sélectionnez ou mappez l’option pour choisir le rapport pour lequel vous souhaitez récupérer des métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du jeu de données pour lequel vous souhaitez récupérer des métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du jeu de données pour lequel vous souhaitez récupérer des métadonnées.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Répertorier des jeux de données]

Ce module de recherche permet d’obtenir une liste de jeux de données.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du rapport dont vous souhaitez récupérer les métadonnées.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit [action] au cours de chaque cycle d’exécution du scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Actualiser un jeu de données]

Ce module d’action actualise un jeu de données spécifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a dataset]</td>
      <td>Sélectionnez ou mappez l’option pour sélectionner le jeu de données que vous souhaitez actualiser.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dataset ID]</td>
      <td>Saisissez ou mappez l’identifiant du jeu de données que vous souhaitez actualiser.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>Saisissez ou mappez le nom du tableau qui contient les lignes que vous souhaitez ajouter ou supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>Saisissez ou mappez l’identifiant du groupe propriétaire du jeu de données.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Notify Option]  </td>
      <td>
        <p>Sélectionnez ou mappez l’option à notifier :</p>
        <ul>
          <li>
            <p>[!UICONTROL Mail on Completion]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail on Failure]</p>
          </li>
          <li>
            <p>[!UICONTROL No Notification]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Applications

* [Obtention d’une application](#get-an-app)
* [Obtention du tableau de bord d’une application](#get-an-apps-dashboard)
* [Obtention du rapport d’une application](#get-an-apps-report)
* [Liste des tableaux de bord de l’application](#list-apps-dashboards)
* [Liste des rapports de l’application](#list-apps-reports)
* [Lister des applications](#list-apps)
* [Watch Apps](#watch-apps)

#### [!UICONTROL Obtenir une application]

Ce module d’action permet de récupérer les métadonnées d’une application spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Sélectionnez ou mappez l’identifiant de l’application que vous souhaitez récupérer.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtenir le tableau de bord d’une application]

Ce module d’action récupère les métadonnées du tableau de bord d’une application spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Sélectionnez ou mappez l’ID de l’application qui contient le tableau de bord que vous souhaitez récupérer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  Sélectionnez ou mappez l’ID du tableau de bord que vous souhaitez récupérer.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtenir le rapport d’une application]

Ce module d’action permet de récupérer les métadonnées du rapport d’une application donnée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Sélectionnez ou mappez l’identifiant de l’application qui contient le rapport que vous souhaitez récupérer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  Sélectionnez ou mappez l’identifiant du rapport que vous souhaitez récupérer.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Répertorier les applications]

Ce module de recherche permet d’obtenir une liste de toutes les applications installées.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Répertorier les tableaux de bord d’une application]

Ce module de recherche permet d’obtenir une liste de tableaux de bord à partir d’une application donnée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Sélectionnez ou mappez l’identifiant de l’application à partir de laquelle vous souhaitez répertorier les tableaux de bord.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Répertorier les rapports d’une application]

Ce module de recherche permet d’obtenir une liste de tous les rapports de l’application spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Sélectionnez ou mappez l’identifiant de l’application à partir de laquelle vous souhaitez répertorier les rapports.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Surveiller des applications]

Ce module déclencheur lance un scénario lorsqu’une application est mise à jour.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Power BI] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

### Autre

#### [!UICONTROL Effectuer un appel API]

Ce module d’action effectue un appel API à l’API [!DNL Power BI].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour savoir comment connecter votre compte [!DNL Power BI] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Saisissez un chemin d’accès relatif à <code>https://api.powerbi.com</code>. Exemple : <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
        <p>Sélectionnez la méthode de requête [!UICONTROL HTTP] dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, consultez les méthodes de requête [!UICONTROL HTTP].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p>
        <p>Par exemple, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] ajoute automatiquement des en-têtes d’autorisation et des en-têtes x-api-key.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Saisissez la chaîne de requête.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
