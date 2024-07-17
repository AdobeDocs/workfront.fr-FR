---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Exécution, cycles et phases du scénario dans  [!DNL Adobe Workfront Fusion]
description: Cet article décrit les événements qui se produisent pendant l’exécution d’un scénario  [!DNL Adobe Workfront Fusion] , tels que l’initialisation, les opérations, les validations et les restaurations.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 23%

---

# Exécution de scénarios, cycles et phases dans [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] est un système transactionnel, similaire aux bases de données relationnelles. Chaque exécution de scénario commence par la phase d’initialisation, se poursuit par au moins un cycle composé des phases d’opération et de validation/restauration, et se termine par la phase de finalisation :

>[!INFO]
>
>**Exemple**
>
>Initialisation
>
>#1 de cycle
>
>Opération (lecture ou écriture)
>
>Validation ou restauration
>
>#2 de cycle
>
>Opération (lecture ou écriture)
>
>Validation ou restauration
>
>..
>
>#N de cycle
>
>Opération (lecture ou écriture)
>
>Validation ou restauration
>
>Finalisation

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
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Initialisation

Lors de la phase d’initialisation, toutes les connexions nécessaires (connexion à une base de données, service de messagerie, etc.) sont créées. Elles sont également vérifiées si chaque module est capable d’effectuer les opérations prévues.

## Cycles

Chaque cycle représente une unité de travail inséparable composée d&#39;une série d&#39;opérations. Il est possible de définir le nombre maximal de cycles dans le panneau [!UICONTROL paramètres du scénario]. Le nombre par défaut est 1.

Pour plus d’informations, voir [Panneau des paramètres de scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Opération

Pendant la phase d&#39;opération, l&#39;opération de lecture et/ou d&#39;écriture est effectuée :

* L’opération de lecture consiste à obtenir des données d’un service qui est ensuite traité par d’autres modules selon un scénario prédéfini. Par exemple, le module [!UICONTROL Dropbox] >[!UICONTROL Fichiers de contrôle] renvoie les nouveaux lots (fichiers) créés depuis la dernière exécution du scénario.
* L’opération d’écriture consiste à envoyer des données à un service donné en vue d’un traitement ultérieur. Par exemple, le module [!DNL Dropbox] >[!UICONTROL Télécharger un fichier] charge un fichier dans un dossier [!DNL Dropbox].

## Valider

Si la phase d’opération est réussie pour tous les modules, la phase de validation commence au cours de laquelle toutes les opérations effectuées par les modules sont validées. Cela signifie que [!DNL Workfront Fusion] envoie des informations sur son succès à tous les services impliqués dans la phase d&#39;opération.

## Restaurer

Si une erreur se produit pendant la phase d’opération ou de validation d’un module, la phase est abandonnée et la phase de restauration démarre, ce qui rend nulles toutes les opérations pendant le cycle donné. Certains modules ne prennent pas en charge la restauration et les opérations effectuées par ces modules ne peuvent pas être récupérées. Pour plus d’informations, voir la section [Modules ACID](#acid-modules) .

## Finalisation

Pendant la phase de finalisation, les connexions ouvertes (par exemple, connexions FTP, connexions à la base de données, etc.) sont fermées et le scénario est terminé.

## Modules ACID

Tous les modules [!DNL Workfront Fusion] qui prennent en charge la restauration (également appelés transactionalité) sont marqués avec la balise ACID.

![](assets/acid-modules-350x189.png)

Les modules non marqués par cette balise ne peuvent pas revenir à leur état initial lorsque des erreurs se produisent dans d’autres modules. Exemple type de module non-ACID : l’action [!UICONTROL Email] >[!UICONTROL Envoyer un email]. Une fois l&#39;email envoyé, vous ne pouvez pas annuler l&#39;envoi.
