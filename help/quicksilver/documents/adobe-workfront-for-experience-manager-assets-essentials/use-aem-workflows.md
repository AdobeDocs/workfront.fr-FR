---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilisation des workflows dans l’intégration de Experience Manager Assets Essentials
description: Utilisation des workflows dans l’intégration de Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 038f5f3c941ea69feb43492a30b5abea39f7c932
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Utilisation des workflows dans l’intégration Experience Manager Assets

Un workflow est un ensemble d’actions qui connectent Workfront à Adobe Experience Manager as a Cloud Service. Un administrateur Workfront peut configurer des workflows dans Workfront, puis les affecter à des modèles de projet. Lorsqu’un projet est créé à l’aide d’un modèle de projet auquel un workflow est affecté, les actions définies dans le workflow sont déclenchées.

>[!NOTE]
>
>Les workflows sont disponibles uniquement dans une intégration Adobe Experience Manager as a Cloud Service. Ils ne sont pas disponibles dans les intégrations avec Adobe Experience Manager Assets Essentials.


## Exigences d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>Formule Adobe Workfront*</strong>
   </td>
   <td>Tous
   </td>
  </tr>
  <tr>
   <td><strong>Licences Adobe Workfront*</strong>
   </td>
   <td>Requête ou supérieure
   </td>
  </tr>
  <tr>
   <td><strong>Produit</strong>
   </td>
   <td><p>Vous devez disposer d’Experience Manager Assets as a Cloud Service ou d’Assets Essentials, et vous devez être ajouté au produit en tant qu’utilisateur dans le Admin Console.</p><p>Pour créer des dossiers liés, vous devez disposer d’un accès en écriture au référentiel dans Adobe Experience Manager.</p>&gt;
   </td>
  </tr>
  <tr>
   <td><strong>Paramétrages du niveau d'accès*</strong>
   </td>
   <td>Modifier l’accès aux documents
<p>
<strong>Remarque : </strong>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <strong>Création ou modification de niveaux d’accès personnalisés</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Autorisations d’objet</strong>
   </td>
   <td>Gérer l’accès ou une version ultérieure sur le projet 
<p>
Pour plus d’informations sur la demande d’accès supplémentaire, voir <strong>Demande d’accès aux objets </strong>.
   </td>
  </tr>
</table>

## Conditions préalables

Avant de commencer,

* Votre administrateur Workfront doit configurer les workflows dans une intégration Adobe Experience Manager. Pour plus d’informations, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Ajouter un workflow à un modèle

Vous pouvez ajouter un workflow à un modèle de projet. Le workflow sera appliqué à tous les projets créés à partir du modèle.

1. <!-- main menu snippet??--> Ouvrez un modèle en cliquant sur **Modèles** dans le menu principal, puis en sélectionnant le modèle dans la liste.
1. Cliquez sur **Experience Manager Assets** dans le panneau de navigation de gauche.

   >[!NOTE]
   >
   >Si la section Experience Manager Assets n’est pas visible dans le volet de navigation de gauche, votre administrateur Workfront n’a pas activé les workflows pour votre organisation. <!--Is this right?-->

1. Dans le **Sélection d’une intégration pour un champ de workflows automatisés**, sélectionnez l&#39;intégration aux workflows que vous souhaitez utiliser pour les projets créés à partir de ce modèle.
1. (Facultatif) Modifiez les valeurs de workflow que vous souhaitez appliquer aux projets créés à partir de ce modèle.

   Par exemple, pour créer un dossier lié à un emplacement autre que la valeur par défaut, saisissez l’emplacement du dossier lié.

   Seuls les workflows qui ont été activés dans la zone Experience Manager de la configuration sont disponibles dans les modèles ou les projets.

1. Vos modifications sont automatiquement enregistrées. <!-- do they though??-->

## Ajout d’un workflow à un projet

Vous pouvez ajouter un workflow lors de la création d’un projet ou un workflow à un projet existant. Dans les deux cas, vous utiliserez un modèle de projet pour ajouter le workflow.

### Ajout d’un workflow lors de la création d’un projet

1. Commencez à créer un projet.

   Pour obtenir des instructions, voir [Création d’un projet à l’aide d’un modèle](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Lors de la sélection d’un modèle pour le projet, sélectionnez le modèle contenant les workflows que vous souhaitez utiliser pour ce projet.
1. (Facultatif) Modifiez toutes les valeurs de workflow du projet, comme décrit dans la section [Modification des valeurs d’un workflow dans un projet](#edit-workflow-values-in-a-project).

   Seuls les workflows qui ont été activés dans la zone Experience Manager de la configuration sont disponibles dans les modèles ou les projets.


### Ajout d’un workflow à un projet existant

1. Commencez à ajouter un modèle au projet.

   Pour obtenir des instructions, voir [Joindre un modèle à un projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Lors de la sélection d’un modèle pour le projet, sélectionnez le modèle contenant les workflows que vous souhaitez utiliser pour ce projet.
1. (Facultatif) Modifiez toutes les valeurs de workflow du projet, comme décrit dans la section [Modification des valeurs d’un workflow dans un projet](#edit-workflow-values-in-a-project).

### Modification des valeurs d’un workflow dans un projet

Vous pouvez modifier les valeurs de workflow au niveau du projet. Les valeurs de workflow au niveau du projet remplacent les valeurs définies sur le modèle de projet, qui remplacent les valeurs par défaut définies dans l’intégration d’Adobe Experience Manager Assets.

Toutes les valeurs de workflow se trouvent dans :

* La section Workflows de la fenêtre Créer un projet ou Modifier le projet .
* La section Adobe Experience Manager du volet de navigation de gauche.


   >[!NOTE]
   >
   >Si ces zones ne sont pas visibles, votre administrateur Workfront n’a pas activé les workflows pour votre organisation.

#### Dossiers liés

Pour éditer le workflow des dossiers liés :

1. Activez/désactivez la variable **[!UICONTROL Créer un dossier lié]** sur .
1. Sélectionnez un chemin d’accès au dossier pour indiquer où vous souhaitez tous les dossiers liés associés à cette intégration.
1. Cliquez sur Enregistrer si vous utilisez la fenêtre Créer un projet ou Modifier le projet .

   Ou

   Si vous vous trouvez dans la zone Adobe Experience Manager, vos modifications sont automatiquement enregistrées. <!--Do they though?-->

