---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configuration de la Place sur la liste autorisée de votre pare-feu
description: Si votre pare-feu ou serveur de messagerie est configuré pour accorder l’accès uniquement à certains fournisseurs, vous devez ajouter certaines adresses IP à sa liste autorisée. Cette action ouvre la communication entre votre environnement et les serveurs Adobe Workfront et permet à vos utilisateurs et à vos utilisatrices d’envoyer des messages à partir de Workfront et d’utiliser la fonction SSO avec Active Directory ou LDAP.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 3c680b39685e650dd442adbb49e4091d558d1410
workflow-type: tm+mt
source-wordcount: '1603'
ht-degree: 89%

---

# Configurer la liste autorisée de votre pare-feu

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>La procédure décrite sur cette page ne s’applique qu’aux entreprise qui n’ont pas encore été intégrées à l’Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, vous devez effectuer cette action via Adobe Admin Console.
>
>Pour configurer votre liste autorisée si votre organisation a été intégrée à Adobe Admin Console, consultez la section [Domaines autorisés pour les applications et services d’Adobe](https://helpx.adobe.com/fr/enterprise/kb/network-endpoints.html).
>
>Pour obtenir une liste des procédures qui diffèrent selon que votre organisation a été intégrée ou non à Adobe Admin Console, consultez la section [Différences d’administration en fonction de la plateforme (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>Chaque organisation a sa propre méthode pour définir sa liste autorisée. Collaborez avec votre équipe informatique afin de clarifier la démarche de votre entreprise et réaliser ces intégrations.

Si votre pare-feu ou serveur de messagerie est configuré pour accorder l’accès uniquement à certains fournisseurs, vous devez ajouter certaines adresses IP à sa liste autorisée. Cette configuration facilite les échanges entre votre système et les serveurs Adobe Workfront, permettant ainsi les opérations suivantes :

* Envoyer des messages à partir de l’application Workfront

  >[!NOTE]
  >
  >Cette option n’est pas disponible si l’instance Workfront de votre organisation repose sur Adobe IMS. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

* Utiliser des webhooks de documents lors de la configuration d’intégrations personnalisées de documents
* Utiliser des abonnements à des événements Workfront

  Pour plus d’informations, consultez la section [API des abonnements aux événements](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

Vous devez également ouvrir certains ports pour que les e-mails soient chiffrés lors de leur diffusion.

## Listes autorisées Workfront utilisables

Si votre entreprise dispose de la formule Entreprise, vous pouvez également configurer deux listes autorisées Workfront :

* **Liste autorisée d’e-mails** : vous permet de contrôler où les utilisateurs et les utilisatrices peuvent envoyer par e-mail des données stockées dans Workfront. Pour plus d’informations, consultez la section [Configurer votre liste autorisée d’e-mails](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **Liste autorisée d’adresses IP** : l’accès à Workfront est limité à 75 adresses IP ou plages d’adresses que vous spécifiez, fournissant ainsi une couche de sécurité supplémentaire pour l’application Workfront. Pour plus d’informations, consultez la section [Limiter l’accès à Adobe Workfront par adresse IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Localiser votre cluster Workfront

Les adresses IP que vous devez ajouter à votre liste autorisée sur votre pare-feu dépendent du cluster sur lequel s’exécute votre environnement de production.

Pour localiser le cluster de votre entreprise, procédez comme suit :

{{step-1-to-setup}}

1. Dans la navigation de gauche, cliquez sur **Système**, puis sélectionnez **Infos client**.
1. Localisez le champ **Configuration du cluster** dans le coin supérieur droit de la page. Le cluster de votre entreprise est répertorié ici.

   CL01 fait référence au cluster 1, CL02 au cluster 2, etc.

Pour plus d’informations, consultez la section [Afficher le cluster et la formule Workfront de votre organisation](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) dans l’article [Vue d’ensemble du pare-feu](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## Adresses IP à ajouter à la liste autorisée

>[!IMPORTANT]
>
>Certaines intégrations Workfront ne fonctionnent pas lorsque la liste autorisée est activée, car elles ne peuvent pas être configurées avec une adresse IP statique. Pour utiliser les intégrations suivantes, vous devez désactiver la liste autorisée.
>
>* Workfront pour Microsoft Outlook

* [Adresses IP à autoriser pour les clusters 1, 2, 3, 5, 7, 8 et 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [Adresses IP à autoriser pour le cluster 4](#ip-addresses-to-allow-for-cluster-4)
* [Adresses IP à autoriser pour le cluster 6](#ip-addresses-to-allow-for-cluster-6)
* [Adresses IP à autoriser pour le cluster 10](#ip-addresses-to-allow-for-cluster-10)
* [Adresses IP à autoriser pour un lecteur de test](#IP%20Addre2)
* [Adresses IP à autoriser lors de l’implémentation des abonnements aux événements](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Adresses IP à ajouter pour accéder à Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Adresses IP à ajouter pour utiliser Workfront pour Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [URL à ajouter pour tous les cluster Workfront](#urls-to-add-for-all-clusters-workfront)

### Adresses IP à autoriser pour les clusters 1, 2, 3, 5, 7, 8 et 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Si votre environnement de production se trouve sur le cluster 1, 2, 3, 5, 7, 8 ou 9, vous devez autoriser les adresses IP suivantes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pour l’authentification unique (SSO), les webhooks de documents ou d’autres fonctionnalités</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.36.154.34</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>54.203.255.135/32</li> 
     <li>35.155.2.51/32</li> 
     <li>52.34.192.77/32</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pour recevoir un e-mail de l’application Workfront</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li>
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
     <li>206.55.149.212</li>
     <li>206.55.149.214</li>
     <li>206.55.149.215</li>
     <li>206.55.149.213</li>
     <li>206.55.149.211</li>
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Adresses IP à autoriser pour la cluster 4 {#ip-addresses-to-allow-for-cluster-4}

Si votre environnement de production se trouve sur le cluster 4, ajoutez les adresses IP suivantes pour l’authentification unique, les intégrations de webhook de document et pour recevoir les e-mails de l’application Workfront :

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69.169. 230,232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32
* 23.251.239.98
* 23.251.239.99
* 24.110.76.224
* 24.110.76.223

### Adresses IP à autoriser pour le cluster 6 {#ip-addresses-to-allow-for-cluster-6}

Si votre environnement de production se trouve sur le cluster 6, ajoutez les adresses IP suivantes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pour recevoir les e-mails de l’application Workfront</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227.65</li> 
     <li>34.94.227.66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    <li>206.55.149.212</li>
   <li>206.55.149.214</li>
   <li>206.55.149.215</li>
   <li>206.55.149.213</li>
   <li>206.55.149.211</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pour utiliser le service de messagerie</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65 </li> 
    </ul> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">Pour utiliser le service de messagerie Mailgun</td> 
   <td> 
    <ul> 
     <li>143.55.228.56 </li> 
     <li>209.61.151.229</li> 
     <li>69.72.43.7</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Adresses IP à autoriser pour le cluster 10

* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

### Adresses IP à autoriser pour le cluster 11

Pour recevoir un e-mail de l’application Workfront sur le cluster 11, ajoutez les adresses IP suivantes :

* 24.110.76.224
* 24.110.76.223

### Adresses IP pour autoriser un lecteur de test

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pour recevoir un e-mail de l’application Workfront lors de l’utilisation d’un lecteur de test</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pour les intégrations SSO et webhook de document lors de l’utilisation d’un lecteur de test</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188 :</p> <p>Cette adresse doit également être ajoutée à votre liste autorisée pour que vos utilisateurs et utilisatrices puissent recevoir des e-mails de Workfront.</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Adresses IP à autoriser lors de l’implémentation des abonnements aux événements  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

Pour tous les environnements, ajoutez les adresses IP suivantes afin de recevoir les payloads des abonnements aux événements Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Pour la clientèle européenne</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pour les clientes et clients situés ailleurs qu’en Europe</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Adresses IP à ajouter pour accéder à Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Ajoutez les adresses IP suivantes à votre liste autorisée pour permettre à Workfront Fusion d’accéder à votre système.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Centre de données de l’UE Adobe Workfront</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Centre de données des États-Unis Adobe Workfront</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] sur le cluster Microsoft Azure</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

De même, si votre entreprise utilise le filtrage de réseau sortant, ajoutez le domaine suivant à votre place sur la liste autorisée pour permettre à votre système d’accéder à Workfront Fusion. Ces URL sont utilisées pour les Webhooks dans Fusion.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Centre de données de l’UE Adobe Workfront</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Centre de données des États-Unis Adobe Workfront</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] sur le cluster Microsoft Azure</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Le filtrage de réseau sortant est rare. Vérifiez auprès de votre équipe d’administration réseau si vous devez mettre à jour votre liste autorisée pour l’adapter.

### Adresses IP à ajouter pour l’utilisation de Workfront pour Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Ajoutez les adresses IP suivantes à votre liste autorisée pour utiliser l’intégration Workfront pour Jira.

Le domaine jira.workfront.com doit également être accessible à partir des serveurs de votre entreprise. Ce domaine est requis, car il sert de middleware entre Workfront et Jira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Pour la clientèle européenne</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pour les clientes et clients situés ailleurs qu’en Europe</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Domaines à ajouter pour accéder à Workfront

Si votre entreprise utilise le filtrage de réseau sortant, ajoutez les domaines suivants à votre liste autorisée pour permettre à votre système d’accéder à Workfront.

>[!NOTE]
>
>Le filtrage de réseau sortant est rare. Vérifiez auprès de votre équipe d’administration réseau si vous devez mettre à jour votre liste autorisée pour l’adapter.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* fonts.gstatic.com
* dpm.demdex.net
* storage.googleapis.com
* snippet.maze.co
* *.aptrinsic.com
* *.static.workfront.com


  Il s’agit d’un domaine statique qui englobe tous les domaines suivants. Vous pouvez ajouter des domaines individuels si vous préférez :

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com

Si votre organisation utilise l’expérience unifiée Adobe, elle utilise les domaines suivants. Ces domaines sont couverts sous `*.adobe.com`, mais peuvent être ajoutés si vous le souhaitez.

* &lt;votre domaine>.my.workfront.adobe.com
* &lt;votre domaine>.preview.workfront.adobe.com
* &lt;votre domaine>.sb01.workfront.adobe.com
* &lt;votre domaine>.sb02.workfront.adobe.com


Pour Workfront Fusion, ajoutez les domaines suivants :

* Pour les organisations qui ne disposent pas d’une expérience unifiée Adobe :
   * app.workfrontfusion.com (US AWS)
   * app-eu.workfrontfusion.com (EU AWS)
   * app-az.workfrontfusion.com (US Azure)

* Pour l’organisation sur l’expérience unifiée Adobe
(Ces domaines sont couverts sous `*.adobe.com`, mais peuvent être ajoutés si vous le souhaitez.)

   * fusion.adobe.com
   * app-eu.fusion.adobe.com
   * app-az.fusion.adobe.com



## URL à ajouter pour tous les clusters Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pour autoriser l’affichage du contenu d’aide dans votre environnement Workfront</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pour permettre à Workfront Proof d’accéder à Workfront sur n’importe quel cluster, ajoutez les éléments suivants à tous les environnements :</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Obligatoire pour afficher les épreuves dans Workfront</li> 
     <li>*.proofhq.com - Obligatoire pour afficher les épreuves dans Workfront Proof</li> 
     <li>*.proofhq.eu - Obligatoire pour afficher les épreuves dans Workfront Proof</li> 
    </ul> <p><b>NOTE</b> :  <p>Nous ne prenons pas en charge l’ajout d’adresses IP à votre liste autorisée pour Workfront Proof. Elles sont devenues dynamiques depuis que Workfront a migré vers AWS. Nous vous recommandons plutôt d’autoriser uniquement les domaines de Workfront Proof.</p> <p>En cas de problème lors de l’ajout de ces domaines à votre liste autorisée et si vous avez besoin d’une adresse IP à la place, contactez le service clientèle de Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Adresses IP et URL à ajouter pour accéder à Workfront Proof

Vous devez ajouter les adresses IP suivantes à votre liste autorisée pour pouvoir utiliser différentes fonctions.

* [Pour les rappels et les épreuves de capture web](#for-callbacks-and-webcapture-proofs)
* [Pour les e-mails sortants](#for-outgoing-email)

### Pour les rappels et les épreuves de capture web {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-É.-U. (clusters 1, 2, 3, 5 et 7)</td> 
   <td> 
    <ul> 
    <li>35.84.172.250</li>
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54.184.151.122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (cluster 4)</td> 
   <td> 
    <ul> 
    <li>34.255.252.190</li>
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>NOTE</b> : les options du serveur DNS ne sont plus prises en charge.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pour les e-mails sortants {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-É.-U. (clusters 1, 2, 3, 5 et 7)</p> </td> 
   <td> 
    <ul> 
     <li> 23.251.237.106</li> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (cluster 4)</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Ports à ouvrir pour de meilleures performances de Workfront Proof

Ouvrez les ports suivants si vous rencontrez des problèmes de chargement des épreuves ou si vous ne travaillez pas dans Workfront Proof :

* 5671
* 5672
* 15671

## Ports à ouvrir pour les e-mails chiffrés

Les e-mails de l’application Workfront sont envoyés chiffrés à l’aide des ports 465 et 587. Si votre serveur d’e-mail ne prend pas en charge les e-mails chiffrés, les e-mails sont diffusés sans chiffrement à l’aide du port 25.

## Notifications par e-mail de l’assistance Workfront

Si vous ne recevez pas d’e-mails de l’assistance Workfront, veillez à ajouter les adresses IP et domaines Salesforce dont vous avez besoin. Pour plus d’informations, reportez-vous à l’article d’aide de Salesforce sur les adresses IP et domaines Salesforce à autoriser.
