---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: "Exemple de scénario de fusion Adobe Workfront : connexion d’un courrier électronique, d’un analyseur de texte et de feuilles de calcul Google"
description: Ce scénario vous permet de créer un journal de tous les emails et de les baliser pour effectuer d’autres actions dans une feuille de calcul. Il capture le corps d’un email dans deux tableaux distincts dans une feuille de calcul à l’aide d’expressions régulières (Regex) comme modèles de recherche. Le premier modèle recherche une expression et le second recherche la même expression et une adresse électronique.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 9%

---

# [!DNL Adobe Workfront Fusion] exemple de scénario : Connectez un email, [!UICONTROL analyseur de texte] et [!DNL Google Sheets]

Ce scénario vous permet de créer un journal de tous les emails et de les baliser pour effectuer d’autres actions dans une feuille de calcul. Il capture le corps d’un email dans deux tableaux distincts dans une feuille de calcul à l’aide d’expressions régulières (Regex) comme modèles de recherche. Le premier modèle recherche une expression et le second recherche la même expression et une adresse électronique.

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
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
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

Ce tutoriel nécessite des connaissances de base sur les expressions régulières. Pour en savoir plus sur Regex, consultez le site [https://regexone.com](https://regexone.com/).

Ajouter le premier module et le configurer

1. Recherchez Email et sélectionnez **[!UICONTROL Watch emails]** comme déclencheur.

   >[!NOTE]
   >
   >Bien que vous puissiez connecter un compte [!DNL Google] à l&#39;aide du module Email, vous pouvez également utiliser un module [!DNL Gmail].

1. Connectez un compte [!DNL Google] ou tout autre client de messagerie IMAP (tel que [!DNL Outlook]).
1. Une fois connecté, sélectionnez un dossier dont vous souhaitez consulter les courriers électroniques entrants, par exemple [!UICONTROL Boîte de réception].
1. Sous [!UICONTROL Critère], sélectionnez **[!UICONTROL Tous les emails]** (ou réduisez-le pour lire ou non les emails).

   Vous pouvez également choisir de marquer les emails récupérés comme lus ou non lus.

1. Définissez le [!UICONTROL nombre maximal de résultats] sur 1.

   ![](assets/save-max-as-1-350x304.png)

   Vous pouvez le modifier en fonction du volume de messages que vous recevez. Cependant, il est recommandé de définir une valeur basse et d’exécuter le scénario plus souvent.

1. Cliquez sur **[!UICONTROL Afficher les paramètres avancés]** en bas de la page.

   ![](assets/show-adv-settings-350x332.png)

1. Filtrez les emails par [!UICONTROL Adresse de l&#39;expéditeur], [!UICONTROL Objet] et [!UICONTROL Expression].

   Vous avez ainsi la possibilité de ne consulter que les emails pertinents. Dans cet exemple, nous avons ajouté uniquement un filtre Objet et laissé les 2 autres vides.

   >[!NOTE]
   >
   >Nous allons ajouter un routeur pour rechercher des expressions dans un email à l’aide de l’itérateur [!UICONTROL Modèle de correspondance] et d’une Expression régulière (Regex) comme modèle de recherche. Cela nous permet également de créer un scénario multi-utilitaire.

1. Une fois la configuration terminée, et lorsque vous êtes invité à spécifier où commencer à regarder vos emails, cliquez sur **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. Continuez à [Rechercher le [!UICONTROL contrôle de flux] et ajoutez un [!UICONTROL routeur]](#search-for-flow-control-and-add-a-router)

## Recherchez [!UICONTROL Contrôle de flux] et ajoutez un [!UICONTROL routeur]

1. Ajoutez un routeur après tout module pour fractionner ou dupliquer les données avant de les envoyer au module suivant.

   Ici, nous avons utilisé un [!UICONTROL routeur] pour envoyer le texte du corps de l&#39;email à 2 tables distinctes dans un [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## Utilisation du module [!UICONTROL analyseur de texte]

1. Ajoutez un transformateur [!UICONTROL Correspondance avec le modèle] pour rechercher une expression dans un email.

   Nous allons rechercher l’expression &quot;[!UICONTROL module d’analyseur de texte]&quot; dans tous les emails entrants pour capturer le texte du corps et le nom de l’expéditeur de ceux qui correspondent à cette expression.

   1. Ecrivez le modèle en tant qu’expression régulière :

      text\sparser\smodule

   1. (Facultatif) Utilisez l’une des autres options de modèle.

      ![](assets/pattern-350x318.png)

      La multiligne est utile si votre texte contient plusieurs lignes et si vous devez rechercher le modèle dans chaque ligne. Pour ce tutoriel, nous devons rechercher le modèle dans tout le texte du corps de l’email. Par conséquent, nous ne le vérifierons pas.

   1. Dans le champ [!UICONTROL Texte] , cliquez sur l’attribut **Contenu texte** dans la liste.

      ![](assets/text-content-350x264.png)

      Il s’agit de l’attribut qui stocke le texte dans le corps de l’email dans lequel nous allons rechercher le modèle.

1. Ajoutez un autre [!UICONTROL Modèle de correspondance] qui recherche la même expression et une adresse électronique.

   Cela s’avère particulièrement utile si vous disposez de comptes clients avec plusieurs utilisateurs. Pour gagner du temps, vous pouvez cloner le module [!UICONTROL analyseur de texte] que vous venez de créer et le lier au routeur.

   ![](assets/clone.png)

1. Modifiez le modèle comme suit :

   text\sparser\smodule.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   Ce modèle recherche l’expression &quot;[!UICONTROL module d’analyseur de texte]&quot; et une adresse électronique telle que john.doe@gmail.com et renvoie uniquement l’adresse électronique.

   >[!NOTE]
   >
   >Il est important d’écrire votre expression régulière conformément aux spécifications des adresses électroniques que vous acceptez, mais celle ci-dessus s’occupe de la plupart des adresses électroniques standard.

   * Si vous souhaitez rechercher uniquement les adresses électroniques, vous pouvez utiliser l’expression régulière suivante :

     ([\w.-]+@[\w.-]+)

   * Vous pouvez également rechercher uniquement les numéros de téléphone en utilisant l’expression régulière ci-dessous :

     ^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4}
Le modèle ci-dessus couvre les formats les plus courants dans lesquels un numéro de téléphone est écrit.

   Pour tester vos modèles, nous vous recommandons d’utiliser [[!DNL https://regex101.com]](https://regex101.com/) avec [!DNL javascript] comme Flavor.

   Le reste de la configuration reste le même que précédemment.

## Ajout des modules [!DNL Google Sheets]

Pour [!DNL Sheets], nous devons d’abord créer une feuille de calcul avec les en-têtes requis.

1. Créez une feuille de calcul contenant les colonnes sous lesquelles vous souhaitez capturer les données utilisateur. (N’hésitez pas à utiliser un fichier existant également).

   Par exemple, créez un champ appelé &quot;Email Data: Support Ticket&quot; (Données de messagerie : assistance technique) avec les colonnes Nom de l’expéditeur, Email de l’expéditeur et Contenu de l’email. Nommez la feuille de calcul &quot;contient : module d’analyseur de texte&quot;.

1. Ajoutez le module [!UICONTROL Google Sheets] avec **[!UICONTROL Ajouter une ligne]** comme action.

   ![](assets/add-a-row-350x174.png)

1. Connectez votre compte [!DNL Google] (si ce n&#39;est déjà fait). Sélectionnez le Fichier que vous avez créé précédemment, puis choisissez la feuille de calcul dans laquelle vous capturez les données.

   Votre configuration doit se présenter comme suit :

   ![](assets/connect-google-acct-350x279.png)

1. Mappez les attributs dans les champs (colonnes) pertinents pour terminer la configuration du module.

   ![](assets/map-attributes-350x282.png)

1. Cloner le module que vous venez de créer et le lier au deuxième module [!UICONTROL Analyseur de texte].

   1. Dans la feuille de calcul, dupliquez la feuille de calcul que vous avez créée précédemment et nommez-la.

      Par exemple, nommez-le &quot;contient : module d’analyseur de texte et courrier électronique&quot;.

   1. Ajoutez une autre colonne pour stocker l’adresse électronique que le corps de l’email contient.

      Par exemple, nommez-le &quot;Adresse électronique partagée&quot;.

   1. Cliquez sur le module [!DNL Google Sheets] cloné pour configurer la configuration.
   1. Remplacez la feuille de calcul par la nouvelle que vous venez de créer.
   1. Faites correspondre la sortie du module [!UICONTROL Correspondance avec le modèle] (1 $) à la colonne dans laquelle vous souhaitez stocker l’adresse électronique (adresse électronique partagée).

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. Cliquez sur **[!UICONTROL OK]**, enregistrez le scénario et préparez-le pour une exécution de test.

      Vous devrez envoyer deux emails distincts à l’adresse email connectée comme suit :

      * Contenant l’expression &quot;[!UICONTROL module d’analyseur de texte]&quot; (sans adresse électronique)

        ![](assets/text-parser-module-350x103.png)

      * Contenant l’expression ci-dessus et une adresse électronique

        ![](assets/above-phrase-and-email-350x106.png)

        S’il n’y a aucune erreur dans votre configuration, vous verrez que la première feuille de calcul capture tous les emails contenant l’expression &quot;[!UICONTROL module d’analyseur de texte]&quot;, tandis que la deuxième feuille de calcul capture uniquement ceux contenant l’expression &quot;[!UICONTROL module d’analyseur de texte]&quot; et une adresse électronique. Reportez-vous aux captures d’écran ci-dessous.

        Feuille de calcul 1 :

        ![](assets/worksheet-1-350x57.png)

        Feuille de calcul 2 :

        ![](assets/worksheet-2-350x41.png)

## Ressources

* [Exercices gratuits](https://regexone.com/) pour en savoir plus sur les expressions régulières
* [En savoir plus sur la correspondance des numéros de téléphone](https://regexone.com/problem/matching_phone_numbers) à l’aide de Regex
* [En savoir plus sur la correspondance des emails](https://regexone.com/problem/matching_emails) à l’aide de Regex
* [Test de vos expressions régulières](https://regex101.com/)
