---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Dépannage des échecs de création de BAT
description: Le processus de création de BAT comprend l’importation et la génération de BAT. Parfois, lorsque vous créez un BAT, un fichier peut ne pas être importé ou le BAT peut ne pas être généré après l’importation du fichier.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# Dépannage des échecs de création de BAT

Le processus de création de BAT comprend l’importation et la génération de BAT. Parfois, lorsque vous créez un BAT, un fichier peut ne pas être importé ou le BAT peut ne pas être généré après l’importation du fichier.

>[!NOTE]
>
> Si le document que vous tentez de tester ne correspond à aucun des critères répertoriés dans cette section, veuillez contacter le support Adobe Workfront pour plus d’informations.

## Raisons de l’échec de l’importation

* Vous avez créé un BAT combiné contenant plus de 50 fichiers.

## Raisons de l’échec de génération de BAT

* Le type de fichier n’est pas pris en charge.\
  Pour obtenir la liste des types de fichiers pris en charge, reportez-vous à la section [ Types de fichiers de vérification pris en charge et présentation des limites de taille](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* La structure du fichier est une structure non standard pour le type de fichier.
* Le fichier est protégé par un mot de passe ou la copie de contenu est désactivée.

  Contrairement à d’autres types de fichiers, les fichiers du PDF peuvent être générés dans des bons à tirer si le paramètre de sécurité pour la copie de contenu est défini sur Autorisé sur le PDF.

* La longueur de la page ou le nombre de pages dépasse la limite.

  La longueur maximale autorisée des pages est de 195 pouces après la pixellisation ; le nombre maximal autorisé de pages est de 1 000 pages pour un seul BAT.

* Le fichier est endommagé ou corrompu.
* La date limite du workflow pour une nouvelle version du BAT se situe dans le passé.

  Cela se produit lorsque vous créez une version de BAT à l’aide d’une méthode de BAT rapide et que l’option **Générer automatiquement des BAT lors du téléchargement des documents** est sélectionnée. La nouvelle version du BAT tente de prendre les délais du workflow du BAT généré précédemment. La génération de la preuve échoue si ces délais sont passés. Pour remédier à ce problème, vous pouvez définir à l’avenir les échéances du workflow sur la version précédente ou générer une nouvelle version du BAT. Si vous générez une nouvelle version, utilisez **Plus > Nouvelle version > Bon à tirer** et sélectionnez **Les échéances des workflows à l&#39;avenir**.

* Lors de la vérification des fichiers de PDF, les raisons de l’échec de génération de BAT sont les suivantes :

   * Les polices et les images sont liées à des sources externes (telles que votre système de fichiers local).

     Les polices et les images doivent être incorporées dans le fichier du PDF pour s’afficher sur un autre ordinateur ou dans Workfront Proof.

   * Votre fichier de PDF contient des calques vides ou des champs transparents ou superposés.

     Si vous ne parvenez pas à déterminer quel calque ou objet est à l’origine de ce problème, exportez la conception/le document en tant que PDF optimisé (cela supprime tous les éléments indésirables).

