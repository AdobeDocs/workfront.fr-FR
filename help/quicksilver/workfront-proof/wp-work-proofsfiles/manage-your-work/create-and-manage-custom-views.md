---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Création et gestion des vues personnalisées dans [!DNL Workfront Proof]
description: Vous pouvez créer des vues personnalisées de vos fichiers et BAT pour répertorier les éléments de votre choix comme vous le souhaitez. Vous pouvez également exporter les informations dans votre vue personnalisée sous la forme d’un rapport (au format CSV, valeur séparée par des virgules, format de fichier).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2457'
ht-degree: 1%

---

# Création et gestion des vues personnalisées dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Vous pouvez créer des vues personnalisées de vos fichiers et BAT pour répertorier les éléments de votre choix comme vous le souhaitez. Vous pouvez également exporter les informations dans votre vue personnalisée sous la forme d’un rapport (au format CSV, valeur séparée par des virgules, format de fichier).

>[!NOTE]
>
>Les vues personnalisées sont disponibles uniquement sur les plans Select et Premium. Veuillez contacter notre équipe des ventes pour obtenir un devis.

## Création d’une vue personnalisée

Lorsque vous créez une vue personnalisée, vous pouvez choisir :

* Si vous souhaitez inclure des bons à tirer, des fichiers ou les deux
* Les colonnes affichées
* Quelle colonne doit trier ?
* Ordre de tri de la colonne (ascendant ou descendant)
* Quels types de filtres utiliser pour déterminer les informations incluses dans la vue ?

Une fois la vue personnalisée créée, elle peut être utilisée immédiatement. Le nom de la nouvelle vue est également inclus dans le menu déroulant sous le titre Mes vues personnalisées (sous les vues standard).

Pour créer une vue personnalisée :

1. Accédez au **[!UICONTROL Vues]** page.
1. Pour plus d’informations sur les vues, voir [Gestion des éléments sur la page Vues dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. Effectuez l’une des opérations suivantes, selon que vous souhaitez créer une vue personnalisée à partir de zéro ou créer une vue personnalisée basée sur une vue standard existante :

   * Pour créer une vue personnalisée basée sur une vue standard existante : Dans le menu déroulant, sélectionnez la vue standard existante que vous souhaitez utiliser comme base de votre nouvelle vue personnalisée. Cliquez sur le bouton **[!UICONTROL Paramètres d’affichage]** puis cliquez sur **[!UICONTROL Copier]** vers la nouvelle vue personnalisée.

   * ![](assets/proof-custom-view-icon.png)

   * Pour créer entièrement une vue personnalisée : Cliquez sur le bouton **[!UICONTROL Nouvelle vue]** icône .
   * ![](assets/proof-newview.png)

1. Dans le **[!UICONTROL Détails]** , renseignez les informations suivantes :

   * **[!UICONTROL Nom]** (obligatoire) : Nom de la nouvelle vue. Utilisez un nom unique afin que les utilisateurs puissent facilement trouver la vue personnalisée dans le menu déroulant des vues.
   * **[!UICONTROL Éléments]**: Indiquez si vous souhaitez que les bons à tirer et le fichier, les bons à tirer uniquement ou les fichiers ne soient inclus que dans la vue. Par défaut, les bons à tirer et les fichiers sont inclus.

1. Dans le **[!UICONTROL Colonnes]** , déterminez les colonnes à inclure dans la vue personnalisée.

   1. Cliquez sur l’icône de flèche vers la droite.
   1. ![](assets/proof-view-rightarrow.png)

   1. Double-cliquez sur le nom de la colonne sélectionnée.
   1. Vous devez sélectionner au moins une colonne et une seule colonne peut être ajoutée.
   1. Sélectionnez une colonne dans le **[!UICONTROL Colonnes disponibles]** zone que vous souhaitez inclure dans la nouvelle vue.
   1. Les colonnes sont déplacées du **[!UICONTROL Colonnes disponibles]** à la liste **[!UICONTROL Colonnes sélectionnées]** liste.

   1. Vous pouvez choisir parmi les colonnes standard ou les champs personnalisés et les motifs de décision à afficher dans votre vue personnalisée. (Si votre compte les a configurés, ils s’affichent sous la liste standard de la zone Colonnes disponibles .)
   1. Colonnes standard que vous pouvez inclure

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>Principal nom de l’étape</strong></td>   
      <td>Nom de la principale étape du workflow automatisé.</td>  
      </tr>  
      <tr>   
      <td><strong>Commentaires</strong></td>   
      <td>Nombre de commentaires reçus.</td>
      </tr>  
      <tr>   
      <td><strong>Compteur</strong></td>
      <td>Affiche un certain nombre de BAT qui ont été chargés sur votre compte (une option de compteur de BAT doit être activée dans les paramètres du compte).</td>
      </tr>
      <tr>
      <td><strong>Créé</strong></td>
      <td>Date et heure de création de l’élément.</td>
      </tr>
      <tr>
      <td><strong>Créateur</strong></td>
      <td>L’utilisateur qui a créé l’élément.</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Date ajoutée au BAT]</strong></td>
      <td>La date à laquelle vous avez été ajouté au BAT. </td>
      </tr>
      <tr>
      <td><strong>Échéance</strong></td>
      <td>La date limite pour la totalité de la preuve.</td>
      </tr>
      <tr>
      <td><strong>Décisions</strong></td>
      <td>Le nombre de décisions prises par rapport au nombre attendu (par exemple 0 sur 1, 1 sur 1, etc.)</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Téléchargements]</strong></td>
      <td>Nombre de téléchargements du fichier d’origine.</td>
      </tr>
      <tr>
      <td><strong>Nom du fichier</strong></td>
      <td>Nom du fichier ou du BAT.</td>
      </tr>
      <tr>
      <td><strong>Dossier</strong></td>
      <td>Le dossier contenant l’élément.</td>
      </tr>
      <tr>
      <td><strong>Dernière activité</strong></td>
      <td>Date et heure de la dernière activité sur l’élément.</td>
      </tr>
      <tr>
      <td><strong>Dernière décision sur</strong></td>
      <td>Date et heure de la dernière décision prise.</td>
      </tr>
      <tr>
      <td><strong>Ma date limite</strong></td>
      <td>Votre propre délai d’expiration sur les bons à tirer pour lesquels vous êtes explicitement ajouté en tant que réviseur/approbateur (le cas échéant).</td>
      </tr>
      <tr>
      <td><strong>Propriétaire</strong></td>
      <td>Propriétaire de l’élément.</td>
      </tr>
      <tr>
      <td><strong>Pays propriétaire</strong></td>
      <td>Le pays s'est inscrit dans le système pour le propriétaire du BAT. </td>
      </tr>
      <tr>
      <td><strong>BAT parent</strong></td>
      <td>Nom du BAT parent.</td>
      </tr>
      <tr>
      <td><strong>Progression</strong></td>
      <td><p>Barre de progression. Affiche les bons à tirer qui ne sont pas encore démarrés, ouverts, commentés ou décidés le.</p><p>Ces informations ne sont pas triées.</p></td>
      </tr>
      <tr>
      <td><strong>Nom de l'épreuve</strong></td>
      <td>Le nom du BAT.</td>
      </tr>
      <tr>
      <td><strong>Type de BAT</strong></td>
      <td><p>Le type de BAT : Fichier statique, page web statique, web interactif (téléchargement .zip), page web interactive (https), vidéo, audio et autre. </p><p>Les BAT combinés sont identifiés comme "Type de BAT combiné". Type de fichier du BAT.</p></td>
      </tr>
      <tr>
      <td><strong>Taille de fichier (Mo)</strong></td>
      <td><p>Taille de fichier du BAT en ce qui concerne le quota d’utilisation du disque.</p><p>Cette information est fournie pour la version actuelle du BAT. S’il n’existe pas de version actuelle, il s’agit de la version la plus récente.</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>Principal délai</strong></p></td>
      <td>Délai des étapes dans le workflow automatisé.</td>
      </tr>
      <tr>
      <td><strong>Nom de l’étape</strong></td>
      <td>Nom de chaque étape du workflow automatisé. Il s’agit notamment des étapes passées, principales et futures.</td>
      </tr>
      <tr>
      <td><strong>Département</strong></td>
      <td>Principal, Verrouillé, Version préliminaire ou Envoyé.</td>
      </tr>
      <tr>
      <td><strong>Statut</strong></td>
      <td>En attente, Modifications requises, Approuvé avec modifications, Approuvé ou Non pertinent.</td>
      </tr>
      <tr>
      <td><strong>Balises</strong></td>
      <td>Toutes les balises associées à l’élément.</td>
      </tr>
      <tr>
      <td><strong>Noms des étapes à venir</strong></td>
      <td> Nom de chaque étape qui n’a pas encore commencé dans le workflow automatisé. </td>
      </tr>
      <tr>
      <td><strong>compteur de versions</strong></td>
      <td> Nombre de versions de l’élément. </td>
      </tr>
      <tr>
      <td><strong>Numéro de version du BAT</strong></td>
      <td><i>Numéro de version du BAT.</i></td>
      </tr> 
      </tbody>
      </table>

   1. (Facultatif) Pour déplacer la colonne vers le **[!UICONTROL Colonnes sélectionnées]** pour qu’elle soit incluse dans la nouvelle vue :

      * Réorganisez toutes les colonnes du **[!UICONTROL Colonnes sélectionnées]** liste.
      * L’ordre dans lequel les colonnes sont affichées dans la variable **[!UICONTROL Colonnes sélectionnées]** détermine l’ordre dans lequel les colonnes sont affichées dans la vue personnalisée.
      * Les colonnes sont visibles dans la variable **[!UICONTROL Colonnes sélectionnées]** dans l’ordre dans lequel vous les avez ajoutés à partir de la **[!UICONTROL Colonnes disponibles]** liste.

      * Pour réorganiser une colonne dans le **[!UICONTROL Colonnes sélectionnées]** , sélectionnez le nom de la colonne et faites-la glisser vers le haut ou vers le bas dans la liste.

      * Supprimez une colonne de la **[!UICONTROL Colonnes sélectionnées]** en cliquant sur le nom de la colonne sélectionnée, puis sur la variable **[!UICONTROL Left]** flèche. Vous pouvez également double-cliquer sur le nom de la colonne sélectionnée (la colonne est de nouveau déplacée vers le **[!UICONTROL Colonnes disponibles]** liste).

      * Une colonne ne peut être ajoutée qu&#39;une seule fois. Par exemple, si vous déplacez la colonne Commentaires depuis [!UICONTROL Disponible] to [!UICONTROL Colonnes sélectionnées] liste, le nom de cette colonne disparaîtra de [!UICONTROL Colonnes disponibles] liste.

1. Dans le **[!UICONTROL Tri]** , renseignez les informations suivantes :

   * **Trier par :** Utilisez la variable [!UICONTROL Tri] si vous souhaitez définir un ordre particulier dans lequel les éléments sont répertoriés dans votre vue personnalisée. Si vous ne sélectionnez pas de colonne à trier, la valeur par défaut est Aucune colonne, c’est-à-dire pas de colonne de tri ou d’ordre spécial.
   * Seules les colonnes que vous avez sélectionnées sur l’objet [!UICONTROL Colonnes] sont inclus dans la variable [!UICONTROL Tri par colonne] Liste déroulante.
   * **ascendant ou descendant :** Indiquez si vous souhaitez trier la colonne par défaut, ascendante ou descendante.

1. Utilisez la variable **[!UICONTROL Filtres]** pour définir un ou plusieurs critères de sélection des éléments à inclure dans votre vue personnalisée. Les filtres s’avèrent particulièrement utiles si vous souhaitez utiliser votre vue personnalisée comme rapport.
1. Pour inclure tous les éléments dans votre vue personnalisée, ignorez la variable **[!UICONTROL Filtres]** .
1. Filtres disponibles :

   * **Champ :** Sélectionnez le champ de ce filtre (le champ par défaut Commentaires ). La liste Champ contient tous les champs standard (comme dans la section [!UICONTROL Colonnes] ). La liste ne se limite pas aux colonnes que vous avez sélectionnées pour l’affichage.
   * **Opérateur :** Les opérateurs disponibles pour le filtre dépendent du type de champ sélectionné. Sélectionnez un Opérateur qui affiche la relation entre le champ et le champ de valeur. Vous renseignez ces informations ultérieurement.
   * **Valeur :** Sélectionnez ou saisissez la valeur de votre choix dans ce champ, en fonction du champ et de l&#39; Opérateur que vous avez sélectionné. Selon l’opérateur que vous avez choisi, il peut y avoir un champ Valeur ou deux ou aucun. Consultez les exemples ci-dessous.
   * **Les filtres sont appliqués selon la logique suivante :** Les critères de filtrage entre différents champs utiliseront l’opérateur AND. Plusieurs critères de filtrage utilisant le même champ utiliseront l’opérateur OU pour le même champ.

      Si vous souhaitez afficher uniquement les bons à tirer sans commentaires, sélectionnez les valeurs suivantes :

      * Champ : Commentaires
      * Opérateur : Est égal à
      * Champ Valeur : 0

      Si vous souhaitez afficher uniquement les bons à tirer avec deux commentaires ou plus, sélectionnez les valeurs suivantes :

      * Champ : Commentaires
      * Opérateur : Supérieur ou égal à
      * Champ Valeur : 2

      Si vous souhaitez afficher uniquement les bons à tirer avec entre 1 et 4 commentaires, sélectionnez les valeurs suivantes :

      * Champ : Commentaires
      * Opérateur : Entre
      * Champ de valeur (premier champ) : 1
      * Champ de valeur (deuxième champ) : 4

         Vous pouvez modifier un filtre que vous avez ajouté à votre vue personnalisée sans aucun problème ou le supprimer en cliquant sur l’icône croisée en regard de l’ [!UICONTROL setup] si nécessaire.

         Parce que la liste Champ ne se limite pas aux colonnes sélectionnées sur la [!UICONTROL Colonnes] soyez prudent lorsque vous créez un filtre qui inclut une colonne que vous n’avez pas sélectionnée pour l’affichage dans votre vue personnalisée. Par exemple, le filtre suivant pour la vue sélectionne tous les bons à tirer avec une valeur de compteur Version de 2 ou plus :

         * Champ = compteur de version
         * Opérateur = Supérieur ou égal à
         * Champ Valeur = 2

            >[!NOTE]
            >
            >Vous pouvez modifier un filtre que vous avez ajouté à votre vue personnalisée sans aucun problème ou le supprimer en cliquant sur l’icône croisée en regard de l’ [!UICONTROL setup] si nécessaire.





1. Dans le **[!UICONTROL Partage]** , sélectionnez les utilisateurs de votre compte qui pourront afficher votre vue personnalisée.
1. Les vues personnalisées sont spécifiques à l’utilisateur qui les crée. Par défaut, la nouvelle vue personnalisée n’est visible que pour son créateur. toutefois, vous pouvez choisir de partager votre vue personnalisée en choisissant l’une des options suivantes :

   * **Seule la vue personnalisée s’affiche** (par défaut) : Sélectionnez cette option si vous souhaitez que la vue personnalisée ne soit disponible que pour vous.
   * **Tous les utilisateurs peuvent afficher cette vue personnalisée**: Sélectionnez cette option pour rendre la vue personnalisée disponible pour tous les utilisateurs de votre compte.
   * **Sélectionner les utilisateurs qui peuvent afficher cette vue personnalisée**: Sélectionnez cette option pour rendre la vue personnalisée disponible uniquement pour des utilisateurs spécifiques.
   * Commencez à saisir le nom ou l’adresse électronique de l’utilisateur qui doit avoir accès à la vue personnalisée, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.
   * Si vous choisissez de ne pas partager votre vue avec d’autres utilisateurs à ce stade, vous pouvez le faire ultérieurement en modifiant la vue personnalisée.

1. Cliquez sur **[!UICONTROL Créer]**.
1. La vue personnalisée s’affiche et est disponible dans la [!DNL Views] page. Pour plus d’informations sur les vues, voir [Gestion des éléments dans [!DNL Views] Page dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## Modification de vues personnalisées

Vous pouvez facilement modifier une vue personnalisée. Pour modifier une vue personnalisée :

1. Accédez au **[!UICONTROL Vues]** page.\
   Pour plus d’informations sur les vues, voir [Gestion des éléments sur la page Vues dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Cliquez sur le bouton [!UICONTROL Vues] bouton (1)
1. Sélectionnez la vue à modifier dans le menu déroulant.\
   ![](assets/proof-view-edit.png)

1. Cliquez sur le bouton **[!UICONTROL Options d’affichage]** , puis cliquez sur **[!UICONTROL Modifier la vue]**.\
   ![](assets/proof-view-options.png)\
   La page Modifier la vue personnalisée s’affiche.

1. Cliquez sur le bouton [!UICONTROL Actions] . (3)\
   Ce bouton est disponible uniquement si vous incluez la colonne Nom du BAT dans votre vue.
1. Sélectionner [!UICONTROL Modifier la vue] dans le menu. (4) \
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)

1. La page Modifier l’affichage personnalisé s’affiche.

![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>Si vous modifiez la vue personnalisée, les colonnes de la liste Colonnes sélectionnées s’organisent automatiquement dans l’ordre alphabétique. Vous devrez les réorganiser si nécessaire avant de mettre à jour la vue.


## Copie de vues personnalisées

La fonction Copier la vue vous permet de créer facilement une copie d’une vue personnalisée existante. Cela s’avère très utile, par exemple, si vous souhaitez configurer des vues distinctes pour tous vos concepteurs, chaque vue étant identique, à l’exception du propriétaire du BAT (designer).

Pour copier une vue personnalisée :

1. Accédez au **[!UICONTROL Vues]** page.\
   Pour plus d’informations sur les vues, voir [Gestion des éléments sur la page Vues dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Cliquez sur le bouton **[!UICONTROL Vues]** bouton . (1)
1. Sélectionnez votre vue personnalisée dans la liste. (2)
1. Cliquez sur le bouton **[!UICONTROL Actions]** . (3)\
   Ce bouton est disponible uniquement si vous incluez la colonne Nom du BAT dans votre vue.

1. Sélectionner [!UICONTROL Copier] dans le menu. (4)\
   ![copy_custom_view.png](assets/copying-custom-view-350x258.png)

1. Dans la page Copier l’affichage personnalisé , tous les paramètres d’origine sont renseignés. Modifiez la vue personnalisée selon votre choix et cliquez sur le bouton **[!UICONTROL Copier la vue]** bouton . Vous serez immédiatement dirigé vers votre nouvelle vue.\
   ![](assets/copy-custom-view-page-350x542.png)

## Partage de vues personnalisées

La fonction Partager la vue permet de partager une vue avec d&#39;autres utilisateurs de votre compte si vous ne les avez pas déjà sélectionnées dans la section Partage de la vue. Lorsque vous partagez une vue personnalisée avec d’autres utilisateurs, la vue apparaît dans leur [!UICONTROL Mes vues personnalisées] dans le menu déroulant Vues .

Pour partager une vue personnalisée avec d’autres utilisateurs :

1. Accédez au **[!UICONTROL Vues]** page.\
   Pour plus d’informations sur les vues, voir [Gestion des éléments sur la page Vues dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Cliquez sur le bouton **[!UICONTROL Vues]** bouton (1)
1. Sélectionnez votre vue personnalisée dans la liste (2)
1. Cliquez sur le bouton **[!UICONTROL Actions]** . (3)\
   Ce bouton est disponible uniquement si vous incluez la colonne Nom du BAT dans votre vue.

1. Sélectionner [!UICONTROL Partager la vue] du menu (4)
1. La page Modifier l’affichage personnalisé s’affiche.
1. Dans le [!UICONTROL Partage] Sélectionnez les utilisateurs avec lesquels partager la vue, puis cliquez sur **[!UICONTROL Mettre à jour la vue]**.

   ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)

## Exportation de vues personnalisées vers des fichiers CSV

Pour exporter les données d’une vue personnalisée vers un fichier CSV :

1. Accédez au **[!UICONTROL Vues]** page.\
   Pour plus d’informations sur les vues, voir [Gestion des éléments sur la page Vues dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Cliquez sur le bouton **[!UICONTROL Vues]** bouton . (1)
1. Sélectionnez votre vue personnalisée dans la liste. (2)
1. Cliquez sur le bouton **[!UICONTROL Actions]** . (3)\
   Ce bouton est disponible uniquement si vous incluez la colonne Nom du BAT dans votre vue.

1. Sélectionner [!UICONTROL Exportation au format CSV] dans le menu. (4)\
   ![export_custom_view.png](assets/exporting-custom-view-350x258.png)\
   Dans une fenêtre de navigateur distincte, &quot;Générer le rapport : 100 % apparaît, plus le nombre d’enregistrements (le nombre d’éléments inclus dans le rapport depuis votre vue personnalisée)

1. (Conditionnel) Si un message de sécurité s’affiche indiquant que le téléchargement du rapport est actuellement bloqué, cliquez pour autoriser le téléchargement.
1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque la fenêtre Téléchargement de fichier s’affiche, vous demandant si vous souhaitez ouvrir ou enregistrer le fichier.
1. Sélectionnez un emplacement sur votre ordinateur et enregistrez le fichier.

## Suppression de vues personnalisées

Vous pouvez facilement supprimer une vue personnalisée. Pour ce faire :

1. Accédez au **[!UICONTROL Vues]** page.\
   Pour plus d’informations sur les vues, voir [Gestion des éléments sur la page Vues dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Cliquez sur le bouton **[!UICONTROL Vues]** bouton .
1. Sélectionnez votre vue personnalisée dans la liste.
1. Cliquez sur le bouton **[!UICONTROL Actions]** . (3)\
   Ce bouton est disponible uniquement si vous incluez la colonne Nom du BAT dans votre vue.

1. Sélectionner [!UICONTROL Supprimer] dans le menu. (4)\
   ![delete_custom_view.png](assets/deleting-custom-view-350x258.png)

1. Cliquez sur **[!UICONTROL Supprimer]** (5) pour confirmer que vous souhaitez supprimer la vue personnalisée actuelle\
   ![delete__1_.png](assets/delete--1--350x187.png)

1. La vue par défaut Tous les éléments s’affiche et votre vue personnalisée supprimée n’apparaît plus dans la **[!UICONTROL Vues]** menu déroulant.
