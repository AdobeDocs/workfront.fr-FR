---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incorporation d’une file d’attente de requêtes dans un tableau de bord
description: Vous pouvez incorporer une nouvelle file d’attente de requêtes dans un tableau de bord pour fournir un accès direct à la file d’attente de requêtes à vos utilisateurs, sans avoir à accéder à la zone Demandes .
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# Incorporation d’une file d’attente de requêtes dans un tableau de bord

Vous pouvez incorporer une nouvelle file d’attente de requêtes dans un tableau de bord pour fournir un accès direct à la file d’attente de requêtes à vos utilisateurs, sans avoir à accéder à la zone Demandes . 

Par exemple, si vous disposez d’une file d’attente de demandes ouverte à l’ensemble de l’organisation, telle qu’une file d’attente du service d’assistance ou une file d’attente de demandes PTO à laquelle tout le monde doit accéder régulièrement, il peut s’avérer pratique d’insérer la file d’attente de demandes directement dans l’un de leurs tableaux de bord pour un accès rapide et facile. Le processus de configuration est similaire à celui de la création d’une page externe sur un tableau de bord.

Tout d’abord, vous devez obtenir une URL vers la file d’attente des demandes. Deuxièmement, vous pouvez incorporer l’URL dans un tableau de bord en ajoutant une page externe.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Gestion des autorisations pour le tableau de bord</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Vous devez créer les deux éléments suivants avant d’incorporer une file d’attente de requêtes dans un tableau de bord :

* **Le tableau de bord**: Pour plus d’informations sur la création de tableaux de bord, voir [Création d’un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).
* **File d’attente des demandes**: Pour plus d’informations sur la création de files d’attente de requête, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## Obtention de l’URL de la file d’attente des demandes {#obtain-the-url-of-the-request-queue}

Vous pouvez obtenir l’URL d’une file d’attente de demandes de plusieurs manières, en fonction de la partie de la file d’attente de demandes que vous souhaitez afficher aux utilisateurs lorsqu’ils y accèdent à partir d’un tableau de bord.

* [Obtention d’un lien vers une rubrique de file d’attente spécifique avec possibilité de modifier le type de requête](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)
* [Obtention d’un lien vers une file d’attente de requêtes et possibilité de modifier le type de requête](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)
* [Obtention d’un lien vers une file d’attente de requêtes sans possibilité de modifier le type de requête](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### Obtention d’un lien vers une rubrique de file d’attente spécifique avec possibilité de modifier le type de requête {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

Lorsque vous partagez avec d’autres utilisateurs un lien vers une rubrique de file d’attente spécifique, le formulaire de requête s’ouvre sur la rubrique de file d’attente exacte dont ils ont besoin pour envoyer la requête. Cela s’avère utile lorsque les utilisateurs peuvent ne pas être certains de la rubrique de file d’attente à choisir lors de la journalisation des requêtes pour une file d’attente de requêtes spécifique.

Les utilisateurs peuvent modifier le type de requête ou choisir une autre rubrique s’ils le souhaitent. La navigation de la zone Demandes s’affiche également.

1. Cliquez sur le bouton **Menu Principal** > **Demandes** > **Nouvelle requête**.
1. Continuez à sélectionner les groupes de rubriques et les rubriques de la file d’attente jusqu’à ce que vous atteigniez la file d’attente que vous souhaitez partager sur le tableau de bord, si vous souhaitez partager une file d’attente spécifique. Pour plus d’informations sur l’envoi de requêtes, voir [Création et envoi de requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >La sélection de groupes de rubriques et de rubriques de file d’attente est facultative.

1. Cliquez sur **Partager le chemin** dans le coin supérieur droit de la zone Nouvelle requête.

   Cette opération copie le lien vers la file d’attente des demandes ou la rubrique de la file d’attente lorsque vous l’affichez à l’écran. Les utilisateurs peuvent mettre à jour le type de requête ou l’un des groupes de rubriques et des rubriques de file d’attente disponibles.

   ![](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### Obtention d’un lien vers une file d’attente de requêtes et possibilité de modifier le type de requête {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

Lorsque vous partagez un lien vers un type de requête, le type de requête est sélectionné pour l’utilisateur. Cela s’avère utile lorsque les utilisateurs doivent choisir parmi plusieurs groupes de rubriques ou rubriques de file d’attente pour le même type de requête. Les utilisateurs peuvent modifier le type de requête et en choisir un autre. La navigation de la zone Demandes s’affiche également.

1. Accédez à un projet désigné comme une file d’attente de requêtes.

   Pour plus d’informations sur la création d’une file d’attente de requêtes à partir d’un projet, accédez à [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Accédez à **Détails de la file**.
1. Copiez le code que vous trouverez dans la variable **URL d’accès direct** champ .

   Le code doit ressembler à ce qui suit :

   ```
   <samp>https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=</samp>
   ```

   Il s’agit du lien vers la file d’attente des demandes associée au projet sélectionné. Le type de demande est présélectionné.

   Les utilisateurs peuvent sélectionner n’importe quel groupe de rubriques ou rubrique de file d’attente, ou choisir un autre type de requête.

   ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### Obtention d’un lien vers une file d’attente de requêtes sans possibilité de modifier le type de requête {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

Lorsque vous partagez un lien vers un type de requête présélectionné, le type de requête est sélectionné pour l’utilisateur et ne peut pas être modifié (il est grisé). Les utilisateurs peuvent choisir les groupes de rubriques ou les rubriques de la file d’attente dont ils ont besoin. Cela s’avère utile lorsque vous ne souhaitez pas que les utilisateurs visualisent et sélectionnent d’autres types de requêtes. La navigation de la zone Demandes ne s’affiche pas.

1. Accédez à un projet désigné comme une file d’attente de requêtes.

   Pour plus d’informations sur la création d’une file d’attente de requêtes à partir d’un projet, accédez à [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Accédez à **Détails de la file**.
1. Copiez le code que vous trouverez dans la variable **Code incorporé** champ .

   Le code doit ressembler à ce qui suit :

   ```
   <samp><iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe></samp>
   ```

1. Modifiez le code afin de ne conserver que les informations ci-dessous :

   ```
   <samp>https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71</samp>
   ```

   >[!TIP]
   >
   >Vous pouvez conserver la variable `<samp>iframe </samp>` lors de l’incorporation du code dans une application autre que Workfront.

   Il s’agit du lien vers la file d’attente des demandes associée au projet sélectionné. Le type de requête est présélectionné et ne peut pas être modifié.

   Les utilisateurs peuvent sélectionner n’importe quel groupe de rubriques ou rubrique de file d’attente pour le type de requête sélectionné. Les utilisateurs ne peuvent pas sélectionner un autre type de requête.

   ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## Incorporation d’une file d’attente de requêtes dans un tableau de bord

Vous pouvez incorporer un lien vers la file d’attente des demandes ou vers une rubrique de la file d’attente imbriquée sous une file d’attente des demandes dans un tableau de bord pour donner aux utilisateurs un accès direct à la saisie des demandes.

1. Obtenez une URL de file d’attente des demandes à l’aide de l’une des méthodes décrites dans la section [Obtention de l’URL de la file d’attente des demandes](#obtain-the-url-of-the-request-queue) de cet article.
1. Cliquez sur le bouton **Menu Principal** > **Tableaux de bord** > **Nouveau tableau de bord**.
1. Saisissez un **Nom** pour le tableau de bord. Champ obligatoire.
1. Cliquez sur **Ajouter une page externe**.

   ![](assets/add-external-page-highlighted---nwe-350x214.png)

1. Dans le **Ajouter une page externe** modifiez les champs suivants :

   * **Nom**: saisissez le nom de la file d’attente des demandes tel que vous souhaitez le voir apparaître dans le tableau de bord. Champ obligatoire.

   * **Description**: saisissez une description de l’affichage de cette page externe. Ce champ n’est pas obligatoire et il est important uniquement à des fins de création de rapports. Il ne s’affiche pas dans le tableau de bord.
   * **URL**: collez l’URL que vous avez obtenue à l’aide de l’une des méthodes décrites à l’étape 1.

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <MadCap:conditionalText data-mc-conditions="">   
     (NOTE: ensure this stays accurate)   
     </MadCap:conditionalText>   
     </MadCap:conditionalText>   
     -->

   * **Hauteur**: saisissez la hauteur de la page externe. Cela définit l’espace occupé par la page externe contenant la file d’attente des demandes sur le tableau de bord. Il s’agit d’un champ obligatoire dont la valeur par défaut est 500.

1. Cliquer sur **Enregistrer**.
1. Cliquez sur **Enregistrer + Fermer**. 

   La file d’attente des demandes s’affiche dans le tableau de bord sous la forme d’un composant de tableau de bord distinct.

   ![](assets/new-dashboard-with-embedded-request-queue-nwe-350x260.png)

1. (Facultatif) Cliquez sur **Actions du tableau de bord**, puis **Modifier** pour ajouter des rapports, des calendriers ou d’autres pages externes au même tableau de bord.\
   Pour plus d’informations sur l’ajout de composants à un tableau de bord, voir [Création d’un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

 

 

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - old information)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> > Requests >&nbsp;<strong>New Request</strong>. </p> </li>
<li class="preview" value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Continue entering the request.&nbsp;For information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>. </p> </li>
<li value="3"> <p>Select the <strong>Request Type</strong> for the queue you would like added to the dashboard.</p> </li>
<li value="4"> <p>(Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance.</p> </li>
<li class="preview" value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <strong>Share path</strong> to obtain a shared link from the request queue you want to embed on a dashboard.</p> <p>For information about sharing a request queue, see <a href="../../../manage-work/requests/create-requests/share-link-to-request-queue.md" class="MCXref xref">Share a link to a request queue</a></p> </li>
<li value="6"> <p>For example, enter a URL similar to one of the following: </p> </li>
</ol>
-->
