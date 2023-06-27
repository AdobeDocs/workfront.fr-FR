---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Exécution de scénarios, cycles et phases dans [!DNL Adobe Workfront Fusion]
description: Cet article décrit les événements qui se produisent pendant une [!DNL Adobe Workfront Fusion] est en cours d’exécution (initialisation, opérations, validations et restaurations, par exemple).
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

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
>...
>
>#N de cycle
>
>Opération (lecture ou écriture)
>
>Validation ou restauration
>
>Finalisation

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
  <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail, [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Initialisation

Lors de la phase d’initialisation, toutes les connexions nécessaires (connexion à une base de données, service de messagerie, etc.) sont créées. Elles sont également vérifiées si chaque module est capable d’effectuer les opérations prévues.

## Cycles

Chaque cycle représente une unité de travail inséparable composée d&#39;une série d&#39;opérations. Il est possible de définir le nombre maximal de cycles dans la variable [!UICONTROL paramètres de scénario] du panneau. Le nombre par défaut est 1.

Pour plus d’informations, voir [Le panneau des paramètres de scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Opération

Pendant la phase d&#39;opération, l&#39;opération de lecture et/ou d&#39;écriture est effectuée :

* L’opération de lecture consiste à obtenir des données d’un service qui est ensuite traité par d’autres modules selon un scénario prédéfini. Par exemple, la variable [!UICONTROL Dropbox] >[!UICONTROL Fichiers de contrôle] Le module renvoie les nouveaux lots (fichiers) créés depuis la dernière exécution du scénario.
* L’opération d’écriture consiste à envoyer des données à un service donné en vue d’un traitement ultérieur. Par exemple, la variable [!DNL Dropbox] >[!UICONTROL Chargement d’un fichier] charge un fichier dans un [!DNL Dropbox] dossier.

## Valider

Si la phase d’opération est réussie pour tous les modules, la phase de validation commence au cours de laquelle toutes les opérations effectuées par les modules sont validées. Cela signifie que [!DNL Workfront Fusion] envoie des informations sur son succès à tous les services impliqués dans la phase d&#39;opération.

## Retour arrière

Si une erreur se produit pendant la phase d’opération ou de validation d’un module, la phase est abandonnée et la phase de restauration démarre, ce qui rend nulles toutes les opérations pendant le cycle donné. Certains modules ne prennent pas en charge la restauration et les opérations effectuées par ces modules ne peuvent pas être récupérées. Pour plus d’informations, voir [Modules ACID](#acid-modules) .

## Finalisation

Pendant la phase de finalisation, les connexions ouvertes (par exemple, connexions FTP, connexions à la base de données, etc.) sont fermées et le scénario est terminé.

## Modules ACID

Tous [!DNL Workfront Fusion] Les modules qui prennent en charge la restauration (également appelés transactionalité) sont marqués par la balise ACID.

![](assets/acid-modules-350x189.png)

Les modules non marqués par cette balise ne peuvent pas revenir à leur état initial lorsque des erreurs se produisent dans d’autres modules. Exemple type de module non ACID : [!UICONTROL Email] >[!UICONTROL Envoyer un courrier électronique] action. Une fois l&#39;email envoyé, vous ne pouvez pas annuler l&#39;envoi.
