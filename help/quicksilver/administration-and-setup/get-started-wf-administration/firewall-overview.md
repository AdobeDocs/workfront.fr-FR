---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Vue d’ensemble du pare-feu
description: Comme Adobe Workfront communique avec le réseau de votre entreprise, le pare-feu de votre entreprise doit être configuré pour autoriser cette communication. Les pare-feu sont des mesures de sécurité très efficaces qui isolent le réseau d’une entreprise d’Internet. Ils garantissent que seules les données et le trafic réseau sélectionnés peuvent entrer ou sortir du réseau de l’entreprise. Le pare-feu autorise ou bloque les données en fonction du site qui envoie ou reçoit les données. En tant qu’administrateur ou administratrice d’Adobe Workfront, vous devez vous assurer que les données envoyées vers ou à partir de Workfront sont autorisées par le pare-feu de votre entreprise.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 98%

---

# Vue d’ensemble du pare-feu

Comme Adobe Workfront communique avec le réseau de votre entreprise, le pare-feu de votre entreprise doit être configuré pour autoriser cette communication. Les pare-feu sont des mesures de sécurité très efficaces qui isolent le réseau d’une entreprise d’Internet. Ils garantissent que seules les données et le trafic réseau sélectionnés peuvent entrer ou sortir du réseau de l’entreprise. Le pare-feu autorise ou bloque les données en fonction du site qui envoie ou reçoit les données. En tant qu’administrateur ou administratrice d’Adobe Workfront, vous devez vous assurer que les données envoyées vers ou à partir de Workfront sont autorisées par le pare-feu de votre entreprise.

Pour ce faire, vous devez créer une liste autorisée, soit une « liste » des sites « autorisés » à envoyer ou recevoir des données par le biais du pare-feu. Les sites peuvent être identifiés de deux façons :

* **Adresse IP** : une suite de chiffres similaire à 52.31.132.175
* **Domaine** : composante d’une URL, comme « this domain » dans www.thisdomain.com

Workfront utilise des adresses IP et des domaines spécifiques lors des communications web. Elles doivent être ajoutées à la liste autorisée de votre entreprise avant de pouvoir utiliser Workfront dans votre entreprise.

Une liste autorisée est généralement configurée par un administrateur ou une administratrice réseau. Contactez l’administrateur ou l’administratrice réseau de votre entreprise pour vous assurer que votre pare-feu autorise ces adresses IP. Si vous ne savez pas qui est votre administrateur ou administratrice réseau, contactez le service informatique de votre entreprise pour obtenir plus d’informations.

>[!IMPORTANT]
>
>En tant qu’administrateur ou administratrice de Workfront, vous devez vous assurer que ces adresses et domaines IP sont ajoutés à la liste autorisée de votre entreprise. Ce principe s’applique même si vous ne les ajoutez pas vous-même. Workfront ne peut pas configurer la liste autorisée de votre entreprise.

## Collecter les informations pour la configuration de votre pare-feu

Pour configurer votre pare-feu pour Workfront, votre administrateur ou administratrice réseau doit connaître les adresses IP et domaines à ajouter. Certaines de ces informations sont accessibles uniquement à un administrateur ou une administratrice Workfront. En tant qu’administrateur ou administratrice de Workfront, vous devez localiser ces informations et les fournir à votre administrateur ou administratrice réseau.

>[!NOTE]
>
>Il est recommandé d’ajouter uniquement les adresses IP et les domaines qui accèdent aux fonctionnalités que votre entreprise utilise activement. Assurez-vous de suivre cette bonne pratique et de fournir ces informations.

Fournissez les informations suivantes à votre administrateur ou administratrice réseau :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adresses IP et domaines spécifiques à autoriser</td> 
   <td> <p>L’article <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Configurer la liste autorisée de votre pare-feu</a> contient la liste des adresses IP et des domaines que votre entreprise doit ajouter à sa liste autorisée. </p> <p>Votre administrateur ou administratrice réseau peut ne pas avoir accès à l’article « Configurer la liste autorisée de votre pare-feu ». Dans ce cas, vous devez le lui fournir. Il est déconseillé d’imprimer une copie papier. Une copie numérique permet à l’administrateur ou l’administratrice réseau de copier et coller les adresses, ce qui est plus rapide et plus précis que la saisie sur une page papier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Votre cluster</td> 
   <td>Pour localiser le cluster de votre entreprise, consultez la section <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Afficher le cluster et le plan Workfront de votre entreprise</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Votre plan Workfront</td> 
   <td> <p>Pour localiser le plan de votre entreprise, consultez la section <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Afficher le cluster et le plan Workfront de votre entreprise.</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Votre domaine</td> 
   <td> <p>Pour localiser votre domaine, consultez l’adresse web que vous utilisez pour vous connecter à Workfront.</p> <p>Exemple : dans l’adresse web <code>greatcompany.my.workfront.com</code>, le domaine est « greatcompany ».</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autres produits Adobe Workfront</td> 
   <td> <p>Indiquez à votre administrateur ou administratrice réseau si vous disposez de licences pour l’un des produits suivants :</p> 
    <ul> 
     <li> <p>Adobe Workfront Proof</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Intégrations Adobe Workfront</td> 
   <td>Si vous utilisez l’une des intégrations suivantes, informez votre administrateur ou administratrice réseau :
    <ul>
     <li><p>Workfront pour Jira</p></li>
     <li><p>Workfront pour Google Workspace</p></li>
     <li><p>Workfront pour Microsofts Teams</p></li>
     <li><p>Workfront pour Outlook</p></li>
     <li><p>Workfront pour Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fonctionnalités supplémentaires</td> 
   <td> <p>Si vous utilisez les fonctionnalités suivantes, informez votre administrateur ou administratrice réseau :</p> 
    <ul> 
     <li> <p>Lecteur de test Workfront</p> </li> 
    </ul> </td>
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Si vous ajoutez l’un de ces produits ou l’une de ces intégrations ou fonctionnalités ultérieurement, vous devez contacter l’administration réseau afin qu’elle puisse mettre à jour la liste autorisée.

### Afficher le cluster et le plan Workfront de votre entreprise {#view-your-organization-s-cluster-and-workfront-plan}

{{step-1-to-setup}}

1. Cliquez sur **Système** dans le panneau de gauche.
1. Pour afficher le cluster, sélectionnez **Infos client**.

   Votre cluster s’affiche dans le coin supérieur droit de la section **Informations de base**.

   ![](assets/locate-cluster.png)

1. Pour afficher votre plan Workfront, sélectionnez **Licences**.

   Votre plan s’affiche près du coin supérieur droit de la page.

   ![](assets/locate-plan.png)
