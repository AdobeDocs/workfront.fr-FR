---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Ajouter un champ personnalisé à un formulaire personnalisé avec le créateur de formulaire hérité
description: Lorsque vous travaillez sur un formulaire personnalisé, vous pouvez créer un champ personnalisé et l’ajouter au formulaire personnalisé. Vous pouvez également ajouter un champ personnalisé déjà ajouté à un autre formulaire personnalisé.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 99%

---

# Ajouter un champ personnalisé à un formulaire personnalisé avec le créateur de formulaire hérité

<!-- Audited: 02/2024 -->

{{form-designer-default}}

Lorsque vous travaillez sur un formulaire personnalisé, vous pouvez créer un champ personnalisé et l’ajouter au formulaire personnalisé.

Vous pouvez également ajouter un champ personnalisé déjà ajouté à un autre formulaire personnalisé. Pour obtenir des instructions, voir [Réutiliser un champ ou un widget personnalisé dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

Pour plus d’informations sur l’ajout d’un widget de ressource à un formulaire personnalisé, processus similaire à l’ajout d’un champ personnalisé, voir [Ajouter ou modifier un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>Dans un formulaire personnalisé contenant un grand nombre de champs personnalisés ou de nombreuses options à choix multiples dans des champs personnalisés, les performances risquent d’être plus lentes lors de l’ajout ou de la modification de valeurs dans ces champs. Par exemple, un formulaire contenant 100 champs personnalisés ou des champs personnalisés à choix multiples avec plus de 200 options peut occasionner des interactions plus lentes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Forfait Adobe Workfront</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouvelle : standard</p>
   <p>ou</p>
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td>Accès administratif aux formulaires personnalisés </td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter un champ personnalisé à un formulaire personnalisé {#add-custom-field-to-custom-form}

1. Commencez à créer ou modifier un formulaire personnalisé, comme décrit dans la section [Créer ou modifier un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Sélectionnez l’onglet **Ajouter un champ**.

   ![Ajouter un onglet de champ](assets/add-a-field.jpg)

1. Avec **Nouveau champ** l’icône ![Nouveau champ](assets/new-field.jpg) sélectionnée, sélectionnez l’un des types de champ suivants :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Zone de texte à ligne simple</td> 
      <td>Permet de saisir une seule ligne de texte dans le champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zone de texte</td> 
      <td>Permet de saisir plusieurs lignes de texte dans le champ.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Champ de texte avec mise en forme</td> 
      <td>Permet de saisir plusieurs lignes de texte dans le champ et de mettre en forme le texte (gras, italique, souligné, puces, numérotation, liens hypertexte et guillemets) Cette option est disponible dans la section Accueil, la zone Mises à jour, les listes et la zone Détails des objets Workfront. La limite de 15 000 caractères permet d’utiliser du texte et des mises en forme variés.</p> <p>Ce type de champ personnalisé n’est pas pris en charge dans les filtres sur les listes et les rapports.</p> <p>Pour plus d’informations sur l’accès à ce champ par le biais de l’API, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">Stockage de champs de texte enrichi dans l’API</a>.</p> <p><b>NOTE</b> : les champs de texte avec mise en forme ne sont pas disponibles pour les applications mobiles Workfront. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Menu déroulant</td> 
      <td>Fournit une liste des choix sous forme de liste déroulante.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frappe continue </td> 
      <td>Permet de saisir le nom d’un objet existant dans Workfront. Une liste de suggestions s’affiche lorsque la personne commence à saisir du texte.
      Ce type de champ prend en charge les objets suivants :
      <ul><li>l’utilisateur ou de l’utilisatrice</li>
      <li>Groupe</li>
      <li>Fonction</li>
      <li>Portfolio</li>
      <li>Programme</li>
      <li>Projet</li>
      <li>Equipe</li>
      <li>Modèle</li>
      <li>Entreprise</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calculé</td> 
      <td>Permet de définir une expression et d’afficher le résultat sur le formulaire personnalisé. Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Ajouter des données calculées à un formulaire personnalisé</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date</td> 
      <td>Affiche un calendrier permettant de sélectionner une date et une heure.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cases à cocher</td> 
      <td>Permet de sélectionner plusieurs choix.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cases d’option</td> 
      <td>Les personnes ne peuvent effectuer qu’une seule sélection.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texte descriptif</td> 
      <td>Permet d’inclure des instructions et de créer des liens vers des pages en dehors de Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Saut de section</td> 
      <td>Un saut de section ne constitue pas un champ. Vous pouvez utiliser un saut de section pour organiser vos champs et widgets personnalisés en sections et, si nécessaire, configurer différentes autorisations d’affichage et de modification pour chaque section. Pour plus d’informations sur l’ajout et la configuration des sauts de section, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Ajouter un saut de section à un formulaire personnalisé</a>.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Les champs qui autorisent plusieurs sélections, tels que la case à cocher et la liste déroulante, sont difficiles à illustrer et à regrouper dans les rapports. Pour simplifier la création de graphiques et de regroupements dans les rapports, vous pouvez créer des champs distincts pour chaque choix (par exemple, un champ de texte d’une seule ligne).

1. Dans l’onglet **Paramètres des champs**, configurez les options disponibles pour le type de champ personnalisé que vous ajoutez :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ personnalisé. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b> : évitez d’utiliser des caractères spéciaux dans cette étiquette. Ils ne s’affichent pas correctement dans les rapports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom est la manière dont le système identifie le champ personnalisé lorsque vous l’ajoutez à différentes zones dans Workfront, telles que les rapports, l’accueil et les interactions avec l’API.</p> <p>Lorsque vous configurez le champ personnalisé pour la première fois et que vous saisissez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la liberté de modifier le libellé que vos utilisateurs et utilisatrices voient sans avoir à modifier le nom que le système voit.</p> 
      <p><b>IMPORTANT</b> :   
      <ul> 
      <li>Bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom si vous ou d’autres personnes utilisez le formulaire personnalisé dans Workfront. Dans le cas contraire, le système ne reconnaîtra plus le champ personnalisé lorsqu’il sera référencé dans d’autres zones de Workfront. <p>Par exemple, si vous ajoutez le champ personnalisé à un rapport et que vous changez ensuite son nom, Workfront ne le reconnaîtra pas dans le rapport et il cessera de fonctionner correctement, à moins que vous ne l’ajoutiez à nouveau au rapport en utilisant le nouveau nom.</p> </li>
      <li> <p>Nous vous recommandons de ne pas saisir un nom qui est déjà utilisé pour des champs Workfront intégrés.</p> </li>
      <li><p>Nous vous recommandons de ne pas utiliser le caractère « point » dans le nom du champ personnalisé, afin d’éviter les erreurs lors de l’utilisation du champ dans différentes zones de Workfront.</p></li>
      </ul> <p>Chaque nom de champ personnalisé doit être unique dans l’instance Workfront de votre entreprise. Vous pouvez ainsi en réutiliser un déjà créé pour un autre formulaire personnalisé. Pour plus d’informations, voir <a href="#add-a-custom-field-to-a-custom-form">Ajouter un champ personnalisé à un formulaire personnalisé</a> dans cet article.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le champ personnalisé. Lorsque les personnes remplissent le formulaire personnalisé, ils peuvent pointer sur l’icône en forme de point d’interrogation pour afficher une info-bulle contenant les informations que vous saisissez ici.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>Sélectionnez le type de données qui sera capturé dans le champ personnalisé. Vous pouvez modifier le format de sélection après l’enregistrement du formulaire, mais le nouveau format doit prendre en charge la valeur saisie.</p>

   <p><strong>Exemple :</strong> si vous enregistrez une valeur numérique pour un champ au format Texte sur au moins un objet et que vous modifiez ensuite le format en Nombre ou Devise, aucune erreur ne se produira. </p>
      <p>Cependant, si vous enregistrez une valeur alphanumérique dans un champ au format Texte sur au moins un objet et que vous essayez ensuite de modifier le format en Nombre ou Devise, une erreur se produira, car la valeur alphanumérique enregistrée n’est pas compatible avec les formats Nombre ou Devise. </p>

   <p><strong>Note :</strong> la limite de caractères pour les champs Nombre est de 16. Vous pouvez également utiliser un champ Texte pour saisir des nombres et éviter la limite.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type d'affichage</td> 
      <td>(Menu déroulant, cases à cocher et boutons radio uniquement) Modifiez le type de sélection d’option souhaité pour le champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taille</td> 
      <td>(Champs de texte uniquement) Sélectionnez une largeur pour le champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher l'heure</td> 
      <td>(Champs de date uniquement) Sélectionnez cette option pour afficher l’heure et la date dans le champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type d'objet référencé</td> 
      <td> <p>(Champ de saisie automatique uniquement) Sélectionnez le type d’objet à associer au champ.</p> <p>Une fois que vous avez cliqué sur Appliquer ou sur Enregistrer+Fermer, vous ne pouvez pas modifier le type d’objet du champ.</p> <p><b>NOTE</b> :   
        <ul> 
         <li>Si votre administration Workfront a personnalisé le nom des portfolios, programmes ou projets dans l’interface utilisateur de Workfront, le nom Workfront par défaut de l’objet s’affiche dans cette liste déroulante et non dans le nom personnalisé. Contactez votre équipe d’administration Workfront si vous avez besoin d’aide.<br></li> 
         <li>Les types d’objets suivants sont pris en charge dans les applications mobiles iOS et Android Workfront : utilisateur/utilisatrice, entreprise, groupe, fonction, portfolio, programme, projet et modèle.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ajouter filtre</td> 
      <td> <p>(Champ de saisie automatique uniquement) Ajoutez un filtre pour un type d’objet afin de limiter les objets que les personnes peuvent sélectionner lorsqu’elles utilisent le champ. </p> <p>Par exemple, vous pouvez limiter un champ afin que les noms d’utilisateur et d’utilisatrice ne puissent être sélectionnés que s’ils répondent aux critères suivants :</p> 
       <ul> 
        <li>Ils appartiennent à un ou plusieurs groupes que vous spécifiez.</li> 
        <li>Ils sont associés à un rôle ou à un titre de poste que vous spécifiez.</li> 
        <li>Ils appartiennent au même groupe que la personne qui utilise le champ.</li> 
       </ul> <p>Vous devez définir le filtre correspondant au type d’objet sélectionné à l’aide de la syntaxe Mode texte. Pour plus d’informations sur la création d’un filtre à l’aide du mode Texte, voir <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modifier un filtre en mode texte</a>.</p>
       <p><b>NOTE</b> :   
        <ul> 
         <li>Si vous modifiez un formulaire personnalisé existant, l’ajout d’un filtre à un champ de type anticipée ne supprime aucun objet (hors portée du filtre) déjà ajouté par les personnes à l’aide du champ.</li> 
         <li>Ce filtre n’est pas disponible sur les appareils mobiles. Si vous utilisez le filtre pour un champ de frappe continue, il apparaîtra sur les appareils mobiles des personnes qui ne sont pas affectées par le filtre.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texte descriptif</td> 
      <td>(Champs de texte descriptif uniquement) Saisissez le texte que vous souhaitez afficher pour fournir des instructions ou un lien sur le formulaire personnalisé. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lien hypertexte</td> 
      <td>(Champs de texte descriptif uniquement) Si vous souhaitez appliquer un lien hypertexte au texte descriptif que vous avez saisi, ajoutez-le ici.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Créer un champ obligatoire</td> 
      <td>Sélectionnez cette option si vous souhaitez que le champ soit obligatoire pour que l’utilisateur ou l’utilisatrice puisse remplir le formulaire personnalisé. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suivre les modifications de champ dans les messages de mise à jour</td> 
      <td><p>Cliquez dans la liste déroulante, puis sélectionnez les types d’objets pour lesquels effectuer automatiquement le suivi des modifications de valeur du champ.</p> 
      <p><b>NOTE</b> : cette option n’est pas disponible pour les éléments suivants :</p> 
      <ul> 
      <li>Formulaires personnalisés associés aux types d’objets suivants : Frais, Société, Itération, Enregistrement de facturation, Document et Groupe.</li> 
      <li>Types de champ suivants : Calculé, Texte descriptif et Saut de section</li> 
      </ul>
      <p><b>IMPORTANT</b> : ici, la sélection ou la désélection d’un type d’objet affecte tous les formulaires personnalisés associés au type d’objet sélectionné et contenant ce champ. Par exemple, si vous désélectionnez ici un type d’objet et enregistrez le formulaire personnalisé, les modifications de valeur du champ ne sont plus suivies pour ce type d’objet dans un formulaire personnalisé qui contient le champ.</p>
       <p>Après avoir sélectionné ici un type d’objet pour un champ et enregistré le formulaire personnalisé, le champ s’affiche dans l’onglet Champs personnalisés de la zone Mettre à jour les flux dans Configuration.</p> 
       <p>Inversement, si ce champ est supprimé dans la zone Mettre à jour les flux dans Configuration, le type d’objet de ce paramètre est désélectionné sur tous les formulaires personnalisés associés au type d’objet et contenant ce champ.</p> 
       <p>Pour plus d’informations, voir la section <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#add-fields-you-want-workfront-to-track">Ajouter des champs dont Workfront doit effectuer le suivi</a> dans l’article <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md">Configurer les mises à jour système</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajouter une logique</td>
      <td>Indiquez les champs qui doivent apparaître dans le formulaire en fonction des sélections effectuées dans les champs existants. Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Ajouter une logique d’affichage et une logique de saut dans un formulaire personnalisé</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Choix </td> 
      <td> <p>(Menu déroulant, cases à cocher ou boutons radio uniquement ; facultatif)</p> 
       <ol> 
        <li> <p>Cliquez sur <b>Options</b>, puis activez l’une des options suivantes :</p> 
           <ul> 
            <li><strong>Afficher les valeurs</strong> : affiche les valeurs de chaque choix dans le champ. Le libellé de chaque choix s’affiche par défaut.</li> 
            <li><strong>Trier les choix dans l’ordre alphabétique</strong> : trie par ordre alphabétique les choix que vous ajoutez dans le champ.</li> 
           </ul> 
        </li> 
        <li> <p>Pour chaque choix que vous ajoutez à l’utilisateur ou l’utilisatrice, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-settings.png">, puis sélectionnez l’une des options suivantes :</p> 
           <ul> 
            <li><strong>Sélectionner par défaut</strong> : sélectionnez le choix par défaut dans le champ.</li> 
            <li> <p><strong>Masquer le choix</strong> : masquez le choix dans le champ. Les choix masqués restent accessibles dans les rapports.</p> </li> 
            <li> <p><strong>Supprimer le choix</strong> : supprimez le choix du champ.</p> <p><b>Avertissement</b> : si ce choix est utilisé pour les objets en cours, ne le supprimez pas du champ. Sa suppression entraînera la perte de données historiques. Sélectionnez plutôt l’option de masquage, ce qui empêche toute sélection ultérieure.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Le cas échéant) Pour modifier le type d’affichage d’un champ du formulaire personnalisé, cliquez sur le menu-déroulant **Type d’affichage**, puis cliquez sur le type de votre choix.

   Vous pouvez basculer entre les types d’affichage de champ suivants :

   * **Champs de type sélection** : cases à cocher, liste déroulante, boutons radio.
   * **Champs de type texte** : champ de texte sur une seule ligne, champ de texte de paragraphe. (Vous ne pouvez pas appliquer un autre type d’affichage à un champ de texte avec mise en forme. Vous pouvez toutefois le supprimer et ajouter un autre type de champ.)

   Par exemple, si vous avez créé un champ de cases à cocher, vous pouvez le transformer en champ de liste déroulante ou en champ de boutons radio. Si vous avez créé un champ de texte sur une seule ligne, vous pouvez également le remplacer par un champ de texte de paragraphe.

   >[!NOTE]
   >
   >Tenez compte des points suivants lorsque vous changez le type d’affichage d’un champ de case à cocher ou de liste déroulante à sélection multiple (liste déroulante permettant de sélectionner plusieurs options) en type de champ à sélection unique :
   >
   >* Si vous choisissez Boutons radio, Workfront conserve toutes les valeurs à sélection multiple qu’une personne peut avoir saisies dans le champ jusqu’à ce que l’elle modifie et enregistre les données dans n’importe quelle partie du formulaire. À ce stade, toutes les valeurs qui ont été sélectionnées à l’aide du champ à sélection multiple sont remplacées par la valeur de bouton radio sélectionnée.
   >* Si vous choisissez une liste déroulante à sélection unique, Workfront conserve toutes les valeurs à sélection multiple qu’une personne peut avoir saisies dans le champ jusqu’à ce qu’elle modifie et enregistre les valeurs dans le champ. À ce stade, toutes les valeurs qui ont été sélectionnées à l’aide du champ à sélection multiple sont remplacées par la valeur de liste déroulante sélectionnée.

1. (Facultatif) Répétez les étapes 3 à 5 pour ajouter d’autres champs personnalisés.

   Ou

   Ajoutez des champs déjà créés pour votre organisation, en suivant la procédure décrite à la section [Réutiliser un champ personnalisé ou un widget dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   >[!NOTE]
   >
   >Vous pouvez ajouter jusqu’à 500 champs et widgets sur un seul formulaire personnalisé. Cependant, une dégradation des performances peut se produire lorsque le formulaire comporte plus de 100 champs, en fonction de sa complexité. Parmi les exemples de formulaires complexes, citons les formulaires avec des paramètres en cascade, des champs de données personnalisés calculés et plusieurs options de valeur dans un seul champ.

1. Cliquez sur **Appliquer**.
1. Si vous souhaitez continuer à créer votre formulaire personnalisé d’une autre manière, consultez les articles suivants :

   * [Positionner des champs personnalisés et des widgets dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Ajouter ou modifier un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Ajouter des données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Ajouter un saut de section dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Réutiliser un champ personnalisé calculé existant dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Ajouter une logique d’affichage et une logique de saut dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Prévisualiser et finaliser un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
