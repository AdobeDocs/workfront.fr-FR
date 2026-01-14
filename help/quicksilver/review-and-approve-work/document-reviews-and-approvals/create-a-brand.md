---
product-area: documents
navigation-topic: approvals
title: Configurer des marques pour le réviseur de l’IA
description: Configurer des marques pour le réviseur de l’IA
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cf1d4bfeedb94e8607dad47177d804169254ee85
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 10%

---

# Configurer des marques pour le réviseur de l’IA

>[!IMPORTANT]
>
>Cette fonctionnalité est actuellement en version bêta.

Le réviseur de l’IA utilise des directives de marque pour évaluer le contenu pendant le processus de révision. Vous pouvez créer des marques dans Workfront en chargeant des fichiers PDF qui contiennent vos directives de marque ou en saisissant manuellement des éléments de marque.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur système.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations Admin Console</td> 
   <td> <p>Vous devez utiliser GenStudio Brand Manager.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Conditions préalables

* Votre organisation doit avoir migré vers Adobe IMS (système Identity Management).
* Les approbations unifiées doivent être activées pour votre instance Workfront.
  <!--* Your organization must have GenStudio Foundation.-->
* Adobe doit disposer d’un contrat Adobe Gen AI signé dans ce fichier.
Pour plus d’informations sur la signature du contrat, voir [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## Création d’une marque à l’aide d’un PDF

{{step-1-to-setup}}

1. Dans le panneau de gauche, accédez à **Révision et approbation** > **Marques**.
1. Cliquez sur **Ajouter une marque** dans le coin supérieur droit de l’écran.
1. Nommez la marque.
1. Cliquez sur Charger des PDF pour charger des fichiers de marque.
   ![télécharger des fichiers pdf de marque](assets/upload-PDF.png)
1. Cliquez sur **Continuer**.
1. Chargez un ou plusieurs fichiers PDF contenant les directives de votre marque, puis cliquez sur **Ajouter une marque**.
1. Une fois les fichiers chargés, passez en revue les éléments de marque extraits pour vous assurer qu’ils sont conformes à vos directives de marque.

   >[!IMPORTANT]
   >
   >Les directives sont générées à l’aide de vos fichiers et de la technologie d’IA générative et peuvent être inexactes. Vérifiez les instructions extraites pour les détails manquants ou incorrects et modifiez-les avant de publier cette marque.

1. Lorsque vous avez terminé, cliquez sur **Publier** pour mettre la marque à la disposition du réviseur de l’IA.

## Création manuelle d’une marque

{{step-1-to-setup}}

1. Dans le panneau de gauche, accédez à **Révision et approbation** > **Marques**.
1. Cliquez sur **Ajouter une marque** dans le coin supérieur droit de l’écran.
1. Nommez la marque.
1. Cliquez sur **Ajouter manuellement** pour créer une marque avec des éléments individuels.
1. Renseignez les détails de la marque selon vos besoins. Vous pouvez ajouter les éléments suivants :

   <table>
    <tr>
        <td>Quand l’utiliser</td>
        <td>Indiquez aux professionnels du marketing quand utiliser cette marque.</td>
    </tr>
    <tr>
        <td>Instructions vocales</td>
        <td>Donnez des conseils sur le ton et le style de la voix de la marque.</td>
    </tr>
    <tr>
        <td>Instructions relatives aux images</td>
        <td>Spécifiez les types d’images qui correspondent à l’identité de la marque.</td>
    </tr>
    <tr>
        <td>Instructions relatives aux canaux</td>
        <td>Décrivez les canaux appropriés pour la communication de la marque.</td>
    </tr>
    <tr>
        <td>logos</td>
        <td>Incluez les logos officiels associés à la marque.</td>
    </tr>
    <tr>
        <td>Couleurs</td>
        <td>Spécifiez la palette de couleurs de la marque.</td>
    </tr>
    </table>

   ![ajout manuel d’éléments de marque](assets/brand-elements.png)


1. Lorsque vous avez terminé, cliquez sur **Publier** pour mettre la marque à la disposition du réviseur de l’IA.
