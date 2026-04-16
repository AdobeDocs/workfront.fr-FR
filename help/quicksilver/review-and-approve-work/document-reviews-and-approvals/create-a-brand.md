---
product-area: documents
navigation-topic: approvals
title: Créer et gérer des marques pour le réviseur de contenu
description: Créer et gérer des marques pour le réviseur de contenu
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 243aa2b0893e3034d37b959384a50b8a5e4a4bf0
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 7%

---

# Créer et gérer des marques pour le réviseur de contenu

Le réviseur de contenu utilise les directives de la marque pour évaluer le contenu pendant le processus de révision. Vous pouvez créer des marques dans Workfront en chargeant des fichiers PDF qui contiennent vos directives de marque ou en saisissant manuellement des éléments de marque.

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
   <td role="rowheader">Autorisations Admin Console*</td> 
   <td> <p>Vous devez être un Brand Manager GenStudio.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions

* Les approbations unifiées doivent être activées pour votre instance Workfront.

* Votre organisation doit disposer de GenStudio Foundation.
   * Content Reviewer dans Workfront fournit les fonctionnalités disponibles dans GenStudio Foundation pour les workflows de révision et d’approbation de ressources. Vous n’avez pas besoin d’accéder directement à GenStudio Foundation pour terminer votre travail. Votre accès à la fonctionnalité GenStudio Foundation par l’intermédiaire de l’analyseur de contenu est soumis aux conditions de votre contrat Workfront.
* Adobe doit disposer d’un contrat Adobe Gen AI signé dans ce fichier.
Pour plus d’informations sur la signature du contrat, voir [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Conditions préalables

1. Vous devez accorder l’accès aux autorisations de marque dans les niveaux d’accès Admin Console et Workfront avant de pouvoir créer des marques. Pour obtenir des instructions, voir [Octroi de l’accès aux autorisations de marque](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md).


## Création d’une marque à l’aide d’un PDF

{{step-1-to-setup}}

1. Dans le panneau de gauche, accédez à **Révision et approbation** > **Marques**.
1. Cliquez sur **Ajouter une marque** dans le coin supérieur droit de l’écran.
1. Nommez la marque.
1. Cliquez sur **Charger des PDF** pour charger des fichiers de marque.
   ![télécharger des fichiers pdf de marque](assets/upload-PDF.png)
1. Cliquez sur **Continuer**.
1. Chargez un ou plusieurs fichiers PDF contenant les directives de votre marque, puis cliquez sur **Ajouter une marque**.
1. Une fois les fichiers chargés, passez en revue les éléments de marque extraits pour vous assurer qu’ils sont conformes à vos directives de marque.

   >[!IMPORTANT]
   >
   >Les directives sont générées à l’aide de vos fichiers et de la technologie d’IA générative et peuvent être inexactes. Vérifiez les instructions extraites pour les détails manquants ou incorrects et modifiez-les avant de publier cette marque.

1. Lorsque vous avez terminé, cliquez sur **Publier** pour rendre la marque disponible pour le réviseur de contenu.

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
        <td>Logos</td>
        <td>Incluez les logos officiels associés à la marque.</td>
    </tr>
    <tr>
        <td>Couleurs</td>
        <td>Spécifiez la palette de couleurs de la marque.</td>
    </tr>
    </table>

   ![ajout manuel d’éléments de marque](assets/brand-elements.png)


1. Lorsque vous avez terminé, cliquez sur **Publier** pour rendre la marque disponible pour le réviseur de contenu.


## Bonnes pratiques relatives à l’écriture de directives de marque

*  Rédiger des directives sur la marque qui décrivent les critères mesurables. Le réviseur de contenu évalue le contenu littéralement, de sorte que les règles objectives génèrent des scores plus cohérents que les règles subjectives.

* Recherchez des mots comme « éviter », « conserver » ou « s’assurer » dans vos directives. Ceux-ci signalent souvent une règle que vous pouvez resserrer. Remplacez l’instruction vague par une liste spécifique de mots, de formats ou de limites. Par exemple, remplacez « évitez les clichés de ski les plus courants » par « n’utilisez ni « gnar », ni « pow », ni « shred ».

* Si vous ne pouvez pas supprimer la subjectivité, réduisez-la. Remplacez les adjectifs généraux par des contraintes spécifiques. Par exemple, « Direct et orienté vers l’action » devient « Direct et orienté vers l’action ; omettez les mots de remplissage et le langage de couverture ».