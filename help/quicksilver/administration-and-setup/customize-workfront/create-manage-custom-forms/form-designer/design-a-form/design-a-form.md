---
title: Création d’un formulaire personnalisé
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez concevoir un formulaire personnalisé à l’aide du concepteur de formulaires. Vous pouvez joindre des formulaires personnalisés à différents objets Workfront pour capturer des données en rapport avec ces objets.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: 45bc1820e4f6416e3d47139bbcf1a2156c5900dc
workflow-type: tm+mt
source-wordcount: '6941'
ht-degree: 49%

---

# Créer un formulaire personnalisé

<!-- Audited: 6/2025 -->

Vous pouvez concevoir un formulaire personnalisé à l’aide du concepteur de formulaire dans Adobe Workfront. Vous pouvez joindre des formulaires personnalisés à différents objets Workfront pour capturer des données en rapport avec ces objets.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Commencer à concevoir un formulaire personnalisé

{{step-1-to-setup}}

1. Dans le volet de gauche, cliquez sur **Forms personnalisé**, puis sélectionnez **Forms**.

1. Cliquez sur **Nouveau formulaire personnalisé**.
1. Sélectionnez les types d’objets auxquels vous souhaitez joindre le formulaire personnalisé, puis cliquez sur **Continuer**.

   ![Choisir les types d’objet](assets/new-custom-form-select-objects.png)

1. Dans la zone **Ajouter un nom de formulaire**, saisissez le titre du formulaire personnalisé.
1. (Facultatif) Si vous souhaitez ajouter d’autres types d’objets au formulaire afin qu’il puisse être joint à d’autres objets, cliquez sur l’icône **Ajouter** ![icône Ajouter des objets](assets/add-objects-icon.png) en regard de **Types d’objets**, puis sélectionnez le type de votre choix dans le menu qui s’affiche. Vous pouvez répéter cette opération pour ajouter autant de types d’objet que vous le souhaitez.

   Une fois que plusieurs objets ont été ajoutés au formulaire, vous pouvez cliquer sur le X d’un type d’objet pour le supprimer du formulaire.

   >[!CAUTION]
   >
   >La suppression d’un formulaire personnalisé supprime également toutes les données personnalisées sur les objets associés au formulaire. Les données supprimées ne peuvent pas être récupérées. Vous pouvez également désactiver un formulaire personnalisé que vous n’utilisez plus, ce qui conservera toutes les données historiques associées.
   >
   >Pour plus d’informations, voir [Ajouter ou supprimer des types d’objet d’un formulaire personnalisé existant](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/add-or-remove-objects-from-a-form.md) et [Désactiver ou réactiver un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/activate-deactivate-form.md).


1. Ensuite, vous pouvez commencer à ajouter des champs à votre formulaire personnalisé. Pour plus d’informations, consultez les sections suivantes :
   * [Réutiliser un champ ou un widget existant déjà utilisé dans un autre formulaire personnalisé](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Remarques sur les noms et les libellés des champs](#notes-on-field-names-and-labels)
   * [Ajouter des champs de texte](#add-text-fields)
   * [Ajouter des champs calculés](#add-calculated-fields)
   * [Ajout de boutons radio, de groupes de cases à cocher et de listes déroulantes](#add-radio-buttons-checkbox-groups-and-drop-downs)
   * [Ajouter des champs de frappe continue et des champs de date](#add-typeahead-and-date-fields)
   * [Ajouter des champs de recherche externes](#add-external-lookup-fields)
   * [&#128279;](#add-images-pdfs-and-videos)Ajouter des images, des fichiers PDF et des vidéos

   * [Ajouter des champs natifs Workfront](#add-workfront-native-fields)
   * [Ajouter des fichiers Adobe XD](#add-adobe-xd-files)
   * [Ajouter des champs de connexion Planning](#add-planning-connection-fields)

## Ajouter des champs nouveaux ou existants à votre formulaire personnalisé

Vous pouvez utiliser des champs nouveaux ou existants lors de la conception de votre formulaire personnalisé.

Les formulaires personnalisés sont limités à 500 champs. Un compteur en bas à gauche affiche le nombre de champs utilisés dans le formulaire. Il est toujours visible lorsque vous faites défiler l’écran dans le concepteur de formulaire.

### Réutiliser un champ ou un widget existant déjà utilisé dans un autre formulaire personnalisé

1. Dans le coin supérieur gauche de l’écran, cliquez sur **Bibliothèque de champs**.

1. Faites glisser et déposez le champ ou le widget de votre choix sur la zone de travail. Répétez cette étape pour ajouter d’autres champs ou widgets.

   >[!NOTE]
   >
   >Vous pouvez ajouter jusqu’à 500 champs sur un seul formulaire personnalisé. Cependant, une dégradation des performances peut se produire lorsque le formulaire comporte plus de 100 champs, en fonction de la complexité de votre formulaire personnalisé.
   >
   >
   >Parmi les exemples de formulaires complexes, citons les formulaires avec des paramètres en cascade, des champs de données personnalisées calculés et plusieurs options de valeur dans un même champ.

   >[!NOTE]
   >
   >Le fait de marquer un champ existant comme inactif le rend indisponible pour une utilisation dans les éléments de rapports et les formulaires personnalisés à partir de ce moment. Si le champ inactif est actuellement utilisé dans un rapport ou un formulaire, le champ et ses données historiques restent en place.

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

### Remarques sur les noms et les libellés des champs {#notes-on-field-names-and-labels}

Le libellé est disponible pour la plupart des champs. Il s’agit d’un libellé descriptif qui s’affiche au-dessus du champ ou du widget sur le formulaire personnalisé. Vous pouvez modifier le libellé à tout moment.

>[!NOTE]
>
>Évitez d’utiliser des caractères spéciaux dans ce libellé, car ils ne s’affichent pas correctement dans les rapports.

Un nom est requis pour chaque champ. Ce nom est la manière dont le système identifie le champ personnalisé lorsque vous l’ajoutez à diverses zones de Workfront, telles que les rapports, l’Accueil et les interactions d’API. Lorsque vous configurez le champ ou le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour le faire correspondre. Les champs Libellé et Nom ne sont pas synchronisés. Vous avez ainsi la possibilité de modifier le libellé visible par vos utilisateurs et utilisatrices sans avoir à modifier le nom visible par le système.

Chaque nom de champ personnalisé doit être unique dans l’instance Workfront de votre entreprise. Ainsi, vous pouvez réutiliser un nom de champ déjà créé pour un autre formulaire personnalisé.

>[!NOTE]
>
>Bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom après que vous ou d’autres utilisateurs avez commencé à utiliser le formulaire personnalisé dans Workfront. Si vous le faites, le système ne reconnaîtra plus le champ personnalisé là où il peut être référencé actuellement dans d’autres zones de Workfront.
>Par exemple, si vous ajoutez le champ personnalisé à un rapport et que vous modifiez ensuite son nom, Workfront ne le reconnaît pas dans le rapport et il ne fonctionnera plus correctement, à moins que vous ne le rajoutiez au rapport en utilisant le nouveau nom.
>
>Nous vous recommandons de ne pas saisir un nom déjà utilisé pour les champs Workfront intégrés.
>
>Nous vous recommandons de ne pas utiliser le point dans le nom du champ personnalisé afin d’éviter les erreurs lors de l’utilisation du champ dans différentes zones de Workfront.

Les caractères spéciaux suivants ne sont pas pris en charge dans les libellés et noms de champs personnalisés.

* \t
* \n
* \r
* \f
* `[`
* `]`
* (
* )
* :
* `{`
* `}`

### Ajouter des champs de texte

Vous pouvez ajouter plusieurs champs de texte différents à un formulaire personnalisé.

+++ Développez pour afficher les descriptions des champs de texte disponibles.

* **Champ de texte monoligne** : permet aux utilisateurs de saisir une seule ligne de texte dans le champ.
* **Champ de paragraphe** : permet aux utilisateurs de saisir plusieurs lignes de texte dans le champ.
* **Champ de texte avec mise en forme** : permet aux utilisateurs de saisir plusieurs lignes de texte dans le champ et de mettre en forme le texte avec du gras, de l’italique, du soulignement, des puces, de la numérotation, des liens hypertexte et des guillemets. La limite de 15 000 caractères permet d’utiliser du texte et des mises en forme variés.

  Ce type de champ personnalisé n’est pas pris en charge dans les filtres sur les listes et les rapports.

  Pour plus d’informations sur l’accès à ce champ par le biais de l’API, voir [Stockage de champs de texte enrichi dans l’API](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md).

  >[!NOTE]
  >
  >Les champs de texte avec mise en forme ne sont pas disponibles pour les applications mobiles Workfront (disponibilité dans les prochaines versions).

* **Texte descriptif** : vous permet d’inclure des instructions et des liens vers des pages extérieures à Workfront.

+++

Pour ajouter un champ de texte, procédez comme suit :

1. Dans l’onglet **Nouveau champ** sur le côté gauche de l’écran, recherchez l’un des champs de texte suivants et faites-le glisser vers une section de la zone de travail :

   * Texte sur une seule ligne
   * Paragraphe
   * Texte avec formatage
   * Texte descriptif

   ![Faire glisser le champ vers la section](assets/drag-field-to-section.png)

1. Dans la partie droite de l’écran, configurez les options disponibles pour le type de champ personnalisé que vous ajoutez :

   <table>
    <tr>
    <td>Entrée dans</td>
    <td>Description</td>
    <td>Disponible pour </td>
    </tr>
    <tr>
    <td>Taille</td>
    <td><p>(Facultatif) Modifiez la taille des champs de texte du formulaire.<p>
   </td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe</li>
    <li>Texte avec formatage</li>
    <li>Texte descriptif</li>
    </ul></td>
    </tr>
    <tr>
    <td>Étiquette</td>
    <td><p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ. Vous pouvez modifier le libellé à tout moment.<p>
    <p><b>Important</b> : évitez d’utiliser des caractères spéciaux dans ce libellé, car ils ne s’affichent pas correctement dans les rapports. Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p></td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe</li>
    <li>Texte avec formatage</li>
    </ul></td>
    </tr>
    <tr>
     <td>Nom</td>
    <td><p>(Obligatoire) Ce nom est la façon dont le système identifie le champ. Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Les champs Libellé et Nom ne sont pas synchronisés. Vous avez ainsi la possibilité de modifier le libellé visible par vos utilisateurs et utilisatrices sans avoir à modifier le nom visible par le système.</p>
    <p>Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p>
    </td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe</li>
    <li>Texte avec formatage</li>
    <li>Texte descriptif</li>
    </ul></td>
    </tr>
    <tr>
    <td>Instructions</td>
    <td>Saisissez toute information supplémentaire concernant le champ. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe</li>
    <li>Texte avec formatage</li>
    </ul></td>
    </tr>
    <tr>
    <td>Format</td>
    <td><p>Sélectionnez le type de données qui seront capturées dans le champ personnalisé.</p> <p><b>Remarque </b> :   
    <ul> 
    <li>Ce champ ne peut pas être modifié une fois le formulaire enregistré. Pour utiliser votre champ dans des calculs mathématiques, assurez-vous de sélectionner le format « Nombre » ou « Devise ».</li> 
    <li>Lorsque vous sélectionnez Nombre ou Devise, le système tronque automatiquement les nombres qui commencent par 0.</li>
    <li>Les champs au format « Nombre » sont limités à 16 caractères. Vous pouvez également utiliser un champ Texte pour saisir des nombres et éviter la limite.</li>
     </ul></p></td> </td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe</li>
    </ul></td>
    </tr>
    <tr>
    <td>Type d'affichage</td>
    <td>Basculer entre des champs de texte d’une seule ligne et des champs de texte de paragraphe.</td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe</li>
    </ul></td>
    </tr>
    <tr>
    <td>Lien hypertexte</td>
    <td> Si vous souhaitez appliquer un lien hypertexte au texte descriptif que vous avez saisi, ajoutez-le ici. Le texte descriptif s’affiche sous forme de lien sur les objets auxquels le formulaire est attaché.</td>
    <td><ul><li>Texte descriptif</li></ul></td>
    </tr>
    <tr>
     <td>Actif</td>
     <td><p>Cette option est activée par défaut.<p><p>Lorsque vous définissez un champ comme Inactif, il est exclu des rapports, filtres et affichages et n’est plus disponible dans la bibliothèque de champs de formulaires personnalisés.</p></td>
     <td><ul>
     <li>Texte sur une seule ligne</li>
     <li>Paragraphe</li>
     <li>Texte avec formatage</li>
     <li>Texte descriptif</li></ul></td>
    </tr>
    <tr> 
      <td role="rowheader">Créer un champ obligatoire</td>
      <td><p>Sélectionnez cette option si vous souhaitez que le champ soit obligatoire pour que l’utilisateur ou l’utilisatrice puisse remplir le formulaire personnalisé.</p></td>
    <td><ul>
    <li>Texte sur une seule ligne</li>
    <li>Paragraphe</li>
    <li>Texte avec formatage</li>
    </ul></td> 
    </tr> 
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   Ou

   Pour copier un champ, pointez dessus et cliquez sur l’icône de copie.

   ![icône de copie](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

### Ajouter des champs calculés

Dans un formulaire personnalisé, vous pouvez ajouter un champ personnalisé calculé qui utilise les données existantes pour générer de nouvelles données lorsque le formulaire personnalisé est joint à un objet.

Pour ajouter un champ calculé, consultez la section [Ajouter des champs calculés avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Ajout de boutons radio, de groupes de cases à cocher et de listes déroulantes

Vous pouvez ajouter des boutons radio, des groupes de cases à cocher, des listes déroulantes et des listes déroulantes à sélection multiple à un formulaire personnalisé.

+++ Développez pour afficher les descriptions des champs disponibles.

* **Cases d’option** : demande aux utilisateurs et aux utilisatrices de ne sélectionner qu’un seul choix.
* **Groupe de cases à cocher** : permet aux utilisateurs de sélectionner plusieurs choix.
* **Liste déroulante à sélection unique** : fournit une liste de choix déroulants.
* **Liste déroulante à sélection multiple** : permet aux utilisateurs et aux utilisatrices de sélectionner plusieurs choix dans une liste déroulante.

+++

>[!NOTE]
>
>Les champs qui autorisent plusieurs sélections, tels que Groupe Case à cocher et Menu déroulant multi-sélection, sont difficiles à représenter sous forme de graphiques et à regrouper dans les rapports. Pour faciliter la création de graphiques et le regroupement dans les rapports, vous pouvez créer des champs distincts pour chaque choix (par exemple un champ de texte d’une seule ligne).

Pour ajouter des boutons radio, des groupes de cases à cocher et des listes déroulantes :

1. Dans l’onglet **Nouveau champ** sur le côté gauche de l’écran, recherchez l’un des champs suivants et faites-le glisser vers une section de la zone de travail :

   * Cases d’option
   * Groupe Case à cocher
   * Liste déroulante à sélection unique
   * Menu déroulant multi-sélection

   ![Faire glisser un champ sur la zone de travail](assets/drag-field-to-section.png)

1. Dans la partie droite de l’écran, configurez les options disponibles pour le type de champ personnalisé que vous ajoutez :

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Entrée dans</td>
    <td>Description</td>
    <td>Disponible pour </td>
    </tr>
    <tr> 
     <td role="rowheader">Étiquette</td> 
     <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ personnalisé. Vous pouvez modifier le libellé à tout moment.</p> <p><b>Important</b> : évitez d’utiliser des caractères spéciaux dans ce libellé, car ils ne s’affichent pas correctement dans les rapports. Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p> </td> 
     <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Liste déroulante à sélection unique</li>
    <li>Menu déroulant multi-sélection</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Nom</td> 
     <td> <p>(Obligatoire) Ce nom est la façon dont le système identifie le champ. Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Les champs Libellé et Nom ne sont pas synchronisés. Vous avez ainsi la possibilité de modifier le libellé visible par vos utilisateurs et utilisatrices sans avoir à modifier le nom visible par le système.</p> 
    <p>Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p> </td>
     <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Liste déroulante à sélection unique</li>
    <li>Menu déroulant multi-sélection</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Instructions</td> 
    <td> <p>Saisissez des informations supplémentaires sur le champ personnalisé. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Liste déroulante à sélection unique</li>
    <li>Menu déroulant multi-sélection</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Format</td> 
    <td> <p>Sélectionnez le type de données qui seront capturées dans le champ personnalisé.</p> <p><b>Remarque </b> :   
     <ul> 
    <li>Ce champ ne peut pas être modifié une fois le formulaire enregistré. Pour utiliser votre champ dans des calculs mathématiques, assurez-vous de sélectionner le format « Nombre » ou « Devise ».<br></li> 
    <li>Lorsque vous sélectionnez Nombre ou Devise, le système tronque automatiquement les nombres qui commencent par 0.</li>
    <li>Les champs au format « Nombre » sont limités à 16 caractères. Vous pouvez également utiliser un champ Texte pour saisir des nombres et éviter la limite.</li>
     </ul></p></td> 
     <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Liste déroulante à sélection unique</li>
    <li>Menu déroulant multi-sélection</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Type d'affichage</td> 
    <td>Basculez entre les boutons radio, le groupe de cases à cocher, la liste déroulante à sélection unique ou la liste déroulante à sélection multiple pour le champ.</td> 
    <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Liste déroulante à sélection unique</li>
    <li>Menu déroulant multi-sélection</li>
    </ul></td>
    </tr> 
    <td role="rowheader">Choix </td> 
    <td> 
    <p>Sélectionnez l’une des options suivantes :</p> 
    <ul> 
    <li><strong>Afficher les valeurs</strong> : affiche les valeurs de chaque choix dans le champ. Le libellé de chaque choix s’affiche par défaut.</li>
   <li><strong>Trier les choix dans l’ordre alphabétique</strong> : trie par ordre alphabétique les choix que vous ajoutez dans le champ.</li>
    </ul>
     <p>Pour chaque choix que vous ajoutez à l’utilisateur ou à l’utilisatrice, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-settings.png">, puis sélectionnez l’une des options suivantes :</p> 
    <ul> 
    <li><strong>Sélectioner par défaut</strong> : sélectionnez le choix par défaut dans le champ.</li> 
    <li> <p><strong>Masquer le choix</strong> : masquez le choix dans le champ. Les choix masqués restent accessibles dans les rapports.</p> </li> 
    <li> <p><strong>Supprimer le choix</strong> : supprimez le choix du champ.</p> <p><b>Avertissement </b> : si des objets actifs utilisent ce choix, ne le supprimez pas du champ. Sa suppression entraînera la perte de données historiques. Sélectionnez plutôt l’option pour le masquer, ce qui empêchera les utilisateurs et utilisatrices de le sélectionner à l’avenir.</p> </li> 
    </ul>   
    <p><b>Remarque :</b> il n’existe aucune limite au nombre de choix que vous pouvez sélectionner. </p>    
    </td> 
    <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Liste déroulante à sélection unique</li>
    <li>Menu déroulant multi-sélection</li>
    </ul>
    </td>
     </tr>
    <tr>
     <td>Actif</td>
     <td><p>Cette option est activée par défaut.<p><p>Lorsque vous définissez un champ comme Inactif, il est exclu des rapports, filtres et affichages et n’est plus disponible dans la bibliothèque de champs de formulaires personnalisés.</p></td>
     <td><ul>
     <li>Cases d’option</li>
     <li>Groupe Case à cocher</li>
     <li>Liste déroulante à sélection unique</li>
     <li>Menu déroulant multi-sélection</li></ul></td>
    </tr>
    <tr> 
    <td role="rowheader">Créer un champ obligatoire</td> 
    <td>Sélectionnez cette option si vous souhaitez que le champ soit obligatoire pour que l’utilisateur ou l’utilisatrice puisse remplir le formulaire personnalisé. </td> 
    <td><ul>
    <li>Cases d’option</li>
    <li>Groupe Case à cocher</li>
    <li>Liste déroulante à sélection unique</li>
    <li>Menu déroulant multi-sélection</li>
    </ul></td>
     </tr> 
    <tr> 
    </tbody> 
    </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   Ou

   Pour copier un champ, pointez dessus et cliquez sur l’icône de copie.

   ![&#x200B; Icône Copier &#x200B;](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

### Ajouter des champs typeahead et des champs de date

Vous pouvez ajouter des champs de saisie semi-automatique et de date à un formulaire personnalisé.

+++ Développez pour afficher les descriptions des champs disponibles.

* **Saisie semi-automatique** : permet aux utilisateurs et utilisatrices de saisir le nom d’un objet qui existe dans Workfront. Une liste de suggestions s’affiche lorsque l’utilisateur ou l’utilisatrice commence à saisir du texte. Ce type de champ prend en charge les objets suivants :
   * l’utilisateur ou de l’utilisatrice
   * Groupe
   * Fonction
   * Portfolio
   * Programme
   * Projet
   * Equipe
   * Modèle
   * Entreprise
* **Date** : affiche un calendrier dans lequel les utilisateurs peuvent sélectionner une date et une heure.

+++

Pour ajouter des champs de saisie semi-automatique et de date :

1. Dans l’onglet **Nouveau champ** sur le côté gauche de l’écran, recherchez l’un des champs suivants et faites-le glisser vers une section de la zone de travail.

   * Frappe continue
   * Date

   ![Faire glisser le champ vers la section](assets/drag-field-to-section.png)

1. Dans la partie droite de l’écran, configurez les options disponibles pour le type de champ personnalisé que vous ajoutez :

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Paramètre du champ</td>
    <td>Description</td>
    <td>Disponible pour </td>
    </tr>
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ personnalisé. Vous pouvez modifier le libellé à tout moment.</p> <p><b>Important</b> : évitez d’utiliser des caractères spéciaux dans ce libellé, car ils ne s’affichent pas correctement dans les rapports. Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p> </td> 
       <td><ul>
    <li>Frappe continue</li>
    <li>Date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom est la façon dont le système identifie le champ. Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Les champs Libellé et Nom ne sont pas synchronisés. Vous avez ainsi la possibilité de modifier le libellé visible par vos utilisateurs et utilisatrices sans avoir à modifier le nom visible par le système.</p> 
      <p>Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p> </td>
    <td><ul>
    <li>Frappe continue</li>
    <li>Date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le champ personnalisé. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Frappe continue</li>
    <li>Date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Afficher l'heure</td> 
      <td>Sélectionnez cette option si vous souhaitez afficher l’heure et la date du jour dans le champ.</td> 
         <td><ul>
    <li>Date</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Type d'objet référencé</td> 
      <td> <p>Sélectionnez le type d’objet à associer au champ.</p> <p>Une fois que vous avez cliqué sur <b>Appliquer</b> ou <b>Enregistrer et fermer</b>, vous ne pouvez plus modifier le type d’objet du champ.</p> <p><b>Remarque </b> :   
        <ul> 
         <li>Si votre administrateur ou administratrice Workfront a personnalisé le nom des portfolios, programmes ou projets dans l’interface d’utilisation de Workfront, le nom par défaut de l’objet s’affiche dans cette liste déroulante et non dans le nom personnalisé. Contactez l’administration Workfront si vous avez besoin d’aide.<br></li> 
         <li>Les types d’objets suivants sont pris en charge dans les applications mobiles iOS et Android Workfront : « Utilisateur ou utilisatrice », « Société », « Groupe », « Fonction », « Portfolio », « Programme », « Projet » et « Modèle ».</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Frappe continue</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">Ajouter filtre</td>
      <td><p>Ajoutez un filtre pour un type d’objet afin de limiter les objets que les personnes peuvent sélectionner lorsqu’elles utilisent le champ. </p> <p>Par exemple, vous pouvez limiter un champ afin que les noms d’utilisateur ne puissent être sélectionnés que s’ils répondent aux critères suivants :</p> 
       <ul> 
        <li>Ils appartiennent à un ou plusieurs groupes que vous spécifiez.</li> 
        <li>Ils sont associés à un rôle ou un titre de poste que vous spécifiez.</li> 
        <li>Ils appartiennent au même groupe que la personne qui utilise le champ .</li> 
       </ul>
       <p>Vous devez définir le filtre correspondant au type d’objet sélectionné à l’aide de la syntaxe mode texte. Pour plus d’informations sur la création d’un filtre à l’aide du mode texte, consultez la section <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Modifier un filtre à l’aide du mode texte</a>.</p>
       <p><b>Conseil :</b> vous pouvez créer un rapport pour tester votre filtre avant de l’ajouter directement au champ de saisie semi-automatique. Cela vous aidera à vérifier que le filtre renvoie les objets corrects. Vous pouvez ensuite passer en mode texte dans le rapport, copier l’instruction de mode texte et l’ajouter au filtre de saisie semi-automatique.</p>
       <p><b>Remarque </b> :
       <ul> 
        <li>Si vous modifiez un formulaire personnalisé existant, l’ajout d’un filtre à un champ de saisie semi-automatique ne supprime aucun objet (hors de portée du filtre) que les utilisateurs ont déjà ajouté à l’aide du champ.</li> 
        <li>Ce filtre n’est pas disponible sur les appareils mobiles. Si vous utilisez le filtre pour un champ de saisie semi-automatique, le champ s’affiche sur les appareils mobiles des utilisateurs non affectés par le filtre.</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>Frappe continue</li>
       </ul>
      </td>
     </tr>
     <tr>
      <td>Actif</td>
      <td><p>Cette option est activée par défaut.<p><p>Lorsque vous définissez un champ comme Inactif, il est exclu des rapports, filtres et affichages et n’est plus disponible dans la bibliothèque de champs de formulaires personnalisés.</p></td>
      <td><ul>
      <li>Frappe continue</li>
      <li>Date</li></ul></td>
     </tr>
     <tr> 
      <td role="rowheader">Créer un champ obligatoire</td> 
      <td>Sélectionnez cette option si vous souhaitez que le champ soit obligatoire pour que l’utilisateur ou l’utilisatrice puisse remplir le formulaire personnalisé. </td> 
       <td><ul>
    <li>Frappe continue</li>
    <li>Date</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   Ou

   Pour copier un champ, pointez dessus et cliquez sur l’icône de copie.

   ![icône de copie](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

### Ajouter des champs de recherche externe

Un champ de recherche externe appelle une API externe et renvoie des valeurs sous forme d’options dans un champ déroulant. Les utilisateurs qui travaillent avec l’objet auquel le formulaire personnalisé est joint peuvent sélectionner une ou plusieurs de ces options dans la liste déroulante, selon que le champ de recherche externe est un champ à sélection unique ou multiple. Les champs de recherche externe sont également disponibles dans les listes et les rapports.

Pour obtenir des exemples d’utilisation du champ de recherche externe pour appeler la même instance de Workfront ou une API publique, voir [Exemples du champ de recherche externe dans un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>* Les champs de recherche externe ne sont pas pris en charge dans le plug-in Outlook.
>* Les champs de recherche externe ne sont pas disponibles dans les listes lorsque le champ possède une dépendance sur un autre champ.

Pour ajouter une recherche externe, procédez comme suit :

1. Dans l’onglet **Nouveau champ** sur le côté gauche de l’écran, recherchez **Recherche externe** ou **Recherche externe à sélection multiple**, puis faites-la glisser vers une section de la zone de travail.
1. Dans la partie droite de l’écran, configurez les options du champ personnalisé :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ personnalisé. Vous pouvez modifier le libellé à tout moment.</p> <p><b>Important</b> : évitez d’utiliser des caractères spéciaux dans ce libellé, car ils ne s’affichent pas correctement dans les rapports. Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom est la façon dont le système identifie le champ. Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Toutefois, les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé visible par vos utilisateurs sans avoir à modifier le nom visible par le système.</p>
      <p>Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p> </td>
     </tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le champ personnalisé. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td>
      <td><p>Sélectionnez le type de données qui seront capturées dans le champ personnalisé.</p>
      <p><strong>Note :</strong></p>
      <ul><li>Il est possible de modifier le type de format une fois le formulaire enregistré, mais toutes les valeurs existantes sur les objets doivent être convertibles au nouveau type de format. (Par exemple, si le type de format est Texte et qu’un objet stocke la valeur « abc », vous ne pouvez pas convertir le champ et une erreur s’affichera, indiquant que le système ne peut pas convertir « abc » en nombre/devise.) Si vous envisagez d’utiliser votre champ dans des calculs mathématiques, veillez à sélectionner un format numérique ou monétaire.</li>
      <li>Lorsque vous sélectionnez Nombre ou Devise, le système tronque automatiquement les nombres qui commencent par 0.</li>
      <li>Les champs au format « Nombre » sont limités à 16 caractères. Vous pouvez également utiliser un champ Texte pour saisir des nombres et éviter la limite.</li>
      </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">URL API de base</td> 
      <td><p>Saisissez ou collez l’URL de l’API.</p><p>L’URL de l’API doit renvoyer un contenu JSON des options que vous souhaitez afficher dans la liste déroulante. Vous pouvez utiliser le champ Chemin d’accès JSON pour sélectionner les valeurs spécifiques du fichier JSON renvoyé en tant qu’options de liste déroulante.</p><p>Lors de la saisie de l’URL de l’API, vous pouvez éventuellement transmettre les valeurs suivantes dans l’URL :</p>
      <ul>
      <li>$$HOST : il représente l’hôte Workfront actuel et peut être utilisé pour effectuer des appels d’API vers l’API Workfront. Lorsque ce caractère générique est utilisé, l’authentification est prise en charge et les utilisateurs et les utilisatrices n’ont pas besoin d’envoyer des en-têtes d’authentification. (Par exemple, les utilisateurs et les utilisatrices peuvent rechercher des tâches à l’aide de l’URL de base <code>$$HOST/attask/api/task/search</code>, qui permet de rechercher des tâches et de sélectionner des valeurs dans une liste de tâches renvoyée.)</li>
      <li><p>$$QUERY : cette valeur représente le texte de recherche que les utilisateurs et utilisatrices finaux saisissent dans le champ et vous permet d’implémenter le filtrage des requêtes pour ces personnes. (L’utilisateur recherche la valeur dans la liste déroulante.)</p>
      <p>Si l’API à laquelle vous faites référence le permet, vous pouvez également inclure des modificateurs dans votre requête de recherche afin d’identifier comment la recherche doit s’effectuer. Par exemple, vous pouvez utiliser l’URL d’API de base suivante pour permettre aux gens de rechercher tous les projets Workfront qui contiennent un texte spécifique : <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>Pour en savoir plus sur les modificateurs de recherche Workfront, consultez <a href="/help/quicksilver/wf-api/general/api-basics.md">Concepts de base de l’API</a>.</p>
      <p><strong>Remarque :</strong> si vous n’utilisez pas $$QUERY et que l’utilisateur saisit du texte dans la zone de recherche, les choix dont vous disposez déjà seront réduits. Toutefois, si vous utilisez $$QUERY et que l’utilisateur ou l’utilisatrice saisit quelque chose, un nouvel appel réseau à votre API est effectué. Par conséquent, si votre API contient plus de 2 000 valeurs et que l’API prend en charge l’interrogation, vous pouvez utiliser $$QUERY pour effectuer une recherche non seulement à partir des 2 000 valeurs existantes, mais aussi à partir de l’API d’origine avec les options restreintes.</p></li>
      <li><p>{fieldName} - Lorsque fieldName est n’importe quel champ personnalisé ou natif dans Workfront. Vous pouvez ainsi implémenter des filtres d’options de liste déroulante en cascade, lorsque vous transmettez la valeur d’un champ déjà sélectionné au champ Recherche externe pour filtrer les options vers le bas. (Par exemple, le champ Zone géographique existe déjà dans le formulaire et vous réduisez une liste de pays de l’API à ceux qui se trouvent dans une zone géographique spécifique.)</p>
      <p>Pour un champ de recherche externe dépendant d’autres champs (à l’aide de la syntaxe {fieldName}), les options renvoyées par l’API sont limitées à celles qui correspondent aux chaînes ou aux valeurs saisies dans les autres champs. (Cette fonctionnalité n’est pas prise en charge dans les listes et les rapports.)</p></li>
      <li>{referenceObject}.{fieldName} - Lorsque le champ fait partie d’un objet. Cette syntaxe est similaire à celle des expressions personnalisées. (Par exemple, portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>Conseil :</strong> consultez la documentation de l’API que vous utilisez pour les requêtes spécifiques que vous pouvez définir.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Méthode HTTP</td> 
      <td>Sélectionnez <strong>Get</strong>, <strong>Post</strong>, ou <strong>Put</strong> pour la méthode.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Chemin JSON</td>
      <td><p>Saisissez ou collez le chemin JSON pour l’API.</p> <p>Cette option permet d’extraire des données du JSON renvoyé par l’URL de l’API. Cela permet de sélectionner les valeurs à l’intérieur du fichier JSON qui apparaîtront dans les options de liste déroulante.</p><p>Par exemple, si votre URL d’API renvoie le format JSON suivant, vous pouvez utiliser « $.data[*].name » pour sélectionner États-Unis et Canada comme options de liste déroulante : </br>
      <pre>
      &lbrace;
data: &lbrace;
{ name: "USA"},
{ name: "Canada"}
&rbrace;
&rbrace;
      </pre>
      </p>
     <p>Pour plus d’informations sur le chemin JSON et pour vous assurer que vous écrivez le bon chemin JSON, consultez <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">En-têtes</td>
      <td><p>Cliquez sur <strong>Ajouter un en-tête</strong>, puis saisissez ou collez la paire clé-valeur requise pour l’authentification avec l’API.</p><p><strong>Remarque :</strong> les champs d’en-tête ne sont pas un emplacement sécurisé pour stocker les informations d’identification. Vous devez faire attention à ce que vous saisissez et enregistrez.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Menu déroulant multi-sélection</td>
      <td><p>Sélectionnez cette option pour permettre à l’utilisateur de sélectionner plusieurs valeurs dans la liste déroulante.</p></td>
     </tr>
     <tr>
      <td>Actif</td>
      <td><p>Cette option est activée par défaut.<p><p>Lorsque vous définissez un champ comme Inactif, il est exclu des rapports, filtres et affichages et n’est plus disponible dans la bibliothèque de champs de formulaires personnalisés.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Créer un champ obligatoire</td>
      <td><p>Sélectionnez cette option si vous souhaitez que le champ soit obligatoire pour que l’utilisateur ou l’utilisatrice puisse remplir le formulaire personnalisé.</p></td>
     </tr>       
    </tbody>
   </table>

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

>[!NOTE]
>
>Les éléments suivants sont des limitations techniques de l’appel à l’API externe :
>
>* Nombre maximal d’options : 2 000 (seules les 2 000 premières options uniques du JSON renvoyé sont affichées).
>* Délai d’expiration : 30 secondes
>* Nombre de reprises : 3
>* Durée d’attente entre les reprises : 500 ms
>* Statuts de la réponse attendue : 2xx

### Ajouter des images, des fichiers PDF et des vidéos


Vous pouvez ajouter des images, des PDF et des vidéos à un formulaire personnalisé. Les personnes qui travaillent avec l’objet auquel le formulaire personnalisé est attaché ne peuvent voir l’image, le PDF ou la vidéo que dans les zones suivantes :

* la zone Détails de l’objet (par exemple, pour un projet, la zone Détails du projet ).
* La zone d’édition de l’objet, s’il a la nouvelle apparence d’expérience Adobe Workfront (par exemple, les zones Modifier le projet et Modifier la tâche).

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ Développez pour afficher les descriptions des champs disponibles.

* **Image** : permet aux utilisateurs et utilisatrices d’ajouter des fichiers image.
* **PDF** : permet aux utilisateurs et utilisatrices d’ajouter des fichiers PDF.
* **Vidéos** : permet aux utilisateurs et utilisatrices d’ajouter des fichiers vidéo.

+++

Pour ajouter des images, des PDF ou des vidéos, procédez comme suit :

1. Dans l’onglet **Nouveau champ** sur le côté gauche de l’écran, recherchez l’un des champs suivants et faites-le glisser vers une section de la zone de travail.

   * Image
   * PDF
   * Vidéo

   ![Faire glisser le champ vers la section](assets/drag-field-to-section.png)

1. Saisissez ou modifiez l’une des propriétés suivantes du widget :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">Taille</td> 
      <td>(Facultatif) Modifiez la taille d’affichage du widget selon vos besoins.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du widget. Vous pouvez modifier le libellé à tout moment.</p> <p><b>Important</b> : évitez d’utiliser des caractères spéciaux dans ce libellé, car ils ne s’affichent pas correctement dans les rapports. Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom correspond à la manière dont le système identifie le widget. Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Les champs Libellé et Nom ne sont pas synchronisés. Vous avez ainsi la possibilité de modifier le libellé visible par vos utilisateurs et utilisatrices sans avoir à modifier le nom visible par le système.</p> <p>Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoire) Saisissez ou collez l’URL du widget où il est stocké sur Internet.</p> 
      <p>Si vous ajoutez un widget vidéo, vous pouvez le faire en ajoutant ce qui suit dans la zone URL :</p> 
      <ul> 
      <li> <p>Lien YouTube ou Vimeo</p> </li> 
      <li> <p>Lien vidéo Google Drive</p> </li> 
      <li> <p>Lien vers une vidéo avec les extensions MP4 et MOV</p> </li> 
      <li> <p>Lien vers une vidéo déjà chargée dans la zone Documents de votre instance Workfront. Pour obtenir des instructions, voir <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Ajouter un widget vidéo à un formulaire personnalisé à partir de la zone Documents</a> dans cet article.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le widget. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.</p> </td> 
     </tr> 
     <tr>
      <td>Actif</td>
      <td><p>Cette option est activée par défaut.<p><p>Lorsque vous définissez un champ comme Inactif, il est exclu des rapports, filtres et affichages et n’est plus disponible dans la bibliothèque de champs de formulaires personnalisés.</p></td>
     </tr>
    </tbody> 
   </table>

   >[!NOTE]
   >Pour les PDF, il est recommandé d’utiliser Grand pour la taille d’affichage du widget.
   >La visionneuse PDF d’un navigateur affecte l’affichage pour les utilisateurs et utilisatrices, qui peuvent être amenés à ajuster la taille de la fenêtre et le pourcentage de zoom du navigateur si l’affichage de PDF n’est pas optimal.

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   Ou

   Pour copier un champ, pointez dessus et cliquez sur l’icône de copie.

   ![icône de copie](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

#### Ajouter une vidéo à un formulaire personnalisé à partir de la zone Documents{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Lorsque vous ajoutez ainsi une vidéo à un formulaire personnalisé, les autorisations définies dans la zone Documents s’appliquent à la vidéo lorsque les utilisateurs accèdent au formulaire sur un objet.

1. Accédez à la vidéo dans la zone Documents et générez une épreuve, comme décrit dans [Créer une épreuve interactive pour un site web ou un autre contenu web](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Ouvrez l’épreuve.
1. Cliquez avec le bouton droit de la souris n’importe où sur la vidéo, puis sélectionnez **Copier l’adresse de la vidéo**.
1. Dans le formulaire personnalisé où vous ajoutez le widget vidéo, collez l’adresse copiée dans la zone **URL**.
1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

### Ajouter des champs natifs Workfront

Vous pouvez ajouter des champs natifs Workfront à vos formulaires personnalisés. Lorsque le formulaire personnalisé est joint à un objet, le champ est renseigné à partir des données de l’objet. Par exemple, le champ Description d’un formulaire personnalisé joint à un projet extrait la description du projet. (Le champ peut afficher « S.O. » si aucune donnée n’est disponible.)

+++ Développez pour afficher la liste des champs natifs pris en charge.

Ce tableau répertorie les champs natifs disponibles pour des objets Workfront spécifiques dans un formulaire personnalisé.

| Nom du champ | Projet | Tâche | Problème | Modèle | Tâche de modèle | Portfolio | Programme | Groupe |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| Date d’achèvement effective | ✓ | ✓ | ✓ |   |   |   |   |   |
| Durée effective | ✓ |   |   |   |   |   |   |   |
| Heures effectives | ✓ |   | ✓ |   |   |   |   |   |
| Date de début effective | ✓ | ✓ | ✓ |   |   |   |   |   |
| Entreprise | ✓ |   |   | ✓ |   |   |   |   |
| Condition | ✓ | ✓ | ✓ |   |   |   |   |   |
| Type de condition | ✓ |   |   | ✓ |   |   |   |   |
| Description | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Durée |   | ✓ |   |   | ✓ |   |   |   |
| Type de durée |   | ✓ |   |   | ✓ |   |   |   |
| Unité de durée |   | ✓ |   |   | ✓ |   |   |   |
| Entré par | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Date d’entrée | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Groupe | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Dernière mise à jour par | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Date de dernière mise à jour | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Nom | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Propriétaire | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Date d’achèvement prévue | ✓ | ✓ | ✓ |   |   |   |   |   |
| Durée prévue | ✓ |   |   | ✓ |   |   |   |   |
| Heures prévues | ✓ | ✓ | ✓ |   | ✓ |   |   |   |
| Date de début prévue | ✓ |   |   |   |   |   |   |   |
| Portfolio | ✓ |   |   | ✓ |   |   | ✓ |   |
| Priorité | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Programme | ✓ |   |   | ✓ |   |   |   |   |
| Date d’achèvement prévisionnelle | ✓ | ✓ |   |   |   |   |   |   |
| Durée prévisionnelle en minutes |   | ✓ |   |   |   |   |   |   |
| Date de début prévisionnelle | ✓ | ✓ |   |   |   |   |   |   |
| Numéro de référence | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Mode horaire | ✓ |   |   | ✓ |   |   |   |   |
| Gravité |   |   | ✓ |   |   |   |   |   |
| Sponsor | ✓ |   |   | ✓ |   |   |   |   |
| Statut | ✓ | ✓ |   |   |   |   |   |   |
| Points de l’histoire |   | ✓ |   |   |   |   |   |   |
| Modèle | ✓ |   |   |   |   |   |   |   |
| URL | ✓ | ✓ |   | ✓ | ✓ |   |   |   |

{style="table-layout:auto"}

+++

1. Dans l’onglet **Nouveau champ** sur le côté gauche de l’écran, recherchez **Référence de champ native** et faites-la glisser vers une section de la zone de travail.
1. Dans la partie droite de l’écran, configurez les options du champ personnalisé :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">Taille</td> 
      <td>(Facultatif) Modifiez la taille d’affichage du champ selon vos besoins.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ. Vous pouvez modifier le libellé à tout moment.</p> <p><b>Important</b> : évitez d’utiliser des caractères spéciaux dans ce libellé, car ils ne s’affichent pas correctement dans les rapports. Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td>
      <td> <p>(Obligatoire) Ce nom est la façon dont le système identifie le champ. Lorsque vous configurez le champ pour la première fois et que vous saisissez le libellé, le champ Nom est renseigné automatiquement pour correspondre à celui-ci. Les champs Libellé et Nom ne sont pas synchronisés. Vous avez ainsi la possibilité de modifier le libellé visible par vos utilisateurs et utilisatrices sans avoir à modifier le nom visible par le système.</p>
      <p>Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez toute information supplémentaire concernant le champ. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Champ de référence</td> 
      <td><p>(Obligatoire) Sélectionnez un champ natif Workfront.<p><p>Seuls les champs natifs des objets du formulaire sont disponibles. Par exemple, si la liste des types d’objets en haut du concepteur de formulaires affiche Projet, vous pourrez sélectionner des champs natifs pour les projets, mais pas des champs spécifiques aux tâches.</p></td>
     </tr>
     <tr>
      <td role="rowheader">Ajouter filtre</td>
      <td><p>Ajoutez un filtre pour le champ de référence afin de limiter la liste d’éléments que les utilisateurs peuvent choisir lorsqu’ils utilisent le champ. </p> <p>Par exemple, vous pouvez limiter un champ afin que les noms d’utilisateur ne puissent être sélectionnés que s’ils répondent aux critères suivants :</p> 
       <ul>
        <li>Ils appartiennent à un ou plusieurs groupes que vous spécifiez.</li> 
        <li>Ils sont associés à un rôle ou un titre de poste que vous spécifiez.</li> 
        <li>Ils appartiennent au même groupe que la personne qui utilise le champ .</li> 
       </ul>
       <p>Vous devez définir le filtre pour le champ de référence que vous avez sélectionné en utilisant la syntaxe du mode texte. Pour plus d’informations, voir <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Modification d’un filtre en mode texte</a>.</p>
       <p><b>Remarque </b> :
       <ul> 
        <li>L’option de filtre n’est disponible que lorsque vous référencez un champ de saisie semi-automatique natif, tel que Portfolio, Société ou Propriétaire.</li>
        <li>Si vous modifiez un formulaire personnalisé existant, l’ajout d’un filtre à un champ natif ne supprime aucun objet (hors de portée du filtre) que les utilisateurs ont déjà ajouté à l’aide du champ.</li> 
        <li>Ce filtre n’est pas disponible sur les appareils mobiles. Si vous utilisez le filtre pour un champ natif, le champ apparaîtra sur les appareils mobiles des utilisateurs non affectés par le filtre.</li> 
        </ul></p></td> 
      <td>
     </tr>
     <tr>
      <td>Actif</td>
      <td><p>Cette option est activée par défaut.<p><p>Lorsque vous définissez un champ comme Inactif, il est exclu des rapports, filtres et affichages et n’est plus disponible dans la bibliothèque de champs de formulaires personnalisés.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Créer un champ obligatoire</td>
      <td><p>Sélectionnez cette option si vous souhaitez que le champ soit obligatoire pour que l’utilisateur ou l’utilisatrice puisse remplir le formulaire personnalisé.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

### Ajouter des fichiers Adobe XD

Vous pouvez ajouter un prototype Adobe XD directement à un formulaire personnalisé. Les personnes qui travaillent avec l’objet auquel le formulaire personnalisé est attaché ne peuvent voir le fichier Adobe XD que dans les zones suivantes :

* Zone Détails de l’objet (par exemple, pour un projet, la zone Détails du projet)
* La zone Modifier de l’objet, si l’aspect de l’expérience Adobe Workfront est nouveau (par exemple, les zones Modifier le projet et Modifier la tâche).

Pour ajouter un fichier Adobe XD :

1. Dans l’onglet **Nouveau champ** sur la gauche de l’écran, recherchez **Adobe XD** et faites-le glisser vers une section de la zone de travail.
1. Saisissez ou modifiez l’une des propriétés suivantes du widget :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">Taille</td> 
      <td>(Facultatif) Modifiez la taille d’affichage du widget selon vos besoins.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du widget. Vous pouvez modifier le libellé à tout moment.</p> <p><b>Important</b> : évitez d’utiliser des caractères spéciaux dans ce libellé, car ils ne s’affichent pas correctement dans les rapports. Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom correspond à la manière dont le système identifie le widget. Lorsque vous configurez le widget pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Les champs Libellé et Nom ne sont pas synchronisés. Vous avez ainsi la possibilité de modifier le libellé visible par vos utilisateurs et utilisatrices sans avoir à modifier le nom visible par le système.</p>
    <p>Pour plus d’informations, voir <a href="design-a-form.md#notes-on-field-names-and-labels">Notes sur les noms et étiquettes des champs</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoire) Saisissez ou collez un lien de prototype XD valide.</p> 
      <p><b>Remarque </b> : le paramètre Accès aux liens de l’onglet Partager dans Adobe XD doit être défini sur Toute personne disposant du lien. Sinon, les utilisateurs et utilisatrices ne pourront pas afficher le prototype. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le widget. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr>
     <tr>
      <td>Actif</td>
      <td><p>Cette option est activée par défaut.<p><p>Lorsque vous définissez un champ comme Inactif, il est exclu des rapports, filtres et affichages et n’est plus disponible dans la bibliothèque de champs de formulaires personnalisés.</p></td>
     </tr>
    </tbody> 
   </table>

1. (Facultatif) Répétez l’étape précédente pour ajouter d’autres champs ou widgets.

   Ou

   Pour copier un champ, pointez dessus et cliquez sur l’icône de copie.

   ![icône de copie](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

### Ajouter des champs de connexion Planning

>[!IMPORTANT]
>
>Les informations de cette section font référence à Adobe Workfront Planning, une fonctionnalité supplémentaire d’Adobe Workfront.
>
>Vous devez disposer de packages supplémentaires pour accéder à Workfront Planning.
>
>Pour obtenir la liste complète des conditions requises pour accéder à Workfront Planning, consultez la [présentation de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Pour plus d’informations sur Workfront Planning, voir [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Vous pouvez afficher les enregistrements connectés à partir de Workfront Planning dans un champ personnalisé sur un objet Workfront en ajoutant un champ personnalisé de connexion Planning au formulaire personnalisé d&#39;un objet.

Vous pouvez ajouter le champ de connexion Planning aux formulaires personnalisés de tous les objets. Cependant, vous ne pouvez afficher les enregistrements connectés que sur les formulaires personnalisés associés aux objets Workfront qui peuvent être connectés à partir de Workfront Planning.

>[!NOTE]
>
>Les utilisateurs qui consultent des informations dans le champ personnalisé doivent avoir accès à Workfront Planning et aux espaces de travail qui contiennent les types d’enregistrements connectés aux objets Workfront.

Pour ajouter un champ de connexion Planning :

1. Dans l’onglet **Nouveau champ** sur le côté gauche de l’écran, recherchez **Connexion Planning** et faites-la glisser vers une section de la zone de travail.
1. Dans la partie droite de l’écran, configurez les options du champ personnalisé :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Taille</td> 
      <td>(Facultatif) Modifiez la taille d’affichage du widget selon vos besoins.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ. Vous pouvez modifier le libellé à tout moment.</p> <p><b>Important</b> : évitez d’utiliser des caractères spéciaux dans ce libellé.</p> 
      <p>Nous vous recommandons de choisir un libellé qui vous aide à identifier facilement la provenance de l'enregistrement Planning. Ajoutez des informations telles que le nom de l’espace de travail ou le nom du type d’enregistrement. </p>   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td>
      <td> <p>(Obligatoire) Le nom correspond à la manière dont le système identifie le champ. Lorsque vous configurez le champ pour la première fois et que vous saisissez le libellé, le champ Nom est renseigné automatiquement pour correspondre à celui-ci. Les champs Libellé et Nom ne sont pas synchronisés. Vous avez ainsi la possibilité de modifier le libellé visible par vos utilisateurs et utilisatrices sans avoir à modifier le nom visible par le système.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>(Recommandé) Saisissez des informations supplémentaires sur le champ. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.</p>
      <p>Ici, vous pouvez ajouter des informations détaillées sur l’enregistrement et les objets que vous connectez. </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type d’objet</td> 
      <td><p>(Obligatoire) Sélectionnez un type d'objet Workfront connecté à un type d'enregistrement dans Workfront Planning.</p>
      Vous pouvez effectuer une sélection parmi les types d’objets suivants :
      <ul><li> Projet</li>
      <li> Portfolio</li><li> Programme</li><li> Entreprise</li><li> Groupe</li></ul>
       <p>Seuls les types d’objet Workfront pour les types d’objet de formulaire sont disponibles.</p> <p> Par exemple, si la liste Types d’objet en haut du concepteur de formulaire affiche Projet, vous pouvez uniquement sélectionner Projet dans ce champ et non Portfolios, bien que les portfolios puissent également être connectés à des types d’enregistrement.</p>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Espace de travail</td> 
      <td> <p>(Obligatoire) Sélectionnez l’espace de travail Planning d’où proviennent les enregistrements à afficher dans Workfront.</p> <p> Seuls les espaces de travail connectés aux types d'objet que vous avez sélectionnés dans le champ Type d'objet s'affichent. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type d’enregistrement</td> 
      <td><p>(Obligatoire) Sélectionnez le type d’enregistrement Workfront Planning ayant une connexion avec le type d’objet Workfront.</p><p>Seuls les types d’enregistrement ayant des connexions avec le type d’objet que vous avez sélectionné dans le champ Type d’objet s’affichent. </p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Champ de connexion</td> 
      <td><p>(Obligatoire) Sélectionnez le champ de connexion entre le type d'enregistrement Planning sélectionné que vous souhaitez afficher dans les objets Workfront et le type d'objet Workfront. </p> <p> <b>Remarque </b> : vous pouvez avoir plusieurs champs de connexion entre le même objet et les mêmes types d’enregistrement, mais vous ne pouvez sélectionner qu’un seul champ.</p>  </td> 
     </tr>

<tr> 
      <td role="rowheader">Champs des types d’enregistrements</td> 
      <td><p>(Facultatif) Sélectionnez jusqu’à 7 champs de recherche à partir du type d’enregistrement connecté à afficher dans le formulaire personnalisé. Le champ principal est sélectionné par défaut et ne peut pas être modifié. </p> <p> Les champs de l’enregistrement connecté que vous sélectionnez s’affichent dans une vue de tableau sur le formulaire personnalisé. Lorsque le formulaire est joint à un objet Workfront, la vue Tableau est en lecture seule. </p>  
    <img src="assets/planning-connections-field-with-table-on-form-preview.png"></td> 
     </tr>
     <tr>
      <td>Actif</td>
      <td><p>Cette option est activée par défaut.<p><p>Lorsque vous définissez un champ comme Inactif, il est exclu des rapports, filtres et affichages et n’est plus disponible dans la bibliothèque de champs de formulaires personnalisés.</p></td>
     </tr>
      </tbody> 
   </table>

1. (Facultatif) Répétez les étapes précédentes pour ajouter d’autres champs.

   Ou

   Pour copier un champ, pointez dessus et cliquez sur l’icône de copie.

   ![icône de copie](assets/copy-field.png)

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et passez à une autre section pour continuer à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

   Vous pouvez désormais joindre le formulaire à un objet connecté à partir de Workfront Planning et effectuer l&#39;une des opérations suivantes :

   * Affichez les types d’enregistrements Workfront Planning connectés à l’objet Workfront, le cas échéant.
   * Connecter ou déconnecter des enregistrements de l’objet Workfront.

   Pour plus d’informations, voir [Gérer les connexions d’enregistrement à partir d’objets Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md)

### Ajouter des extensions d’interface utilisateur

Une application peut être incorporée dans un formulaire personnalisé Workfront à l’aide du type de champ Extensions de l’interface utilisateur . Pour créer des extensions d’interface utilisateur, vous devez avoir accès à Adobe App Builder dans Adobe Developer Console. Pour plus d’informations, consultez la section [Incorporer une application à l’aide d’un formulaire personnalisé Workfront](/help/quicksilver/app-builder/app-builder.md#embed-an-app-using-a-workfront-custom-form) dans l’article [Créer des applications personnalisées pour Workfront avec Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Organiser et prévisualiser un formulaire avec le concepteur de formulaire

Pour plus d’informations sur l’organisation d’un formulaire personnalisé avec des sauts de section et consulter un aperçu du formulaire, voir [Organisation et prévisualisation d’un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).



