---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Power BI
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 30e9b175e29acaed638f005eb6a701777f65e0bc
workflow-type: tm+mt
source-wordcount: '2352'
ht-degree: 0%

---

# [!DNL Power BI] Modules

[!DNL Power BI] est une application qui vous permet de visualiser et de présenter des données aux parties prenantes. Il peut prendre des données provenant de diverses sources.

>[!NOTE]
>
>[!DNL Workfront Fusion] n’est pas une source de données. while [!DNL Workfront Fusion] peut créer et utiliser des sources de données, mais ne stocke pas vos données.


## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL Fusion Workfront pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

&#42;&#42;Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI] modules et leurs champs

Lorsque vous configurez [!DNL Power BI], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de cela, des champs supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Tableaux de bord

#### [!UICONTROL Tableaux de bord de liste]

Ce module de recherche récupère une liste de tableaux de bord.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>
        <p>Sélectionnez ou mappez l'identifiant du groupe propriétaire des tableaux de bord que vous souhaitez répertorier.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Mosaïques du tableau de bord de liste]

Ce module de recherche récupère une liste de mosaïques de tableau de bord.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Saisissez un ID de tableau de bord]</td>
    <td>
      <p>Sélectionnez ou mappez l’option pour choisir le tableau de bord dont vous souhaitez répertorier les mosaïques.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID du tableau de bord]</td>
    <td>
      <p>Saisissez ou mappez l’identifiant du tableau de bord qui contient les mosaïques que vous souhaitez répertorier.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ID de groupe]  </td>
    <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire des tableaux de bord contenant les mosaïques que vous souhaitez répertorier.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limite]  </td>
    <td>
      <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Obtention d’un tableau de bord]

Ce module d’action récupère les métadonnées d’un tableau de bord spécifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Saisissez un ID de tableau de bord]</td>
      <td>
        <p>Sélectionnez ou mappez l’option pour choisir le tableau de bord pour lequel vous souhaitez récupérer les métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID du tableau de bord]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du tableau de bord pour lequel vous souhaitez récupérer des métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire des tableaux de bord pour lesquels vous souhaitez récupérer les métadonnées.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtention d’une mosaïque de tableau de bord]

Ce module d’action récupère les métadonnées d’une mosaïque de tableau de bord spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Saisissez un ID de tableau de bord]</td>
      <td>
        <p>Sélectionnez ou mappez l’option pour choisir les détails du tableau de bord que vous souhaitez récupérer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID du tableau de bord]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du tableau de bord pour lequel vous souhaitez récupérer les détails.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de mosaïque]</td>
      <td>Saisissez ou mappez l’identifiant de la variable [!DNL Power BI] pour laquelle vous souhaitez récupérer les détails.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire de la mosaïque que vous souhaitez récupérer.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Création d’un tableau de bord]

Ce module d’action crée un tableau de bord.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Saisissez ou mappez un nom pour le tableau de bord.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe qui sera propriétaire du nouveau tableau de bord.</td>
    </tr>
  </tbody>
</table>

### Rapports

#### [!UICONTROL Rapports de liste]

Ce module de recherche récupère une liste de rapports.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>
        <p>Sélectionnez ou mappez l’identifiant du groupe propriétaire des rapports que vous souhaitez répertorier.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtention d’un rapport]

Ce module d’action récupère les métadonnées d’un rapport spécifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Entrez un identifiant de rapport]</td>
      <td>
        <p>Sélectionnez ou mappez l’option pour choisir le rapport pour lequel vous souhaitez récupérer les métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de rapport]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du rapport pour lequel vous souhaitez récupérer des métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du rapport pour lequel vous souhaitez récupérer les métadonnées.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Copier un rapport]

Ce module d’action copie un rapport existant.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Entrez un identifiant de rapport]</td>
      <td>
        <p>Sélectionnez ou mappez l’option pour choisir le rapport à copier.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de rapport]</td>
      <td>
        <p>Saisissez ou mappez l'identifiant du rapport à copier.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du rapport que vous souhaitez copier.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nouveau nom du rapport copié]</td>
      <td>Saisissez ou mappez un nom pour le nouveau rapport.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Suppression d’un rapport]

Ce module d’action supprime un rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Entrez un identifiant de rapport]</td>
      <td>
        <p>Sélectionnez ou mappez l’option pour choisir le rapport à supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de rapport]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du rapport à supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du rapport que vous souhaitez supprimer.</td>
    </tr>
  </tbody>
</table>

### Jeu de données

#### [!UICONTROL Jeux de données de liste]

Ce module de recherche récupère une liste de jeux de données.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du rapport pour lequel vous souhaitez récupérer les métadonnées.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]</td>
      <td>
        <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit [agir] au cours de chaque cycle d’exécution de scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtention d’un jeu de données]

Ce module d’action récupère les métadonnées d’un jeu de données spécifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Entrez un identifiant de rapport]</td>
      <td>
        <p>Sélectionnez ou mappez l’option pour choisir le rapport pour lequel vous souhaitez récupérer les métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de rapport]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du jeu de données pour lequel vous souhaitez récupérer des métadonnées.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du jeu de données pour lequel vous souhaitez récupérer les métadonnées.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Création d’un jeu de données]

Ce module d’action crée un jeu de données.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Saisissez ou mappez un nom pour le jeu de données.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe qui sera propriétaire du nouveau jeu de données.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Mode par défaut]</td>
      <td>
        <p>Sélectionnez ou mappez le mode par défaut du jeu de données :</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>: Un jeu de données avec une connexion en direct à [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL Comme sur Prem]</b>: Un jeu de données avec une connexion en direct à [!DNL On-premise Analysis] Service</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: Jeu de données qui permet un accès programmatique pour transférer des données dans [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: Un jeu de données qui prend en charge la diffusion de données en continu et permet un accès programmé pour transférer des données dans [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: Un jeu de données prenant en charge la diffusion de données en continu</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tableaux]</td>
      <td>Ajoutez des tableaux au jeu de données. Pour les champs, voir <a href="#Table" class="MCXref_0">Champs de tableau</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>Ajoutez les sources de données. Pour les champs, voir <a href="#Data" class="MCXref_0">Champs de sources de données</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>Sélectionnez ou mappez la stratégie intentionnelle pour le jeu de données :</p>
        <ul>
          <li>
            <p>[!UICONTROL Aucun]</p>
          </li>
          <li>
            <p>[!UICONTROL Basic FIFO]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Champs de tableau

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
      <td role="rowheader">[!UICONTROL Colonnes]</td>
      <td>
        <p>Ajoutez les colonnes :</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Saisissez (map) un nom de colonne.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Data Type]</b>
            </p>
            <p>Sélectionnez ou mappez le type de données :</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Booléen]</p>
              </li>
              <li>
                <p>[!UICONTROL Date Time]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Format String]</b>
            </p>
            <p>Saisissez (map) la chaîne de format.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>Renseignez ou mappez les détails des lignes.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Mesures]</td>
      <td>Ajoutez la mesure pour les tableaux.</td>
    </tr>
  </tbody>
</table>

##### Champs de sources de données

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Base de données]  </td>
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
        <p>Saisissez ou mappez l’URL à utiliser.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de source de données]</td>
      <td>
        <p>  Saisissez ou mappez l’identifiant de la source de données.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type de source de données]  </td>
      <td>
        <p>Sélectionnez ou mappez le type de source de données. Exemple : SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de passerelle]  </td>
      <td>Saisissez ou mappez l’identifiant de la passerelle que vous souhaitez utiliser.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Ajout ou suppression de lignes dans un tableau de jeu de données]

Ce module d’action ajoute ou supprime des lignes d’une table de jeux de données push spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Entrer un tableau]</td>
      <td>Sélectionnez ou mappez l’option pour sélectionner le jeu de données contenant le tableau que vous souhaitez ajuster.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de jeu de données]</td>
      <td>Saisissez ou mappez l’identifiant du jeu de données contenant les lignes à ajouter ou à supprimer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nom de la table]  </td>
      <td>
        <p>Saisissez ou mappez le nom du tableau contenant les lignes à ajouter ou supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Saisissez ou mappez l’identifiant du groupe propriétaire du jeu de données.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sélectionner l’action]</td>
      <td>
        <p>Sélectionnez ou mappez l’action que vous souhaitez effectuer.</p>
        <ul>
          <li>
            <p>[!UICONTROL Ajouter des lignes]</p>
          </li>
          <li>
            <p>[!UICONTROL Supprimer toutes les lignes]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>
        <p>Ajoutez les champs de ligne.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Key]</b>
            </p>
            <p>Saisissez ou mappez le nom de la clé.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Field Type]</b>
            </p>
            <p>Sélectionnez ou mappez le type de champ :</p>
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
            <p>Saisissez ou mappez la valeur de clé.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Actualisation d’un jeu de données]

Ce module d’action actualise un jeu de données spécifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Saisie d’un jeu de données]</td>
      <td>Sélectionnez ou mappez l’option pour sélectionner le jeu de données à actualiser.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de jeu de données]</td>
      <td>Saisissez ou mappez l’identifiant du jeu de données que vous souhaitez actualiser.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Nom de la table]  </td>
      <td>
        <p>Saisissez ou mappez le nom du tableau contenant les lignes à ajouter ou supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Saisissez ou mappez l’identifiant du groupe propriétaire du jeu de données.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Option de notification]  </td>
      <td>
        <p>Sélectionnez ou mappez l’option à avertir :</p>
        <ul>
          <li>
            <p>[!UICONTROL Courrier à la fin]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail on Failure]</p>
          </li>
          <li>
            <p>[!UICONTROL Aucune notification]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Suppression d’un jeu de données]

Ce module d’action supprime un jeu de données.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Entrez un identifiant de rapport]</td>
      <td>
        <p>Sélectionnez ou mappez l’option pour choisir le jeu de données à supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de rapport]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du jeu de données à supprimer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de groupe]  </td>
      <td>Sélectionnez ou mappez l’identifiant du groupe propriétaire du jeu de données que vous souhaitez supprimer.</td>
    </tr>
  </tbody>
</table>

### Applications

#### [!UICONTROL Watch Apps]

Ce module de déclenchement lance un scénario lorsqu’une application est mise à jour.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Lister des applications]

Ce module de recherche récupère une liste de toutes les applications installées.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Liste des rapports de l’application]

Ce module de recherche récupère une liste de tous les rapports de l’application spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’application]</td>
      <td>Sélectionnez ou mappez l’identifiant de l’application à partir de laquelle vous souhaitez répertorier les rapports.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Liste des tableaux de bord de l’application]

Ce module de recherche récupère une liste de tableaux de bord à partir d’une application spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’application]</td>
      <td>Sélectionnez ou mappez l’identifiant de l’application à partir de laquelle vous souhaitez répertorier les tableaux de bord.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limite]  </td>
      <td>
        <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtention d’une application]

Ce module d’action récupère les métadonnées d’une application spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’application]  </td>
      <td>
        <p>Sélectionnez ou mappez l’identifiant de l’application que vous souhaitez récupérer.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtention du rapport d’une application]

Ce module d’action récupère les métadonnées du rapport d’une application spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’application]  </td>
      <td>
        <p>Sélectionnez ou mappez l’identifiant de l’application qui contient le rapport que vous souhaitez récupérer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de rapport]</td>
      <td>
        <p>  Sélectionnez ou mappez l’identifiant du rapport que vous souhaitez récupérer.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Obtention du tableau de bord d’une application]

Ce module d’action récupère les métadonnées du tableau de bord d’une application spécifiée.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’application]  </td>
      <td>
        <p>Sélectionnez ou mappez l’identifiant de l’application qui contient le tableau de bord que vous souhaitez récupérer.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de rapport]</td>
      <td>
        <p>  Sélectionnez ou mappez l’identifiant du tableau de bord que vous souhaitez récupérer.</p>
      </td>
    </tr>
  </tbody>
</table>

### Autre

#### [!UICONTROL Lancer un appel API]

Ce module d’action effectue un appel API à la fonction [!DNL Power BI] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Power BI] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Saisissez un chemin relatif à <code>https://api.powerbi.com</code>. Exemple: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>Méthode [!UICONTROL]</p>
      </td>
      <td>
        <p>Sélectionnez la méthode de requête [!UICONTROL HTTP] dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir Méthodes de requête [!UICONTROL HTTP] .</p>
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
        <p>Saisissez la chaîne de requête de requête de requête.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
