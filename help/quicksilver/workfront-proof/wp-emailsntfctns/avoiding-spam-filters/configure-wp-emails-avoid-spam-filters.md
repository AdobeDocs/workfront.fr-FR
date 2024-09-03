---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configurer les e-mails  [!DNL Workfront Proof]  pour éviter les filtres anti-spam
description: '« Le filtre anti-spam de votre client de messagerie a un objectif important : vous protéger contre les spams embêtants et potentiellement malveillants. Cependant, si vous ne disposez pas des paramètres appropriés dans le filtre anti-spam, cela peut vous empêcher de voir les e-mails  [!DNL Workfront Proof]  importants suivants : notifications d’épreuve par e-mail, newsletters, et communications spéciales. »'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 100%

---

# Configurer les e-mails [!DNL Workfront Proof] pour éviter les filtres anti-spam

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Le filtre anti-spam de votre client de messagerie a un objectif important : vous protéger contre les spams embêtants et potentiellement malveillants. Cependant, si vous ne disposez pas des paramètres appropriés dans le filtre anti-spam, cela peut vous empêcher de voir les e-mails [!DNL Workfront Proof] importants suivants : notifications d’épreuve par e-mail, newsletters et communications spéciales.

Pour vous assurer que vos e-mails [!DNL Workfront Proof] sont toujours acheminés vers votre boîte de réception au lieu de votre dossier Spam, vous devez ajouter les éléments suivants à la liste autorisée :

* Serveur de messagerie [!DNL Workfront Proof] : **[!DNL mx.proofhq.com]**
* Adresses e-mail [!DNL Workfront Proof] « [!UICONTROL De] » (par exemple, notification@proofhq.com)

Pour plus d’informations sur les URL à ajouter à votre liste autorisée, voir [Configurer la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) dans l’article [Configurer la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Adresses e-mail [!DNL Workfront Proof] « [!UICONTROL De] »

Selon votre type de client de messagerie, vous devrez peut-être ajouter des adresses e-mail [!DNL Workfront Proof] « [!UICONTROL De] » à l’un des éléments suivants afin d’empêcher le filtre anti-spam d’acheminer vos e-mails vers votre dossier Spam à l’avenir :

* Votre liste de contacts
* Votre liste d’[!UICONTROL Expéditeurs sécurisés]
* Un filtre que vous créez pour envoyer des e-mails depuis ces adresses vers votre boîte de réception

Vous devrez peut-être également supprimer les e-mails [!DNL Workfront Proof] de votre dossier Spam et vérifier si l’une des adresses « [!UICONTROL De] » figure sur la liste des adresses bloquées. Cette page d’aide répertorie les adresses [!DNL Workfront Proof] « [!UICONTROL De] » et indique comment les ajouter au filtre anti-spam dans les clients de messagerie suivants :

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Si vous avez des questions sur une procédure décrite ici, veuillez consulter l’aide de votre client de messagerie.

Pour plus d’informations, voir [Configurer des paramètres anti-spam pour les clients de messagerie courants](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## Adresses e-mail [!DNL Workfront Proof] « [!UICONTROL De] » à copier

Pour vous assurer que vos e-mails [!DNL Workfront Proof] atteignent votre boîte de réception, vous devrez ajouter deux adresses e-mail [!DNL Workfront Proof] séparément au filtre anti-spam de votre client de messagerie :

* L’adresse générale du support, [!DNL support@proofhq.com], à partir de laquelle [!DNL Workfront Proof] envoie de nombreuses communications par e-mail.
* L’adresse de notification à partir de laquelle [!DNL Workfront Proof] envoie des e-mails de notification d’épreuve au créateur ou à la créatrice d’épreuves et aux personnes effectuant la révision avec des liens vers l’épreuve. Il peut s’agir d’une adresse générale, notification@support.proofhq.com ou d’une adresse spécifique si vous disposez d’un sous-domaine personnalisé ou d’un domaine en marque blanche.

Pour ajouter des adresses [!DNL Workfront Proof] « [!UICONTROL De] » au filtre de votre client de messagerie :

1. Copiez l’adresse e-mail générale du support [!DNL Workfront Proof] « [!UICONTROL De] » (support@proofhq.com) et collez-la dans le champ indiqué pour votre client de messagerie.
1. Copiez l’une des adresses e-mail [!DNL Workfront Proof] suivantes « [!UICONTROL De] » et collez-les SÉPARÉMENT dans le champ indiqué pour votre client de messagerie :

   * notification@support.proofhq.com si vous n’avez PAS de sous-domaine personnalisé ou de domaine en marque blanche.
   * notification@yoursubdomain.proofhq.com si vous disposez d’un sous-domaine personnalisé. Remplacez le nom du sous-domaine de cette adresse par le vôtre.
   * notification@yoursubdomain.yourdomain.com si vous disposez d’un domaine en marque blanche. Remplacez le nom et le nom du sous-domaine dans cette adresse par les vôtres.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
