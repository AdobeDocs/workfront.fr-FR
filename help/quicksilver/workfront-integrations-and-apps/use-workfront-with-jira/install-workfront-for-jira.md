---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installer [!DNL Adobe Workfront] pour [!DNL Jira]
description: Vous pouvez utiliser  [!DNL Adobe Workfront] pour [!DNL Jira] pour intégrer vos systèmes  [!DNL Jira] et [!DNL Workfront] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 7%

---

# Installer [!DNL Adobe Workfront for Jira]

Vous pouvez utiliser [!DNL Adobe Workfront for Jira] pour intégrer vos systèmes [!DNL Jira] et [!DNL Workfront].

Après l’installation du module complémentaire, vous pouvez définir des workflows qui créent automatiquement des problèmes [!DNL Jira] lors de la création d’éléments de travail [!DNL Workfront]. Les éléments des deux applications sont liés et certaines de leurs informations peuvent être automatiquement mises à jour dans les deux systèmes.

Tous les utilisateurs de [!DNL Workfront] et [!DNL Jira] peuvent bénéficier de cette intégration. Ils n&#39;ont besoin d&#39;une licence que pour le système dans lequel ils travaillent le plus, et non pour les deux systèmes.

Ce module complémentaire est disponible pour les versions [!UICONTROL Serveur] et [!UICONTROL OnDemand] (ou [!UICONTROL Cloud]) du logiciel [!DNL Jira]. Ce module complémentaire n’est pas disponible pour la version [!DNL Data Center] du logiciel [!DNL Jira].

Pour obtenir la liste des [!DNL Jira] versions actuellement prises en charge par [!DNL Workfront for Jira], voir [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) sur Atlassian Marketplace.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> 
   <p>Nouveau : Tous</p>
   <p>Actuel : [!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Présentation des licences d’Adobe [!DNL Workfront]</td> 
   <td> 
   <p>Nouvelle : standard</p>
   <p>Actuelle : [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Accès administrateur système</p> <p>Important : Nous vous recommandons de créer des comptes d’administrateur système distincts dans [!DNL Jira] et [!DNL Workfront] afin de vous consacrer à cette intégration, plutôt que d’utiliser des comptes existants pouvant être joints aux utilisateurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td><p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Installer [!DNL Workfront] pour [!DNL Jira]

L&#39;installation de [!DNL Workfront] pour [!DNL Jira] OnDemand est identique à son installation sur une instance de serveur [!DNL Jira].

Vous devez être un administrateur [!DNL Jira] pour installer le module complémentaire [!DNL Workfront].

Si vous n&#39;êtes pas administrateur [!DNL Jira], vous pouvez rechercher le module complémentaire [!DNL Workfront] et le demander pour l&#39;installer. Votre demande est envoyée à l’administrateur [!DNL Jira] pour approbation et installation.

Pour plus d&#39;informations sur la demande d&#39;un module complémentaire à installer sur votre application [!DNL Jira], consultez la section [Gestion des demandes d&#39;utilisateurs pour les modules complémentaires.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Pour installer [!DNL Workfront for Jira] :

1. Connectez-vous à [!DNL Jira] en tant qu’administrateur [!DNL Jira].
1. Recherchez le module complémentaire **[!DNL Workfront for Jira]** dans [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Cliquez sur **[!UICONTROL Obtenir maintenant]** pour l’installer.

   Une fois l’installation terminée, vous pouvez vous connecter à [!DNL Workfront] à partir de [!DNL Jira] et configurer votre intégration.

   Pour plus d’informations, voir [Configuration d’Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Considérations pour une installation [!DNL Jira Server]

>[!NOTE]
>
>Ces exigences ne s’appliquent pas à la version [!UICONTROL OnDemand] ([!UICONTROL Cloud]) du logiciel [!DNL Jira].

Bien que l&#39;installation du module complémentaire [!DNL Workfront] dans les deux environnements [!DNL Jira] soit similaire, vous devez tenir compte des points suivants lorsque vous travaillez avec une installation [!DNL Jira Server] :

* Lors de la configuration du module complémentaire dans [!DNL Jira], l&#39;adresse spécifiée dans le champ **[!DNL JIRA Base URL]** peut ne pas être la même URL que celle utilisée pour accéder à [!DNL Jira] sur votre serveur privé. **[!DNL JIRA Base URL]** doit être une adresse accessible au public connectée à votre serveur privé à l’aide de protocoles NAT ou de proxy inverse, de sorte que [!DNL Workfront] puisse y accéder pour envoyer des requêtes à votre serveur.

* Vous devez utiliser le cryptage SSL pour sécuriser la communication entre [!DNL Jira] et [!DNL Workfront]. Lorsque vous activez SSL, vous devez disposer d’une pile complète de certificats SSL provenant d’une autorité de certification. Nous ne prenons pas en charge les certificats auto-signés.
* Vous devez vous assurer que le domaine [!DNL jira.workfront.com] est accessible à partir de vos serveurs d’entreprise. Il sert d’environnement intermédiaire entre [!DNL Workfront] et [!DNL Jira] et est nécessaire au fonctionnement du module complémentaire.

  Vous devez également ajouter les adresses IP statiques suivantes à la liste autorisée de votre pare-feu pour les connexions sortantes et entrantes.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Pour plus d’informations sur la configuration de votre pare-feu pour des fonctionnalités optimales avec [!DNL Workfront], voir [Configuration de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
