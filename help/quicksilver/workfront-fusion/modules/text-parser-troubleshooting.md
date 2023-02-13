---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Dépannage de l’analyseur de texte dans [!DNL Adobe Workfront Fusion]
description: Utilisez ces informations si vous ne parvenez pas à obtenir l’analyseur de texte pour produire une sortie.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Dépannage de l’analyseur de texte dans [!DNL Adobe Workfront Fusion]

Utilisez ces informations si vous ne pouvez pas obtenir qu’un analyseur de texte génère une sortie.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Dépannage

Exemple de scénario : vous souhaitez analyser le type de fichier d’un document &quot;filename.docx&quot; et l’extension du nom de fichier varie toujours de DOCX à PDF en passant par CSV.

L’expression que vous pouvez choisir d’utiliser dans ce cas est [!DNL \..+]

Si vous l&#39;utilisez sur expression regex sur regex101.com vous obtiendrez une correspondance complète.

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

Dans la sortie affichée dans l’image ci-dessous, le groupe capturant correspond à n’importe quel caractère (sauf aux terminateurs de ligne).

![](assets/text-parser-output-350x389.png)

Une autre solution qui intègre également l’expression régulière consiste à utiliser la fonction replace .

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

Ensuite, remplacez `abcdefghijklmno pqr stuvw xyz.docx` avec votre variable de nom de fichier.
