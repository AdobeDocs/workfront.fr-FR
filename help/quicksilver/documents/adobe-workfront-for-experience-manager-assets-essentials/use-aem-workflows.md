---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Utilisation des workflows dans l’intégration de Experience Manager Assets Essentials
description: Utilisation des workflows dans l’intégration de Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 83cd0960947108186f8d1d8ef2ad6c35c89820bd
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 0%

---

# Utilisation des workflows dans l’intégration Experience Manager Assets

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Elle est disponible uniquement dans l’environnement Aperçu de l’environnement de test.</span>

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
   <td>Quelconque
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
   <td><p>Vous devez disposer d’Experience Manager Assets as a Cloud Service ou d’Assets Essentials, et vous devez être ajouté au produit en tant qu’utilisateur dans le Admin Console.</p><p>Vous devez disposer d’un accès en écriture au référentiel dans Adobe Experience Manager.</p>
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

* Votre administrateur Workfront doit configurer des workflows dans une intégration Adobe Experience Manager. Pour plus d’informations, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Ajouter un workflow à un modèle

Vous pouvez ajouter un workflow à un modèle de projet. Le workflow sera appliqué à tous les projets créés à partir du modèle.

1. Ouvrez un modèle en cliquant sur **Modèles** dans le menu principal, puis sélectionnez le modèle dans la liste.
1. Cliquez sur **Experience Manager Assets** dans le panneau de navigation de gauche.

   >[!NOTE]
   >
   >Si la section Experience Manager Assets n’est pas visible dans le volet de navigation de gauche, votre administrateur Workfront n’a pas activé les workflows pour votre organisation. <!--Is this right?-->

1. Dans le **Sélection d’une intégration pour un champ de workflows automatisés**, sélectionnez l&#39;intégration aux workflows que vous souhaitez utiliser pour les projets créés à partir de ce modèle.
1. (Facultatif) Modifiez les valeurs de workflow que vous souhaitez appliquer aux projets créés à partir de ce modèle.

   Pour obtenir des instructions sur des workflows spécifiques, voir [Modification des valeurs d’un workflow dans un projet](#edit-workflow-values-in-a-project) dans cet article.

   Seuls les workflows qui ont été activés dans la zone Experience Manager de la configuration sont disponibles dans les modèles ou les projets.

1. Vos modifications sont automatiquement enregistrées. <!-- do they though??-->

## Ajout d’un workflow à un projet

Vous pouvez ajouter un workflow lors de la création d’un projet ou un workflow à un projet existant. Dans les deux cas, vous utiliserez un modèle de projet pour ajouter le workflow.

### Ajouter un workflow lors de la création d’un projet

1. Commencez à créer un projet.

   Pour obtenir des instructions, voir [Créer un projet à l’aide d’un modèle](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Lors de la sélection d’un modèle pour le projet, sélectionnez le modèle contenant les workflows que vous souhaitez utiliser pour ce projet.
1. (Facultatif) Modifiez toutes les valeurs de workflow du projet, comme décrit dans la section [Modification des valeurs d’un workflow dans un projet](#edit-workflow-values-in-a-project).

   Seuls les workflows qui ont été activés dans la zone Experience Manager de la configuration sont disponibles dans les modèles ou les projets.


### Ajouter un workflow à un projet existant

>[!NOTE]
>
>Les workflows qui s’exécutent lors de la création d’un projet (comme la création de dossiers liés) ne s’exécutent pas lorsque le modèle est joint à un projet existant. Elles ne s’exécutent que lorsqu’un projet est créé à partir d’un modèle.

1. Commencez à ajouter un modèle au projet.

   Pour obtenir des instructions, voir [Joindre un modèle à un projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Lors de la sélection d’un modèle pour le projet, sélectionnez le modèle contenant les workflows que vous souhaitez utiliser pour ce projet.
1. (Facultatif) Modifiez toutes les valeurs de workflow du projet, comme décrit dans la section [Modification des valeurs d’un workflow dans un projet](#edit-workflow-values-in-a-project).

   Seuls les workflows qui ont été activés dans la zone Experience Manager de la configuration sont disponibles dans les modèles ou les projets.



### Modification des valeurs d’un workflow dans un projet

Vous pouvez modifier les valeurs de workflow au niveau du projet. Les valeurs de workflow au niveau du projet remplacent les valeurs définies sur le modèle de projet, qui remplacent les valeurs par défaut définies dans l’intégration Adobe Experience Manager Assets.

Toutes les valeurs de workflow se trouvent dans :

* La section Workflows de la fenêtre Créer un projet ou Modifier le projet .
* La section Adobe Experience Manager du volet de navigation de gauche.


  >[!NOTE]
  >
  >Si ces zones ne sont pas visibles, votre administrateur Workfront n’a pas activé les workflows pour votre organisation.



#### Dossiers liés

>[!NOTE]
>
>Les dossiers liés étant créés lors de la création du projet, la modification du workflow des dossiers liés sur un projet existant est inefficace. La modification de ces valeurs lors de la création d’un projet fonctionne normalement.

Pour éditer le workflow des dossiers liés :

Dans l’environnement de production :

1. Basculer **[!UICONTROL Créer un dossier lié]** activé ou désactivé selon vos besoins.
1. (Conditionnel) Si vous activez les dossiers liés, choisissez un chemin d’accès au dossier pour indiquer où vous souhaitez tous les dossiers liés associés à cette intégration.
1. Cliquez sur **[!UICONTROL Enregistrer]** si vous utilisez la variable [!UICONTROL Créer un projet] ou [!UICONTROL Modifier le projet] fenêtre.

   Ou

   Si vous vous trouvez dans la variable [!DNL Adobe Experience Manager area], vos modifications sont enregistrées automatiquement. <!--Do they though?-->

Dans l’environnement Preview Sandbox :

<div class="preview">

1. Activez/désactivez la variable **[!UICONTROL Créer un dossier lié]** activé ou désactivé selon vos besoins. Si vous l’activez, vous pouvez ensuite modifier la configuration des dossiers liés.

   Pour plus d’informations sur la configuration des dossiers liés, voir [Création de dossiers liés à Adobe Experience Manager](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) dans l’article [Configurez la variable [!UICONTROL Experience Manager Assets as a Cloud Service] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Facultatif) Si vous souhaitez que l’arborescence de dossiers ne soit créée que si certaines valeurs sont présentes sur un formulaire personnalisé joint au projet, cliquez sur le bouton **Appliquer un filtre** pour cette arborescence de dossiers, sélectionnez le formulaire personnalisé qui contient le champ, le champ et la valeur du champ. Si le champ du formulaire personnalisé associé au nouveau projet contient la valeur choisie, l’arborescence de dossiers est créée.
1. (Facultatif) Lors de la configuration des noms de dossier, vous pouvez choisir parmi les options suivantes :

   * **Nom**: saisissez un nom pour le dossier.

   * **Données d’objet**: sélectionnez la source du nom du dossier, par exemple Nom du projet.

   * **Données de formulaire personnalisées**: sélectionnez les données de formulaire personnalisées à utiliser comme nom de dossier.

     L’utilisation de données de formulaire personnalisées pour les noms de dossiers est disponible uniquement au niveau du modèle et ne peut pas être configurée au niveau de l’intégration.

     Si un nom de dossier est défini sur des données personnalisées qui n’existent pas sur la personnalisation pour le joint au projet, un ID aléatoire sera attribué comme nom de dossier.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

</div>


#### Publication de ressources

Pour modifier le workflow de publication de ressources :

1. Basculer **Publier automatiquement les ressources** activé ou désactivé selon vos besoins.
1. (Conditionnel) Si vous activez la publication, choisissez si vous souhaitez publier du contenu sur le service de publication, sur le portail de marque ou les deux.
1. Cliquer sur **[!UICONTROL Enregistrer]**.
