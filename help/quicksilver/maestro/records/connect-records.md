---
title: Connexion d’enregistrements
description: Après avoir créé des connexions entre les types d’enregistrement, vous pouvez connecter des enregistrements individuels les uns aux autres.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '1804'
ht-degree: 0%

---


<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Connexion d’enregistrements

>[!IMPORTANT]
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta fermé ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Vous pouvez connecter des enregistrements Adobe Maestro les uns aux autres ou aux objets d’autres applications.

Vous devez d’abord associer deux types d’enregistrement ou un type d’enregistrement à un type d’objet à partir d’une autre application, puis vous pouvez utiliser la vue Tableau du type d’enregistrement pour connecter des enregistrements les uns aux autres ou des enregistrements à d’autres objets.

Pour plus d’informations sur la connexion des types d’enregistrement les uns aux autres ou sur les types d’objets d’autres applications, voir [Connexion des types d’enregistrement](../architecture-and-fields/connect-record-types.md).

Pour un exemple de connexion des types d’enregistrement, voir [Exemple de connexion de types d&#39;enregistrements et d&#39;enregistrements](../architecture-and-fields/example-connect-record-types-and-records.md).

Vous pouvez connecter les éléments suivants :

* Enregistrements opérationnels du maître
* Enregistrements opérationnels Maestro et enregistrements de taxonomie
* Enregistrements opérationnels Maestro et objets provenant d&#39;autres applications.

  Les applications et types d’objets suivants sont actuellement pris en charge :

   * Adobe Workfront

      * Projets
      * Portefeuilles
      * Programmes
      * Entreprise
      * Groupe

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
<tbody>
<td>
   <p> Adobe de produit</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé Adobe Maestro. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Formule Adobe Workfront</p></td>
   <td>
<p>Tous</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td><p>Tout, pour créer des enregistrements Maestro</p> 
<p>Utilisation ou version ultérieure pour afficher les projets dans Workfront</p>
  <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Présentation des licences Adobe Workfront</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">Niveau d’accès</td>
   <td> <p>Tout, pour créer des enregistrements Maestro</p>
<p>Affichage ou accès supérieur à Projets, Portfolios, programmes</p> 
<p>Accès supplémentaire aux groupes et aux entreprises, lorsque vous affichez des groupes ou des entreprises, les utilisateurs n’appartenant pas à</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td> <p>Affichage ou autorisations supérieures des objets que vous souhaitez lier aux enregistrements Maestro  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur système doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/grant-access.md">Accorder l’accès à Adobe Maestro</a>. </p></td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Connexion d’enregistrements

### Considérations relatives à la connexion des enregistrements

* Une fois la connexion entre les types d’enregistrement établie, les types d’enregistrement connectés s’affichent sous forme de champs d’enregistrement liés dans la table des types d’enregistrement à partir desquels ils sont liés.
* Vous pouvez parcourir et ajouter des enregistrements et des objets de l’enregistrement et des types d’objets liés à partir des champs d’enregistrement liés.
* Vous pouvez ajouter des champs provenant des types d’enregistrement liés à la table du type d’enregistrement à partir duquel vous liez.
* Vous ne pouvez pas mettre à jour manuellement les valeurs des champs liés sur les enregistrements à partir desquels vous effectuez la liaison.

  Les valeurs des champs liés des enregistrements liés renseignent l’enregistrement Maestro à partir duquel vous effectuez automatiquement la liaison.

* Toute personne ayant accès à Maestro peut voir les connexions que vous faites entre les enregistrements Maestro ou entre les enregistrements Maestro et les objets Workfront. Vous pouvez également afficher et modifier les connexions de tous les autres utilisateurs. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* Vous pouvez connecter un enregistrement Maestro à un ou plusieurs objets d’une autre application.
* Vous ne pouvez pas connecter de taxonomies à des types d’enregistrement ou à des objets à partir d’une autre application. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* Actuellement, vous ne pouvez lier les enregistrements Maestro qu’aux objets Workfront. Pour lier des enregistrements Maestro à des objets Workfront, vous devez disposer des éléments suivants :

   * Objets Workfront. Par exemple, vous devez d’abord créer des projets, des portefeuilles, des programmes, des entreprises ou des groupes dans Workfront.
   * Espaces de travail Maestro, types d’enregistrement et enregistrements. Pour plus d’informations, voir les articles suivants :

      * [Créer des espaces de travail](../architecture-and-fields/create-workspaces.md)
      * [Création de types d’enregistrement](../architecture-and-fields/create-record-types.md)
      * [Créer des enregistrements](../records/create-records.md)

   * Connexions entre types d’enregistrement ou entre types d’enregistrement et objets d’autres applications. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture-and-fields/connect-record-types.md).

### Connexion des enregistrements Maestro

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-workfront.png) dans le coin supérieur droit de Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> puis cliquez sur **Maestro** ![](assets/maestro-icon.png).

   L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail à partir duquel vous souhaitez connecter des enregistrements.
1. Cliquez sur la carte d’un type d’enregistrement pour ouvrir la page de type d’enregistrement.
1. Sélectionnez une vue Tableau dans la **Affichage** menu déroulant dans le coin supérieur droit de la page de type enregistrement.
1. Ajoutez une connexion à un autre type d’enregistrement ou d’objet à partir du type d’enregistrement sélectionné. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture-and-fields/connect-record-types.md).

Une nouvelle colonne est ajoutée au tableau pour afficher le type d&#39;enregistrement associé.

1. Ajoutez des enregistrements au type d’enregistrement que vous avez sélectionné en ajoutant une nouvelle ligne au tableau. Pour plus d’informations, voir [Créer des enregistrements](../../maestro/records/create-records.md).
1. Depuis un enregistrement répertorié dans la vue de tableau, accédez à la colonne d’enregistrement lié et survolez la cellule correspondant à l’enregistrement que vous souhaitez lier à d’autres enregistrements Maestro, puis cliquez sur le bouton **+** Icône

   La variable **Connexion d’objets** s’affiche.

   ![](assets/connected-objects-table-for-records.png)

1. Commencez à saisir le nom d’un enregistrement dans la zone de recherche, puis sélectionnez-le à son affichage dans la liste.

   Ou

   Sélectionnez le nom d’un ou de plusieurs enregistrements dans la zone, puis cliquez sur **Connexion d’objets** dans le coin supérieur droit de la zone Connexion aux objets .

   Les éléments suivants sont ajoutés :

   * Les enregistrements liés s&#39;affichent dans le champ enregistrement lié de l&#39;enregistrement que vous avez sélectionné à l&#39;étape 3. La mise à jour des enregistrements liés met automatiquement à jour les champs d’enregistrement liés pour les enregistrements à partir desquels vous créez une liaison. <!--ensure the number of the step stays accurate-->
   * Les champs liés qui appartiennent aux enregistrements liés sont automatiquement renseignés avec les informations des enregistrements liés d&#39;origine. Vous ne pouvez pas modifier manuellement les champs liés.

     >[!TIP]
     >
     >* Nous utilisons de manière interchangeable les &quot;champs liés&quot; et &quot;champs de recherche&quot;.
     >
     >* Si vous avez activé le paramètre Autoriser plusieurs enregistrements lors de la connexion des types d’enregistrements, les valeurs des champs des multiples objets sélectionnés sont affichées séparées par des virgules ou sont agrégées en fonction de l’agrégateur que vous avez choisi.

1. (Facultatif) Fermez la page de type Enregistrement Maestro et accédez à l’espace de travail que vous avez sélectionné.
1. Cliquez sur la carte correspondant au type d’enregistrement auquel vous avez lié.

   Par exemple, si vous avez connecté l’enregistrement Campaign à l’enregistrement Product, cliquez sur le bouton **Produit** carte.

   La carte de type d’enregistrement doit s’ouvrir dans la vue Tableau.

   Le champ Enregistrement lié à Campaign affiche les noms des campagnes auxquelles vous avez lié des produits dans la page Type d’enregistrement de produit . La mise à jour des informations de Campaign met automatiquement à jour le champ d’enregistrement lié à Campaign pour le type d’enregistrement Produit .

### Connexion des enregistrements Maestro aux objets Workfront

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Après avoir créé une connexion entre un type d’enregistrement Maestro et un type d’objet Workfront, vous pouvez connecter des enregistrements Maestro individuels à des objets dans Workfront. Vous pouvez également connecter des champs de l’objet Workfront au type d’enregistrement Maestro .

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-workfront.png) dans le coin supérieur droit de Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> puis cliquez sur **Maestro** ![](assets/maestro-icon.png).

   L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail à partir duquel vous souhaitez connecter des enregistrements.
1. Cliquez sur la carte d’un type d’enregistrement pour ouvrir la page de type d’enregistrement.
1. Sélectionnez une vue Tableau dans la **Affichage** menu déroulant dans le coin supérieur droit de la page de type enregistrement.
1. Ajoutez une nouvelle connexion à un type d’objet à partir de Workfront le type d’enregistrement sélectionné. Sélectionnez l’un des objets suivants sous la section Workfront :

   * Projet
   * Portfolio
   * Programme
   * Entreprise
   * Groupe

   Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture-and-fields/connect-record-types.md).

   Une nouvelle colonne est ajoutée au tableau pour afficher le type d’objet associé.

1. Ajoutez des enregistrements individuels au type d’enregistrement que vous avez sélectionné en ajoutant une nouvelle ligne au tableau. Pour plus d’informations, voir [Créer des enregistrements](../../maestro/records/create-records.md).
1. Dans un enregistrement répertorié dans la vue de tableau, accédez à la colonne d’objet lié et survolez la cellule correspondant à l’enregistrement que vous souhaitez lier à d’autres objets de Workfront, puis cliquez sur le bouton **+** Icône <!--change Workfront to other applications, when this will be possible-->

   La variable **Connexion d’objets** s’affiche.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Commencez à saisir le nom d’un objet Workfront dans la zone de recherche, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   Ou

   Sélectionnez le nom d’un ou de plusieurs objets dans la zone, puis cliquez sur **Connexion d’objets** dans le coin supérieur droit de la zone Connexion aux objets .

   Les éléments suivants sont ajoutés à Maestro :

   * Les objets Workfront sélectionnés sont ajoutés au champ d’enregistrement associé.
   * Un nouveau champ lié (ou champ de recherche) est créé pour chaque champ lié que vous avez sélectionné lors de l’ajout des champs à votre enregistrement lié.
   * Un nouveau type d’enregistrement appelé &quot;Objet Workfront&quot; est créé dans le même espace de travail que l’enregistrement Maestro à partir duquel vous liez. Le nom de l’objet fait partie du nom de ce type d’enregistrement. Par exemple, la liaison à des projets Workfront crée le type d’enregistrement de projet Workfront dans Maestro.

     Il s’agit d’un type d’enregistrement en lecture seule qui affiche les objets Workfront sélectionnés dans le nouveau champ d’objet lié que vous avez créé à partir de l’enregistrement Maestro. Les champs liés de l&#39;objet lié s&#39;affichent également sur les enregistrements Workfront liés en lecture seule.

     >[!IMPORTANT]
     >
     > Le type d’enregistrement d’objet Workfront en lecture seule est créé uniquement lorsque des projets individuels sont ajoutés aux enregistrements Maestro. La simple création d’une connexion entre un type d’enregistrement Maestro et un type d’objet Workfront ne crée pas le type d’enregistrement Workfront.

     Toutes les informations existantes des champs des objets Workfront s’affichent dans les champs liés ou de recherche.

     >[!TIP]
     >
     >
     >* Si vous avez activé le paramètre Autoriser plusieurs enregistrements , les valeurs de plusieurs objets sont affichées séparées par des virgules ou sont agrégées selon l’agrégateur que vous avez choisi.
     >
     >* Un champ d’enregistrement lié aux enregistrements liés à Maestro n’est pas créé pour les objets Workfront liés.


1. (Facultatif) Fermez la page de type Enregistrement Maestro et accédez à l’espace de travail que vous avez sélectionné.
1. Cliquez sur la carte correspondant au type d’enregistrement de l’objet Workfront. Par exemple, cliquez sur le bouton **Projet Workfront** si vous avez lié à des projets Workfront. La carte de type d’enregistrement Workfront en lecture seule doit s’ouvrir dans la vue Tableau.

   >[!NOTE]
   >
   >    * Les enregistrements répertoriés dans la page de type Enregistrement Workfront sont des objets Workfront en lecture seule. Les champs liés à partir du type d’enregistrement Workfront s’affichent également sous forme de colonnes en lecture seule et sont renseignés automatiquement lorsqu’ils sont renseignés dans Workfront.
   >    * Vous ne pouvez pas mettre à jour manuellement les champs Workfront dans Maestro. Les champs d’objet Workfront doivent être renseignés dans Workfront et les valeurs de champ s’affichent automatiquement sur l’enregistrement Workfront dans Maestro.
   >
   >    * Pour afficher le type d’enregistrement de l’objet Workfront dans la vue Chronologie, au moins deux champs de date doivent s’afficher dans la vue Tableau de la page de type d’enregistrement Workfront en lecture seule.

1. (Facultatif) Cliquez sur le **Plus** menu ![](assets/more-menu.png) en regard du nom de type d’enregistrement de l’objet Workfront dans l’en-tête de la page, puis cliquez sur **Renommer** pour modifier le nom de l’enregistrement.

   >[!NOTE]
   >
   >    Vous ne pouvez pas supprimer un type d’enregistrement Workfront lié ni aucun objet de la page de type d’enregistrement Workfront.

1. (Facultatif) Cliquez sur le **Ajouter des champs** icon ![](assets/add-fields-icon.png) dans le coin supérieur droit de la vue de tableau de la page de type d’enregistrement Workfront, pour ajouter ou supprimer des champs Workfront du type d’enregistrement Workfront.

   >[!NOTE]
   >
   >  Les champs que vous ajoutez ou supprimez dans la page Type d’enregistrement d’objet Workfront ne sont pas ajoutés ni supprimés du type d’enregistrement Maestro lié au type d’objet Workfront. Les champs ne sont visibles que sur la page de type d’enregistrement Workfront en lecture seule. Vous pouvez donc les consulter dans Maestro.

1. (Facultatif) Dans le menu déroulant Affichage de la page de type d’enregistrement d’objet Workfront, choisissez la vue Chronologie pour afficher les objets liés Workfront dans la vue de la chronologie.












