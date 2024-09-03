---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: '« Exemple de scénario Adobe Workfront Fusion : connecter un e-mail, un analyseur de texte et Google Sheets »'
description: Ce scénario vous permet de créer un journal de tous les e-mails et de les baliser pour effectuer d’autres actions dans une feuille de calcul. Il capture le corps d’un e-mail dans deux tableaux distincts dans une feuille de calcul à l’aide d’expressions régulières (Regex) comme modèles de recherche. Le premier modèle recherche une expression et le second recherche la même expression et une adresse e-mail.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 100%

---

# Exemple de scénario [!DNL Adobe Workfront Fusion] : connecter un e-mail, [!UICONTROL un analyseur de texte] et [!DNL Google Sheets]

Ce scénario vous permet de créer un journal de tous les e-mails et de les baliser pour effectuer d’autres actions dans une feuille de calcul. Il capture le corps d’un e-mail dans deux tableaux distincts dans une feuille de calcul à l’aide d’expressions régulières (Regex) comme modèles de recherche. Le premier modèle recherche une expression et le second recherche la même expression et une adresse e-mail.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Ce tutoriel nécessite des connaissances de base sur les expressions régulières. Pour en savoir plus sur Regex, rendez-vous sur [https://regexone.com](https://regexone.com/).

Ajouter le premier module et le configurer

1. Recherchez E-mail et choisissez **[!UICONTROL Surveiller les e-mails]** comme déclencheur.

   >[!NOTE]
   >
   >Vous pouvez connecter un compte [!DNL Google] utilisant le module Email, vous pouvez également utiliser un module [!DNL Gmail].

1. Connectez un compte [!DNL Google] ou tout autre client de messagerie IMAP (tel que [!DNL Outlook]).
1. Une fois la connexion établie, sélectionnez un Dossier dont vous souhaitez consulter les e-mails entrants, par exemple [!UICONTROL Boîte de réception].
1. Sous [!UICONTROL Critères], choisissez **[!UICONTROL Tous les e-mails]** (ou réduisez à e-mails lus ou non lus).

   Vous pouvez également choisir de marquer les e-mails récupérés comme lus ou non lus.

1. Définissez le [!UICONTROL nombre maximal de résultats] sur 1.

   ![](assets/save-max-as-1-350x304.png)

   Vous pouvez le modifier en fonction du volume de messages que vous recevez. Cependant, il est recommandé de définir une valeur basse et d’exécuter le scénario plus souvent.

1. Cliquez sur **[!UICONTROL Afficher les paramètres avancés]** en bas.

   ![](assets/show-adv-settings-350x332.png)

1. Filtrez les e-mails par [!UICONTROL Adresse expéditeur], [!UICONTROL Objet] et [!UICONTROL Expression].

   Vous avez ainsi la possibilité de ne consulter que les e-mails pertinents. Dans cet exemple, nous avons ajouté uniquement un filtre Objet et laissé les 2 autres vides.

   >[!NOTE]
   >
   >Nous allons ajouter un routeur pour rechercher des expressions dans un e-mail à l’aide de l’itérateur [!UICONTROL Modèle de correspondance] et une expression régulière (Regex) comme modèle de recherche. Cela nous permet également de créer un scénario à plusieurs utilités.

1. Une fois la configuration terminée, et lorsque vous recevez une invitation à indiquer où commencer à regarder vos e-mails, cliquez sur **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. Passer à [Rechercher [!UICONTROL Contrôle des flux] et ajouter un [!UICONTROL Routeur]](#search-for-flow-control-and-add-a-router)

## Rechercher [!UICONTROL Contrôle des flux] et ajouter un [!UICONTROL Routeur]

1. Ajoutez un routeur après tout module pour partager ou dupliquer les données avant de les envoyer au module suivant.

   Ici, nous avons utilisé un [!UICONTROL routeur] pour envoyer le texte du corps de l’e-mail à deux tableaux distincts dans un document [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## Utilisez le module [!UICONTROL Analyseur de texte].

1. Ajoutez un transformateur de [!UICONTROL Motif correspondant] pour rechercher une expression dans un e-mail.

   Nous rechercherons l’expression « [!UICONTROL text parser module] » (module analyseur de texte) dans tous les e-mails entrants pour capturer le corps de texte et le nom de la personne ayant expédié ceux qui correspondent à cette expression.

   1. Ecrivez le Motif en tant qu’expression régulière :

      text\sparser\smodule

   1. (Facultatif) Utilisez l’une des autres options de Motif.

      ![](assets/pattern-350x318.png)

      L’option Multiligne est utile si votre texte contient plusieurs lignes et si vous devez rechercher le motif dans chaque ligne. Pour ce tutoriel, nous devons rechercher le motif dans tout le corps du texte de l’e-mail. Par conséquent, nous ne cocherons pas cette option.

   1. Dans le champ [!UICONTROL Texte], cliquez sur l’attribut **Contenu du texte** dans la liste.

      ![](assets/text-content-350x264.png)

      Il s’agit de l’attribut qui stocke le texte dans le corps de l’e-mail dans lequel nous allons rechercher le motif.

1. Ajouter un autre [!UICONTROL Motif correspondant] qui recherche la même expression et une adresse e-mail.

   Cela s’avère particulièrement utile si vous disposez de comptes clients avec plusieurs utilisateurs et utilisatrices. Pour gagner du temps, vous pouvez cloner le module [!UICONTROL Analyseur de texte] que vous venez de créer et le lier au routeur.

   ![](assets/clone.png)

1. Modifiez le motif comme suit :

   text\sparser\smodule.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   Ce motif recherche l’expression « [!UICONTROL text parser module] » et une adresse e-mail telle que john.doe@gmail.com, et renvoie uniquement l’adresse e-mail.

   >[!NOTE]
   >
   >Il est important d’écrire votre expression régulière conformément aux spécifications des adresses e-mail que vous acceptez, mais celle ci-dessus est adaptée à la plupart des adresses e-mail standard.

   * Si vous souhaitez rechercher uniquement des adresses e-mail, vous pouvez utiliser l’expression régulière suivante :

     ([\w.-]+@[\w.-]+)

   * Vous pouvez également rechercher uniquement es numéros de téléphone en utilisant l’expression régulière suivante :

     ^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4}
Le motif ci-dessus couvre les formats les plus courants dans lesquels un numéro de téléphone est écrit.

   Pour tester vos motifs, nous vous recommandons d’utiliser [[!DNL https://regex101.com]](https://regex101.com/) avec [!DNL javascript] comme Flavor.

   Le reste de la configuration est la même que précédemment.

## Ajouter les modules [!DNL Google Sheets]

Pour [!DNL Sheets], nous devons d’abord créer une feuille de calcul avec les en-têtes requis.

1. Créez une feuille de calcul contenant les colonnes sous lesquelles vous souhaitez capturer les données des utilisateurs et utilisatrices. (N’hésitez pas à utiliser un fichier existant également.)

   Par exemple, créez un champ appelé « Données d’e-mail : ticket d’assitance » avec les colonnes Nom de l’expéditeur ou de l’expéditrice, E-mail de l’expéditeur ou de l’expéditrice et Contenu de l’e-mail. Nommez la feuille de travail « contient : module d’analyseur de texte ».

1. Ajoutez le module [!UICONTROL Google Sheets] avec **[!UICONTROL Ajouter une ligne]** comme action.

   ![](assets/add-a-row-350x174.png)

1. Connectez-vous à votre compte [!DNL Google] (si ce n’est déjà fait). Sélectionnez le Fichier que vous avez créé précédemment, puis choisissez la feuille de travail dans laquelle vous capturez les données.

   Votre configuration devrait ressembler à ceci :

   ![](assets/connect-google-acct-350x279.png)

1. Mappez les attributs dans les champs (colonnes) pertinents pour terminer la configuration du module.

   ![](assets/map-attributes-350x282.png)

1. Clonez le module que vous venez de créer et liez-le au second module [!UICONTROL Analyseur de texte].

   1. Dans la feuille de calcul, dupliquez la feuille de travail que vous avez créée précédemment et nommez-la.

      Par exemple, nommez-la « contient : module d’analyseur de texte et e-mail ».

   1. Ajoutez une autre colonne pour stocker l’adresse e-mail que le corps de l’e-mail contient.

      Par exemple, nommez-la « Adresse e-mail partagée ».

   1. Cliquez sur le module [!DNL Google Sheets] cloné pour définir la configuration.
   1. Remplacez la feuille de travail par la nouvelle feuille que vous venez de créer.
   1. Mappez la sortie du module [!UICONTROL Motif correspondant] ($1) à la colonne dans laquelle vous souhaitez stocker l’adresse e-mail (Adresse e-mail partagée).

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. Cliquez sur **[!UICONTROL OK]**, enregistrez le scénario, puis testez-le.

      Vous devrez envoyer deux e-mails distincts à l’adresse e-mail connectée comme suit :

      * Contenant l’expression « [!UICONTROL text parser module] » (et aucune adresse e-mail)

        ![](assets/text-parser-module-350x103.png)

      * Contenant l’expression ci-dessus et une adresse e-mail

        ![](assets/above-phrase-and-email-350x106.png)

        Si votre configuration ne comporte aucune erreur, vous verrez que la première feuille de calcul capture tous les e-mails contenant l’expression « [!UICONTROL text parser module] » tandis que la deuxième feuille de calcul capture uniquement ceux contenant l’expression « [!UICONTROL text parser module] » ainsi qu’une adresse e-mail. Reportez-vous aux captures d’écran ci-dessous.

        Feuille de travail 1 :

        ![](assets/worksheet-1-350x57.png)

        Feuille de travail 2 :

        ![](assets/worksheet-2-350x41.png)

## Ressources

* [Exercices gratuits](https://regexone.com/) pour en savoir plus sur les expressions régulières
* [En savoir plus sur la correspondance des numéros de téléphone](https://regexone.com/problem/matching_phone_numbers) à l’aide de Regex
* [En savoir plus sur la correspondance des e-mails](https://regexone.com/problem/matching_emails) à l’aide de Regex
* [Tester vos expressions régulières](https://regex101.com/)
