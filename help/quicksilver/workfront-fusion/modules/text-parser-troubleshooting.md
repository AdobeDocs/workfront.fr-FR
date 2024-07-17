---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Résolution des problèmes de l’analyseur de texte dans [!DNL Adobe Workfront Fusion]
description: Utilisez ces informations si vous ne parvenez pas à obtenir l’analyseur de texte pour produire une sortie.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 28%

---

# Résolution des problèmes de l’analyseur de texte dans [!DNL Adobe Workfront Fusion]

Utilisez ces informations si vous ne pouvez pas obtenir qu’un analyseur de texte génère une sortie.

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

## Dépannage

Exemple de scénario : vous souhaitez analyser le type de fichier d’un document &quot;filename.docx&quot; et l’extension du nom de fichier varie toujours de DOCX à PDF en passant par CSV.

L’expression que vous pouvez choisir d’utiliser dans ce cas est [!DNL \..+]

Si vous l’utilisez sur l’expression regex sur regex101.com, vous obtiendrez une correspondance complète.

![](assets/regex-expression-350x130.png)

Sur l’image ci-dessus, l’extension de fichier était correctement mise en correspondance. Si vous prenez ceci et essayez de l’implémenter dans votre analyseur de texte :

![](assets/text-parser-350x602.png)

vous n’obtiendrez pas de correspondance :

![](assets/text-parser-you-dont-get-a-match-350x365.png)

Cela s’explique par le fait que la valeur &quot;i&quot; indique uniquement le nombre de correspondances par correspondance. Dans ce cas, nous avons donc 2 correspondances, donc après la valeur &quot;i&quot; il y a une valeur numérique 1 et 2. Le cas d’utilisation est que si vous n’avez jamais besoin de faire correspondre ou transmettre des données à un filtre, seule la seconde valeur correspondante que vous pouvez spécifier la valeur représentée par la valeur numérique.

![](assets/text-parser-matches-350x355.png)

Pour pouvoir obtenir les valeurs de correspondance dont vous avez besoin pour ajouter des crochets à la partie que vous souhaitez analyser (par exemple, pour extraire de &quot;filename.docx&quot; - &quot;docx&quot; uniquement), puis, selon l’expression regex que nous utilisons pour ce scénario, les crochets doivent être appliqués sur \.(.+)

Cela capture le DOCX, le place dans un groupe et laisse le &quot;.&quot; en dehors de ça.

![](assets/text-parser-get-matches-350x592.png)

Dans la sortie affichée dans l’image ci-dessous, le groupe capturant correspondra à n’importe quel caractère (sauf pour les terminateurs de ligne).

![](assets/text-parser-output-350x389.png)

Une autre solution qui intègre également l’expression régulière consiste à utiliser la fonction replace .

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

Ensuite, remplacez `abcdefghijklmno pqr stuvw xyz.docx` par votre variable de nom de fichier.
