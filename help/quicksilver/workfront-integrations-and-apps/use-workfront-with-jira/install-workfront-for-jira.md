---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installer [!DNL Adobe Workfront] pour [!DNL Jira]
description: Vous pouvez utiliser [!DNL Adobe Workfront] pour [!DNL Jira] pour intégrer votre [!DNL Jira] et [!DNL Workfront] systèmes.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Installer [!DNL Adobe Workfront for Jira]

Vous pouvez utiliser [!DNL Adobe Workfront for Jira] pour intégrer votre [!DNL Jira] et [!DNL Workfront] systèmes.

Après l’installation du module complémentaire, vous pouvez définir des workflows qui créent des [!DNL Jira] se déclenche automatiquement lorsque [!DNL Workfront] les tâches sont créées. Les éléments des deux applications sont liés et certaines de leurs informations peuvent être automatiquement mises à jour dans les deux systèmes.

Tous les utilisateurs de [!DNL Workfront] et [!DNL Jira] peuvent bénéficier de cette intégration. Ils n&#39;ont besoin d&#39;une licence que pour le système dans lequel ils travaillent le plus, et non pour les deux systèmes.

Ce module complémentaire est disponible pour la [!UICONTROL Serveur] et [!UICONTROL OnDemand] (ou [!UICONTROL Cloud]) [!DNL Jira] Logiciel. Ce module complémentaire n’est pas disponible pour la variable [!DNL Data Center] version de [!DNL Jira] Logiciel.

Pour une liste de [!DNL Jira] versions qui [!DNL Workfront for Jira] actuellement pris en charge, voir [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) sur l&#39;Atlassian Marketplace.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] Présentation des licences</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accès</td> 
   <td> <p>Accès administrateur système</p> <p>Important : Nous vous recommandons de créer des comptes d’administrateur système distincts dans [!DNL Jira] et [!DNL Workfront] pour dédier à cette intégration, plutôt que d’utiliser des qui peuvent être associés à des utilisateurs existants.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Installer [!DNL Workfront] pour [!DNL Jira]

Installation [!DNL Workfront] pour [!DNL Jira] OnDemand est identique à l’installation sur un [!DNL Jira] Instance du serveur.

Vous devez être un [!DNL Jira] administrateur pour installer le [!DNL Workfront] module complémentaire .

Si vous n’avez pas [!DNL Jira] administrateur, vous pouvez rechercher la variable [!DNL Workfront] module complémentaire et demandez-le d’être installé. Votre demande est envoyée à la fonction [!DNL Jira] pour la validation et l&#39;installation.

Pour plus d’informations sur la demande d’un module complémentaire à installer sur votre [!DNL Jira] application, voir [Gestion des demandes d’utilisateurs pour les modules complémentaires.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Pour installer [!DNL Workfront for Jira]:

1. Connectez-vous à [!DNL Jira] as a [!DNL Jira] administrateur.
1. Recherchez le **[!DNL Workfront for Jira]** module complémentaire dans le [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Cliquez sur **[!UICONTROL Obtenir maintenant]** pour l’installer.

   Une fois l’installation terminée, vous pouvez vous connecter à [!DNL Workfront] de [!DNL Jira] et configurez votre intégration.
   [!DNL ]
Pour plus d’informations, voir [Configuration d’Adobe Workfront pour Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Considérations pour un [!DNL Jira Server] installation

>[!NOTE]
>
>Ces exigences ne s’appliquent pas à la variable [!UICONTROL OnDemand] ([!UICONTROL Cloud]) version de [!DNL Jira] Logiciel.

Lors de l’installation du [!DNL Workfront] module complémentaire dans les deux [!DNL Jira] Les environnements sont similaires. Vous devez tenir compte des points suivants lorsque vous utilisez une [!DNL Jira Server] installation :

* Lors de la configuration du module complémentaire dans [!DNL Jira], l’adresse spécifiée dans la variable **[!DNL JIRA Base URL]** peut ne pas être la même URL que celle utilisée pour accéder à [!DNL Jira] sur votre serveur privé. Le **[!DNL JIRA Base URL]** doit être une adresse accessible au public connectée à votre serveur privé à l’aide de protocoles NAT ou de proxy inverse, [!DNL Workfront] peut y accéder pour envoyer des requêtes à votre serveur.

* Vous devez utiliser le chiffrement SSL pour sécuriser la communication entre les [!DNL Jira] et [!DNL Workfront]. Lorsque vous activez SSL, vous devez disposer d’une pile complète de certificats SSL provenant d’une autorité de certification. Nous ne prenons pas en charge les certificats auto-signés.
* Vous devez vous assurer que la variable [!DNL jira.workfront.com] est accessible à partir des serveurs de votre entreprise. Il sert d’environnement intermédiaire entre les [!DNL Workfront] et [!DNL Jira] et est requis pour que le module complémentaire fonctionne.

   Vous devez également ajouter les adresses IP statiques suivantes à la liste autorisée de votre pare-feu pour les connexions sortantes et entrantes.

   `35.162.128.73`

   `34.213.36.118`

   `35.160.0.242`

   `3.209.27.146`

   `18.205.251.4`

   Pour plus d’informations sur la configuration de votre pare-feu pour des fonctionnalités optimales avec [!DNL Workfront], voir [Configuration du pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
