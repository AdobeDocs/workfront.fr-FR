---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configurer [!DNL Workfront Proof] emails pour éviter les filtres anti-spam
description: "Le filtre de messages indésirables de votre client de messagerie a un objectif important : vous protégeant contre les emails indésirables et potentiellement malveillants. Cependant, si vous ne disposez pas des paramètres appropriés dans le filtre de messages indésirables, cela peut vous empêcher de voir les éléments importants suivants : [!DNL Workfront Proof] emails : des notifications par courrier électronique, des newsletters et des communications spéciales."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Configurer [!DNL Workfront Proof] emails pour éviter les filtres anti-spam

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Le filtre de messages indésirables de votre client de messagerie a un objectif important : vous protégeant contre les emails indésirables et potentiellement malveillants. Cependant, si vous ne disposez pas des paramètres appropriés dans le filtre de messages indésirables, cela peut vous empêcher de voir les éléments importants suivants : [!DNL Workfront Proof] emails : notifications par courrier électronique, newsletters et communications spéciales.

Pour vérifier que la variable [!DNL Workfront Proof] Les emails sont toujours routés vers votre boîte de réception au lieu de votre dossier de messages indésirables. Vous devez ajouter les éléments suivants à la liste autorisée :

* [!DNL Workfront Proof] serveur de messagerie : **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; Adresses électroniques (par exemple, notification@proofhq.com)

Pour plus d’informations sur les URL à ajouter à votre liste autorisée, voir [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) dans l’article [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; adresses électroniques

Selon votre type de client de messagerie, vous devrez peut-être ajouter [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot;adresses électroniques à l’une des suivantes afin d’empêcher le filtre de messages indésirables de router vos messages électroniques vers votre dossier de messages indésirables à l’avenir :

* Votre liste de contacts
* Votre [!UICONTROL Expéditeurs sécurisés] list
* Un filtre que vous créez pour envoyer des emails depuis ces adresses vers votre boîte de réception

Vous devrez peut-être également supprimer les [!DNL Workfront Proof] des emails provenant de votre dossier de messages indésirables et vérifiez si l’un des éléments &quot;[!UICONTROL de]Les adresses figurent sur la liste des adresses bloquées. Cette page d’aide répertorie les [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot;adresse et indique comment les ajouter au filtre de spam dans les clients de messagerie suivants :

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Si vous avez des questions sur une procédure décrite ici, veuillez consulter l’aide de votre client de messagerie.

Pour plus d’informations, voir [Configuration des paramètres de courrier indésirable pour les clients de messagerie courants](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## Le [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; adresses électroniques à copier

Pour vérifier que la variable [!DNL Workfront Proof] les courriers électroniques atteignent votre boîte de réception, vous devrez ajouter deux [!DNL Workfront Proof] les adresses électroniques séparément au filtre de messages indésirables de votre client de messagerie :

* l&#39;adresse générale du support, [!DNL support@proofhq.com], à partir de laquelle [!DNL Workfront Proof] envoie de nombreuses communications par courrier électronique ;
* Adresse de notification à partir de laquelle [!DNL Workfront Proof] envoie des emails de notification de BAT au créateur du BAT et aux validants avec des liens vers le BAT. Il peut s’agir d’une adresse générale, notification@support.proofhq.com ou d’une adresse spécifique si vous disposez d’un sous-domaine personnalisé ou d’un domaine d’étiquette blanche.

Pour ajouter [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; adresses au filtre de votre client de messagerie :

1. Copiez le général [!DNL Workfront Proof] support &quot;[!UICONTROL de]&quot; Adresse électronique (support@proofhq.com) et collez-la dans le champ indiqué pour votre client de messagerie.
1. Copiez l’une des options suivantes [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; des adresses électroniques et collez-les SÉPARÉMENT dans le champ indiqué pour votre client de messagerie :

   * notification@support.proofhq.com si vous n’avez PAS de sous-domaine personnalisé ou de domaine d’étiquette blanche
   * notification@yoursubdomain.proofhq.com si vous disposez d’un sous-domaine personnalisé ; remplacer le nom du sous-domaine par cette adresse
   * notification@yoursubdomain.yourdomain.com si vous disposez d’un domaine d’étiquette blanche ; remplacer le nom du sous-domaine par le nom de domaine dans cette adresse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
