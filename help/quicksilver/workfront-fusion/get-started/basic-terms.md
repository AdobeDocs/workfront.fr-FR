---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Termes de base dans Adobe Workfront Fusion
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: eb39c26b076e89acb8bc4eef1a459b6ef8cd389b
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 96%

---

# Termes de base dans [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une licence [!DNL Adobe Workfront Fusion] en plus d’une licence [!UICONTROL Adobe Workfront].


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Action</p> </td> 
   <td>Module qui vous permet de lire ou d’écrire des lots à partir de ou vers une application ou un service sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aggregator]</p> </td> 
   <td> <p>Type de module qui fusionne plusieurs lots (plusieurs tableaux de données) en un seul lot. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">Module [!UICONTROL Aggregator] dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Clé API</td> 
   <td>Code unique qui identifie l’utilisateur ou l’utilisatrice, la personne chargée du développement ou le programme qui appelle l’API d’un logiciel, utilisée pour l’authentification. Comme les modules [!DNL Adobe Workfront Fusion] fonctionnent en connectant des API, des clés API sont parfois nécessaires. Les clés API sont distribuées par l’application qui en a besoin. Par exemple, si vous avez besoin d’une clé API pour [!DNL ActiveCampaign], vous la demandez via votre compte [!DNL ActiveCampaign].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Application ou service</td> 
   <td> <p>Une application logicielle, le plus souvent.</p> <p>Une application peut également être une fonction spéciale qui manipule des données, comme un itérateur ou un agrégateur. </p> <p>Un service est une source de lots qui peuvent inclure une API web, une page web, différents types de serveurs (FTP, SMTP, IMAP), etc. </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connecteur d’application</td> 
   <td>Application qui se connecte à un autre système.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Lot</p> </td> 
   <td> <p>Un lot est une unité de base qui est renvoyée ou reçue par les modules. Un lot se compose de plusieurs éléments.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Lorsque vous ajoutez une application ou un service à un scénario, vous devrez très probablement créer une connexion entre [!DNL Workfront Fusion] et l’application ou le service afin de récupérer ou d’envoyer les données sélectionnées. Pour plus d’informations, voir <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">Vue d’ensemble des connexions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Cycle</p> </td> 
   <td> <p>Un cycle fait référence à deux phases du déroulement du scénario : l’opération et l’engagement. Le scénario peut consister en un ou plusieurs cycles. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Exécution du scénario, cycles et phases dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Entrepôt de données</p> </td> 
   <td> <p>Outil qui stocke les données des scénarios ou qui vous permet de transférer des données entre des scénarios spécifiques ou des exécutions de scénarios. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">Entrepôts de données dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transfert de données</p> </td> 
   <td> <p>Quantité de données transférées par le biais de votre scénario. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Détails du scénario dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Filtre</p> </td> 
   <td> <p>Fonctionnalités supplémentaires pouvant être appliquées entre deux modules. Un filtre vous permet de ne travailler qu’avec les lots qui répondent à certains critères. Il existe un certain nombre de filtres différents que vous pouvez appliquer. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Ajouter un filtre à un scénario dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>Nom utilisé pour identifier de manière unique un lot. Un ID est généralement utilisé pour différencier un lot qui doit être mis à jour ou supprimé d’un service donné.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Éléments</p> </td> 
   <td> <p>Partie d’un lot. Les lots peuvent être composés de plusieurs éléments. Il existe plusieurs types d’éléments : texte, nombre, booléen (oui/non), date, heure, buffer (données binaires), collections, menu de sélection, tableau et validation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Iterator]</p> </td> 
   <td> <p>Type de module qui vous permet de prendre un lot de données (un tableau de données) et de le diviser en lots distincts. Pour plus d’informations, consultez le module [!UICONTROL Iterator] <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref"> dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Module</p> </td> 
   <td> <p>Étape unique dans un scénario qui exécute une fonction, telle que la création d’un enregistrement, dans l’application associée ou le service associé.</p> <p>Chaque application ou service possède différents modules qui définissent la manière sa manière de répondre à une requête.</p> <p>Il existe quatre types de modules : les actions, les déclencheurs, les itérateurs et les agrégateurs.</p> <p> <img src="assets/module.jpg"> </p> <p>Pour plus d’informations, consultez la section <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Types de modules</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Opération</p> </td> 
   <td> <p>Tâche effectuée par un module.</p><p>Pour plus d’informations, consultez la section <a href="../../workfront-fusion/get-started/operations-in-workfront-fusion.md" class="MCXref xref">Opérations dans [!DNL Adobe Workfront Fusion]</a>.</p>
  </tr> 
  <tr> 
   <td role="rowheader">Clés publiques/privées</td> 
   <td>Les clés publiques et privées sont utilisées pour chiffrer et déchiffrer les données. La clé publique peut être distribuée, et toute personne la possédant peut chiffrer des données, mais seule la clé privée peut les déchiffrer. De même, un utilisateur ou une utilisatrice disposant d’une clé privée peut chiffrer des données que toute personne disposant de la clé publique peut déchiffrer. Le chiffrage de la clé privée garantit que les données proviennent de la personne qui la possède et sert de validation de la source des données.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Router]</p> </td> 
   <td>Permet de dupliquer des données ou d’ajouter de nouveaux itinéraires à un scénario, afin de réacheminer les données et de traiter séparément différents groupes de données. Pour plus d’informations, consultez le module <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">[!UICONTROL Router] dans [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Scénario</p> </td> 
   <td> <p>Série d’étapes automatisées créées par l’utilisateur ou par l’utilisatrice, chacune représentée et exécutée par un module. L’objectif d’un scénario est de déplacer et de manipuler des données.</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> Pour plus d’informations, consultez la section <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Segment de scénario</p> </td> 
   <td> <p> Section d’un scénario composée d’une série de modules qui se connectent tous à la même application. Les segments de scénario représentent souvent un processus court dans l’application.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transactions</p> </td> 
   <td> <p>[!DNL Workfront Fusion] Utilise le traitement transactionnel pour capturer le cycle de vie des scénarios. À travers plusieurs phases, une transaction fait passer les données d’un statut cohérent à un autre. Le processus se décompose en quatre phases : initialisation, exploitation (lecture ou écriture), validation/restauration et finalisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Déclencheur</p> </td> 
   <td> <p>Module qui vous permet de saisir les lots qui ont été ajoutés ou mis à jour depuis la dernière exécution d’un scénario. Il existe deux types de déclencheurs : attente active et instantané (webhooks). Pour plus d’informations, consultez la section <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>Type spécial de déclencheur qui vous permet d’exécuter un scénario immédiatement après la mise à disposition d’un nouveau lot. Pour plus d’informations, consultez la section <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheurs instantanés (webhooks) dans [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
