---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Exécution de scénarios, cycles et phases dans  [!DNL Adobe Workfront Fusion]
description: Cet article décrit les événements qui se produisent pendant l’exécution d’un scénario  [!DNL Adobe Workfront Fusion] , tels que l’initialisation, les opérations, les engagements et les restaurations.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 100%

---

# Exécution de scénarios, cycles et phases dans [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] est un système transactionnel, similaire aux bases de données relationnelles. Chaque exécution de scénario commence par la phase d’initialisation, se poursuit par au moins un cycle composé des phases d’opération et d’engagement/de restauration, puis se termine par la phase de finalisation :

>[!INFO]
>
>**Exemple**
>
>Initialisation
>
>Cycle 1
>
>Opération (lecture ou écriture)
>
>Engagement ou restauration
>
>Cycle 2
>
>Opération (lecture ou écriture)
>
>Engagement ou restauration
>
>...
>
>Cycle N
>
>Opération (lecture ou écriture)
>
>Engagement ou restauration
>
>Finalisation

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
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Initialisation

Pendant la phase d’initialisation, toutes les connexions nécessaires (connexion à une base de données, à un service de messagerie, etc.) sont créées. On vérifie également si chaque module est capable d’effectuer les opérations prévues.

## Cycles

Chaque cycle représente une unité de travail indivisible composée d’une série d’opérations. Il est possible de définir le nombre maximum de cycles dans le panneau [!UICONTROL Paramètres de scénario]. Le nombre par défaut est 1.

Pour plus d’informations, consultez le [panneau des paramètres de scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Opération

Pendant la phase de fonctionnement, des opérations de lecture et/ou d’écriture sont effectuées :

* L’opération de lecture consiste à obtenir des données d’un service qui sont ensuite traitées par d’autres modules selon un scénario prédéfini. Par exemple, le module [!UICONTROL Dropbox] > [!UICONTROL Surveiller des fichiers] renvoie les nouveaux lots (fichiers) créés depuis la dernière exécution du scénario.
* L’opération d’écriture consiste à envoyer des données à un service particulier en vue d’un traitement ultérieur. Par exemple, le module [!DNL Dropbox] > [!UICONTROL Charger un fichier] charge un fichier dans un dossier [!DNL Dropbox].

## Valider

Si la phase de fonctionnement est réussie pour tous les modules, la phase de validation commence, au cours de laquelle toutes les opérations effectuées par les modules sont validées. Cela signifie que [!DNL Workfront Fusion] envoie des informations sur son succès à tous les services impliqués dans la phase de fonctionnement.

## Restaurer

Si une erreur se produit pendant la phase d’opération ou d’engagement d’un module, la phase est interrompue et la phase de retour en arrière est lancée, ce qui annule toutes les opérations effectuées pendant le cycle en question. Certains modules ne prennent pas en charge la restauration et les opérations effectuées par ces modules ne peuvent pas être reprises. Pour plus d’informations, voir la section [Modules ACID](#acid-modules).

## Finalisation

Au cours de la phase de finalisation, les connexions ouvertes (par exemple, les connexions FTP, les connexions aux bases de données, etc.) sont fermées et le scénario terminé.

## Modules ACID

Tous les modules [!DNL Workfront Fusion] qui prennent en charge la restauration (également connue sous le nom de transactionnalité) comportent la balise ACID.

![](assets/acid-modules-350x189.png)

Les modules qui ne portent pas cette balise ne peuvent pas être ramenés à leur état initial lorsque des erreurs se produisent dans d’autres modules. Un exemple typique de module non-ACID est l’action [!UICONTROL E-mail] > [!UICONTROL Envoyer un e-mail]. Une fois l’e-mail envoyé, vous ne pouvez pas annuler l’envoi.
