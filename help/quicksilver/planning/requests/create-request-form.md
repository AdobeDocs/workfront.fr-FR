---
title: Création et gestion d’un formulaire de demande dans Adobe Workfront Planning
description: Après avoir sélectionné un type d’enregistrement dans la zone Adobe Workfront Planning, vous pouvez créer un formulaire de demande et l’associer à ce type d’enregistrement. Vous pouvez ensuite partager un lien vers celle-ci avec d’autres utilisateurs internes ou externes. Les utilisateurs disposant d’un lien vers le formulaire peuvent remplir les valeurs de champ et, en l’envoyant, ajouter un nouvel enregistrement pour le type d’enregistrement qui y est associé.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: a8d2447eea4ca8d814035d183f40921cad49a0d8
workflow-type: tm+mt
source-wordcount: '2184'
ht-degree: 8%

---

# Création et gestion d’un formulaire de demande dans Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Vous pouvez créer un formulaire de demande et l&#39;associer à un type d&#39;enregistrement dans Adobe Workfront Planning. Vous pouvez ensuite partager un lien vers celle-ci avec d’autres utilisateurs internes ou externes.

Les utilisateurs disposant d’un lien vers le formulaire peuvent mettre à jour les valeurs de champ et ajouter de nouveaux enregistrements en l’envoyant.

Cet article décrit comment un gestionnaire d’espace de travail peut créer un formulaire de demande associé à un type d’enregistrement.

Pour plus d’informations sur la soumission d’une demande à un type d’enregistrement pour créer un enregistrement, voir [ Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produits</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Planification d’Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td>
   <td>
<p>L’un des plans Workfront suivants :</p>
<ul><li>Sélectionner</li>
<li>Principal</li>
<li>Final</li></ul>
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p>
   </td>

<tr>
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td>
   <td>
<p>Tous </p>  
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </td>

<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td>
   <ul>
   <li><p>Gestion des autorisations relatives à un espace de travail <!--<span class="preview">and record type</span>--> </p></li>
    <li><p>L’administration système peut gérer les espaces de travail qu’elle n’a pas créés. </p></li>
    </ul>
   <p>Pour plus d’informations sur les autorisations de partage pour les objets Workfront Planning, voir <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning</a>. 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p>  
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limites d’affichage des champs et des valeurs dans les formulaires de demande

Il existe des limitations dans l’affichage de certains champs sur le formulaire de demande et dans l’affichage ultérieur de leurs valeurs sur les enregistrements ou la page des détails de la demande, après l’envoi d’une demande.

Pour plus d’informations sur l’envoi de demandes Workfront Planning, voir [Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

* Vous trouverez ci-dessous les limites d’affichage de certains champs dans les formulaires de demande, les enregistrements créés par un formulaire de demande ou sur la page des détails de la demande :

   * Vous ne pouvez pas ajouter de champs des types suivants à un formulaire de demande :

      * Créé par et Dernière modification par
      * Date de création et date de dernière modification
      * Formule. <span class="preview">Les champs de formule sont pris en charge dans l’environnement Aperçu.</span>
      * Champs de recherche d’objets Workfront
      * Champs de recherche des enregistrements connectés de Workfront Planning

* Voici les différences entre la façon dont les formats de champ s’affichent dans le créateur de formulaires de demande et la façon dont les valeurs des champs sont formatées dans l’enregistrement ou dans la page des détails de la demande :

   * Les champs Devise, Nombre et Pourcentage s’affichent sous la forme d’un type de champ de texte monoligne dans le créateur de formulaires.

     Cependant, le format des champs est conservé et les valeurs des champs s’affichent sous la forme de devise, de nombres et de pourcentages une fois la demande soumise, sur le type d’enregistrement et dans la page des détails de la demande.

<div class="preview">

* Vous trouverez ci-dessous une description de l’affichage de certaines valeurs de champ dans les formulaires de demande et les pages de détails de la demande :

   * Le formatage spécial des champs Devise, Nombre et Pourcentage n’est pas conservé. Par exemple, la précision décimale n’est pas conservée pour les valeurs de ces champs dans ces zones.
   * Les valeurs des champs Personnes s’affichent sous la forme d’identifiants.
   * Les champs de formule qui ne font pas référence à d’autres champs ou calculs n’affichent aucune valeur. Par exemple, un champ avec une formule `STRING` affiche une valeur « N/A ».
   * Les champs de formule qui font référence à des champs Devise affichent les valeurs sans tenir compte des taux de change.
   * Les valeurs des champs de paragraphe affichent une valeur « S/O » sur le formulaire de demande et affichent des balises HTML au lieu du texte formaté dans la page des détails de la demande.

</div>

## Création d’un formulaire de demande pour un type d’enregistrement

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails. Pour plus d’informations sur la création d’un type d’enregistrement, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page du type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type d’enregistrement s’ouvre en mode Tableau.

1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Créer un formulaire de demande** <span class="preview">ou **Gérer les formulaires de demande**, si vous disposez déjà d’un formulaire et que vous souhaitez en créer d’autres</span>.
1. <span class="preview">(Conditionnel) Si vous souhaitez ajouter un autre formulaire, cliquez sur **Nouveau formulaire de demande**</span>.
1. Mettez à jour le nom du formulaire de demande. Par défaut, le nom du formulaire est **Formulaire sans titre**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Facultatif) Ajoutez une **Description** pour le formulaire de demande.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Cliquez sur **Créer**. Le formulaire de demande pour le type d’enregistrement sélectionné s’ouvre dans l’onglet Formulaire .

   ![Mode de modification du formulaire de demande de campagne](assets/campaigns-request-form-edit-mode.png)

   Le formulaire de demande contient par défaut les informations suivantes :

   * Champs d’enregistrement disponibles dans la vue Tableau du type d’enregistrement sélectionné. <!--they are working on removing the limitation below-->

   * **Section par défaut** : il s’agit du saut de section par défaut que Workfront applique au formulaire de demande. Tous les champs d’enregistrement s’affichent dans la zone **Section par défaut**.
   * Champ **Subject** : champ qui identifiera la demande dans Workfront. La configuration et la valeur du champ Objet ne sont pas modifiables.

     >[!NOTE]
     >
     >* Le champ **Objet** nécessite une valeur lorsqu’il est visible sur le formulaire de demande. Cependant, vous pouvez supprimer le champ **Objet** si nécessaire, et les demandeurs ne le verront pas dans le formulaire lorsqu’ils soumettent la demande.
     >* Lorsque le champ Objet est manquant dans un formulaire de demande, mais qu&#39;il existe un champ Nom pour le nom de l&#39;enregistrement futur, le nom de la demande est automatiquement attribué au même nom que l&#39;enregistrement créé.
     >* Lorsque les champs Objet et Nom sont manquants dans le formulaire de demande, la demande est nommée selon le modèle suivant : `< Record name > request form < Entry date of the request >` ; l’enregistrement est nommé **Sans titre**.

   * Tous les champs associés au type d’enregistrement.

     Les champs contenus dans le formulaire de demande seront visibles pour toutes les personnes soumettant une demande à ce type d&#39;enregistrement.

1. (Facultatif) Pointez sur un champ du formulaire à supprimer, puis cliquez sur l’icône **x** pour le supprimer. Elles sont ajoutées à l’onglet **Champs** situé à gauche du formulaire.

   Par exemple, supprimez le champ **Objet**, car il n’est pas visible dans Workfront Planning. <!--remove this example if this becomes visible in Planning?-->

1. (Facultatif) Pour supprimer la **section Par défaut** du formulaire, procédez comme suit :

   1. Supprimez tous les champs de la section Par défaut.
   1. Cliquez sur **Éléments de contenu** et ajoutez une nouvelle section, puis ajoutez un nom pour la section.
   1. Ajoutez des champs à la nouvelle section.
   1. Cliquez sur l’icône **x** pour supprimer la **section par défaut**.
1. Cliquez sur n’importe quel champ, puis utilisez les commandes du panneau de droite du formulaire pour définir leur taille ou l’une des informations suivantes :

   * **Libellé** : il s&#39;agit du nom du champ tel qu&#39;il apparaîtra sur le formulaire de demande. Le nom du champ d’enregistrement n’est pas modifié.
   * **Instructions** : ajoutez plus d’informations sur le champ .
   * **Rendre un champ obligatoire** : lorsqu’il est sélectionné, le champ doit avoir une valeur. Dans le cas contraire, le formulaire ne peut pas être envoyé.
   * **Ajouter une logique** : définissez les conditions qui doivent être remplies pour que le champ s’affiche ou soit masqué.

   >[!TIP]
   >
   >   Le type de champ de chaque champ s’affiche dans la partie supérieure du panneau de droite, une fois que vous avez sélectionné le champ dans le formulaire.
   >     

1. (Facultatif) Cliquez sur l’onglet **Éléments de contenu** sur le côté gauche du formulaire, puis ajoutez l’un des éléments suivants :

   * **Texte descriptif**
   * **Saut de section**

   Pour plus d’informations sur la création d’un formulaire personnalisé, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Facultatif) Cliquez sur **Aperçu** pour voir comment le formulaire s’affichera pour les autres utilisateurs lorsqu’ils l’utiliseront pour envoyer un nouvel enregistrement.

1. (Facultatif) Cliquez sur l’onglet **Configuration**, puis ajoutez au moins un utilisateur au champ **Approbateurs** pour approuver de nouvelles demandes pour ce formulaire d’enregistrement.

   ![Onglet Configuration](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Lorsque vous associez un formulaire de demande à des approbateurs, toute nouvelle demande doit d&#39;abord être approuvée par tous les approbateurs avant de générer un nouvel enregistrement.
   * Vous pouvez ajouter un ou plusieurs approbateurs à un formulaire de demande.
   * Si au moins un approbateur rejette la demande, celle-ci est rejetée et l&#39;enregistrement n&#39;est pas créé.
   * Tous les approbateurs doivent prendre une décision avant qu&#39;une demande ne soit approuvée ou rejetée.

     Pour plus d’informations sur l’ajout d’approbations à des formulaires de demande, voir [ Ajouter une approbation à un formulaire de demande ](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Facultatif) Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du formulaire dans l’en-tête, puis cliquez sur **Modifier** pour mettre à jour le nom du formulaire.
1. Cliquez sur **Publier** pour publier le formulaire et obtenir un lien unique pour celui-ci.

   Les événements suivants se produisent :

   * Le bouton **Publier** est supprimé.
   * Le bouton **Dépublier** est ajouté au formulaire. Cliquez dessus pour empêcher l’accès au formulaire.
   * Un bouton **Partager** est ajouté au formulaire.

1. Cliquez sur **Partager** pour partager le formulaire avec d’autres personnes.

   ![Zone de partage pour le formulaire de demande](assets/share-box-for-request-form.png)

1. Sélectionnez l’une des options suivantes pour indiquer quels types d’utilisateurs peuvent accéder à ce formulaire :

   * Toute personne disposant d’un accès en affichage ou supérieur à l’espace de travail
   * Toute personne disposant d’un accès en contribution ou supérieur à l’espace de travail
   * Toute personne disposant du lien

   >[!WARNING]
   >
   >* Lorsque vous sélectionnez **Personne disposant du lien**, n’importe qui peut accéder au formulaire et envoyer un nouvel enregistrement, même les personnes extérieures à votre organisation qui ne disposent pas d’un compte Workfront.
   >
   >* Un formulaire contenant les types de champs suivants ne peut pas être partagé publiquement :
   >
   >     * Connexions Workfront ou AEM Assets
   >     * Personnes
   >

1. (Conditionnel) Si vous avez sélectionné **Personne disposant du lien** à l’étape précédente, sélectionnez la **Date d’expiration du lien** dans le calendrier disponible. <!--take out this tip when we release to production as in multiple forms this is no longer happening-->

   >[!TIP]
   >
   >Lorsque c’est le cas, cela indique que le lien est partagé publiquement.
   >![Lien partagé publiquement vers le formulaire dans le menu de type enregistrement](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)

   Les personnes recevront une erreur après l’expiration du lien et vous devez mettre à jour la date du lien et générer un nouveau lien à partager avant que les personnes puissent à nouveau accéder au formulaire.

   Vous pouvez sélectionner des dates futures dans les 180 jours à compter de la date actuelle.

   >[!TIP]
   >
   ><span class="preview">À l’expiration de la date de partage, le formulaire de demande n’est plus disponible dans la zone des Demandes de Workfront et les liens partagés avec d’autres utilisateurs ne sont plus accessibles.</span>


1. <span class="preview">(Facultatif)</span> Cliquez sur **Enregistrer et copier le lien** pour enregistrer les détails de partage du formulaire. Si le formulaire a été précédemment enregistré, cliquez sur **Copier le lien**.

   Les options de partage de formulaire sont enregistrées et le lien est copié dans le presse-papiers. Vous pouvez maintenant le partager avec d’autres personnes.

   Pour plus d&#39;informations sur la création d&#39;enregistrements à l&#39;aide d&#39;un lien vers un formulaire de demande, voir [Soumettre des demandes Adobe Workfront Planning](/help/quicksilver/planning/requests/submit-requests.md).

1. Cliquez sur **Enregistrer** dans le coin inférieur droit de l’onglet **Formulaire** pour enregistrer le formulaire.

1. Cliquez sur la flèche pointant vers la gauche du nom du formulaire dans l’en-tête pour fermer le formulaire.

   <span class="preview">La vue de tableau **Formulaires de demande** s’ouvre et le formulaire y est ajouté.</span>

1. <span class="preview">(Facultatif) Passez la souris sur le nom d’un formulaire de demande en mode Tableau, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du formulaire, et cliquez sur l’une des options suivantes :</span>

   * <span class="preview">**Modifier le formulaire** : cliquez sur cette option pour modifier davantage les informations du formulaire. </span>
   * <span class="preview"> **Dépublier** : cliquez sur cette option pour dépublier le formulaire et le supprimer de la zone des Demandes dans Workfront. </span>
   * <span class="preview">**Partager** : cliquez sur cette option pour modifier la personne qui a accès au formulaire. </span>
   * <span class="preview">**Copier le lien** : cliquez sur cette option pour copier rapidement le lien du formulaire de demande sans ouvrir le formulaire. </span>
   * <span class="preview">**Supprimer** : cliquez sur cette icône pour supprimer le formulaire. Toutes les demandes et tous les enregistrements ajoutés à l’aide du formulaire ne sont pas supprimés. Le formulaire ne peut pas être récupéré. </span>

   ![Menu Plus sur le formulaire de demande de la liste des formulaires de demande](assets/more-menu-on-request-form-from-request-forms-list.png)


1. <span class= "preview">Cliquez sur la flèche pointant vers la gauche de **Formulaires de demande** dans l’en-tête pour fermer le tableau des formulaires de demande.   </span>

   <span class= "preview">La page de type d’enregistrement s’ouvre. </span>
1. (Facultatif et conditionnel) Pour modifier un formulaire existant, effectuez l’une des opérations suivantes, en fonction de l’environnement utilisé :

   * Dans l’environnement de production :

      1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement dans l’en-tête, puis effectuez l’une des opérations suivantes :

      1. Cliquez sur **Mettre à jour le formulaire de demande** pour apporter des modifications au formulaire de demande.
      1. Cliquez sur **Copier le lien pour demander un formulaire** pour partager le lien vers le formulaire avec d’autres personnes.

   * <span class="preview">Dans l’environnement de prévisualisation :

      1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement dans l’en-tête, puis cliquez sur **Gérer les formulaires de demande**. </span>

         <span class="preview">Cette action ouvre la vue du tableau Formulaires de demande . </span>

      1. <span class="preview">Cliquez sur un formulaire de demande pour l’ouvrir et le modifier.</span>
      1. <span class= "preview">(Facultatif) Accédez à la zone **Demandes** dans Workfront et recherchez le formulaire partagé pour envoyer une demande. Pour plus d’informations, voir [Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).</span>
