---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utiliser des workflows dans l’intégration d’Experience Manager Assets Essentials
description: Utiliser des workflows dans l’intégration d’Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 99924f690c53584c090d19fff90d23d84ec306d4
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 98%

---

# Utiliser des workflows dans l’intégration d’Experience Manager Assets

Un workflow est un ensemble d’actions qui connectent Workfront à Adobe Experience Manager as a Cloud Service. Un administrateur Workfront peut configurer des workflows dans Workfront, puis les affecter à des modèles de projet.

Lorsqu’un projet est créé à l’aide d’un modèle de projet auquel un workflow est affecté, les actions définies dans le workflow sont déclenchées.

>[!NOTE]
>
>Les workflows sont disponibles uniquement dans une intégration d’Adobe Experience Manager as a Cloud Service. Ils ne sont pas disponibles dans les intégrations d’Adobe Experience Manager Assets Essentials.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>Plan Adobe Workfront*</strong>
   </td>
   <td>Tous
   </td>
  </tr>
  <tr>
   <td><strong>Licences Adobe Workfront*</strong>
   </td>
   <td>Requête ou supérieure
   </td>
  </tr>
  <tr>
   <td><strong>Produit</strong>
   </td>
   <td><p>Vous devez disposer d’Experience Manager Assets as a Cloud Service ou d’Assets Essentials, et quelqu’un doit vous ajouter au produit en tant qu’utilisateur ou utilisatrice dans Admin Console.</p><p>Vous devez disposer d’un accès en écriture au référentiel dans Adobe Experience Manager.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Configurations du niveau d’accès*</strong>
   </td>
   <td>Modifier l’accès aux documents
<p>
<strong>Remarque :</strong> si vous ne disposez toujours pas d’un accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires ont été configurées pour votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <strong>Créer ou modifier des niveaux d’accès personnalisés</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Autorisations d’objets</strong>
   </td>
   <td>Accès Gérer ou de niveau supérieur au projet 
<p>
Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <strong>Demander un accès aux objets</strong>.
   </td>
  </tr>
</table>

+++

## Conditions préalables

Avant de commencer

* Votre administrateur ou administratrice Workfront doit configurer des workflows dans une intégration d’Adobe Experience Manager. Pour plus d’informations, voir [Configurer l’intégration d’Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Ajouter un workflow à un modèle

Vous pouvez ajouter un workflow à un modèle de projet. Le workflow est appliqué à tous les projets créés à partir du modèle.

1. Ouvrez un modèle en cliquant sur **Modèles** dans le menu principal, puis sélectionnez le modèle dans la liste.
1. Cliquez sur **Experience Manager Assets** dans le panneau de navigation de gauche.

   >[!NOTE]
   >
   >Si la section Experience Manager Assets n’est pas visible dans le panneau de navigation de gauche, votre administrateur ou administratrice Workfront n’a pas activé les workflows pour votre organisation. <!--Is this right?-->

1. Dans le champ **Sélectionner une intégration pour les workflows automatisés**, sélectionnez l’intégration aux workflows que vous souhaitez utiliser pour les projets créés à partir de ce modèle.
1. (Facultatif) Modifiez les valeurs du workflow que vous souhaitez appliquer aux projets créés à partir de ce modèle.

   Pour obtenir des instructions sur des workflows spécifiques, voir [Modifier les valeurs d’un workflow dans un projet](#edit-workflow-values-in-a-project) dans cet article.

   Seuls les workflows qui ont été activés dans la zone Experience Manager de la configuration sont disponibles dans les modèles ou les projets.

1. Vos modifications sont automatiquement enregistrées. <!-- do they though??-->

## Ajouter un workflow à un projet

Vous pouvez ajouter un workflow lors de la création d’un projet ou ajouter un workflow à un projet existant. Dans les deux cas, vous utilisez un modèle de projet pour ajouter le workflow.

### Ajouter un workflow lors de la création d’un projet

1. Commencez à créer un projet.

   Pour plus d’informations, voir [Créer un projet à l’aide d’un modèle](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Lors de la sélection d’un modèle pour le projet, sélectionnez le modèle qui contient les workflows que vous souhaitez utiliser pour ce projet.
1. (Facultatif) Modifiez les valeurs du workflow pour le projet, comme décrit dans [Modifier les valeurs d’un workflow dans un projet](#edit-workflow-values-in-a-project).

   Seuls les workflows qui ont été activés dans la zone Experience Manager de la configuration sont disponibles dans les modèles ou les projets.


### Ajouter un workflow à un projet existant

>[!NOTE]
>
>Les workflows qui s’exécutent lors de la création d’un projet (comme la création de dossiers liés) ne s’exécutent pas lorsque le modèle est joint à un projet existant. Ils ne s’exécutent que lorsqu’un projet est créé à partir d’un modèle.

1. Commencez à ajouter un modèle au projet.

   Pour plus d’informations, voir [Joindre un modèle à un projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Lors de la sélection d’un modèle pour le projet, sélectionnez le modèle qui contient les workflows que vous souhaitez utiliser pour ce projet.
1. (Facultatif) Modifiez les valeurs du workflow pour le projet, comme décrit dans [Modifier les valeurs d’un workflow dans un projet](#edit-workflow-values-in-a-project).

   Seuls les workflows qui ont été activés dans la zone Experience Manager de la configuration sont disponibles dans les modèles ou les projets.



### Modifier les valeurs d’un workflow dans un projet

Vous pouvez modifier les valeurs d’un workflow au niveau d’un projet. Les valeurs d’un workflow au niveau d’un projet remplacent les valeurs définies dans le modèle de projet, qui remplacent elles-mêmes les valeurs par défaut définies dans l’intégration d’Adobe Experience Manager Assets.

Toutes les valeurs du workflow peuvent être consultées aux emplacements suivants :

* Section Workflows ou Dossiers liés de la fenêtre Créer un projet ou Modifier le projet.
* Section Adobe Experience Manager du panneau de navigation de gauche.


  >[!NOTE]
  >
  >Si ces zones ne sont pas visibles, c’est que votre administrateur ou administratrice Workfront n’a pas activé les Workflows pour votre organisation.



#### Dossiers liés

>[!NOTE]
>
>Les dossiers liés étant créés lors de la création du projet, la modification du workflow des dossiers liés sur un projet existant est inefficace. La modification de ces valeurs lors de la création d’un projet fonctionne comme prévu.

Pour modifier le workflow des dossiers liés :

1. Activez ou désactivez l’option **[!UICONTROL Créer un dossier lié]**. Si vous l’activez, vous pouvez ensuite modifier la configuration des dossiers liés.

   Pour plus d’informations sur la configuration des dossiers liés, voir [Créer des dossiers liés à Adobe Experience Manager](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) dans l’article [Configurer l’intégration [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Facultatif) Si vous souhaitez que l’arborescence de dossiers ne soit créée que si certaines valeurs sont présentes sur un formulaire personnalisé joint au projet, cliquez sur **Appliquer un filtre** pour cette arborescence de dossiers, sélectionnez le formulaire personnalisé qui contient le champ et la valeur du champ. Si le champ du formulaire personnalisé associé au nouveau projet contient la valeur choisie, l’arborescence de dossiers est créée.
1. (Facultatif) Lors de la configuration des noms de dossier, vous pouvez choisir parmi les options suivantes :

   * **Nom** : saisissez un nom pour le dossier.

   * **Données d’objet** : sélectionnez la source du nom du dossier, par exemple Nom du projet.

   * **Données de formulaire personnalisé** : sélectionnez les données de formulaire personnalisé à utiliser comme nom de dossier.

     L’utilisation de données de formulaire personnalisé pour les noms de dossiers est disponible uniquement au niveau du modèle et ne peut pas être configurée au niveau de l’intégration.

     Si un nom de dossier est défini sur des données personnalisées qui n’existent pas sur le formulaire personnalisé joint au projet, un ID aléatoire sera attribué comme nom de dossier.

1. Pour afficher l’arborescence de dossiers, cliquez sur l’icône **Aperçu** ![Preview icon](assets/preview-icon.png).
1. Cliquer sur **[!UICONTROL Enregistrer]**.

#### Publier des ressources

Pour modifier le workflow pour la publication des ressources :

1. Activez ou désactivez l’option **Publier automatiquement les ressources**.
1. (Le cas échéant) Si vous activez la publication, sélectionnez si vous souhaitez publier vers le service de publication, vers Brand Portal, ou les deux.
1. Cliquer sur **[!UICONTROL Enregistrer]**.
