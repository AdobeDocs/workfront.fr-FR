---
title: Configuration du mappage des métadonnées
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Les métadonnées sont des informations descriptives associées à un document. Vous pouvez configurer [!DNL Adobe Workfront] pour inclure des métadonnées aux documents envoyés à [!DNL Workfront] applications.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# Configuration du mappage des métadonnées

Les métadonnées sont des informations descriptives associées à un document. Vous pouvez configurer [!DNL Adobe Workfront] pour inclure des métadonnées aux documents envoyés à [!DNL Workfront] applications.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## A propos [!DNL Workfront] metadata

Métadonnées des documents dans [!DNL Workfront] peut inclure des informations telles que le nom du projet, la description de la tâche ou la date d’achèvement prévue associée. Comme [!DNL Workfront] administrateur, vous pouvez configurer [!DNL Workfront] pour inclure des métadonnées aux documents envoyés depuis [!DNL Workfront] à ce qui suit : [!DNL Workfront] applications :

* [!DNL Workfront DAM]

Avant de pouvoir envoyer des métadonnées avec des documents, vous devez d’abord spécifier, ou mapper, les métadonnées que vous souhaitez inclure. Vous pouvez mapper n’importe quel champ utilisé dans [!DNL Workfront]. Une fois que vous avez configuré le mappage des métadonnées, tous les documents chargés dans un [!DNL Workfront] l’application comprend les métadonnées mappées.

Lorsqu’un utilisateur envoie un document à partir d’ [!DNL Workfront] à [!DNL Workfront] , les métadonnées mappées sont transférées le long du document. Pendant que la version du document dans la variable [!DNL Workfront] l’application est liée à [!DNL Workfront], modifications apportées aux métadonnées du document dans [!DNL Workfront] ne sont pas reflétées dans les métadonnées du document dans la variable [!DNL Workfront] application. Si un champ mappé dans [!DNL Workfront] est modifié, vous devez envoyer une nouvelle version du document avec les métadonnées mises à jour à la variable [!DNL Workfront] application.

>[!NOTE]
>
>Vous ne pouvez mapper les métadonnées que dans une seule direction : de [!DNL Workfront] to [!DNL Workfront DAM]. Métadonnées pour les documents liés à [!DNL Workfront] de [!DNL Workfront DAM] ne peut pas être transféré vers Workfront.

Vous pouvez mapper la même [!DNL Workfront] de différents champs de métadonnées dans [!DNL Workfront DAM], mais vous ne pouvez pas utiliser un champ de métadonnées dans l’une de ces applications pour plusieurs [!DNL Workfront] champs de métadonnées.

Pour configurer plusieurs [!DNL Workfront] champs à exporter vers un champ de métadonnées dans un [!DNL Workfront] application, commencez par créer un champ personnalisé calculé dans [!DNL Workfront] pour afficher tous les champs personnalisés d’un objet. Associez ensuite le calcul [!DNL Workfront] à un champ de métadonnées dans la variable [!DNL Workfront] application. Pour plus d’informations sur les champs personnalisés calculés, voir [Ajout de données calculées à un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Avant de pouvoir mapper des champs pour le processus de mappage des métadonnées, vous devez activer l’application dans [!DNL Workfront]. Pour plus d’informations, voir [Configuration des intégrations de documents](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configurer [!DNL Workfront] envoi de métadonnées

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Mappage des métadonnées]**.

   ![](assets/metadata-mapping.png)

1. Dans le **[!UICONTROL Sélectionner le champ source pour le mappage]** , commencez à saisir le nom du champ Workfront auquel vous souhaitez mapper l’élément. [!DNL Workfront DAM], puis sélectionnez-le lorsque vous le verrez dans la liste.
1. Dans le **[!UICONTROL Sélectionner le champ cible pour le mappage]** , sélectionnez le champ à renseigner avec les informations dans la [!DNL Workfront] champ .

1. Cliquez sur **[!UICONTROL Ajouter un mappage]**.

   Le champ mappé s’affiche dans les champs mappés répertoriés au bas de la page.

1. Répétez les étapes 5 et 6 jusqu’à ce que vous ajoutiez tous les éléments de votre choix. [!DNL Workfront] les champs et leurs [!DNL Workfront DAM] champs.

## Suppression des champs mappés

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur.
1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Mappage des métadonnées]**.

1. Dans la liste des champs mappés, sélectionnez les champs à supprimer du mappage des métadonnées.
1. Cliquez sur **[!UICONTROL Supprimer]**.

   Les champs désignés ne sont plus mappés. Maintenant, lorsqu’un utilisateur envoie un document à partir d’ [!DNL Workfront] to [!DNL Workfront DAM], les métadonnées contenues dans les champs supprimés ne sont pas transférées avec le document.

   Un document envoyé avant la suppression des champs mappés conserve les métadonnées d’origine qui lui sont envoyées, y compris les métadonnées des champs supprimés.
