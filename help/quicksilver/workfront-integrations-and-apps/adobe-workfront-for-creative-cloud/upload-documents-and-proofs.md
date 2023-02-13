---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Téléchargement de documents et de BAT depuis le [!DNL Adobe Workfront plugin] au [!DNL Creative Cloud]
description: Téléchargement de documents et de BAT depuis le [!DNL Adobe Workfront plugin] au [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
source-git-commit: 67952bf88a782595e13e559bfbc14ce1c622d432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Téléchargement de documents et de BAT depuis le [!DNL Adobe Workfront plugin] au [!DNL Creative Cloud]

Vous pouvez télécharger vos projets sous la forme de documents pour un examen et une approbation rapides ou simplement les stocker dans [!DNL Adobe Workfront].

>[!NOTE]
>
>Le téléchargement de documents et de bons à tirer n’est actuellement pas pris en charge dans Premiere Pro et After Effects.


## Limites du document

Cette section décrit les limites connues des documents dans [!DNL Workfront for Adobe Creative Cloud plugins].

### Les nouvelles versions de document n’acceptent qu’un seul fichier pour le chargement

Parce que [!DNL Workfront] Les documents ne peuvent pas contenir plusieurs fichiers. Certains paramètres doivent être désactivés pour télécharger de nouvelles versions de documents vers Workfront.

>[!NOTE]
>
>Si vous devez générer plusieurs fichiers, vous pouvez créer un BAT à la place. Le nouveau BAT ne sera pas associé au document d’origine.



Pour rétablir un fichier unique dans [!DNL InDesign]:

1. Ouvrez le **Définition des paramètres d’exportation de fichier** de la boîte de dialogue

   ![](assets/file-export-settings.png)

1. Recherchez le type de ressource que vous souhaitez exporter et ajustez les paramètres comme décrit ci-dessous :

   <table>
    <tr>
    <td><strong>PDF et PDF-PRINT</strong>
    </td>
    <td>Désélectionner <strong>Création de fichiers de PDF distincts</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Sélectionner <strong>Plages</strong> et saisissez un numéro de page unique. 
    <p>
    <strong>Remarque</strong>: Si vous souhaitez télécharger le document complet, vous devez créer un BAT. 
    </td>
    </tr>
    <tr>
    <td><strong>L'EPUB et l'EPUB</strong>
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
    <td>Sélectionner <strong>Plages</strong> et saisissez un numéro de page unique. 
    <p>
    <strong>Remarque</strong>: Si vous souhaitez télécharger le document complet, vous devez créer un BAT. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Sélectionner <strong>Plages</strong> et saisissez un numéro de page unique. 
    <p>
    <strong>Remarque</strong>: Si vous souhaitez télécharger le document complet, vous devez créer un BAT. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Aucun ajustement n’est nécessaire. 
    </td>
    </tr>
    </table>
