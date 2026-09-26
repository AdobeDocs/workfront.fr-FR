---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Charger des documents et des épreuves d’[!DNL Adobe Workfront plugin] à [!DNL Creative Cloud]
description: Charger des documents et des épreuves d’[!DNL Adobe Workfront plugin] à [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
TQID: 'https://experienceleague.adobe.com/bZsOnrrwZ7ksCaoM3jfIyeTO00XqG1hDTEmG5VmWOcA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 98%
---
# Charger des documents et des épreuves d’[!DNL Adobe Workfront plugin] à [!DNL Creative Cloud]

Vous pouvez charger vos projets sous forme de documents pour un examen et une approbation rapides ou simplement pour les stocker dans [!DNL Adobe Workfront].

>[!NOTE]
>
>Charger des documents et des épreuves n’est pas pris en charge actuellement dans Premiere Pro et After Effects.


## Limites du document

Cette section décrit les limites connues des documents dans [!DNL Workfront for Adobe Creative Cloud plugins].

### Les nouvelles versions des documents autorisent le chargement d’un fichier uniquement.

Compte tenu du fait que les documents [!DNL Workfront] ne peuvent pas contenir plusieurs fichiers, certains paramètres doivent être désactivés pour charger de nouvelles versions de documents vers Workfront.

>[!NOTE]
>
>Si vous devez générer plusieurs fichiers, vous pouvez créer une épreuve à la place. La nouvelle épreuve ne sera pas associée au document d’origine.



Pour revenir à un fichier unique dans [!DNL InDesign], procédez comme suit :

1. Ouvrez la boîte de dialogue **Définir des paramètres d’export de fichier**.

   ![Paramètres d’exportation de fichiers](assets/file-export-settings.png)

1. Recherchez le type de ressource que vous souhaitez exporter et ajustez les paramètres comme décrit ci-dessous :

   <table>
    <tr>
    <td><strong>PDF et PDF-PRINT</strong>
    </td>
    <td>Désélectionnez <strong>Créer des fichiers PDF séparés</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Sélectionnez <strong>Plages</strong> et saisissez un numéro de page unique. 
    <p>
    <strong>Note</strong> : si vous souhaitez charger le document complet, vous devez créer une épreuve. 
    </td>
    </tr>
    <tr>
    <td><strong>EPUB et EPUB-FIXED</strong>
    </td>
    <td>Aucun ajustement n’est nécessaire.
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>Aucun ajustement n’est nécessaire.
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>Sélectionnez <strong>Plages</strong> et saisissez un numéro de page unique. 
    <p>
    <strong>Note</strong> : si vous souhaitez charger le document complet, vous devez créer une épreuve. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Sélectionnez <strong>Plages</strong> et saisissez un numéro de page unique. 
    <p>
    <strong>Note</strong> : si vous souhaitez charger le document complet, vous devez créer une épreuve. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Aucun ajustement n’est nécessaire. 
    </td>
    </tr>
    </table>
