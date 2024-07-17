---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Charger des documents et des épreuves à partir du  [!DNL Adobe Workfront plugin]  sur  [!DNL Creative Cloud]
description: Charger des documents et des épreuves à partir du  [!DNL Adobe Workfront plugin]  sur  [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
source-git-commit: 0ca335bf0db934d23f607d3f8ce7cfb67e629053
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 7%

---

# Télécharger des documents et des bons à tirer de [!DNL Adobe Workfront plugin] vers le [!DNL Creative Cloud]

Vous pouvez télécharger vos projets sous forme de documents pour une révision et une approbation rapides ou simplement pour les stocker dans [!DNL Adobe Workfront].

>[!NOTE]
>
>Le téléchargement de documents et de bons à tirer n’est actuellement pas pris en charge dans Premiere Pro et After Effects.


## Limites du document

Cette section décrit les limites connues des documents dans [!DNL Workfront for Adobe Creative Cloud plugins].

### Les nouvelles versions de document n’acceptent qu’un seul fichier pour le chargement

Étant donné que les documents [!DNL Workfront] ne peuvent pas contenir plusieurs fichiers, certains paramètres doivent être désactivés pour télécharger de nouvelles versions de documents vers Workfront.

>[!NOTE]
>
>Si vous devez générer plusieurs fichiers, vous pouvez créer un BAT à la place. Le nouveau BAT ne sera pas associé au document d’origine.



Pour restaurer votre commutateur en un seul fichier dans [!DNL InDesign] :

1. Ouvrez la boîte de dialogue **Définir les paramètres du fichier d’exportation** .

   ![](assets/file-export-settings.png)

1. Recherchez le type de ressource que vous souhaitez exporter et ajustez les paramètres comme décrit ci-dessous :

   <table>
    <tr>
    <td><strong>PDF et PDF-PRINT</strong>
    </td>
    <td>Désélectionnez <strong>Créer des fichiers de PDF distincts</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Sélectionnez <strong>Plages</strong> et saisissez un numéro de page unique. 
    <p>
    <strong>Remarque</strong> : si vous souhaitez télécharger le document complet, vous devez créer un BAT. 
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
    <strong>Remarque</strong> : si vous souhaitez télécharger le document complet, vous devez créer un BAT. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Sélectionnez <strong>Plages</strong> et saisissez un numéro de page unique. 
    <p>
    <strong>Remarque</strong> : si vous souhaitez télécharger le document complet, vous devez créer un BAT. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Aucun ajustement n’est nécessaire. 
    </td>
    </tr>
    </table>
