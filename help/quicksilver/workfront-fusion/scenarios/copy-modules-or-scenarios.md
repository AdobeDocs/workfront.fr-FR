---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Copier des modules ou des scénarios dans  [!DNL Adobe Workfront Fusion]
description: Copier des modules ou des scénarios dans  [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 21%

---

# Copie de modules ou de scénarios dans [!DNL Adobe Workfront Fusion]

Vous pouvez copier des modules, des groupes de modules ou des scénarios entiers dans [!DNL Adobe Workfront Fusion]. Cette fonctionnalité vous permet de réutiliser des scénarios ou des parties de scénarios sans avoir à les créer à nouveau.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Vous devez ajouter des modules à un scénario avant de pouvoir les copier.

## Copier un module ou un groupe de modules

Lorsque vous copiez un module, la copie conserve toutes les valeurs de champ et tous les paramètres du module d’origine.

Vous pouvez coller le module ou les modules dans une autre zone du même scénario ou dans un autre scénario.

Tenez compte de ce qui suit lorsque vous collez des modules dans un scénario différent.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* Les valeurs de champ qui extraient des informations d’un autre module que vous n’avez pas copié ne peuvent plus accéder à ces informations. Vous devez définir ces champs pour extraire les informations du nouveau scénario.
* Si vous collez les modules dans un scénario détenu par une autre équipe ou organisation, toutes les connexions doivent être mises à jour vers les connexions détenues par le groupe ou l’organisation propriétaire du nouveau scénario.

### Copie de modules

La copie d’un groupe de modules est similaire à la copie d’un seul module.

1. Cliquez avec le bouton droit sur le module à copier.

   >[!NOTE]
   >
   >Vous pouvez sélectionner plusieurs modules en maintenant la touche [!UICONTROL shift] enfoncée et en cliquant sur les modules à copier. La copie d’un groupe de modules copie également toutes les lignes de connexion, tous les filtres ou toute logique de routage entre eux.

1. Sélectionnez **[!UICONTROL Copier le module]**.
1. Déplacez le curseur vers la zone du scénario où vous souhaitez obtenir la copie du scénario.
1. Cliquez avec le bouton droit de la souris, puis sélectionnez **[!UICONTROL Coller]**.
1. Connectez les modules collés au scénario en les faisant glisser à l’emplacement approprié dans le scénario.

   Vous pouvez également utiliser des raccourcis clavier pour copier et coller.

## Copie d’un scénario par clonage

Le clonage d’un scénario crée une copie du scénario, que vous pouvez ensuite modifier.

1. Ouvrez la page Détails du scénario :

   1. Cliquez sur l’onglet **[!UICONTROL Scénario]** dans le panneau de gauche, puis cliquez sur un scénario sur lequel vous souhaitez obtenir des détails.

      Ou

      Si vous travaillez sur le scénario dans l’[éditeur de scénario dan s [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md), cliquez sur la flèche gauche ![](assets/exit-editing-arrow.png) près du coin supérieur gauche de la fenêtre.

1. Cliquez avec le bouton droit de la souris sur **[!UICONTROL Options]** dans le coin supérieur droit de la page.
1. Sélectionnez **[!UICONTROL Clone]**.
1. (Facultatif) Saisissez un nom pour le nouveau scénario.
1. (Facultatif) Activez **[!UICONTROL Conserver les états de tous les nouveaux modules identiques à ceux en cours de duplication]** pour vous assurer que le scénario copié inclut également des informations sur les enregistrements les plus récents traités par le scénario d’origine.
1. Cliquez sur **[!UICONTROL Enregistrer]** pour créer le scénario.

## Copier un scénario à l’aide de plans directeurs

Les plans directeurs du scénario représentent la disposition, le mappage et les valeurs de champ d’un scénario donné à un moment donné. Vous pouvez exporter un plan directeur de scénario dans un fichier JSON sur votre ordinateur, puis l’importer lors de la création d’un nouveau scénario. Les scénarios importés à partir d’un plan directeur de scénario peuvent être modifiés.

Un plan directeur de scénario représente l’ensemble du scénario. Si vous souhaitez ne copier que certains modules d’un scénario, reportez-vous à la section [Copie d’un module ou d’un groupe de modules](#copy-a-module-or-a-group-of-modules) de cet article.

>[!NOTE]
>
>Pour plus d’informations sur les plans directeurs dans le contexte de [!DNL Adobe Workfront], voir [Présentation des plans directeurs](../../administration-and-setup/blueprints/blueprints-overview.md).

### Exportation d’un plan directeur de scénario

1. Dans le scénario, cliquez sur le menu **[!UICONTROL Plus]** dans la zone des paramètres du scénario.
1. Cliquez sur **[!UICONTROL Exporter le plan directeur]**.

   Un fichier JSON est créé et téléchargé sur votre ordinateur. Vous pouvez localiser ce fichier dans votre dossier [!DNL Downloads].

### Importation d’un plan directeur

>[!IMPORTANT]
>
>Si vous importez un plan directeur dans un scénario existant, le plan directeur du scénario remplace le scénario existant. Vous ne pouvez pas ajouter un plan directeur à un scénario existant.

1. Commencez à créer un scénario.
1. Dans le scénario, cliquez sur le menu **[!UICONTROL Plus]** dans la zone des paramètres du scénario.
1. Cliquez sur **[!UICONTROL Importer le plan directeur]**.
1. Dans la boîte de dialogue qui s’affiche, cliquez sur **[!UICONTROL Parcourir]**
1. Accédez au plan directeur à importer, puis cliquez sur **[!UICONTROL Ouvrir]**.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Un fichier JSON est créé et téléchargé sur votre ordinateur. Vous pouvez localiser ce fichier dans votre dossier [!UICONTROL Downloads].

## Copier et réutiliser des scénarios à l’aide de modèles

Vous pouvez créer des modèles comme point de départ pour vos scénarios [!DNL Workfront Fusion]. Lorsque vous créez un scénario à partir d’un modèle, vous pouvez le modifier sans le modifier. Les valeurs de champ ne sont pas enregistrées dans les modèles.

Pour plus d’informations sur la création et l’utilisation des modèles, voir [Modèles de scénario](../../workfront-fusion/scenarios/templates/fusion-templates.md).
