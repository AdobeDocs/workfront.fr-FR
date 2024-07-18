---
title: Configurer le mappage des métadonnées
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Les métadonnées sont des informations descriptives associées à un document. Vous pouvez configurer  [!DNL Adobe Workfront]  pour inclure des métadonnées avec des documents envoyés aux applications  [!DNL Workfront] .
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 20%

---

# Configurer le mappage des métadonnées

Les métadonnées sont des informations descriptives associées à un document. Vous pouvez configurer [!DNL Adobe Workfront] pour inclure des métadonnées avec des documents envoyés aux applications [!DNL Workfront].

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices</a>.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## À propos des métadonnées [!DNL Workfront]

Les métadonnées des documents dans [!DNL Workfront] peuvent inclure des informations telles que le nom du projet associé, la description de la tâche ou la date d’achèvement prévue. En tant qu&#39;administrateur [!DNL Workfront], vous pouvez configurer [!DNL Workfront] pour inclure des métadonnées avec des documents envoyés de [!DNL Workfront] aux applications [!DNL Workfront] suivantes :

* [!DNL Workfront DAM]

Avant de pouvoir envoyer des métadonnées avec des documents, vous devez d’abord spécifier, ou mapper, les métadonnées que vous souhaitez inclure. Vous pouvez mapper n’importe quel champ utilisé dans [!DNL Workfront]. Une fois que vous avez configuré le mappage des métadonnées, tous les documents chargés dans une application [!DNL Workfront] incluront les métadonnées mappées.

Lorsqu’un utilisateur envoie un document de [!DNL Workfront] vers une application [!DNL Workfront], les métadonnées mappées sont transférées le long du document. Bien que la version du document dans l’application [!DNL Workfront] soit liée à [!DNL Workfront], les modifications apportées aux métadonnées du document dans [!DNL Workfront] ne sont pas répercutées dans les métadonnées du document dans l’application [!DNL Workfront]. Si un champ mappé dans [!DNL Workfront] est modifié, vous devez envoyer une nouvelle version du document avec les métadonnées mises à jour à l’application [!DNL Workfront].

>[!NOTE]
>
>Vous ne pouvez mapper les métadonnées que dans une seule direction : de [!DNL Workfront] vers [!DNL Workfront DAM]. Les métadonnées des documents liés à [!DNL Workfront] depuis [!DNL Workfront DAM] ne peuvent pas être transférées vers Workfront.

Vous pouvez mapper le même champ [!DNL Workfront] à différents champs de métadonnées dans [!DNL Workfront DAM], mais vous ne pouvez pas utiliser un champ de métadonnées dans l’une de ces applications pour plusieurs champs de métadonnées [!DNL Workfront].

Pour configurer plusieurs champs [!DNL Workfront] à exporter vers un champ de métadonnées dans une application [!DNL Workfront], créez d’abord un champ personnalisé calculé dans [!DNL Workfront] afin d’afficher tous les champs personnalisés individuels d’un objet. Associez ensuite le champ [!DNL Workfront] calculé à un champ de métadonnées dans l’application [!DNL Workfront]. Pour plus d’informations sur les champs personnalisés calculés, voir [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Avant de pouvoir mapper des champs pour le processus de mappage des métadonnées, vous devez activer l’application dans [!DNL Workfront]. Pour plus d’informations, voir [Configuration des intégrations de documents](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configurer [!DNL Workfront] pour envoyer des métadonnées

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Mappage des métadonnées]**.

   ![](assets/metadata-mapping.png)

1. Dans la zone **[!UICONTROL Select Source Field for Mapping]**, commencez à saisir le nom du champ Workfront que vous souhaitez mapper à [!DNL Workfront DAM], puis sélectionnez-le lorsque vous le verrez dans la liste.
1. Dans la zone **[!UICONTROL Sélectionner le champ cible pour le mappage]**, sélectionnez le champ à remplir avec les informations du champ [!DNL Workfront] sélectionné.

1. Cliquez sur **[!UICONTROL Ajouter un mappage]**.

   Le champ mappé s’affiche dans les champs mappés répertoriés au bas de la page.

1. Répétez les étapes 5 et 6 jusqu’à ce que vous ajoutiez tous les champs [!DNL Workfront] souhaités et leurs champs [!DNL Workfront DAM] correspondants.

## Supprimer les champs mappés

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur.
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Mappage des métadonnées]**.

1. Dans la liste des champs mappés, sélectionnez les champs à supprimer du mappage des métadonnées.
1. Cliquez sur **[!UICONTROL Supprimer]**.

   Les champs désignés ne sont plus mappés. Désormais, lorsqu’un utilisateur envoie un document de [!DNL Workfront] à [!DNL Workfront DAM], les métadonnées contenues dans les champs supprimés ne sont pas transférées avec le document.

   Un document envoyé avant la suppression des champs mappés conserve les métadonnées d’origine qui lui sont envoyées, y compris les métadonnées des champs supprimés.
