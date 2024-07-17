---
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-workfront-proofing-viewer
title: Comparer des épreuves dans la visionneuse de relecture
description: Vous pouvez afficher des comparaisons côte à côte de deux bons à tirer. Il peut s’agir de deux versions du même BAT ou de deux bons à tirer complètement distincts.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d4ec0c53-1451-4475-aa38-2319c6432936
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 1%

---

# Comparer des épreuves dans la visionneuse de relecture

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Vous pouvez afficher des comparaisons côte à côte de deux bons à tirer. Il peut s’agir de deux versions du même BAT ou de deux bons à tirer complètement distincts.

## Comparaison des versions de BAT {#compare-proof-versions}

1. Ouvrez le BAT qui comporte plusieurs versions que vous souhaitez comparer.
1. Dans le coin supérieur gauche de la visionneuse de vérification qui s’affiche, cliquez sur le nom du BAT. Ensuite, dans la liste des versions qui s’affiche, cliquez sur l’icône **Comparer** en regard de la version que vous souhaitez ouvrir et comparer.

   ![](assets/compare-proofs-choose-version-350x115.jpg)

   Les bons à tirer s’affichent côte à côte, avec la version la plus récente sur le côté gauche.

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Separate breadcrumbs above each proof allow you to view and go to the work item associated with the proof:</p>
   -->

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/compare-proofs-breadcrumbs-350x148.jpg" style="width: 350;height: 148;"> </p>
   -->

1. Poursuivez en [utilisant les outils de comparaison](#use-the-compare-tools).

## Comparaison de BAT distincts {#compare-separate-proofs}

Vous pouvez comparer deux bons à tirer distincts.

* [Comparaison de BAT distincts dans [!DNL Workfront]](#compare-separate-proofs-in-workfront)
* [Comparaison de BAT distincts dans [!DNL Workfront Proof]](#compare-separate-proofs-in-workfront-proof)

### Comparaison de BAT distincts dans [!DNL Workfront] {#compare-separate-proofs-in-workfront}

Pour plus d’informations sur la comparaison de BAT distincts de la liste de documents dans [!DNL Workfront], reportez-vous à la section [Comparer deux BAT différents](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md#comparing-two-proofs-from-a-document-list) de l’article [Comparer des BAT](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md) .

### Comparaison de BAT distincts dans [!DNL Workfront Proof] {#compare-separate-proofs-in-workfront-proof}

>[!NOTE]
>
>Les bons à tirer comparés doivent se trouver dans le même dossier et au même niveau de hiérarchie au sein de la structure de dossiers. Pour plus d’informations sur l’utilisation de dossiers pour regrouper les bons à tirer que vous souhaitez comparer, voir [Utilisation de plusieurs bons à tirer dans la visionneuse de vérification de la qualité](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/work-with-multiple-proofs.md)

1. Ouvrez l’un des BAT que vous souhaitez comparer dans la visionneuse de BAT.
1. Cliquez sur l’icône **[!UICONTROL Mode de comparaison]** .

   ![BAT_compare_icon.png](assets/proof-compare-icon.png)\
   La zone d’affichage se divise en deux et le BAT s’affiche à la fois sur la gauche et sur le côté droit de la visionneuse de vérification.

   ![Compare_proofs-versions.png](assets/compare-proofs-versions-350x180.png)

1. Cliquez sur l&#39;icône [!UICONTROL folder] au-dessus du BAT, soit sur le côté gauche, soit sur le côté droit, pour répertorier les autres BAT dans le même dossier.

   ![Folder_icons_when_compare_in_proofing_viewer.png](assets/folder-icons-when-comparing-in-proofing-viewer-350x121.png)

1. Dans la liste, cliquez sur le nom du BAT que vous souhaitez comparer au BAT actuellement ouvert dans la visionneuse de BAT.

   ![Comparing_proofs-list_of_proofs_in_folder.png](assets/comparing-proofs-list-of-proofs-in-folder-350x89.png)

   Les deux bons à tirer s’affichent.

1. Poursuivez en [utilisant les outils de comparaison](#use-the-compare-tools).

## Utilisation des outils de comparaison {#use-the-compare-tools}

La visionneuse de vérification fournit divers outils pour comparer les bons à tirer de manière efficace et efficace.

* [Comparaison automatique des bons à tirer](#auto-compare-proofs)
* [Comparaison de BAT dans une superposition](#compare-proofs-in-an-overlay)
* [Comparaison simultanée de navigation](#simultaneous-navigation-comparison)

### Comparaison automatique des bons à tirer {#auto-compare-proofs}

La comparaison automatique effectue une comparaison pixel par pixel entre deux bons à tirer statiques ou vidéo. Toutes les différences détectées sont surlignées en rouge dans le BAT sur la gauche.

La comparaison automatique n’est pas disponible lorsque vous comparez des bons à tirer interactifs.

Pour comparer automatiquement deux bons à tirer :

1. Commencez par comparer les bons à tirer de l’une des façons suivantes :

   * Comparez deux versions du même BAT (voir [Comparaison des versions de BAT](#compare-proof-versions) dans cet article).
   * Comparez deux bons à tirer distincts (voir [Comparer des bons à tirer distincts](#compare-separate-proofs) dans cet article).

1. Cliquez sur l’icône **[!UICONTROL Autocompare]** .

   ![BAT_autocompare_icon.png](assets/proof-autocompare-icon-31x32.png)

   Toutes les différences entre les deux bons à tirer sont indiquées en rouge dans le bon à tirer à gauche.

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer]** pour modifier le côté actif afin que les différences s’affichent sur le BAT sur le côté droit. Par défaut, les différences s’affichent sur le BAT sur le côté gauche.

   ![BAT_autocompare_changeactive.png](assets/proof-autocompare-changeactive.png)

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Couleur]** pour modifier la couleur et l’opacité utilisées lors de la mise en surbrillance des différences.

   ![BAT_compare_color.png](assets/proof-compare-color.png)

### Comparaison de BAT dans une superposition {#compare-proofs-in-an-overlay}

La comparaison des superpositions permet d’afficher les différences entre deux bons à tirer statiques en affichant les deux bons à tirer comme un seul bon à tirer, tout en fournissant un séparateur vertical au centre du bon à tirer. Lorsque vous faites défiler le BAT par-dessus le séparateur vertical, les différences s’affichent.

>[!NOTE]
>
>La comparaison de superpositions n’est pas disponible lorsque vous comparez des bons à tirer vidéo ou interactifs.

Pour activer la comparaison des superpositions :

1. Commencez par comparer les bons à tirer de l’une des façons suivantes :

   * Comparez deux versions du même BAT (voir [Comparaison des versions de BAT](#compare-proof-versions) dans cet article).
   * Comparez deux bons à tirer distincts (voir [Comparer des bons à tirer distincts](#compare-separate-proofs) dans cet article).

1. Cliquez sur l’icône **[!UICONTROL Superposition]** .

   ![BAT_compare_overlay_icon.png](assets/proof-compare-overlay-icon.png)

   Les deux bons à tirer s&#39;affichent sous la forme d&#39;un BAT unique, avec un séparateur vertical au centre du BAT.

1. Effectuez l’une des opérations suivantes :

   * Faites passer le BAT par-dessus le séparateur vertical. Pendant que vous cassez, vous voyez le BAT à gauche sur le côté gauche du séparateur vertical, tandis que le BAT à droite s&#39;affiche sur le côté droit.
   * Déplacez le séparateur vertical vers la gauche et la droite. Lorsque vous déplacez le séparateur, vous voyez le BAT sur la gauche du séparateur vertical, tandis que le BAT sur la droite s&#39;affiche sur le côté droit.

### Comparaison simultanée de navigation {#simultaneous-navigation-comparison}

La navigation simultanée est activée par défaut lors de la comparaison des bons à tirer. Il est disponible lorsque vous comparez un BAT statique et un BAT statique ou lorsque vous comparez un BAT vidéo et un BAT vidéo. Elle n’est pas disponible lors de la comparaison d’un BAT statique et d’un BAT vidéo.

**BAT statique :** Lorsque cette option est activée sur les BAT statiques, la navigation simultanée verrouille le niveau et la position du zoom des deux BAT lors du défilement ou du défilement. Lorsqu’un BAT contient plusieurs pages et que la navigation simultanée est activée, la modification de pages dans un BAT entraîne la modification de la page dans l’autre BAT.

**BAT vidéo :** Lorsqu’elle est activée sur les bons à tirer vidéo, la navigation simultanée mémorise la différence de temps sur les chronologies des deux bons à tirer.

Pour activer la navigation simultanée si elle n’est pas déjà activée :

1. Commencez par comparer les bons à tirer de l’une des façons suivantes :

   * Comparez deux versions du même BAT (voir [Comparaison des versions de BAT](#compare-proof-versions) dans cet article).
   * Comparez deux bons à tirer distincts (voir [Comparer des bons à tirer distincts](#compare-separate-proofs) dans cet article).

1. Cliquez sur l’icône **[!UICONTROL Navigation simultanée]** .

   ![BAT_compare_simultan_icon.png](assets/proof-compare-simultaneous-icon.png)

1. (Facultatif) Cliquez à tout moment sur l’icône **[!UICONTROL Réinitialiser]** pour réinitialiser le niveau et la position du zoom (pour le BAT statique) ou la chronologie (pour les BAT vidéo).

   ![BAT_compare_simultan_reset.png](assets/proof-compare-simultaneous-reset.png)

## Quitter le mode de comparaison

1. Fermez le BAT que vous ne souhaitez plus afficher en cliquant sur l’icône (x) dans le coin supérieur gauche du BAT.

   ![BAT_compare_exit.png](assets/proof-compare-exit-350x163.png)

   La preuve que vous ne fermez pas reste ouverte dans la visionneuse de vérification.
