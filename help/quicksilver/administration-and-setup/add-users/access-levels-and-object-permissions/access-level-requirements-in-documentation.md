---
title: Conditions d’accès préalables dans la documentation Workfront
content-type: reference
product-area: system-administration
keywords: access,level,system,administrator,planner,worker,reviewer,requestor,external,user
navigation-topic: access-levels
description: Les articles pratiques de la documentation Workfront contiennent un tableau qui explique l’accès et les autorisations nécessaires à cette procédure. Cet article explique en détail le tableau des exigences d’accès et contient des liens pour plus d’informations.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: 0a01acd56b3ea10d1cccc31a21e434da55b1ec13
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 7%

---

# Conditions d’accès préalables dans la documentation Workfront

Les articles pratiques de la documentation Workfront contiennent un tableau expliquant les exigences d’accès et d’autorisation nécessaires pour cette procédure. Ce tableau des exigences d’accès vous permet de déterminer si vous pouvez effectuer une action spécifique dans Workfront ou pourquoi vous ne pourrez pas le faire. Cet article explique chaque élément du tableau des exigences d’accès et fournit des conseils de dépannage et des liens vers des informations plus détaillées.

Si une ligne est absente du tableau Exigences d’accès d’un article donné, ce type d’action n’est pas requis.

Certaines lignes contiennent des informations intitulées &quot;Nouveau&quot; et &quot;Actuel&quot;. Cela est dû au fait que Workfront est en train de passer à un nouveau modèle de tarification et de conditionnement, certaines organisations opérant sous le nouveau modèle et d’autres encore utilisant le modèle actuel. Pour savoir quel modèle votre entreprise utilise, contactez votre administrateur Workfront. Vous trouverez des détails et des liens vers des informations dans la section [La table des exigences d’accès](#the-access-requirements-table) de cet article.

>[!NOTE]
>
>Si vous avez des questions sur l’application de l’un des champs de ce tableau, contactez votre administrateur Workfront.

## Le tableau des exigences d’accès

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> Les plans Adobe Workfront se rapportent à l’ensemble des fonctionnalités achetées par votre entreprise. La plupart des fonctionnalités de Workfront sont disponibles dans tous les plans, à quelques exceptions près, notamment en ce qui concerne la planification stratégique et les contrôles d’entreprise. 
   <ul><li>Pour savoir quel plan Adobe Workfront votre organisation utilise, y compris si votre organisation est basée sur le modèle de package actuel ou nouveau, contactez votre administrateur Workfront.</li>
   <li>Pour plus d’informations sur la façon dont un administrateur Workfront peut localiser le plan Workfront de votre entreprise, voir <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">Affichage de la grappe de votre entreprise et du plan Workfront</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> Les licences Adobe Workfront se rapportent à l’ensemble des fonctionnalités Workfront incluses dans la licence qui vous est attribuée. Par exemple, un utilisateur peut disposer d’une licence qui inclut le marquage des tâches terminées et le temps de connexion, tandis qu’un autre utilisateur dispose d’une licence qui lui permet uniquement d’approuver des ressources ou d’envoyer des requêtes. <p> 
   <ul>
   <li>Pour connaître la licence qui vous a été attribuée, contactez votre administrateur Workfront.</li>
   <li>Adobe Workfront passe à un nouveau modèle de tarification et de conditionnement. Pour plus d’informations sur les licences, voir :
   <ul>
   <li>Nouveau : <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Présentation des nouvelles licences</a></li>
   <li>Actuel : <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences</a></li></ul></li>
   <li>Si vous disposez du niveau d’accès correct et que vous n’y avez toujours pas accès, demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Workfront propose certains produits qui peuvent être achetés en plus de Workfront.
   <p>Les articles qui décrivent les procédures effectuées dans ces produits supplémentaires répertorient ici le produit requis.</p>
   <ul>
   <li>Adobe Experience Manager Assets ou Assets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Objectifs Workfront</li>
   <li>Planificateur de scénarios Workfront</li>
   </ul>
   <p>Pour savoir si votre entreprise a acheté l’un de ces produits supplémentaires, contactez votre administrateur Workfront.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> Les niveaux d’accès sont des ensembles d’autorisations pour les actions que vous pouvez effectuer dans Workfront, définis par votre administrateur Workfront. <p>Workfront dispose de niveaux d’accès intégrés qui correspondent aux licences Workfront, mais votre administrateur Workfront peut créer plus de niveaux d’accès pour refléter plus précisément les jeux d’autorisations nécessaires à votre entreprise.</p>
   <ul>
    <li>Adobe Workfront passe à un nouveau modèle de tarification et de conditionnement. Pour plus d’informations sur les niveaux d’accès pour chaque modèle, voir :
   <ul>
   <li>Nouveau : <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">New access levels overview</a></li>
   <li>Actuel : <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Présentation des niveaux d’accès</a></li></ul></li>
    <li>Pour connaître les détails de votre niveau d’accès, contactez votre administrateur Workfront.</li>
    <li>Si vous êtes administrateur Workfront, consultez la section <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurer l’accès à Adobe Workfront</a> pour en savoir plus sur l’octroi de l’accès à des objets spécifiques du niveau d’accès.</li>  
   <li>Si vous disposez du niveau d’accès correct et que vous n’y avez toujours pas accès, demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td><p>Les autorisations d’objet se rapportent à l’accès à des objets Workfront individuels lorsque vous les créez ou lorsqu’ils sont partagés avec vous. Par exemple, vous devez disposer de l’accès Affichage à un projet spécifique pour afficher le projet, même si votre niveau d’accès vous permet d’afficher les projets. Cette section du tableau Exigences d’accès décrit toutes les autorisations d’objet spécifiques dont vous avez besoin pour effectuer l’action dans l’article.</p>
   <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un objet, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets</a>.</p><p>Pour plus d'informations sur le partage d'un objet, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">Partage d'un objet</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Modèle de disposition</td> 
   <td><p>Les modèles de mise en page contrôlent ce que vous pouvez voir dans votre menu principal et sont configurés par votre administrateur Workfront. Cette ligne indique toutes les zones spécifiques de Workfront qui doivent être incluses dans votre menu principal pour exécuter l’action.</p><p>En règle générale, si un article vous demande de cliquer sur une zone du menu principal et que cette zone n’est pas visible dans votre menu principal, contactez votre administrateur Workfront pour déterminer si cette zone peut être mise à votre disposition.</p><p>
   Pour plus d’informations sur la façon dont un administrateur Workfront peut configurer le menu principal, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Personnaliser le menu principal à l’aide d’un modèle de mise en page</a>.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront Fusion</td> 
   <td>Adobe Workfront Fusion possède un modèle de licence distinct de Workfront. 
   <ul><li>Actuel : le modèle de licence actuel est basé sur le nombre d’opérations effectuées et n’a aucune limite sur les actions qu’une organisation peut effectuer. </li>
   <li>Hérité : les licences héritées sont basées sur la capacité des scénarios à se connecter à des applications tierces ou sur l’utilisation des scénarios pour l’automatisation de Workfront uniquement. </li>
   </ul>
   Pour plus d’informations sur les licences Fusion, voir <a href="/help/quicksilver/workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">Licences de fusion Workfront</a>.
   </td> 
  </tr> 
 </tbody> 
</table>
