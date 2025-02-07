---
title: Configurer le mappage des métadonnées
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Les métadonnées sont des informations descriptives associées à un document. Vous pouvez configurer  [!DNL Adobe Workfront]  pour inclure des métadonnées aux documents envoyés aux applications  [!DNL Workfront] .
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 96%

---

# Configurer le mappage des métadonnées

Les métadonnées sont des informations descriptives associées à un document. Vous pouvez configurer [!DNL Adobe Workfront] pour inclure des métadonnées aux documents envoyés aux applications [!DNL Workfront].

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations, consultez <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à un utilisateur ou à une utilisatrice un accès d’administration complet</a>.</p> <p><b>REMARQUE</b> : si vous ne disposez toujours pas de l’accès, demandez à votre administrateur ou administratrice [!DNL Workfront] si des restrictions supplémentaires ont été définies concernant votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## À propos des métadonnées [!DNL Workfront]

Les métadonnées des documents dans [!DNL Workfront] peuvent inclure des informations telles que le nom du projet, la description de la tâche ou la date d’achèvement prévue associée. En tant qu’administrateur ou administratrice [!DNL Workfront], vous pouvez configurer [!DNL Workfront] pour inclure des métadonnées aux documents envoyés depuis [!DNL Workfront] aux applications [!DNL Workfront] suivantes :

* [!DNL Workfront DAM]

Avant de pouvoir envoyer des métadonnées avec des documents, vous devez d’abord indiquer, ou mapper, les métadonnées que vous souhaitez inclure. Vous pouvez mapper n’importe quel champ utilisé dans [!DNL Workfront]. Une fois que vous avez configuré le mappage des métadonnées, tous les documents chargés dans une application [!DNL Workfront] inclut les métadonnées mappées.

Lorsqu’une personne envoie un document à partir de [!DNL Workfront] vers une application [!DNL Workfront], les métadonnées mappées sont transférées le long du document. Alors que la version du document dans l’application [!DNL Workfront] est liée à [!DNL Workfront], les modifications apportées aux métadonnées du document dans [!DNL Workfront] ne sont pas reflétées dans les métadonnées du document dans l’application [!DNL Workfront]. Si un champ mappé dans [!DNL Workfront] est modifié, vous devez envoyer une nouvelle version du document avec les métadonnées mises à jour à l’application [!DNL Workfront].

>[!NOTE]
>
>Vous ne pouvez mapper les métadonnées que dans une seule direction : de [!DNL Workfront] vers [!DNL Workfront DAM]. Les métadonnées pour les documents liés à [!DNL Workfront] de [!DNL Workfront DAM] ne peut pas être transférées vers Workfront.

Vous pouvez mapper le même champ [!DNL Workfront] à différents champs de métadonnées dans [!DNL Workfront DAM], mais vous ne pouvez pas utiliser un champ de métadonnées dans l’une de ces applications pour plusieurs champs de métadonnées [!DNL Workfront].

Pour configurer plusieurs champs [!DNL Workfront] à exporter vers un champ de métadonnées dans une application [!DNL Workfront], commencez par créer un champ personnalisé calculé dans [!DNL Workfront] pour afficher tous les champs personnalisés d’un objet. Associez ensuite le champ calculé [!DNL Workfront] à un champ de métadonnées dans l’application [!DNL Workfront]. Pour plus d’informations sur les champs calculés personnalisés, voir [ Ajouter des champs calculés à un formulaire ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Avant de pouvoir mapper des champs pour le processus de mappage des métadonnées, vous devez activer l’application dans [!DNL Workfront]. Pour plus d’informations, voir [Configurer des intégrations de documents](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configurer [!DNL Workfront] pour l’envoi de métadonnées

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Mappage des métadonnées]**.

   ![Mappage des métadonnées](assets/metadata-mapping.png)

1. Dans la boîte **[!UICONTROL Sélectionner le champ source pour le mappage]**, commencez à saisir le nom du champ Workfront que vous souhaitez mapper à [!DNL Workfront DAM], puis sélectionnez-le lorsque vous le verrez dans la liste.
1. Dans la boîte **[!UICONTROL Sélectionner le champ cible pour le mappage]**, sélectionnez le champ à renseigner avec les informations du champ [!DNL Workfront] sélectionné.

1. Cliquez sur **[!UICONTROL Ajouter un mappage]**.

   Le champ mappé s’affiche dans les champs mappés répertoriés au bas de la page.

1. Répétez les étapes 5 et 6 jusqu’à ce que vous ajoutiez tous les champs [!DNL Workfront] voulus et leurs champs [!DNL Workfront DAM] correspondants.

## Supprimer des champs mappés

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur ou administratrice.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Mappage des métadonnées]**.

1. Dans la liste des champs mappés, sélectionnez les champs à supprimer du mappage des métadonnées.
1. Cliquez sur **[!UICONTROL Supprimer]**.

   Les champs désignés ne sont plus mappés. Maintenant, lorsqu’une personne envoie un document à partir de [!DNL Workfront] vers [!DNL Workfront DAM], les métadonnées contenues dans les champs supprimés ne sont pas transférées avec le document.

   Un document envoyé avant la suppression des champs mappés conserve les métadonnées d’origine envoyées avec lui, y compris les métadonnées des champs supprimés.
