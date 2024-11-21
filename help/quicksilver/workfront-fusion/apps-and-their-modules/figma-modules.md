---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules Figma
description: Avec les modules Figma  [!DNL Adobe Workfront Fusion] , vous pouvez récupérer des listes de commentaires, de fichiers, de versions de fichiers ou de projets. Vous pouvez également publier un commentaire ou faire un appel à l’API Figma.
author: Becky
feature: Workfront Fusion
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2331'
ht-degree: 98%

---

# Modules [!DNL Figma]

Avec les modules [!DNL Figma] [!DNL Adobe Workfront Fusion], vous pouvez récupérer des listes de commentaires, de fichiers, de versions de fichiers ou de projets. Vous pouvez également publier un commentaire ou faire un appel à l’API [!DNL Figma].

Si vous avez besoin d’instructions sur la création d’un scénario, consultez la section [Créer un scénario](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
      <td>
        <p>[!UICONTROL Pro] ou version supérieure</p>
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
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td>
    </tr>
  </tbody>
</table>


Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL Figma], vous devez disposer d’un compte [!DNL Figma].

## Informations sur l’API Figma

Le connecteur Figma utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td> https://api.figma.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Version de l’API</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v1.8.25</td> 
  </tr>
 </tbody> 
 </table>

## Modules [!DNL Figma] et leurs champs

Lorsque vous configurez les modules [!DNL Figma], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Figma] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Commentaires](#comments)

* [Projets et fichiers](#projects-and-files)

* [Composants et styles](#components-and-styles)

* [Autre](#other)


### Commentaires

* [Supprimer un commentaire](#delete-a-comment)

* [Répertorier les commentaires](#list-comments)

* [Publier un commentaire](#post-a-comment)


#### [!UICONTROL Supprimer un commentaire]

Ce module d’action supprime un seul commentaire d’un fichier.

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour savoir comment connecter votre compte [!DNL Figma] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Se connecter à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>Saisissez ou mappez l’ID du fichier auquel vous souhaitez ajouter ou supprimer un commentaire. </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Comment]</td>
      <td>Saisissez le texte du commentaire que vous souhaitez supprimer.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Répertorier les commentaires]

Ce module de recherche répertorie tous les commentaires attachés à un seul fichier dans [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour savoir comment connecter votre compte [!DNL Figma] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Se connecter à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Saisissez ou mappez l’ID du fichier dont vous voulez récupérer les commentaires. </p>
        <ul>
          <li>
            <p>Si vous ne connaissez pas l’ID, cliquez sur <b>[!UICONTROL Find Files]</b> et saisissez ou mappez l’ID du projet auquel le fichier est associé, puis sélectionnez le fichier.</p>
          </li>
          <li>
            <p>Si vous ne connaissez pas l’ID du projet, cliquez sur <b>[!UICONTROL Find Projects]</b> et saisissez ou mappez l’ID de l’équipe qui possède le projet auquel le fichier est associé, puis sélectionnez le projet et enfin le fichier.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximum de commentaires que vous souhaitez que le module renvoie lors de chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Publier un commentaire]

Ce module d’action publie un commentaire dans un fichier Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour savoir comment connecter votre compte [!DNL Figma] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Se connecter à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Saisissez ou mappez l’ID du fichier sur lequel vous souhaitez publier un commentaire. </p>
        <ul>
          <li>
            <p>Si vous ne connaissez pas l’ID du fichier, cliquez sur <b>[!UICONTROL Find Files]</b> et saisissez ou mappez l’ID du projet auquel le fichier est associé, puis sélectionnez le fichier.</p>
          </li>
          <li>
            <p>Si vous essayez de trouver l’ID du fichier et que vous ne connaissez pas l’ID du projet, cliquez sur <b>[!UICONTROL Find Projects]</b> et saisissez ou mappez l’ID de l’équipe qui possède le projet auquel le fichier est associé. Sélectionnez le projet, puis le fichier.</p>
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

* [Répertorier l’historique des versions des fichiers](#list-file-version-history)

* [Répertorier les fichiers du projet](#list-project-files)

* [Répertorier les projets](#list-projects)


#### [!UICONTROL Obtenir un fichier ou une image]

Ce module d’action permet de récupérer un seul fichier ou une seule image dans une bibliothèque Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour savoir comment connecter votre compte [!DNL Figma] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Se connecter à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
      <td>
        <p>Sélectionnez le type d’objet que vous souhaitez récupérer.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL File]</b>
            </p>
            <p>Le module renvoie le document auquel se réfère la [!UICONTROL Key] sous la forme d’un objet JSON. La clé de fichier peut être analysée à partir de n’importe quelle URL de fichier Figma.</p>
            <p>Pour les champs, consultez <a href="#Get2" class="MCXref xref" >[!UICONTROL Get a file or image: File]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL File nodes]</b>
            </p>
            <p>Renvoie les nœuds référencés par les ID sous la forme d’un objet JSON. Les nœuds sont extraits du fichier [!DNL Figma] auquel renvoie la [!UICONTROL Key].</p>
            <p>Pour les champs, consultez <a href="#Get3" class="MCXref xref" >[!UICONTROL Get a file or image: File nodes]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image]</b>
            </p>
            <p>Le module rend les images à partir d’un fichier.</p>
            <p>Pour les champs, consultez <a href="#Get4" class="MCXref xref" >[!UICONTROL Get a file or image: Image]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Image fills]</b>
            </p>
            <p>Le module renvoie les liens de téléchargement pour toutes les images présentes dans les champs d’images d’un document. Les remplissages d’images sont la façon dont [!DNL Figma] représente les images fournies par l’utilisateur ou l’utilisatrice. Lorsque vous faites glisser une image dans [!DNL Figma], [!DNL Figma] crée un rectangle avec un remplissage unique qui représente l’image, et l’utilisateur ou l’utilisatrice peut transformer le rectangle (et les propriétés du remplissage).</p>
            <p>Pour les champs, consultez <a href="#Get5" class="MCXref xref" >[!UICONTROL Get a file or image: Image fills]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Obtenir un fichier ou une image : fichier]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Sélectionnez le fichier à partir duquel vous souhaitez renvoyer du JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Saisissez ou mappez la version du fichier que vous souhaitez que le module renvoie. Pour le module actuel, laissez ce champ vide.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Pour ne renvoyer qu’un sous-ensemble du document, saisissez les nœuds que vous souhaitez que le module renvoie. Le module renvoie les nœuds répertoriés, leurs tâches enfant et tout ce qui se trouve entre le nœud racine et les nœuds répertorés.</p>
        <p>Pour chaque nœud que vous souhaitez renvoyer, cliquez sur <b>[!UICONTROL Add]</b> et saisissez le texte du nœud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Saisissez ou mappez un nombre entier représentant la profondeur de l’arborescence du document pour laquelle vous souhaitez obtenir des résultats. </p>
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
        <p>Pour renvoyer tous les nœuds, laissez ce champ vide.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Pour renvoyer des données vectorielles, saisissez <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>Liste d’ID de plug-ins séparés par des virgules et/ou la chaîne de caractères « [!UICONTROL shared] ». Toute donnée présente dans le document écrit par ces plug-ins sera incluse dans le résultat dans les propriétés <code>pluginData</code> et <code>sharedPluginData</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Branch data]</td>
      <td>Activez cette option pour renvoyer les métadonnées de la branche pour le fichier demandé. Si le fichier est une branche, la clé du fichier principal est incluse dans la réponse renvoyée. Si le fichier comporte des branches, leurs métadonnées sont incluses dans la réponse renvoyée. Par défaut : <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Obtenir un fichier ou une image : nœuds de fichiers]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Sélectionnez le fichier à partir duquel vous souhaitez renvoyer du JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Saisir les nœuds que vous souhaitez que le module renvoie et convertisse.</p>
        <p>Pour chaque nœud que vous souhaitez renvoyer, cliquez sur <b>[!UICONTROL Add]</b> et saisissez le texte du nœud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Saisissez ou mappez la version du fichier que vous souhaitez que le module renvoie. Pour le module actuel, laissez ce champ vide.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Depth]</td>
      <td>
        <p>Saisissez ou mappez un nombre entier représentant la profondeur de l’arborescence du document pour laquelle vous souhaitez obtenir des résultats. </p>
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
        <p>Pour renvoyer tous les nœuds, laissez ce champ vide.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Geometry]</td>
      <td>Pour renvoyer des données vectorielles, saisissez <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Plugin data]</td>
      <td>Liste d’ID de plug-ins séparés par des virgules et/ou la chaîne de caractères « shared ». Toute donnée présente dans le document écrit par ces plug-ins sera incluse dans le résultat dans les propriétés pluginData et sharedPluginData.</td>
    </tr>
  </tbody>
</table>


##### Obtenir un fichier ou une image : image

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Sélectionnez le fichier à partir duquel vous souhaitez renvoyer du JSON.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Node IDs]</td>
      <td>
        <p>Saisissez les nœuds que vous souhaitez que le module renvoie.</p>
        <p>Pour chaque nœud que vous souhaitez voir renvoyé, cliquez sur <b>[!UICONTROL Add]</b> et saisissez le texte du nœud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Scale]</td>
      <td>Pour mettre l’image à l’échelle, saisissez ou mappez le facteur d’échelle. Ce nombre doit être compris entre 0,01 et 4.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Format]</td>
      <td>
        <p>Sélectionnez le format de l’image en sortie.</p>
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
      <td role="rowheader">[!UICONTROL SVG - Include ID]</td>
      <td>Activez cette option pour inclure des attributs d’identification pour tous les éléments SVG. Valeur par défaut : [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SVG - Simplify Stroke]</td>
      <td>Activez cette option pour simplifier les traits intérieurs/extérieurs et utilisez l’attribut stroke si possible au lieu de &lt;mask&gt;. Valeur par défaut : [!UICONTROL true].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Use absolute bounds]</td>
      <td>Activez cette option pour utiliser les dimensions intégrales du nœud, qu’il soit ou non recadré ou que l’espace autour de lui soit vide. Cette option permet d’exporter des nœuds de texte sans recadrage. Valeur par défaut : [!UICONTROL false].</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Version ID]</td>
      <td>Saisissez ou mappez la version du fichier que vous souhaitez que le module renvoie. Pour le module actuel, laissez ce champ vide.</td>
    </tr>
  </tbody>
</table>

##### Obtenir un fichier ou une image : remplissages de l’image

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL File key]</td>
      <td>Sélectionnez le fichier à partir duquel vous souhaitez renvoyer du JSON.</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL Répertorier l’historique des versions des fichiers]

Ce module de recherche renvoie l’historique des versions d’un seul fichier dans [!UICONTROL Figma].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour savoir comment connecter votre compte [!DNL Figma] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Se connecter à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Saisissez ou mappez l’ID du fichier dont vous souhaitez récupérer l’historique des versions. </p>
        <ul>
          <li>
            <p>Si vous ne connaissez pas l’ID du fichier, cliquez sur <b>[!UICONTROL Find Files]</b> et saisissez ou mappez l’ID du projet auquel le fichier est associé, puis sélectionnez le fichier.</p>
          </li>
          <li>
            <p>Si vous essayez de trouver l’ID du fichier et que vous ne connaissez pas l’ID du projet, cliquez sur <b>[!UICONTROL Find Projects]</b> et saisissez ou mappez l’ID de l’équipe qui possède le projet auquel le fichier est associé. Sélectionnez le projet, puis le fichier.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Répertorier les fichiers du projet]

Ce module de recherche renvoie une liste de tous les fichiers du projet spécifié.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour savoir comment connecter votre compte [!DNL Figma] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Se connecter à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL File ID]</td>
      <td>
        <p>Saisissez ou mappez l’ID du projet pour lequel vous souhaitez récupérer les fichiers. </p>
        <ul>
          <li>
            <p>Si vous ne connaissez pas l’ID du projet, cliquez sur <b>[!UICONTROL Find Projects]</b> et saisissez ou mappez l’ID de l’équipe à laquelle le projet est associé, puis sélectionnez le projet.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Répertorier les projets]

Ce module de recherche renvoie une liste de tous les projets de l’équipe spécifiée.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour savoir comment connecter votre compte [!DNL Figma] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Se connecter à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Saisissez ou mappez l’ID du projet pour lequel vous souhaitez récupérer les fichiers. L’identifiant de l’équipe se trouve dans l’URL de la page de l’équipe dans Figma.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td>
    </tr>
  </tbody>
</table>


### Composants et styles

#### [!UICONTROL Obtenir un style ou un composant]

Ce module d’action permet de récupérer un style ou un composant unique, ou un ensemble de styles ou de composants.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour savoir comment connecter votre compte [!DNL Figma] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Se connecter à [!DNL Adobe Workfront Fusion] - Instructions de base.</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Object&gt; key]</td>
      <td>Saisissez la clé (identifiant unique) de l’objet que vous souhaitez récupérer.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Team ID]</td>
      <td>Saisissez ou mappez l’ID de l’équipe à laquelle l’enregistrement ou les enregistrements sont associés.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Page Size]</td>
      <td>Saisissez ou mappez le nombre de résultats à renvoyer par page. Valeur par défaut : 30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL After]</td>
      <td>
        <p>Saisissez ou mappez le numéro du résultat après lequel vous souhaitez commencer à extraire des résultats. Ce champ peut être combiné avec le champ [!UICONTROL Page Size] pour paginer les résultats.</p>
        <p>Cette valeur ne correspond pas aux ID des objets.</p>
        <p>Ce champ ne peut pas être utilisé en combinaison avec le champ [!UICONTROL Before].</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Before]</td>
      <td>
        <p>Saisissez ou mappez le numéro du résultat avant lequel vous souhaitez commencer à extraire des résultats. Ce champ peut être combiné avec le champ [!UICONTROL Page Size] pour paginer les résultats.</p>
        <p>Cette valeur ne correspond pas aux ID des objets.</p>
        <p>Ce champ ne peut pas être utilisé en combinaison avec le champ [!UICONTROL After].</p>
      </td>
    </tr>
  </tbody>
</table>


### Autre

* [Effectuer un appel API](#make-an-api-call)

* [Surveiller les événements](#watch-events)


#### [!UICONTROL Effectuer un appel API]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API Figma sans avoir à réfléchir à l’authentification. De cette façon, vous pouvez créer une automatisation des flux de données qui ne peut pas être réalisée par les autres modules Figma.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Pour savoir comment connecter votre compte [!DNL Figma] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base.</a>.</p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Saisissez un chemin d’accès relatif à <code>https://api.figma.com/v1/</code>.</p>
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
        <p>[!DNL Workfront Fusion] ajoute les en-têtes d’autorisation pour vous.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p>
        <p>Par exemple : <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre JSON, mettez les guillemets à l’extérieur de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Surveiller les événements]

Ce module déclencheur lance un scénario lorsque l’un des événements suivants se produit pour une équipe spécifique dans votre espace d’équipe [!DNL Figma].

* Mise à jour de fichier

* Mise à jour de la version du fichier

* Suppression de fichier

* Publication de bibliothèque

* Commentaire de fichier

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>Sélectionnez le webhook que le module surveille.</p>
        <p>Pour ajouter un nouveau webhook :</p>
        <ol>
          <li value="1">
            <p>Cliquez sur <b>[!UICONTROL Add]</b> à côté du champ [!UICONTROL Webhook].</p>
          </li>
          <li value="2">
            <p>Sélectionnez la connexion que vous souhaitez utiliser pour ce webhook. Pour obtenir des instructions sur la connexion de votre compte [!DNL Figma] à [!UICONTROL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Se connecter à [!UICONTROL Adobe Workfront Fusion] - Instructions de base.</a></p>
          </li>
          <li value="3">
            <p>Sélectionnez le type d’événement que vous voulez que le module surveille.</p>
          </li>
          <li value="4">
            <p>Saisissez l’ID de l’équipe dont vous souhaitez que le webhook surveille les événements.</p>
          </li>
          <li value="5">
            <p>Saisissez le [!UICONTROL Status] ou la [!UICONTROL Description] des événements que vous souhaitez que le webhook surveille.</p>
          </li>
          <li value="6">
            <p>Cliquez sur <b>[!UICONTROL Save]</b> pour enregistrer le webhook et revenir au module.</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
