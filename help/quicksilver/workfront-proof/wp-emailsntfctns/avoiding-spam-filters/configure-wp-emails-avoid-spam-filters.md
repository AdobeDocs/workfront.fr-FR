---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configuration des  [!DNL Workfront Proof] emails pour éviter les filtres de spam
description: "Le filtre de spam de votre client de messagerie a un objectif important : vous protéger contre les emails de spam embêtants et potentiellement malveillants. Cependant, si vous ne disposez pas des paramètres corrects dans le filtre de spam, cela peut vous empêcher de voir les  [!DNL Workfront Proof] emails suivants : notifications de BAT, newsletters et communications spéciales."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Configuration des [!DNL Workfront Proof] emails pour éviter les filtres de spam

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Le filtre de spam de votre client de messagerie a un objectif important : vous protéger contre les emails de spam embêtants et potentiellement malveillants. Cependant, si vous ne disposez pas des paramètres appropriés dans le filtre de spam, cela peut vous empêcher de voir les [!DNL Workfront Proof] emails importants suivants : notifications de BAT, newsletters et communications spéciales.

Pour vous assurer que vos [!DNL Workfront Proof] emails sont toujours routés vers votre boîte de réception au lieu de votre dossier de messages indésirables, vous devez ajouter les éléments suivants à la liste autorisée :

* [!DNL Workfront Proof] serveur de messagerie : **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] Adresses électroniques &quot;[!UICONTROL de]&quot; (par exemple, notification@proofhq.com)

Pour plus d’informations sur les URL à ajouter à votre liste autorisée, voir [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) dans l’article [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] Adresses email &quot;[!UICONTROL from]&quot;

Selon votre type de client de messagerie, vous devrez peut-être ajouter [!DNL Workfront Proof] &quot;[!UICONTROL depuis]&quot; adresses électroniques à l’une des adresses suivantes pour empêcher le filtre de messages indésirables de router vos emails vers votre dossier de messages indésirables à l’avenir :

* Votre liste de contacts
* Votre liste [!UICONTROL Expéditeurs approuvés]
* Un filtre que vous créez pour envoyer des emails depuis ces adresses vers votre boîte de réception

Vous devrez peut-être également supprimer tous les emails [!DNL Workfront Proof] de votre dossier de messages indésirables et vérifier si l’une des adresses &quot;[!UICONTROL de]&quot; se trouve sur la liste des adresses bloquées. Cette page d’aide répertorie les adresses &quot;[!UICONTROL de]&quot; [!DNL Workfront Proof] et indique comment les ajouter au filtre de messages indésirables dans les clients de messagerie suivants :

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Si vous avez des questions sur une procédure décrite ici, veuillez consulter l’aide de votre client de messagerie.

Pour plus d’informations, voir [Configuration des paramètres de spam pour les clients de messagerie courants](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## Les adresses électroniques [!DNL Workfront Proof] &quot;[!UICONTROL de]&quot; à copier

Pour vous assurer que vos [!DNL Workfront Proof] emails atteignent votre boîte de réception, vous devez ajouter deux [!DNL Workfront Proof] adresses électroniques séparément au filtre de messages indésirables de votre client de messagerie :

* L’adresse d’assistance générale, [!DNL support@proofhq.com], à partir de laquelle [!DNL Workfront Proof] envoie de nombreuses communications par courrier électronique.
* Une adresse de notification à partir de laquelle [!DNL Workfront Proof] envoie des emails de notification de BAT au créateur du BAT et aux réviseurs avec des liens vers le BAT. Il peut s’agir d’une adresse générale, notification@support.proofhq.com ou d’une adresse spécifique si vous disposez d’un sous-domaine personnalisé ou d’un domaine d’étiquette blanche.

Pour ajouter [!DNL Workfront Proof] &quot;[!UICONTROL depuis]&quot; adresses au filtre de votre client de messagerie :

1. Copiez l&#39;adresse email générale du [!DNL Workfront Proof] support &quot;[!UICONTROL de]&quot; (support@proofhq.com) et collez-la dans le champ indiqué pour votre client de messagerie.
1. Copiez l’une des adresses électroniques &quot;[!UICONTROL de ]&quot; suivantes et collez-la SÉPARÉMENT dans le champ indiqué pour votre client de messagerie :[!DNL Workfront Proof]

   * notification@support.proofhq.com si vous n’avez PAS de sous-domaine personnalisé ou de domaine d’étiquette blanche
   * notification@yoursubdomain.proofhq.com si vous disposez d’un sous-domaine personnalisé ; remplacez le nom de votre sous-domaine par cette adresse
   * notification@yoursubdomain.yourdomain.com si vous disposez d’un domaine de libellé blanc ; remplacez le nom et le nom du sous-domaine par celui de votre adresse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
