---
title: Conditions d’accès dans la documentation Workfront
content-type: reference
product-area: system-administration
keywords: niveau d’accès, système, administrateur ou administratrice, planificateur ou planificatrice, travailleur ou travailleuse, réviseur ou réviseuse, demandeur ou demandeuse, utilisateur ou utilisatrice externe
navigation-topic: access-levels
description: Les articles pratiques de la documentation Workfront contiennent un tableau qui explique l’accès et les autorisations nécessaires à cette procédure. Cet article explique en détail le tableau des conditions d’accès et contient des liens pour plus d’informations.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: 469242118429fa37835766737b88d35d2baefb69
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 67%

---

# Conditions d’accès préalables dans la documentation Workfront

Les articles pratiques de la documentation Workfront contiennent un tableau expliquant les conditions d’accès et d’autorisation nécessaires pour cette procédure. Ce tableau des conditions d’accès vous permet de déterminer si vous pouvez effectuer une action spécifique dans Workfront ou pourquoi vous ne pouvez pas le faire. Cet article explique chaque élément du tableau des conditions d’accès et fournit des conseils de dépannage et des liens vers des informations plus détaillées.

Si une ligne est absente du tableau des conditions d’accès dans un article donné, il n’y a aucune condition pour ce type d’action.

Certaines lignes contiennent des informations intitulées « Nouveau » et « Actuel ». Cela est dû au fait que Workfront est en train de passer à un nouveau modèle de tarification et de conditionnement, certaines organisations fonctionnant selon le nouveau modèle et d’autres selon le modèle actuel. Pour savoir quel modèle votre organisation utilise, contactez votre administrateur ou administratrice Workfront. Vous trouverez des détails et des liens vers des informations dans la section [Tableau des conditions d’accès](#the-access-requirements-table) de cet article.

>[!NOTE]
>
>Si vous avez des questions sur l’application de l’un des champs de ce tableau, contactez votre administrateur ou administratrice Workfront.

## Le tableau des conditions d’accès

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> Les packages Adobe Workfront font référence à l’ensemble des fonctionnalités achetées par votre entreprise. La plupart des fonctionnalités de Workfront sont disponibles dans tous les packages, à quelques exceptions près, principalement liées à la planification stratégique et aux contrôles d’entreprise. <p>Les packages qui existaient avant 2022 ne sont pas répertoriés.</p>
   <p>Les packages Workfront sont divisés en trois zones. Chaque zone propose différents packages, tels que Select, Prime et Ultimate.<p>
   <ul>
   <li><b>Workflow Workfront </b> : inclut des fonctionnalités liées aux opérations, telles que la gestion des tâches, les approbations et les feuilles de temps.</li>
   <li><b>Planification Workfront </b> : inclut les fonctionnalités liées à la planification stratégique.</li>
   <li><b>Automatisation et intégration de Workfront </b> : comprend des fonctionnalités liées à l’automatisation des processus et à l’intégration à d’autres applications.</li>
   </ul>
  <p>Votre entreprise a peut-être acheté un package Workfront dans une ou plusieurs de ces zones.</p>
  <p>Auparavant, Workfront offrait des packages Workfront Select, Workfront Prime et Workfront Ultimate, sans faire de distinction entre les workflows, la planification, l’automatisation et l’intégration. Votre entreprise peut se trouver sur l’un de ces packages hérités. 
   <ul><li>Pour savoir quel package Adobe Workfront votre organisation utilise, et notamment si votre organisation dispose du modèle de package actuel ou hérité, contactez votre administrateur Workfront.</li>
   <li>Pour obtenir des instructions sur la manière dont un administrateur Workfront peut localiser le package Workfront de votre organisation, voir <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Afficher le cluster et le package Workfront de votre organisation</a>.</li><li>Pour plus d’informations sur les packages Workfront, voir <a href="https://business.adobe.com/products/workfront/pricing.html">Tarification et package Adobe Workfront</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> Les licences Adobe Workfront se rapportent à l’ensemble des fonctionnalités Workfront incluses dans la licence qui vous est attribuée. Par exemple, un utilisateur ou une utilisatrice peut disposer d’une licence qui inclut le marquage des tâches comme terminées et le temps de connexion, tandis qu’un autre utilisateur ou utilisatrice peut disposer d’une licence qui lui permet uniquement d’approuver des ressources ou d’envoyer des requêtes. <p> 
   <ul>
   <li>Pour connaître la licence qui vous est attribuée, contactez votre administrateur ou administratrice Workfront.</li>
   <li>Pour plus d’informations sur les licences, consultez :
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Vue d’ensemble des nouvelles licences</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences</a></li></ul></li>
   <li>Si vous disposez du bon niveau d’accès et que vous n’y avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td><p>Workfront travaillant en étroite collaboration avec d’autres produits Adobe, certaines procédures de Workfront interagissent directement avec ces produits. Pour suivre ces procédures, votre entreprise doit avoir acheté ce produit. Par exemple, pour utiliser la fonctionnalité qui permet à Workfront d’interagir avec Adobe Experience Manager Assets, votre entreprise doit avoir acheté Adobe Experience Manager Assets.</p>
   <p>Les articles qui décrivent les procédures effectuées avec des produits supplémentaires répertorient les produits requis dans la ligne de produits de ce tableau.</p>
   <p>Pour savoir si votre organisation a acheté l’un de ces produits supplémentaires, contactez votre administrateur ou administratrice Workfront.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> Les niveaux d’accès sont des ensembles d’autorisations pour les actions que vous pouvez effectuer dans Workfront, définis par votre administrateur ou administratrice Workfront. <p>Workfront dispose de niveaux d’accès intégrés qui correspondent aux licences Workfront, mais votre administrateur ou administratrice Workfront peut créer plus de niveaux d’accès pour refléter plus précisément les jeux d’autorisations nécessaires à votre organisation.</p>
   <ul>
    <li>Pour plus d’informations sur les niveaux d’accès, voir :
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Vue d’ensemble des nouveaux niveaux d’accès</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Vue d’ensemble des niveaux d’accès</a></li></ul></li>
    <li>Pour connaître les détails de votre niveau d’accès, contactez votre administrateur ou administratrice Workfront.</li>
    <li>Si vous êtes administrateur ou administratrice Workfront, reportez-vous à la section <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurer l’accès à Adobe Workfront</a> pour en savoir plus sur l’octroi de l’accès à des objets spécifiques dans le niveau d’accès.</li>  
   <li>Si vous disposez du bon niveau d’accès et que vous n’y avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, consultez <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td><p>Les autorisations d’objet se rapportent à l’accès à des objets Workfront individuels lorsque vous les créez ou lorsqu’ils sont partagés avec vous. Par exemple, vous devez disposer de l’accès en affichage à un projet spécifique pour afficher le projet, même si votre niveau d’accès vous permet d’afficher les projets. Cette section du tableau Condition d’accès décrit toutes les autorisations d’objet spécifiques dont vous avez besoin pour effectuer l’action dans l’article.</p>
   <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un objet, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p><p>Pour plus d’informations sur le partage d’un objet, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">Partager un objet</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Modèle de mise en page</td> 
   <td><p>Les modèles de mise en page contrôlent ce que vous pouvez voir dans votre menu principal et sont configurés par votre administrateur ou administratrice Workfront. Cette ligne indique toutes les zones spécifiques de Workfront qui doivent être incluses dans votre menu principal pour exécuter l’action.</p><p>En règle générale, si un article vous demande de cliquer sur une zone du menu principal et que cette zone n’est pas visible dans votre menu principal, contactez votre administrateur ou administratrice Workfront pour déterminer si cette zone peut être mise à votre disposition.</p><p>
   Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut configurer le menu principal, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Personnaliser le menu principal à l’aide d’un modèle de mise en page</a>.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront Fusion</td> 
   <td>Adobe Workfront Fusion a un modèle d’attribution de licence distinct de Workfront. 
   <ul><li>Le modèle de licence actuel est basé sur le nombre d’opérations effectuées et n’a aucune limitation sur les actions qu’une organisation peut effectuer. </li>
   <li>Les licences héritées dépendent de la possibilité ou non pour les scénarios de se connecter à des applications tierces, ou de l’utilisation ou non des scénarios pour l’automatisation de Workfront uniquement. </li>
   </ul>
   Pour plus d’informations sur l’attribution de licence Fusion, voir <a href="https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Licences Workfront Fusion</a>.
   </td> 
  </tr> 
 </tbody> 
</table>
