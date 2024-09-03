---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Résoudre les problèmes d’échec de création d’épreuve
description: Le processus de création d’épreuve comprend l’importation et la génération de l’épreuve. Parfois, lorsque vous créez une épreuve, un fichier peut ne pas être importé ou l’épreuve peut ne pas être générée après l’importation du fichier.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 100%

---


# Résoudre les problèmes d’échec de création d’épreuve

Le processus de création d’épreuve comprend l’importation et la génération de l’épreuve. Parfois, lorsque vous créez une épreuve, un fichier peut ne pas être importé ou l’épreuve peut ne pas être générée après l’importation du fichier.

>[!NOTE]
>
> Si le document que vous tentez de relire ne correspond à aucun des critères répertoriés dans cette section, veuillez contacter le service d’assistance Adobe Workfront pour plus d’informations.

## Raisons de l’échec de l’importation

* Vous avez créé une épreuve combinée contenant plus de 50 fichiers.

## Raisons de l’échec de la génération de l’épreuve

* Le type de fichier n’est pas pris en charge.\
  Pour obtenir la liste des types de fichiers pris en charge, voir [Vue d’ensemble des types et limites de taille des fichiers de relecture pris en charge](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* La structure du fichier est une structure non standard pour le type de fichier.
* Le fichier est protégé par un mot de passe ou la copie de contenu est désactivée.

  Contrairement à d’autres types de fichiers, les fichiers PDF peuvent être générés dans des épreuves si le paramètre de sécurité pour la copie de contenu est défini sur Autorisé sur le PDF.

* La longueur de la page ou le nombre de pages dépasse la limite.

  La longueur maximale autorisée des pages est de 195 pouces après la pixellisation ; le nombre maximal autorisé de pages est de 1 000 pages pour une seule épreuve.

* Le fichier est endommagé ou corrompu.
* L’échéance du workflow pour une nouvelle version de l’épreuve se situe dans le passé.

  Cela se produit lorsque vous créez une nouvelle version d’épreuve à l’aide d’une méthode d’épreuve rapide et que **Générer automatiquement des épreuves lors du téléchargement de documents** est sélectionné. La nouvelle version d’épreuve tente de prendre les échéances du workflow de l’épreuve générée précédemment. La génération de l’épreuve échoue si ces échéances sont passées. Pour remédier à ce problème, vous pouvez définir les échéances du workflow sur la version précédente pour qu’elles soit situées dans le futur, ou générer une nouvelle version de l’épreuve. Si vous générez une nouvelle version, utilisez **Plus > Nouvelle version > Épreuve** et sélectionnez **Échéances du workflow dans le furur**.

* Lors de la relecture des fichiers PDF, les raisons de l’échec de la génération de l’épreuve comprennent :

   * Les polices et les images sont liées à des sources externes (telles que votre système de fichiers local).

     Les polices et les images doivent être incorporées dans le fichier PDF afin de s’afficher sur un autre ordinateur ou dans Workfront Proof.

   * Votre fichier PDF contient des calques vides ou des champs transparents ou superposés.

     Si vous ne parvenez pas à déterminer quel calque ou objet est à l’origine de ce problème, exportez la conception/le document en tant que PDF optimisé (cela supprime tous les éléments indésirables).

