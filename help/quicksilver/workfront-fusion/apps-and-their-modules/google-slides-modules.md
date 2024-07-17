---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Google Slides
description: Les modules Adobe Workfront Fusion Google Slides vous permettent de créer, de mettre à jour, de répertorier et/ou de supprimer des présentations et de télécharger des images vers des présentations dans votre compte Google Slides.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1618'
ht-degree: 19%

---

# Modules [!DNL Google Slides]

Les modules [!DNL Adobe Workfront Fusion] [!DNL Google Slides] vous permettent de créer, de mettre à jour, de répertorier et/ou de supprimer des présentations et de télécharger des images vers des présentations dans votre compte [!DNL Google Slides].

Pour utiliser [!DNL Google Slides] avec [!DNL Workfront Fusion], il est nécessaire d&#39;avoir un compte [!DNL Google]. Si vous n&#39;avez pas encore de compte [!DNL Google], vous pouvez en créer un sur la page d&#39;aide du compte [!DNL Google].

Vous avez également besoin de [!DNL Google Slides] dans votre [!DNL Google Drive].

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

## Conditions préalables

Pour utiliser des modules [!DNL Google Slides], vous devez disposer d’un compte [!DNL Google].

## Modules [!DNL Google Slides] et leurs champs

Lorsque vous configurez [!DNL Google Slides] modules, Workfront Fusion affiche les champs répertoriés ci-dessous. Des champs [!DNL Google Slides] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Présentation](#presentation)
* [Autre](#other)

### Présentation

* [[!UICONTROL Watch Presentations]](#watch-presentations)
* [[!UICONTROL Lister Presentations]](#list-presentations)
* [[!UICONTROL Obtenir une présentation]](#get-a-presentation)
* [[!UICONTROL Obtenir une page/miniature]](#get-a-pagethumbnail)
* [[!UICONTROL Créer une présentation à partir d’un modèle]](#create-a-presentation-from-a-template)
* [[!UICONTROL Télécharger une image vers une présentation]](#upload-an-image-to-a-presentation)
* [[!UICONTROL Actualiser un graphique]](#refresh-a-chart)
* [[!UICONTROL Ajouter/Supprimer une diapositive]](#adddelete-a-slide)

#### [!UICONTROL Watch Presentations]

Déclenche lorsqu’une nouvelle présentation est créée ou mise à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Slides] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch] </td> 
   <td> <p>Sélectionnez l’option pour regarder les présentations :</p> 
    <ul> 
     <li> <p>[!UICONTROL Date de création]</p> </li> 
     <li> <p>[!UICONTROL Date de modification]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Le nombre maximal de présentations que Workfront Fusion doit renvoyer lors d’un cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lister Presentations]

Récupère une liste de toutes les présentations.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Slides] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir l’emplacement d’un lecteur]</td> 
   <td> <p>Sélectionnez l’ [!DNL Google Drive] où se trouvent les présentations que vous souhaitez répertorier :</p> 
    <ul> 
     <li>[!UICONTROL Mon lecteur]</li> 
     <li>[!UICONTROL Partagé Avec Moi]</li> 
     <li>[!UICONTROL [!DNL Google] Lecteur partagé]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier]</td> 
   <td> <p>Sélectionnez l’emplacement du dossier des présentations que vous souhaitez répertorier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Le nombre maximal de présentations [!DNL Workfront Fusion] doit être renvoyé au cours d’un cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir une présentation]

Obtient la dernière version d’une présentation spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Slides] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez l’ [!DNL Google Drive] où se trouvent les présentations que vous souhaitez répertorier :</p> 
    <ul> 
     <li>[!UICONTROL Mon lecteur]</li> 
     <li>[!UICONTROL Partagé Avec Moi]</li> 
     <li>[!UICONTROL [!DNL Google] Lecteur partagé]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de présentation]</td> 
   <td> <p> Sélectionnez la présentation que vous souhaitez récupérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir une page/miniature]

Obtient la dernière version de la page spécifiée ou de la miniature d’une page dans la présentation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Slides] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de présentation]</td> 
   <td> <p> Sélectionnez l’identifiant de présentation que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’objet de page]</td> 
   <td> <p> Sélectionnez la diapositive pour laquelle vous souhaitez afficher les détails de l’objet de page.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Afficher la miniature de page]</td> 
   <td> <p> Cochez la case si vous souhaitez afficher les informations sur la miniature de la page.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer une présentation à partir d’un modèle]

Crée une nouvelle présentation en remplaçant toutes les balises telles que `{{Name}}` et `{{Email}}` dans un modèle par les données fournies.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Slides] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>Saisissez le nom de la nouvelle présentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copier une présentation]</td> 
   <td> <p> Sélectionnez l’option si vous copiez une présentation existante :</p> 
    <ul> 
     <li>[!UICONTROL Par Mappage]</li> 
     <li>[!UICONTROL Par Liste Déroulante]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copie de l’ID de présentation existant]</td> 
   <td> <p> Saisissez le chemin d’accès ou l’identifiant de présentation d’une présentation existante que vous souhaitez copier. Ce champ s’affiche si vous créez la présentation [!UICONTROL Par mappage].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez l’ [!DNL Google Drive] où se trouvent les présentations que vous souhaitez répertorier :</p> 
    <ul> 
     <li>[!UICONTROL Mon lecteur]</li> 
     <li>[!UICONTROL Partagé Avec Moi]</li> 
     <li>[!UICONTROL [!DNL Google] Lecteur partagé]</li> 
    </ul> <p>Ce champ s’affiche si vous créez la présentation [!UICONTROL Par liste déroulante].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de présentation]</td> 
   <td> <p> Sélectionnez l'identifiant de présentation de la présentation que vous souhaitez utiliser comme modèle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values] </td> 
   <td> <p>Ajoutez les valeurs :</p> 
    <ul> 
     <li><strong>[!UICONTROL Tag]</strong> : saisissez la balise à remplacer dans la présentation. Par exemple, <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL Valeur remplacée]</strong> : entrez la valeur avec laquelle la balise existante doit être remplacée. Par exemple, si une chaîne <tr><ul><tr><tr><tr><code>&#123;&#123;Name&#125;&#125;/code> in the presentation and the replaced value is Sample, then the <code>&#123;&#123;Name}}</code> will be replaced by <code>Sample</code>.</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL New Drive Location]</td> 
   <td> <p>Select the [!DNL Google Drive] where you want to store or add the new presentation:</p> 
     
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] Shared Drive]</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader"> <p>[!UICONTROL New Document's Location]</p> </td> 
   <td> <p>Select the folder where you want to store or add the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Shared] </td> 
   <td> <p>Select if you want to share the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Sharing with Other's Email Address]</td> 
   <td> <p> Enter the email address with whom you want to share the presentation. If you are not entering an email address and selecting only shared field, the presentation is shareable to anyone.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger une image vers une présentation]

Télécharge une image avec les données fournies.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Slides] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir une présentation]</td> 
   <td> <p>Choisissez le mode de sélection de la présentation sur laquelle vous téléchargez une image.</p> 
    <ul> 
     <li>[!UICONTROL Par Mappage]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez l’ [!DNL Google Drive] où se trouvent les présentations que vous souhaitez répertorier :</p> 
    <ul> 
     <li>[!UICONTROL Mon lecteur]</li> 
     <li>[!UICONTROL Partagé Avec Moi]</li> 
     <li>[!UICONTROL [!DNL Google] Lecteur partagé]</li> 
    </ul> <p>Ce champ s’affiche si vous créez la présentation [!UICONTROL Par liste déroulante].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de présentation]</td> 
   <td> <p> Sélectionnez l’identifiant de présentation de la présentation sur laquelle vous téléchargez une image.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td> <p>Valeurs Ajoutez les valeurs :</p> 
    <ul> 
     <li><strong>[!UICONTROL Tag]</strong> : entrez la balise à laquelle vous souhaitez ajouter l’URL.</li> 
     <li><strong>[!UICONTROL URL de l’image]</strong> : saisissez le chemin ou l’URL de l’image à télécharger.</li> 
    </ul> <p>Remarque : La taille des images doit être inférieure à 50 Mo, ne peut pas dépasser 25 mégapixels et doit être au format PNG, JPEG ou GIF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualiser un graphique]

Actualise les données du graphique stockées dans une présentation spécifiée par l’identifiant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Slides] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez l’ [!DNL Google Drive] où se trouvent les présentations que vous souhaitez répertorier :</p> 
    <ul> 
     <li>[!UICONTROL Mon lecteur]</li> 
     <li>[!UICONTROL Partagé Avec Moi]</li> 
     <li>[!UICONTROL [!DNL Google] Lecteur partagé]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de présentation]</td> 
   <td> <p>Sélectionnez l’identifiant de présentation de la présentation qui comprend le graphique à actualiser.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’objet de graphique]</td> 
   <td> <p> Sélectionnez le graphique que vous souhaitez actualiser.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter/Supprimer une diapositive]

Crée une diapositive vide ou supprime une diapositive existante sur la présentation spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Slides] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner la méthode]</td> 
   <td> <p>Indiquez si vous souhaitez ajouter une nouvelle diapositive ou supprimer une diapositive.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>Sélectionnez l'identifiant de présentation de la présentation pour laquelle vous souhaitez ajouter ou supprimer une diapositive.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de disposition prédéfinie]</td> 
   <td> <p> Sélectionnez la disposition de diapositives prédéfinie que vous souhaitez que votre diapositive ajoutée utilise. Spécifiez les valeurs de tous les champs supplémentaires (tels que [!UICONTROL Titre]).</p> 
    <ul> 
     <li>[!UICONTROL Mise en page vierge, sans espaces réservés]</li> 
     <li>[!UICONTROL Disposition avec une légende en bas]</li> 
     <li>[!UICONTROL Disposition avec un titre et un sous-titre]</li> 
     <li>[!UICONTROL Disposition avec un titre et un corps]</li> 
     <li>[!UICONTROL Disposition avec un titre et deux colonnes]</li> 
     <li>[!UICONTROL Disposition avec un seul titre]</li> 
     <li>[!UICONTROL Disposition avec un titre de section]</li> 
     <li>[!UICONTROL Disposition avec un titre et un sous-titre d’un côté et une description de l’autre]</li> 
     <li>[!UICONTROL Disposition avec un titre et un corps organisés en une seule colonne]</li> 
     <li>[!UICONTROL Disposition avec un point principal]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>Ce champ est disponible si vous avez choisi d’ajouter une diapositive.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)
* [[!UICONTROL Insérer des liens dans une présentation]](#insert-links-in-a-presentation)

#### [!UICONTROL Effectuer un appel API]

Exécute un appel d’API autorisé arbitraire.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Slides] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Saisissez un chemin relatif à https://developers.google.com/slides/. Par exemple, présentation.</p> <p>Pour obtenir la liste des points de terminaison disponibles, reportez-vous à la <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] documentation de l’API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Saisissez les en-têtes de requête de votre choix. Vous n’avez pas besoin d’ajouter des en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Saisissez la chaîne de requête.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** À l’aide d’un appel API, vous pouvez obtenir les détails de présentation de l’identifiant de présentation que vous avez saisi. Vous pouvez trouver l’identifiant de présentation dans l’URL lorsque vous ouvrez la présentation dans [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>L’appel API suivant renvoie les détails de la présentation :
>
>![](assets/presentation-details.png)
>
>Les correspondances de la recherche se trouvent dans la sortie du module sous [!UICONTROL Bundle] > [!UICONTROL Body] > [!UICONTROL submissionId].
>
>Dans notre exemple, les détails de présentation demandés ont été renvoyés :
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL Insérer des liens dans une présentation]

Ce module rend tous les liens d’une présentation cliquables ou insère un lien dans tous les textes d’entrée correspondants.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Slides] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir une présentation]</td> 
   <td> <p>Choisissez le mode de sélection de la présentation sur laquelle vous téléchargez une image.</p> 
    <ul> 
     <li>[!UICONTROL Par Mappage]</li> 
     <li>[!UICONTROL Par Liste Déroulante]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un lecteur]</td> 
   <td> <p>Sélectionnez l’ [!DNL Google Drive] où se trouvent les présentations que vous souhaitez répertorier :</p> 
    <ul> 
     <li>[!UICONTROL Mon lecteur]</li> 
     <li>[!UICONTROL Partagé Avec Moi]</li> 
     <li>[!UICONTROL [!DNL Google] Lecteur partagé]</li> 
    </ul> <p>Ce champ s’affiche si vous créez la présentation [!UICONTROL Par liste déroulante].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de présentation]</td> 
   <td> <p>Sélectionnez l’emplacement du dossier des présentations que vous souhaitez répertorier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select]</td> 
   <td> <p>Indiquez si vous souhaitez que tous les liens d’une présentation puissent faire l’objet d’un clic ou si vous souhaitez insérer un lien dans tous les textes de saisie correspondants.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrées de texte]</td> 
   <td>Pour chaque élément de texte pour lequel vous souhaitez ajouter un lien, ajoutez l’élément ainsi que le lien associé à la liste. Chaque fois que l’élément apparaît dans la présentation, il est automatiquement lié au site spécifié.</td> 
  </tr> 
 </tbody> 
</table>
