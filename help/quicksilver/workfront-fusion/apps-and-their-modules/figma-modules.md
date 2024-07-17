---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules Figma
description: Avec les modules  [!DNL Adobe Workfront Fusion] Figma, vous pouvez récupérer des listes de commentaires, de fichiers, de versions de fichiers ou de projets. Vous pouvez également publier un commentaire ou lancer un appel à l’API Figma.
author: Becky
feature: Workfront Fusion
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '2312'
ht-degree: 18%

---

# [!DNL Figma] Modules

Avec les modules [!DNL Adobe Workfront Fusion] [!DNL Figma], vous pouvez récupérer des listes de commentaires, de fichiers, de versions de fichiers ou de projets. Vous pouvez également publier un commentaire ou effectuer un appel vers l’API [!DNL Figma].

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Création d’un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
      <td>
        <p>[!UICONTROL Pro] ou un forfait supérieur</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
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

## Conditions préalables

Pour utiliser des modules [!DNL Figma], vous devez disposer d’un compte [!DNL Figma].

## Modules [!DNL Figma] et leurs champs

Lorsque vous configurez des modules [!DNL Figma], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Figma] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Commentaires](#comments)

* [Projets et fichiers](#projects-and-files)

* [Composants et styles](#components-and-styles)

* [Autre](#other)


### Commentaires

* [Suppression d’un commentaire](#delete-a-comment)

* [Lister des commentaires](#list-comments)

* [Post d’un commentaire](#post-a-comment)


#### [!UICONTROL Supprimer un commentaire]

Ce module d’action supprime un seul commentaire d’un fichier.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Figma] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de fichier]</td>
      <td>Saisissez ou mappez l’identifiant du fichier à partir duquel vous souhaitez ajouter un commentaire. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>Saisissez le texte du commentaire à supprimer.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Lister des commentaires]

Ce module de recherche répertorie tous les commentaires associés à un seul fichier dans [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Figma] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de fichier]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du fichier pour lequel vous souhaitez récupérer les commentaires. </p>
        <ul>
          <li>
            <p>Si vous ne connaissez pas l’ID, cliquez sur <b>[!UICONTROL Rechercher des fichiers]</b> et saisissez ou mappez l’ID du projet auquel le fichier est associé, puis sélectionnez le fichier.</p>
          </li>
          <li>
            <p>Si vous ne connaissez pas l’ID du projet, cliquez sur <b>[!UICONTROL Rechercher des projets]</b> et saisissez ou mappez l’ID de l’équipe propriétaire du projet auquel le fichier est associé, puis sélectionnez le projet et sélectionnez le fichier.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximal de commentaires que le module doit renvoyer pour chaque cycle d’exécution de scénario.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Post a comment]

Ce module d’action publie un commentaire dans un fichier Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Figma] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL ID de fichier]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du fichier sur lequel vous souhaitez publier un commentaire. </p>
        <ul>
          <li>
            <p>Si vous ne connaissez pas l’identifiant du fichier, cliquez sur <b>[!UICONTROL Rechercher des fichiers]</b> et saisissez ou mappez l’identifiant du projet auquel le fichier est associé, puis sélectionnez le fichier.</p>
          </li>
          <li>
            <p>Si vous essayez de trouver l’identifiant du fichier et que vous ne connaissez pas l’identifiant du projet, cliquez sur <b>[!UICONTROL Rechercher des projets]</b> et saisissez ou mappez l’identifiant de l’équipe propriétaire du projet auquel le fichier est associé. Sélectionnez le projet, puis le fichier.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>Saisissez le texte du commentaire.</td>
    </tr>
  </tbody>
</table>


### Projets et fichiers

* [Obtenir un fichier ou une image](#get-a-file-or-image)

* [Historique des versions du fichier de liste](#list-file-version-history)

* [Liste des fichiers de projet](#list-project-files)

* [Liste des projets](#list-projects)


#### [!UICONTROL Obtenir un fichier ou une image]

Ce module d’action récupère un seul fichier ou une seule image à partir d’une bibliothèque Figma

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Figma] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
      <td>
        <p>Sélectionnez le type d’objet à récupérer.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL File]</b>
            </p>
            <p>Le module renvoie le document référencé par [!UICONTROL Key] en tant qu’objet JSON. La clé du fichier peut être analysée à partir de n’importe quelle URL de fichier Figma.</p>
            <p>Pour les champs, voir <a href="#Get2" class="MCXref xref" >[!UICONTROL Obtenir un fichier ou une image : Fichier]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Noeuds de fichier]</b>
            </p>
            <p>Renvoie les noeuds référencés par les identifiants sous la forme d’un objet JSON. Les noeuds sont récupérés à partir du fichier [!DNL Figma] référencé par [!UICONTROL Key].</p>
            <p>Pour les champs, voir <a href="#Get3" class="MCXref xref" >[!UICONTROL Obtenir un fichier ou une image : Noeuds de fichier]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image]</b>
            </p>
            <p>Le module effectue le rendu des images à partir d’un fichier.</p>
            <p>Pour les champs, voir <a href="#Get4" class="MCXref xref" >[!UICONTROL Obtention d’un fichier ou d’une image : Image]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Remplissage d’image]</b>
            </p>
            <p>Le module renvoie les liens de téléchargement pour toutes les images présentes dans les remplissages d’images d’un document. Les remplissages d’images représentent la manière dont [!DNL Figma] représente toutes les images fournies par l’utilisateur. Lorsque vous faites glisser une image dans [!DNL Figma], [!DNL Figma] crée un rectangle avec un seul remplissage qui représente l’image, et l’utilisateur peut transformer le rectangle (et les propriétés sur le remplissage).</p>
            <p>Pour les champs, voir <a href="#Get5" class="MCXref xref" >[!UICONTROL Obtention d’un fichier ou d’une image : remplissage d’image]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Obtenir un fichier ou une image : Fichier]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Clé du fichier]</td>
      <td>Sélectionnez le fichier à partir duquel vous souhaitez renvoyer JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de version]</td>
      <td>Saisissez ou mappez la version du fichier que le module doit renvoyer. Pour le module actif, laissez ce champ vide.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de noeud]</td>
      <td>
        <p>Pour renvoyer uniquement un sous-ensemble du document, saisissez les noeuds que vous souhaitez que le module renvoie. Le module renvoie les noeuds répertoriés, leurs enfants et tout ce qui se trouve entre le noeud racine et les noeuds répertoriés.</p>
        <p>Pour chaque noeud que vous souhaitez renvoyer, cliquez sur <b>[!UICONTROL Ajouter]</b> et saisissez le texte du noeud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Saisissez ou mappez un entier qui représente la profondeur de l’arborescence du document pour laquelle vous souhaitez renvoyer des résultats. </p>
        <div class="example"><span class="autonumber"><span><b>Exemple : </b></span></span>
          <ul>
            <li>
              <p>Pour renvoyer des pages uniquement, saisissez <code>1</code>.</p>
            </li>
            <li>
              <p>Pour renvoyer des pages et des objets de niveau supérieur, saisissez <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Pour renvoyer tous les noeuds, laissez ce champ vide.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometrie]</td>
      <td>Pour renvoyer des données vectorielles, saisissez <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Données du module externe]</td>
      <td>Liste séparée par des virgules d’identifiants de module externe et/ou chaîne "[!UICONTROL partagé]". Toutes les données présentes dans le document écrites par ces modules externes seront incluses dans le résultat des propriétés <code>pluginData</code> et <code>sharedPluginData</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Données de branche]</td>
      <td>Activez cette option pour renvoyer les métadonnées de branche pour le fichier demandé. Si le fichier est une branche, la clé du fichier principal est incluse dans la réponse renvoyée. Si le fichier comporte des branches, leurs métadonnées sont incluses dans la réponse renvoyée. Valeur par défaut : <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Obtenir un fichier ou une image : noeuds de fichier]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Clé du fichier]</td>
      <td>Sélectionnez le fichier à partir duquel vous souhaitez renvoyer JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de noeud]</td>
      <td>
        <p>Saisissez les noeuds que vous souhaitez que le module renvoie et convertisse.</p>
        <p>Pour chaque noeud que vous souhaitez renvoyer, cliquez sur <b>[!UICONTROL Ajouter]</b> et saisissez le texte du noeud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de version]</td>
      <td>Saisissez ou mappez la version du fichier que le module doit renvoyer. Pour le module actif, laissez ce champ vide.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Saisissez ou mappez un entier qui représente la profondeur de l’arborescence du document pour laquelle vous souhaitez renvoyer des résultats. </p>
        <div class="example"><span class="autonumber"><span><b>Exemple : </b></span></span>
          <ul>
            <li>
              <p>Pour renvoyer des pages uniquement, saisissez <code>1</code>.</p>
            </li>
            <li>
              <p>Pour renvoyer des pages et des objets de niveau supérieur, saisissez <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>Pour renvoyer tous les noeuds, laissez ce champ vide.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometrie]</td>
      <td>Pour renvoyer des données vectorielles, saisissez <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Données du module externe]</td>
      <td>Liste séparée par des virgules d’identifiants de module externe et/ou de la chaîne "shared". Toutes les données présentes dans le document écrites par ces modules externes seront incluses dans les propriétés pluginData et sharedPluginData.</td>
    </tr>
  </tbody>
</table>


##### Obtenir un fichier ou une image : Image

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Clé du fichier]</td>
      <td>Sélectionnez le fichier à partir duquel vous souhaitez renvoyer JSON.</td>
    </tr>
    <tr>
      <td role="rowheader" [!UICONTROL>ID de noeud]</td>
      <td>
        <p>Saisissez les noeuds dont vous souhaitez que le module soit rendu.</p>
        <p>Pour chaque noeud dont vous souhaitez effectuer le rendu, cliquez sur <b>[!UICONTROL Ajouter]</b> et saisissez le texte du noeud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Échelle]</td>
      <td>Pour mettre l’image à l’échelle, saisissez ou mappez le facteur de mise à l’échelle. Ce nombre doit être compris entre 0,01 et 4.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Format]</td>
      <td>
        <p>Sélectionnez le format de la sortie de l’image.</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Inclure l’ID]</td>
      <td>Activez cette option pour inclure les attributs d’identifiant pour tous les éléments de SVG. Valeur par défaut : [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Simplification du contour]</td>
      <td>Activez cette option pour simplifier les contours internes/externes et utilisez l’attribut de contour si possible au lieu de &lt;mask&gt;. Valeur par défaut : [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Utiliser des limites absolues]</td>
      <td>Activez cette option pour utiliser les dimensions complètes du noeud, qu’il soit recadré ou non ou que l’espace autour soit vide. Utilisez cette option pour exporter des noeuds de texte sans recadrage. Valeur par défaut : [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de version]</td>
      <td>Saisissez ou mappez la version du fichier que le module doit renvoyer. Pour le module actif, laissez ce champ vide.</td>
    </tr>
  </tbody>
</table>

##### Obtention d’un fichier ou d’une image : remplissage d’image

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Clé du fichier]</td>
      <td>Sélectionnez le fichier à partir duquel vous souhaitez renvoyer JSON.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL Historique de version du fichier de liste]

Ce module de recherche renvoie l’historique des versions d’un seul fichier dans [!UICONTROL Figma].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Figma] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL ID de fichier]</td>
      <td>
        <p>Saisissez ou mappez l’identifiant du fichier pour lequel vous souhaitez récupérer l’historique des versions. </p>
        <ul>
          <li>
            <p>Si vous ne connaissez pas l’identifiant du fichier, cliquez sur <b>[!UICONTROL Rechercher des fichiers]</b> et saisissez ou mappez l’identifiant du projet auquel le fichier est associé, puis sélectionnez le fichier.</p>
          </li>
          <li>
            <p>Si vous essayez de trouver l’identifiant du fichier et que vous ne connaissez pas l’identifiant du projet, cliquez sur <b>[!UICONTROL Rechercher des projets]</b> et saisissez ou mappez l’identifiant de l’équipe propriétaire du projet auquel le fichier est associé. Sélectionnez le projet, puis le fichier.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Liste des fichiers de projet]

Ce module de recherche renvoie une liste de tous les fichiers du projet spécifié.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Figma] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID de fichier]</td>
      <td>
        <p>Saisissez ou mappez l’ID de projet pour lequel vous souhaitez récupérer les fichiers. </p>
        <ul>
          <li>
            <p>Si vous ne connaissez pas l’identifiant du projet, cliquez sur <b>[!UICONTROL Rechercher des projets]</b> et saisissez ou mappez l’identifiant de l’équipe à laquelle le projet est associé, puis sélectionnez le projet.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Liste des projets]

Ce module de recherche renvoie une liste de tous les projets de l’équipe spécifiée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Figma] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’équipe]</td>
      <td>Saisissez ou mappez l’ID de projet pour lequel vous souhaitez récupérer les fichiers. L'identifiant de l'équipe se trouve dans l'URL de la page de l'équipe à Figma.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>


### Composants et styles

#### [!UICONTROL Obtenir un style ou un composant]

Ce module d’action récupère un seul style ou composant, ou un ensemble de styles ou de composants.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Figma] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Object&gt; key]</td>
      <td>Saisissez la clé (identifiant unique) de l’objet que vous souhaitez récupérer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ID d’équipe]</td>
      <td>Saisissez ou mappez l’identifiant de l’équipe à laquelle le ou les enregistrements sont associés.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Taille de page]</td>
      <td>Saisissez ou mappez le nombre ou les résultats à renvoyer par page. Valeur par défaut : 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Après]</td>
      <td>
        <p>Saisissez ou mappez le numéro du résultat après lequel vous souhaitez commencer à récupérer les résultats. Cela peut être combiné avec le champ [!UICONTROL Taille de page] pour paginer les résultats.</p>
        <p>Cette valeur ne correspond pas aux identifiants d’objet.</p>
        <p>Ce champ ne peut pas être utilisé conjointement avec le champ [!UICONTROL Avant] .</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Avant]</td>
      <td>
        <p>Saisissez ou mappez le numéro du résultat avant lequel vous souhaitez commencer à récupérer les résultats. Cela peut être combiné avec le champ [!UICONTROL Taille de page] pour paginer les résultats.</p>
        <p>Cette valeur ne correspond pas aux identifiants d’objet.</p>
        <p>Ce champ ne peut pas être utilisé conjointement avec le champ [!UICONTROL After] .</p>
      </td>
    </tr>
  </tbody>
</table>


### Autre

* [Effectuer un appel API](#make-an-api-call)

* [Surveiller les événements](#watch-events)


#### [!UICONTROL Effectuer un appel API]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé vers l’API Figma sans avoir à passer par l’authentification. Ainsi, vous pouvez créer une automatisation des flux de données qui ne peut pas être réalisée par les autres modules Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Figma] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Saisissez un chemin relatif à <code>https://api.figma.com/v1/</code>.</p>
        <p>Par exemple : <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Method]</td>
      <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p>
        <p>Par exemple, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p>
        <p>Par exemple : <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Surveiller les événements]

Ce module de déclenchement lance un scénario lorsque l’un des événements suivants se produit pour une équipe spécifique dans l’espace d’équipe [!DNL Figma]

* Mise à jour du fichier

* Mise à jour de version de fichier

* Suppression de fichier

* Publication de bibliothèque

* Commentaire du fichier

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>Sélectionnez le webhook que le module regarde.</p>
        <p>Pour ajouter un nouveau webhook :</p>
        <ol>
          <li value="1">
            <p>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL Webhook].</p>
          </li>
          <li value="2">
            <p>Sélectionnez la connexion que vous souhaitez utiliser pour ce webhook. Pour plus d’informations sur la connexion de votre compte [!DNL Figma] à [!UICONTROL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base.</a></p>
          </li>
          <li value="3">
            <p>Sélectionnez le type d’événement que le module doit surveiller.</p>
          </li>
          <li value="4">
            <p>Saisissez l’identifiant de l’équipe dont vous souhaitez que le webhook s’affiche.</p>
          </li>
          <li value="5">
            <p>Saisissez le [!UICONTROL Status] ou la [!UICONTROL Description] des événements que le webhook doit surveiller.</p>
          </li>
          <li value="6">
            <p>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
