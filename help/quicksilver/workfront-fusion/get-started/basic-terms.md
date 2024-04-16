---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Termes de base d’Adobe Workfront Fusion
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 1%

---

# Termes de base [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une [!DNL Adobe Workfront Fusion] en plus d’une [!UICONTROL Adobe Workfront] licence.


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Action</p> </td> 
   <td>Module qui vous permet de lire ou d’écrire des bundles depuis ou vers une application ou un service sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Agrégateur]</p> </td> 
   <td> <p>Type de module qui fusionne plusieurs lots (plusieurs tableaux de données) en un seul lot. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">Module [!UICONTROL Agrégateur] dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Clé API</td> 
   <td>Code unique qui identifie l’utilisateur, le développeur ou le programme qui appelle l’API d’un logiciel, utilisé pour l’authentification. Depuis [!DNL Adobe Workfront Fusion] Les modules fonctionnent en connectant les API, les clés d’API sont parfois nécessaires. Les clés d’API sont distribuées par l’application qui en a besoin. Par exemple, si vous avez besoin d’une clé API pour [!DNL ActiveCampaign], vous pouvez la demander via votre [!DNL ActiveCampaign] compte .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Application ou service</td> 
   <td> <p>Une application logicielle, le plus souvent.</p> <p>Une application peut également être une fonction spéciale qui manipule des données, comme un itérateur ou un agrégateur. </p> <p>Un service est une source de lots qui peut inclure une API web, une page web, différents types de serveurs (FTP, SMTP, IMAP), etc. </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connecteur d’application</td> 
   <td>Application se connectant à un autre système.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bundle</p> </td> 
   <td> <p>Un lot est une unité de base renvoyée ou reçue par les modules. Un lot se compose d’éléments.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Lors de l’ajout d’une application ou d’un service à un scénario, il est probable que vous deviez d’abord créer une connexion entre [!DNL Workfront Fusion] et l’application ou le service afin de récupérer ou d’envoyer les données sélectionnées. Pour plus d’informations, voir <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">Présentation des connexions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Cycle</p> </td> 
   <td> <p>Un cycle fait référence à deux phases de l’exécution du scénario : opération et validation. Le scénario peut comprendre un ou plusieurs cycles. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Exécution, cycles et phases d’un scénario [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Entrepôt de données</p> </td> 
   <td> <p>Outil qui stocke les données de scénarios ou vous permet de transférer des données entre des scénarios ou des exécutions de scénarios individuels. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">Stockages de données dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transfert de données</p> </td> 
   <td> <p>La quantité de données transférée par le biais de votre scénario. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Détails du scénario dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Filtre</p> </td> 
   <td> <p>Fonctionnalités supplémentaires pouvant être appliquées entre deux modules. Un filtre vous permet ensuite de ne travailler qu’avec des lots qui correspondent à certains critères. Vous pouvez appliquer différents filtres. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Ajouter un filtre à un scénario dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>Nom utilisé pour identifier de manière unique un lot. Un ID est généralement utilisé pour différencier un lot à mettre à jour ou à supprimer d’un service donné.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Éléments</p> </td> 
   <td> <p>Partie d’un lot. Les lots peuvent être composés de plusieurs éléments. Il existe plusieurs types d’éléments : texte, nombre, valeur booléenne (oui/non), date, heure, mémoire tampon (données binaires), collections, menu de sélection, tableau et validation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Iterator]</p> </td> 
   <td> <p>Type de module qui vous permet de prendre un lot de données (un tableau de données) et de les diviser en plusieurs lots distincts. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Module [!UICONTROL Iterator] dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Module</p> </td> 
   <td> <p>Une seule étape d’un scénario qui exécute une fonction, telle que la création d’un enregistrement, dans l’application ou le service associé.</p> <p>Chaque application ou service comporte différents modules qui définissent la manière dont il répond à une requête.</p> <p>Il existe 4 types de modules : actions, déclencheurs, itérateurs et agrégateurs.</p> <p> <img src="assets/module.jpg"> </p> <p>Pour plus d’informations, voir <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Types de modules</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Opération</p> </td> 
   <td> <p>Tâche effectuée par un module.</p><p>Pour plus d’informations, voir <a href="../../workfront-fusion/get-started/operations-in-workfront-fusion.md" class="MCXref xref">Opérations dans [!DNL Adobe Workfront Fusion]</a>.</p>
  </tr> 
  <tr> 
   <td role="rowheader">Clés publiques/privées</td> 
   <td>Les clés publique et privée sont utilisées pour chiffrer et déchiffrer des données. La clé publique peut être distribuée, et toute personne disposant de la clé publique peut crypter les données, mais seule la clé privée peut le décrypter. De même, un utilisateur disposant d’une clé privée peut chiffrer des données que toute personne disposant d’une clé publique peut déchiffrer. Le cryptage de la clé privée garantit que les données proviennent du propriétaire de la clé privée et sert de validation de la source des données.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Routeur]</p> </td> 
   <td>Permet de dupliquer des données ou d’ajouter de nouvelles routes à un scénario. Vous pouvez ainsi réacheminer les données et gérer différents groupes de données séparément. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">Module [!UICONTROL Routeur] dans [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Scénario</p> </td> 
   <td> <p>Série d’étapes automatisées créée par l’utilisateur, chacune représentée et exécutée par un module. L’objectif d’un scénario est de déplacer et de manipuler des données.</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transactions</p> </td> 
   <td> <p>[!DNL Workfront Fusion] utilise le traitement transactionnel pour capturer le cycle de vie du scénario. Une transaction se compose de plusieurs phases au cours desquelles les données sont transformées d’un état cohérent en un autre état cohérent. Il existe 4 phases : initialisation, opération (lecture ou écriture), validation/restauration et finalisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Déclencheur</p> </td> 
   <td> <p>Module qui vous permet de saisir les lots qui ont été ajoutés ou mis à jour depuis la dernière exécution d’un scénario. Il existe deux types de déclencheurs : url et instantané (webhooks). Pour plus d’informations, voir <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>Type spécial de déclencheur qui vous permet d’exécuter un scénario immédiatement après la disponibilité d’un nouveau lot. Pour plus d’informations, voir <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Triggers instantanés (webhooks) dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
