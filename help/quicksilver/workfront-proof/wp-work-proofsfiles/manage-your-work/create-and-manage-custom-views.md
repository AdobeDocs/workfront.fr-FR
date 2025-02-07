---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Créer et gérer des vues personnalisées dans  [!DNL Workfront Proof]
description: Vous pouvez créer des vues personnalisées de vos fichiers et épreuves pour répertorier les éléments et comme vous souhaitez les afficher. Vous pouvez également exporter les informations dans votre vue personnalisée sous la forme d’un rapport (au format de fichier CSV, valeurs séparées par des virgules).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '2472'
ht-degree: 98%

---

# Créer et gérer des vues personnalisées dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Vous pouvez créer des vues personnalisées de vos fichiers et épreuves pour répertorier les éléments et comme vous souhaitez les afficher. Vous pouvez également exporter les informations dans votre vue personnalisée sous la forme d’un rapport (au format de fichier CSV, valeurs séparées par des virgules).

>[!NOTE]
>
>Les vues personnalisées sont disponibles uniquement sur les plans Select et Premium. Veuillez contacter notre équipe des ventes pour obtenir un devis.

## Créer une vue personnalisée

Lorsque vous créez une vue personnalisée, vous pouvez choisir :

* Si vous souhaitez inclure des épreuves, des fichiers ou les deux.
* Les colonnes affichées.
* La colonne sur laquelle trier.
* L’ordre de tri de la colonne (ascendant ou descendant).
* Les types de filtres à utiliser pour déterminer les informations incluses dans la vue.

Une fois la vue personnalisée créée, elle peut être utilisée immédiatement. Le nom de la nouvelle vue est également inclus dans le menu déroulant sous le titre Mes vues personnalisées (sous les vues standard).

Pour créer une vue personnalisée :

1. Accédez à la page **[!UICONTROL Vues]**.
1. Pour plus d’informations sur les vues, voir [Gérer les éléments de la page Vues dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. Effectuez l’une des opérations suivantes, selon que vous souhaitez créer une vue personnalisée à partir de zéro ou créer une vue personnalisée basée sur une vue standard existante :

   * Pour créer une vue personnalisée basée sur une vue standard existante : dans le menu déroulant, sélectionnez la vue standard existante à utiliser comme base de votre nouvelle vue personnalisée. Cliquez sur l’icône **[!UICONTROL Paramètres de la vue]**, puis sur **[!UICONTROL Copier]** dans la nouvelle vue personnalisée.

   * ![Icône Vue personnalisée](assets/proof-custom-view-icon.png)

   * Pour créer une vue personnalisée à partir de zéro : cliquez sur l’icône **[!UICONTROL Nouvelle vue]**.
   * ![Nouvel affichage](assets/proof-newview.png)

1. Dans la section **[!UICONTROL Détails]**, renseignez les informations suivantes :

   * **[!UICONTROL Nom]** (obligatoire) : nom de la nouvelle vue. Utilisez un nom unique afin que les utilisateurs et utilisatrices puissent facilement trouver la vue personnalisée dans le menu déroulant des vues.
   * **[!UICONTROL Éléments]** : choisissez si vous souhaitez que les épreuves et les fichiers, les épreuves uniquement ou les fichiers uniquement soient inclus dans la vue. Par défaut, les épreuves et les fichiers sont inclus.

1. Dans la section **[!UICONTROL Colonnes]**, déterminez les colonnes que vous souhaitez inclure dans la vue personnalisée.

   1. Cliquez sur l’icône de flèche vers la droite.
   1. ![Flèche droite](assets/proof-view-rightarrow.png)

   1. Double-cliquez sur le nom de la colonne sélectionnée.
   1. Vous devez sélectionner au moins une colonne et une colonne ne peut être ajoutée qu’une seule fois.
   1. Sélectionnez une colonne dans la zone **[!UICONTROL Colonnes disponibles]** que vous souhaitez inclure dans la nouvelle vue.
   1. Les colonnes sont déplacées de la liste **[!UICONTROL Colonnes disponibles]** vers la liste **[!UICONTROL Colonnes sélectionnées]**.

   1. Vous pouvez sélectionner parmi les colonnes standard ou choisir des champs personnalisés et des motifs de décision en tant que colonnes dans votre vue personnalisée. (S’ils sont configurés dans votre compte, ils s’affichent dans la liste standard de la zone Colonnes disponibles.)
   1. Colonnes standard que vous pouvez inclure

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>Nom de l’étape active</strong></td>   
      <td>Nom de l’étape active dans le workflow automatisé.</td>  
      </tr>  
      <tr>   
      <td><strong>Commentaires</strong></td>   
      <td>Nombre de commentaires reçus.</td>
      </tr>  
      <tr>   
      <td><strong>Compteur</strong></td>
      <td>Affiche le nombre d’épreuves qui ont été chargées sur votre compte (une option de compteur d’épreuves doit être activée dans les paramètres du compte).</td>
      </tr>
      <tr>
      <td><strong>Créé</strong></td>
      <td>Date et heure de création de l’élément.</td>
      </tr>
      <tr>
      <td><strong>Créateur ou créatrice</strong></td>
      <td>Personne qui a créé l’élément.</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Date added to proof]</strong></td>
      <td>Date de votre ajout à l’épreuve. </td>
      </tr>
      <tr>
      <td><strong>Échéance</strong></td>
      <td>Date d’échéance pour la totalité de l’épreuve.</td>
      </tr>
      <tr>
      <td><strong>Décisions</strong></td>
      <td>Nombre de décisions prises par rapport au nombre attendu (par exemple 0 sur 1, 1 sur 1, etc.).</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Downloads]</strong></td>
      <td>Nombre de téléchargements du fichier d’origine.</td>
      </tr>
      <tr>
      <td><strong>Nom du fichier</strong></td>
      <td>Nom du fichier ou de l’épreuve.</td>
      </tr>
      <tr>
      <td><strong>Dossier</strong></td>
      <td>Dossier contenant l’élément.</td>
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
      <td><strong>Ma date d’échéance</strong></td>
      <td>Votre propre date d’échéance sur les épreuves pour lesquelles vous êtes explicitement réviseur ou réviseuse/approbateur ou approbatrice (le cas échéant).</td>
      </tr>
      <tr>
      <td><strong>Propriétaire</strong></td>
      <td>Propriétaire de l’élément.</td>
      </tr>
      <tr>
      <td><strong>Pays de la personne propriétaire</strong></td>
      <td>Pays enregistré dans le système pour la personne propriétaire de l’épreuve. </td>
      </tr>
      <tr>
      <td><strong>Épreuve parent</strong></td>
      <td>Nom de l’épreuve parent.</td>
      </tr>
      <tr>
      <td><strong>Progression</strong></td>
      <td><p>Barre de progression. Affiche les épreuves qui ne sont pas encore commencées, ouvertes, commentées ou n’ayant pas reçu de décision.</p><p>Ces informations ne sont pas triées.</p></td>
      </tr>
      <tr>
      <td><strong>Nom de l’épreuve</strong></td>
      <td>Nom de l’épreuve.</td>
      </tr>
      <tr>
      <td><strong>Type d’épreuve</strong></td>
      <td><p>Type d’épreuve : fichier statique, page web statique, web interactif (chargement .zip), page web interactive (https), vidéo, audio, etc. </p><p>Les épreuves combinées sont identifiées comme « Type d’épreuve combinée ». Type de fichier de l’épreuve.</p></td>
      </tr>
      <tr>
      <td><strong>Taille du fichier (Mo)</strong></td>
      <td><p>Taille du fichier de l’épreuve en ce qui concerne le quota d’utilisation du disque.</p><p>Cette information est fournie pour la version actuelle de l’épreuve. S’il n’existe pas de version actuelle, elle est indiquée pour la version la plus récente.</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>Délai des étapes actives</strong></p></td>
      <td>Délai des étapes dans le workflow automatisé.</td>
      </tr>
      <tr>
      <td><strong>Nom de l’étape</strong></td>
      <td>Nom de chaque étape du workflow automatisé. Cela inclut les étapes passées, actives et futures.</td>
      </tr>
      <tr>
      <td><strong>Département</strong></td>
      <td>Actif, Verrouillé, Brouillon ou Envoyé.</td>
      </tr>
      <tr>
      <td><strong>Statut</strong></td>
      <td>En attente, Modifications requises, Approuvé avec des modifications, Approuvé ou Non pertinent.</td>
      </tr>
      <tr>
      <td><strong>Balises</strong></td>
      <td>Toutes les balises associées à l’élément.</td>
      </tr>
      <tr>
      <td><strong>Noms des étapes à venir</strong></td>
      <td> Le nom de chaque étape qui n’a pas encore commencé dans le workflow automatisé. </td>
      </tr>
      <tr>
      <td><strong>Compteur de versions</strong></td>
      <td> Le nombre de versions de l’élément. </td>
      </tr>
      <tr>
      <td><strong>Numéro de version de l’épreuve</strong></td>
      <td><i>Le numéro de version de l’épreuve.</i></td>
      </tr> 
      </tbody>
      </table>

   1. (Facultatif) Effectuez l’une des opérations suivantes pour déplacer la colonne vers la zone **[!UICONTROL Colonnes sélectionnées]** et qu’elle soit incluse dans la nouvelle vue :

      * Réorganisez toutes les colonnes de la liste **[!UICONTROL Colonnes sélectionnées]**.
      * L’ordre dans lequel les colonnes sont affichées dans la liste **[!UICONTROL Colonnes sélectionnées]** détermine l’ordre dans lequel les colonnes sont affichées dans la vue personnalisée.
      * Les colonnes sont visibles dans la liste **[!UICONTROL Colonnes sélectionnées]** dans l’ordre dans lequel vous les avez ajoutées à partir de la liste **[!UICONTROL Colonnes disponibles]**.

      * Pour réorganiser une colonne dans la liste **[!UICONTROL Colonnes sélectionnées]**, sélectionnez le nom de la colonne et faites-la glisser vers le haut ou vers le bas dans la liste.

      * Supprimez une colonne de la liste **[!UICONTROL Colonnes sélectionnées]** en cliquant sur le nom de la colonne sélectionnée, puis en cliquant sur la flèche **[!UICONTROL Gauche]**. Vous pouvez également double-cliquer sur le nom de la colonne sélectionnée (la colonne est de nouveau déplacée dans la liste **[!UICONTROL Colonnes disponibles]**).

      * Une colonne ne peut être ajoutée qu’une seule fois. Par exemple, si vous déplacez la colonne Commentaires depuis la liste [!UICONTROL Colonnes disponibles] vers la liste [!UICONTROL Colonnes sélectionnées], le nom de cette colonne disparaîtra de la liste [!UICONTROL Colonnes disponibles].

1. Dans la section **[!UICONTROL Tri]**, renseignez les informations suivantes :

   * **Trier par :** utilisez l’onglet [!UICONTROL Tri] si vous souhaitez définir un ordre particulier dans lequel les éléments sont répertoriés dans votre vue personnalisée. Si vous ne sélectionnez pas de colonne à trier, le paramètre par défaut est Aucune colonne, c’est-à-dire pas de colonne de tri ou d’ordre spécial.
   * Seules les colonnes que vous avez sélectionnées dans l’onglet [!UICONTROL Colonnes] sont incluses dans la liste déroulante [!UICONTROL Trier par colonne].
   * **Croissant ou décroissant :** indiquez si vous souhaitez trier la colonne de manière croissante ou décroissante par défaut.

1. Utilisez la section **[!UICONTROL Filtres]** pour définir un ou plusieurs critères de sélection des éléments à inclure dans votre vue personnalisée. Les filtres s’avèrent particulièrement utiles si vous souhaitez utiliser votre vue personnalisée comme rapport.
1. Pour inclure tous les éléments dans votre vue personnalisée, ignorez la section **[!UICONTROL Filtres]**.
1. Filtres disponibles :

   * **Champ :** sélectionnez le champ de ce filtre (Commentaires est le champ par défaut). La liste Champ contient tous les champs standard (comme dans l&#39;onglet [!UICONTROL Colonnes]). La liste ne se limite pas aux colonnes que vous avez sélectionnées pour l’affichage.
   * **Opérateur :** les opérateurs disponibles pour le filtre dépendent du type de champ sélectionné. Sélectionnez un opérateur qui affiche la relation entre le champ et le champ de valeur. Vous renseignerez ces informations ultérieurement.
   * **Valeur :** sélectionnez ou saisissez la valeur de votre choix dans ce champ, en fonction du champ et de l’opérateur que vous avez sélectionné. Selon l’opérateur que vous avez choisi, il peut y avoir un, deux ou aucun champ Valeur. Consultez les exemples ci-dessous.
   * **Les filtres sont appliqués selon la logique suivante :** les critères de filtre entre différents champs utilisent l’opérateur AND. Plusieurs critères de filtre utilisant le même champ utilisent l’opérateur OR pour le même champ.

     Si vous souhaitez afficher uniquement les épreuves sans commentaires, sélectionnez les valeurs suivantes :

      * Champ : commentaires
      * Opérateur : égal à
      * Champ de valeur : 0

     Si vous souhaitez afficher uniquement les épreuves avec deux commentaires ou plus, sélectionnez les valeurs suivantes :

      * Champ : commentaires
      * Opérateur : supérieur ou égal à
      * Champ de valeur : 2

     Si vous souhaitez afficher uniquement les épreuves avec entre 1 et 4 commentaires, sélectionnez les valeurs suivantes :

      * Champ : commentaires
      * Opérateur : entre
      * Champ de valeur (premier champ) : 1
      * Champ de valeur (deuxième champ) : 4

        Vous pouvez modifier un filtre que vous avez ajouté à votre vue personnalisée sans aucun problème ou le supprimer en cliquant sur l’icône en forme de croix en regard du filtre [!UICONTROL Configuration] si nécessaire.

        Étant donné que la liste Champ ne se limite pas aux colonnes que vous avez sélectionnées dans l’onglet [!UICONTROL Colonnes], faites attention lorsque vous créez un filtre qui inclut une colonne que vous n’avez pas sélectionnée pour l’affichage dans votre vue personnalisée. Par exemple, le filtre suivant pour la vue sélectionne toutes les épreuves avec une valeur de compteur de version de 2 ou plus :

         * Champ = compteur de version
         * Opérateur = supérieur ou égal à
         * Champ de valeur = 2

           >[!NOTE]
           >
           >Vous pouvez modifier un filtre que vous avez ajouté à votre vue personnalisée sans aucun problème ou le supprimer en cliquant sur l’icône en forme de croix en regard du filtre [!UICONTROL Configuration] si nécessaire.



1. Dans la section **[!UICONTROL Partager]**, sélectionnez les utilisateurs et utilisatrices de votre compte qui pourront voir votre vue personnalisée.
1. Les vues personnalisées sont spécifiques à l’utilisateur ou l’utilisatrice qui les crée. Par défaut, la nouvelle vue personnalisée n’est visible que pour la personne qui l’a créée. Vous pouvez toutefois choisir de partager votre vue personnalisée en sélectionnant l’une des options suivantes :

   * **La vue personnalisée ne s’affiche que pour vous** (par défaut) : sélectionnez cette option si vous souhaitez que la vue personnalisée ne soit disponible que pour vous.
   * **La vue personnalisée s’affiche pour tout le monde** : sélectionnez cette option pour que la vue personnalisée soit disponible pour tous les utilisateurs et toutes les utilisatrices de votre compte.
   * **La vue personnalisée s’affiche pour les personnes sélectionnées** : sélectionnez cette option pour que la vue personnalisée soit disponible uniquement pour des utilisateurs et utilisatrices spécifiques.
   * Commencez à saisir le nom ou l’adresse e-mail de l’utilisateur ou de l’utilisatrice qui doit avoir accès à la vue personnalisée, puis cliquez sur son nom lorsqu’il dans la liste déroulante.
   * Si vous choisissez de ne pas partager votre vue avec d’autres personnes à ce stade, vous pouvez le faire ultérieurement en modifiant la vue personnalisée.

1. Cliquez sur **[!UICONTROL Créer]**.
1. La vue personnalisée s’affiche et est disponible dans la page [!DNL Views]. Pour plus d’informations sur les vues, voir [Gérer les éléments sur la page  [!DNL Views]  de  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## Modifier des vues personnalisées

Vous pouvez facilement modifier une vue personnalisée. Pour modifier une vue personnalisée :

1. Accédez à la page **[!UICONTROL Vues]**.\
   Pour plus d’informations sur les vues, voir [Gérer les éléments sur la page Vues de  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Cliquez sur le bouton [!UICONTROL Vues] bouton (1)
1. Sélectionnez la vue à modifier dans le menu déroulant.\
   ![Vue Modifier](assets/proof-view-edit.png)

1. Cliquez sur le bouton **[!UICONTROL Options de vue]**, puis cliquez sur **[!UICONTROL Modifier la vue]**.\
   ![Options d’affichage](assets/proof-view-options.png)\
   La page Modifier la vue personnalisée s’affiche.

1. Cliquez sur le menu [!UICONTROL Actions]. (3)\
   Ce bouton n’est disponible que si vous incluez la colonne Nom de l’épreuve dans votre vue.
1. Sélectionnez [!UICONTROL Modifier la vue] dans le menu. (4) \
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)

1. La page Modifier la vue personnalisée s’affiche.

![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>Si vous modifiez la vue personnalisée, les colonnes de la liste Colonnes sélectionnées se rangent automatiquement dans l’ordre alphabétique. Vous devrez les réorganiser si nécessaire avant de mettre à jour la vue.


## Copier des vues personnalisées

La fonction Copier une vue vous permet de créer facilement une copie d’une vue personnalisée existante. Cela s’avère très utile, par exemple, si vous souhaitez configurer des vues distinctes pour toutes les personnes responsables de la conception, chaque vue étant identique, à l’exception de la personne propriétaire de l’épreuve (créateur ou créatrice).

Pour copier une vue personnalisée :

1. Accédez à la page **[!UICONTROL Vues]**.\
   Pour plus d’informations sur les vues, voir [Gérer les éléments sur la page Vues de  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Cliquez sur le bouton **[!UICONTROL Vues]**. (1)
1. Sélectionnez votre vue personnalisée dans la liste. (2)
1. Cliquez sur le menu **[!UICONTROL Actions]**. (3)\
   Ce bouton n’est disponible que si vous incluez la colonne Nom de l’épreuve dans votre vue.

1. Sélectionnez [!UICONTROL Copier] dans le menu. (4)\
   ![copying_custom_view.png](assets/copying-custom-view-350x258.png)

1. Dans la page Copier la vue personnalisée, tous les paramètres d’origine sont renseignés. Modifiez la vue personnalisée selon votre choix et cliquez sur le bouton **[!UICONTROL Copier la vue]**. Vous aurez immédiatement accès à votre nouvelle vue.\
   ![Copier la vue personnalisée](assets/copy-custom-view-page-350x542.png)

## Partager des vues personnalisées

La fonction Partager la vue permet de partager une vue avec d’autres personnes de votre compte si vous ne les avez pas déjà sélectionnées dans la section Partage de la vue. Lorsque vous partagez une vue personnalisée avec d’autres personnes, la vue apparaît dans leur section [!UICONTROL Mes vues personnalisées] dans le menu déroulant Vues.

Pour partager une vue personnalisée avec d’autres personnes :

1. Accédez à la page **[!UICONTROL Vues]**.\
   Pour plus d’informations sur les vues, voir [Gérer les éléments sur la page Vues de  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Cliquez sur le bouton **[!UICONTROL Vues]**.(1)
1. Sélectionnez votre vue personnalisée dans la liste. (2)
1. Cliquez sur le menu **[!UICONTROL Actions]**. (3)\
   Ce bouton n’est disponible que si vous incluez la colonne Nom de l’épreuve dans votre vue.

1. Sélectionnez [!UICONTROL Partager la vue] dans le menu. (4)
1. La page Modifier la vue personnalisée s’affiche.
1. Dans la section [!UICONTROL Partage], sélectionnez les personnes avec lesquelles partager la vue, puis cliquez sur **[!UICONTROL Mettre à jour la vue]**.

   ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)

## Exporter des vues personnalisées vers des fichiers CSV

Pour exporter les données d’une vue personnalisée vers un fichier CSV :

1. Accédez à la page **[!UICONTROL Vues]**.\
   Pour plus d’informations sur les vues, voir [Gérer les éléments sur la page Vues de  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Cliquez sur le bouton **[!UICONTROL Vues]**. (1)
1. Sélectionnez votre vue personnalisée dans la liste. (2)
1. Cliquez sur le menu **[!UICONTROL Actions]**. (3)\
   Ce bouton n’est disponible que si vous incluez la colonne Nom de l’épreuve dans votre vue.

1. Sélectionnez [!UICONTROL Exporter au format CSV] dans le menu. (4)\
   ![exporting_custom_view.png](assets/exporting-custom-view-350x258.png)\
   Dans une fenêtre de navigateur distincte, « Génération du rapport : 100 % » apparaît, plus le nombre d’enregistrements (le nombre d’éléments inclus dans le rapport depuis votre vue personnalisée).

1. (Le cas échéant) Si un message de sécurité s’affiche indiquant que le téléchargement du rapport est actuellement bloqué, cliquez pour autoriser le téléchargement.
1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque la fenêtre Téléchargement de fichier s’affiche, vous demandant si vous souhaitez ouvrir ou enregistrer le fichier.
1. Sélectionnez un emplacement sur votre ordinateur et enregistrez le fichier.

## Supprimer des vues personnalisées

Vous pouvez facilement supprimer une vue personnalisée. Pour ce faire :

1. Accédez à la page **[!UICONTROL Vues]**.\
   Pour plus d’informations sur les vues, voir [Gérer des éléments sur la page Vues de  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Cliquez sur le bouton **[!UICONTROL Vues]**.
1. Sélectionnez votre vue personnalisée dans la liste.
1. Cliquez sur le menu **[!UICONTROL Actions]**. (3)\
   Ce bouton n’est disponible que si vous incluez la colonne Nom de l’épreuve dans votre vue.

1. Sélectionnez [!UICONTROL Supprimer] dans le menu. (4)\
   ![delete_custom_view.png](assets/deleting-custom-view-350x258.png)

1. Cliquez sur **[!UICONTROL Supprimer]** (5) pour confirmer la suppression de la vue personnalisée actuelle.\
   ![delete__1_.png](assets/delete--1--350x187.png)

1. La vue par défaut Tous les éléments s’affiche et votre vue personnalisée supprimée n’apparaît plus dans le menu déroulant **[!UICONTROL Vues]**.
