---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Ajout d’un champ personnalisé à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires
description: Lorsque vous travaillez sur un formulaire personnalisé, vous pouvez créer un champ personnalisé et l’ajouter à un formulaire personnalisé. Vous pouvez également ajouter un champ personnalisé déjà ajouté à un autre formulaire personnalisé.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: d2268e50080ddbe306731d034d88fd29b712b86d
workflow-type: tm+mt
source-wordcount: '2327'
ht-degree: 2%

---

# Ajout d’un champ personnalisé à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires

<!-- Audited: 02/2024 -->

Lorsque vous travaillez sur un formulaire personnalisé, vous pouvez créer un champ personnalisé et l’ajouter à un formulaire personnalisé.

Vous pouvez également ajouter un champ personnalisé déjà ajouté à un autre formulaire personnalisé. Pour obtenir des instructions, voir [Réutilisation d’un champ ou d’un widget personnalisé dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

Pour plus d’informations sur l’ajout d’un widget de ressource à un formulaire personnalisé, processus similaire à l’ajout d’un champ personnalisé, voir [Ajout ou modification d’un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>Dans un formulaire personnalisé contenant un grand nombre de champs personnalisés ou de nombreuses options à sélection multiple dans des champs personnalisés, les utilisateurs risquent d’avoir des performances plus lentes lors de l’ajout ou de la modification de valeurs dans ces champs. Par exemple, un formulaire contenant 100 champs personnalisés ou des champs personnalisés à sélection multiple avec plus de 200 options peut être plus lent lorsque les utilisateurs interagissent avec.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td>Accès administratif aux formulaires personnalisés </td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Ajouter un champ personnalisé à un formulaire personnalisé {#add-custom-field-to-custom-form}

1. Commencez à créer ou modifier un formulaire personnalisé, comme décrit dans la section [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Sélectionnez la variable **Ajouter un champ** .

   ![Ajouter un onglet de champ](assets/add-a-field.jpg)

1. Avec **Nouveau champ** ![Icône Nouveau champ](assets/new-field.jpg) sélectionné, sélectionnez l’un des types de champ suivants :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Zone de texte à ligne simple</td> 
      <td>Permet aux utilisateurs de saisir une seule ligne de texte dans le champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zone de texte</td> 
      <td>Permet aux utilisateurs de saisir plusieurs lignes de texte dans le champ.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Champ de texte avec formatage</td> 
      <td>Permet aux utilisateurs de saisir plusieurs lignes de texte dans le champ et de mettre le texte en gras, italique, souligné, puces, numérotation, liens hypertexte et guillemets. Cette option est disponible dans la section Accueil, la zone Mises à jour, les listes et la zone Détails des objets Workfront. Une limite de caractères de 15 000 permet d’utiliser beaucoup de texte et de formatage.</p> <p>Ce type de champ personnalisé n’est pas pris en charge dans les filtres sur les listes et les rapports.</p> <p>Pour plus d’informations sur l’accès à ce champ par le biais de l’API, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">Stockage de champs de texte enrichi dans l’API</a>.</p> <p><b>REMARQUE</b>: les champs de texte avec mise en forme ne sont pas disponibles pour les applications mobiles Workfront. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Menu déroulant</td> 
      <td>Fournit une liste des choix de liste déroulante.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frappe continue </td> 
      <td>Permet aux utilisateurs de saisir le nom d’un objet existant dans Workfront. Une liste de suggestions s’affiche lorsque l’utilisateur commence à saisir du texte.
      Ce type de champ prend en charge les objets suivants :
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
      <td>Permet de définir une expression et d'afficher le résultat sur le formulaire personnalisé. Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Ajout de données calculées à un formulaire personnalisé</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date</td> 
      <td>Affiche un calendrier dans lequel les utilisateurs peuvent sélectionner une date et une heure.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cases à cocher</td> 
      <td>Permet aux utilisateurs de sélectionner plusieurs choix.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Boutons radio</td> 
      <td>Nécessite que les utilisateurs sélectionnent un seul choix.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texte descriptif</td> 
      <td>Permet d’inclure des instructions et des liens vers des pages en dehors de Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Saut de section</td> 
      <td>Un saut de section n’est en fait pas un champ. Vous pouvez utiliser un saut de section pour organiser vos champs et widgets personnalisés en sections et, si nécessaire, configurer différentes autorisations d’affichage et de modification pour chaque section. Pour plus d’informations sur l’ajout et la configuration des sauts de section, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Ajout d’un saut de section à un formulaire personnalisé</a>.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Les champs qui autorisent plusieurs sélections, tels que la case à cocher et la liste déroulante, sont difficiles à associer et à associer dans les rapports. Pour simplifier la création de graphiques et de regroupements dans les rapports, vous pouvez créer des champs distincts pour chaque choix (par exemple, un champ de texte d’une seule ligne).

1. Sur le **Paramètres des champs** , configurez les options disponibles pour le type de champ personnalisé que vous ajoutez :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Étiquette</td> 
      <td> <p>(Obligatoire) Saisissez un libellé descriptif à afficher au-dessus du champ personnalisé. Vous pouvez modifier le libellé à tout moment.</p> <p><b>IMPORTANT</b>: évitez d’utiliser des caractères spéciaux dans ce libellé. Elles ne s’affichent pas correctement dans les rapports.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>(Obligatoire) Ce nom est la manière dont le système identifie le champ personnalisé lorsque vous l’ajoutez à différentes zones dans Workfront, telles que les rapports, l’accueil et les interactions avec l’API.</p> <p>Lorsque vous configurez le champ personnalisé pour la première fois et que vous tapez le libellé, le champ Nom est automatiquement renseigné pour qu’il corresponde. Mais les champs Libellé et Nom ne sont pas synchronisés, ce qui vous donne la possibilité de modifier le libellé que vos utilisateurs voient sans avoir à modifier le nom que le système voit.</p> 
      <p><b>IMPORTANT</b>:   
      <ul> 
      <li>Bien qu’il soit possible de le faire, nous vous recommandons de ne pas modifier ce nom une fois que vous ou d’autres utilisateurs aurez commencé à utiliser le formulaire personnalisé dans Workfront. Si vous le faites, le système ne reconnaîtra plus le champ personnalisé où il peut maintenant être référencé dans d’autres zones de Workfront. <p>Par exemple, si vous ajoutez le champ personnalisé à un rapport et que vous modifiez ensuite son nom, Workfront ne le reconnaît pas dans le rapport et il ne fonctionnera plus correctement à moins de le rajouter au rapport en utilisant le nouveau nom.</p> </li>
      <li> <p>Nous vous recommandons de ne pas saisir de nom déjà utilisé pour les champs Workfront intégrés.</p> </li>
      <li><p>Il est recommandé de ne pas utiliser le caractère point/point dans le nom du champ personnalisé afin d’éviter toute erreur lors de l’utilisation du champ dans différentes zones de Workfront.</p></li>
      </ul> <p>Chaque nom de champ personnalisé doit être unique dans l’instance Workfront de votre entreprise. Ainsi, vous pouvez réutiliser un formulaire déjà créé pour un autre formulaire personnalisé. Pour plus d’informations, voir <a href="#add-a-custom-field-to-a-custom-form">Ajouter un champ personnalisé à un formulaire personnalisé</a> dans cet article.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>Saisissez des informations supplémentaires sur le champ personnalisé. Lorsque les utilisateurs remplissent le formulaire personnalisé, ils peuvent placer le pointeur de la souris sur l’icône de point d’interrogation pour afficher une info-bulle contenant les informations saisies ici.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>Sélectionnez le type de données qui sera capturé dans le champ personnalisé. Vous pouvez modifier le format de sélection après l’enregistrement du formulaire, mais le nouveau format doit prendre en charge la valeur saisie.</p>

   <p><strong>Exemple :</strong> Si vous enregistrez une valeur numérique pour un champ au format Texte sur au moins un objet et que vous modifiez ensuite le format en Nombre ou Devise, aucune erreur ne se produira. </p>
      <p>Cependant, si vous enregistrez une valeur alphanumérique dans un champ au format Texte sur au moins un objet et que vous essayez ensuite de modifier le format en Nombre ou Devise, une erreur se produira car la valeur alphanumérique enregistrée n’est pas compatible avec les formats Nombre ou Devise. </p>

   <p><strong>Remarque :</strong> La limite de caractères pour les champs Nombre est 16. Vous pouvez également utiliser un champ Texte pour saisir des nombres et éviter la limite.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type d'affichage</td> 
      <td>(Menu déroulant, cases à cocher et boutons radio uniquement) Changer le type de sélection d’option souhaité pour le champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taille</td> 
      <td>(Champs de texte uniquement) Sélectionnez une largeur pour le champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher l'heure</td> 
      <td>(Champs de date uniquement) Sélectionnez cette option si vous souhaitez afficher l’heure et la date du jour dans le champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type d'objet référencé</td> 
      <td> <p>(Champ de saisie anticipée uniquement) Sélectionnez le type d’objet à associer au champ.</p> <p>Une fois que vous avez cliqué sur Appliquer ou sur Enregistrer+Fermer, vous ne pouvez pas modifier le type d’objet du champ.</p> <p><b>REMARQUE</b>:   
        <ul> 
         <li>Si votre administrateur Workfront a personnalisé le nom des Portfolios, programmes ou projets dans l’interface utilisateur de Workfront, le nom Workfront par défaut de l’objet s’affiche dans cette liste déroulante et non dans le nom personnalisé. Contactez votre administrateur Workfront si vous avez besoin d’aide.<br></li> 
         <li>Les types d’objets suivants sont pris en charge dans les applications mobiles iOS et Android Workfront : Utilisateur, Société, Groupe, Rôle de tâche, Portfolio, Programme, Projet et Modèle.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ajouter filtre</td> 
      <td> <p>(Champ de saisie anticipée uniquement) Ajoutez un filtre pour un type d’objet afin de limiter les objets que les utilisateurs peuvent choisir lorsqu’ils utilisent le champ. </p> <p>Par exemple, vous pouvez limiter un champ afin que les noms d’utilisateur ne puissent être sélectionnés que s’ils répondent aux critères suivants :</p> 
       <ul> 
        <li>Ils appartiennent à un ou à des groupes que vous spécifiez.</li> 
        <li>Ils sont associés à un rôle ou à un titre de tâche que vous spécifiez.</li> 
        <li>Ils appartiennent au même groupe que la personne qui utilise le champ.</li> 
       </ul> <p>Vous devez définir le filtre correspondant au type d’objet sélectionné à l’aide de la syntaxe Mode texte . Pour plus d’informations sur la création d’un filtre à l’aide du mode Texte, voir <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Modification d’un filtre à l’aide du mode texte</a>.</p>
       <p><b>REMARQUE</b>:   
        <ul> 
         <li>Si vous modifiez un formulaire personnalisé existant, l’ajout d’un filtre à un champ de type anticipée ne supprime aucun objet (hors portée du filtre) déjà ajouté par les utilisateurs à l’aide du champ.</li> 
         <li>Ce filtre n’est pas disponible sur les appareils mobiles. Si vous utilisez le filtre pour un champ Type , il apparaîtra sur les appareils mobiles des utilisateurs qui ne sont pas affectés par le filtre.</li> 
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
      <td>Sélectionnez cette option si vous souhaitez que le champ soit obligatoire pour que l’utilisateur puisse remplir le formulaire personnalisé. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suivre les modifications de champ dans les messages de mise à jour</td> 
      <td><p>Cliquez dans la liste déroulante, puis sélectionnez les types d’objets pour lesquels vous souhaitez effectuer automatiquement le suivi des modifications de valeur du champ.</p> 
      <p><b>REMARQUE</b>: cette option n’est pas disponible pour les éléments suivants :</p> 
      <ul> 
      <li>Formulaires personnalisés associés aux types d’objets suivants : Frais, Société, Itération, Enregistrement de facturation, Document et Groupe.</li> 
      <li>Types de champ suivants : Calcul, Texte descriptif et Saut de section</li> 
      </ul>
      <p><b>IMPORTANT</b>: la sélection ou la désélection d’un type d’objet ici affecte tous les formulaires personnalisés associés au type d’objet sélectionné et contenant ce champ. Par exemple, si vous désélectionnez ici un type d’objet et enregistrez le formulaire personnalisé, les modifications de valeur du champ ne sont plus suivies pour ce type d’objet dans un formulaire personnalisé qui contient le champ.</p>
       <p>Après avoir sélectionné ici un type d’objet pour un champ et enregistré le formulaire personnalisé, le champ s’affiche dans l’onglet Champs personnalisés de la zone Mettre à jour les flux dans Configuration.</p> 
       <p>Inversement, si ce champ est supprimé dans la zone Mettre à jour les flux de la configuration, le type d’objet de ce paramètre est désélectionné sur tous les formulaires personnalisés associés au type d’objet et contenant ce champ.</p> 
       <p>Pour plus d’informations, voir la section <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#add-fields-you-want-workfront-to-track">Ajout de champs dont Workfront doit effectuer le suivi</a> dans l’article <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md">Configuration des mises à jour du système</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajouter une logique</td>
      <td>Indiquez les champs qui doivent apparaître dans le formulaire en fonction des sélections effectuées par les utilisateurs dans les champs existants. Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Ajouter une logique d’affichage et ignorer une logique dans un formulaire personnalisé</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Choix </td> 
      <td> <p>(Menu déroulant, cases à cocher ou boutons radio uniquement ; facultatif)</p> 
       <ol> 
        <li> <p>Cliquez sur <b>Options</b>, puis activez l’une des options suivantes :</p> 
           <ul> 
            <li><strong>Afficher les valeurs</strong>: affiche les valeurs de chaque choix dans le champ. Le libellé de chaque choix s’affiche par défaut.</li> 
            <li><strong>Choix de tri A-Z</strong>: trie par ordre alphabétique les choix que vous ajoutez dans le champ.</li> 
           </ul> 
        </li> 
        <li> <p>Pour chaque choix que vous ajoutez à l’utilisateur, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-settings.png">, puis sélectionnez l’une des options suivantes :</p> 
           <ul> 
            <li><strong>Sélection par défaut</strong>: sélectionnez le choix par défaut dans le champ.</li> 
            <li> <p><strong>Masquer le choix</strong>: masque le choix dans le champ. Les choix masqués restent accessibles dans les rapports.</p> </li> 
            <li> <p><strong>Supprimer le choix</strong>: supprimez le choix du champ.</p> <p><b>Avertissement</b>: si ce choix est utilisé pour les objets en cours, ne le supprimez pas du champ. Sa suppression entraînera la perte de données historiques. Sélectionnez plutôt l’option pour la masquer, ce qui empêche les utilisateurs de la sélectionner ultérieurement.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditionnel) Pour modifier le type d’affichage d’un champ du formulaire personnalisé, cliquez sur le bouton **Type d’affichage** , puis cliquez sur le type de votre choix.

   Vous pouvez basculer entre les types d&#39;affichage de champ suivants :

   * **Champs de type sélection**: cases à cocher, liste déroulante, boutons radio.
   * **Champs de type texte**: champ de texte d’une seule ligne, champ de texte de paragraphe. (Vous ne pouvez pas passer un champ de texte avec mise en forme à un autre type d’affichage. Vous pouvez toutefois le supprimer et ajouter un autre type de champ.)

   Par exemple, si vous avez créé un champ Cases à cocher, vous pouvez le changer en Champ déroulant ou Champ Boutons radio. Si vous avez créé un champ de texte d’une seule ligne, vous pouvez également le remplacer par un champ de texte de paragraphe.

   >[!NOTE]
   >
   >Tenez compte de ce qui suit lorsque vous souhaitez modifier le type d’affichage d’un champ à partir d’un champ de case à cocher ou d’un champ de liste déroulante à sélection multiple (une liste déroulante permettant de sélectionner plusieurs options) en un type de champ à sélection unique :
   >
   >* Si vous choisissez Boutons radio, Workfront conserve toutes les valeurs à sélection multiple qu’un utilisateur peut avoir saisies dans le champ jusqu’à ce que l’utilisateur modifie et enregistre les données dans n’importe quelle partie du formulaire. À ce stade, toutes les valeurs qui ont été sélectionnées à l’aide du champ de type à sélection multiple sont remplacées par la valeur de bouton radio sélectionnée.
   >* Si vous choisissez une liste déroulante à sélection unique, Workfront conserve toutes les valeurs à sélection multiple qu’un utilisateur peut avoir saisies dans le champ jusqu’à ce que l’utilisateur modifie et enregistre les valeurs dans le champ. À ce stade, toutes les valeurs qui ont été sélectionnées à l’aide du champ de type à sélection multiple sont remplacées par la valeur de liste déroulante sélectionnée.

1. (Facultatif) Répétez les étapes 3 à 5 pour ajouter d’autres champs personnalisés.

   Ou

   Ajoutez des champs déjà créés pour votre organisation, en suivant la procédure décrite à la section [Réutilisation d’un champ ou d’un widget personnalisé dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   >[!NOTE]
   >
   >Vous pouvez ajouter jusqu’à 500 champs et widgets sur un seul formulaire personnalisé. Cependant, une dégradation des performances peut se produire lorsque plus de 100 sur un formulaire existent, selon sa complexité. Parmi les exemples de formulaires complexes, citons les formulaires avec des paramètres en cascade, des champs de données personnalisés calculés et plusieurs options de valeur dans un seul champ.

1. Cliquez sur **Appliquer**.
1. Si vous souhaitez continuer à créer votre formulaire personnalisé d’une autre manière, passez à l’un des articles suivants :

   * [Placement de champs et de widgets personnalisés dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Ajout ou modification d’un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Ajout de données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Ajout d’un saut de section à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Réutiliser un champ personnalisé calculé existant dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Ajouter une logique d’affichage et ignorer une logique dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Aperçu et remplissage d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
