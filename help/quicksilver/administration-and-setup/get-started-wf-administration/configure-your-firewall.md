---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurer la liste autorisée de votre pare-feu
description: Si votre pare-feu ou serveur de messagerie est configuré pour autoriser l’accès à certains fournisseurs uniquement, vous devez ajouter certaines adresses IP à sa liste autorisée. Cela ouvre la communication entre votre environnement et les serveurs Adobe Workfront et permet à vos utilisateurs et utilisatrices d’envoyer des messages depuis Workfront et d’utiliser la SSO avec Active Directory ou LDAP.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: d85898a74991b2c634d8bd33c81c127321617cf9
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 97%

---

# Configurer la liste autorisée de votre pare-feu

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées à Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, vous devez effectuer cette action via Adobe Admin Console.
>
>Pour configurer votre liste autorisée si votre entreprise a été intégrée à Adobe Admin Console, voir [Domaines à autoriser pour les applications et services d’Adobe](https://helpx.adobe.com/fr/enterprise/kb/network-endpoints.html).
>
>Pour obtenir une liste des procédures différentes selon que votre entreprise a été intégrée ou non à Adobe Admin Console, voir [Différences d’administration en fonction de la plateforme (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>La manière dont une entreprise configure sa liste autorisée est propre à chacune. Collaborez avec votre équipe informatique pour identifier la procédure de votre entreprise et mettre en œuvre ces ajouts.

Si votre pare-feu ou serveur de messagerie est configuré pour autoriser l’accès à certains fournisseurs uniquement, vous devez ajouter certaines adresses IP à sa liste autorisée. Cela ouvre la communication entre votre environnement et les serveurs Adobe Workfront et permet les processus suivants :

* Envoyer des messages à partir de l’application Workfront

  >[!NOTE]
  >
  >Cette option n’est pas disponible si l’instance Workfront de votre entreprise est activée avec Adobe IMS. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

* Utiliser des webhooks de documents lors de la configuration d’intégrations de documents personnalisées
* Utiliser des abonnements aux événements Workfront

  Pour plus d’informations, voir [API d’abonnement aux événements](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

Vous devez également ouvrir certains ports pour que les e-mails soient cryptés lors de leur diffusion.

## Listes autorisées Workfront pouvant être utilisées

Si votre entreprise dispose de la formule Entreprise, vous pouvez également configurer deux listes autorisées Workfront :

* **Liste autorisée d’e-mails** : vous permet de contrôler où les utilisateurs et les utilisatrices peuvent envoyer par e-mail des données stockées dans Workfront. Pour plus d’informations, voir [Configurer votre liste autorisée d’e-mails](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **Liste autorisée d’adresses IP** : limite l’accès à Workfront à 45 adresses IP ou plages d’adresses IP que vous spécifiez, fournissant ainsi une couche de sécurité supplémentaire pour l’application Workfront. Pour plus d’informations, voir [Limiter l’accès à Adobe Workfront en fonction de l’adresse IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Localiser votre cluster Workfront

Les adresses IP que vous devez ajouter à votre liste autorisée sur votre pare-feu dépendent du cluster sur lequel votre environnement de production s’exécute.

Pour localiser le cluster de votre entreprise :

1. En tant qu’administrateur ou administratrice Workfront, cliquez sur l’icône **Menu principal** ![Menu principal](assets/main-menu-icon.png), puis sur **Configuration**.
1. Dans la navigation de gauche, cliquez sur **Système**, puis sélectionnez **Infos client**.
1. Recherchez le champ **Configuration du cluster** dans le coin supérieur droit de la page. Le cluster de votre entreprise est répertorié ici.

   CL01 fait référence au cluster 1, CL02 au cluster 2, etc.

Pour plus d’informations, voir la section [Afficher le cluster et le plan Workfront de votre entreprise](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) dans l’article [Vue d’ensemble du pare-feu](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## Adresses IP à ajouter à la liste autorisée

>[!IMPORTANT]
>
>Certaines intégrations Workfront ne fonctionnent pas lorsque la liste autorisée est activée, car elles ne peuvent pas être configurées avec une adresse IP statique. Pour utiliser les intégrations suivantes, vous devez désactiver la liste autorisée.
>
>* Workfront pour G Suite
>* Workfront pour Outlook
>* Workfront pour Salesforce

* [Adresses IP à autoriser pour les clusters 1, 2, 3, 5, 7, 8 et 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [Adresses IP à autoriser pour le cluster 4](#ip-addresses-to-allow-for-cluster-4)
* [Adresses IP à autoriser pour le cluster 6](#ip-addresses-to-allow-for-cluster-6)
* [Adresses IP à autoriser pour un lecteur de test](#IP%20Addre2)
* [Adresses IP à autoriser lors de l’implémentation d’abonnements aux événements](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Adresses IP à autoriser pour une authentification améliorée](#ip-addresses-to-allow-for-enhanced-authentication)
* [Adresses IP à ajouter pour accéder à Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Adresses IP à ajouter pour utiliser Workfront pour Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [URL à ajouter pour tous les cluster Workfront](#urls-to-add-for-all-clusters-workfront)

### Adresses IP à autoriser pour les clusters 1, 2, 3, 5, 7, 8 et 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Si votre environnement de production se trouve sur le cluster 1, 2, 3, 5 ou 7, vous devez autoriser les adresses IP suivantes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pour la SSO, les webhooks de documents ou d’autres fonctionnalités</td> 
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
    </ul> <p>Pour plus d’informations sur les adresses IP suivantes, voir <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md" class="MCXref xref">Nouvelles adresses IP pour les e-mails Adobe Workfront avec la version 21.1</a>.</p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Adresses IP à autoriser pour le cluster 4 {#ip-addresses-to-allow-for-cluster-4}

Si votre environnement de production se trouve sur le cluster 4, ajoutez les adresses IP suivantes pour la SSO, les intégrations de webhook de document et pour recevoir des e-mails de l’application Workfront :

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

Pour plus d’informations sur les adresses IP suivantes, voir [Nouvelles adresses IP pour les e-mails Adobe Workfront avec la version 21.1](../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)

* 23.251.239.98
* 23.251.239.99

### Adresses IP à autoriser pour le cluster 6 {#ip-addresses-to-allow-for-cluster-6}

Si votre environnement de production se trouve sur le cluster 6, ajoutez les adresses IP suivantes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pour recevoir un e-mail de l’application Workfront</td> 
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
   <td role="rowheader">Pour utiliser le service de messagerie Mailgun</td> 
   <td> 
    <ul> 
     <li>143.55.228.56 </li> 
     <li>209.61.151.229</li> 
     <li>69.72.43.7</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Adresses IP à autoriser pour un lecteur de test

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

### Adresses IP à autoriser lors de l’implémentation des abonnements aux événements  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

Pour tous les environnements, ajoutez les adresses IP suivantes afin de recevoir les payloads des abonnements aux événements Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Pour les clientes et les clients en Europe</td> 
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
   <td role="rowheader">Pour les clientes et les clients situés à des emplacements autres que l’Europe</td> 
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

### Adresses IP à autoriser pour une authentification améliorée {#ip-addresses-to-allow-for-enhanced-authentication}

Ajoutez les adresses IP suivantes pour utiliser une authentification améliorée pour la version préliminaire ou de production.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Si votre environnement se trouve sur le cluster 1, 2, 3, 5, 7, 8 ou 9</td> 
   <td> 
    <ul> 
     <li>35.167.74.121</li> 
     <li>35.166.202.113</li> 
     <li>35.160.3.103</li> 
     <li>54.183.64.135</li> 
     <li>54.67.77.38</li> 
     <li>54.67.15.170</li> 
     <li>54.183.204.205</li> 
     <li>35.171.156.124</li> 
     <li>18.233.90.226</li> 
     <li>3.211.189.167</li> 
     <li>18.232.225.224</li> 
     <li>34.233.19.82</li> 
     <li>52.204.128.250</li> 
     <li>3.132.201.78</li> 
     <li>3.19.44.88</li> 
     <li>3.20.244.231</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Si votre environnement se trouve sur le cluster 4</td> 
   <td> 
    <ul> 
     <li>52.28.56.226</li> 
     <li>52.28.45.240</li> 
     <li>52.16.224.164</li> 
     <li>52.16.193.66</li> 
     <li>34.253.4.94</li> 
     <li>52.50.106.250</li> 
     <li>52.211.56.181</li> 
     <li>52.213.38.246</li> 
     <li>52.213.74.69</li> 
     <li>52.213.216.142</li> 
     <li>35.156.51.163</li> 
     <li>35.157.221.52</li> 
     <li>52.28.184.187</li> 
     <li>52.28.212.16</li> 
     <li>52.29.176.99</li> 
     <li>52.57.230.214</li> 
     <li>54.76.184.103</li> 
     <li>52.210.122.50</li> 
     <li>52.208.95.174</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Adresses IP à ajouter pour accéder à Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Ajoutez les adresses IP suivantes à votre liste autorisée pour permettre à Workfront Fusion d’accéder à votre système.

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

En outre, si votre entreprise utilise le filtrage réseau sortant, ajoutez le domaine suivant à votre liste autorisée pour permettre à votre système d’accéder à Workfront Fusion.

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
>Le filtrage de réseau sortant n’est pas monnaie courante. Vérifiez auprès de l’administration réseau si vous devez mettre à jour votre liste autorisée pour autoriser le trafic sortant.

### Adresses IP à ajouter pour utiliser Workfront pour Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Ajoutez les adresses IP suivantes à votre liste autorisée pour utiliser l’intégration Workfront pour Jira.

Le domaine jira.workfront.com doit également être accessible à partir des serveurs de votre entreprise. Ce domaine est requis, car il sert de middleware entre Workfront et Jira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Pour les clientes et les clients en Europe</td> 
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
   <td role="rowheader">Pour les clientes et les clients situés à des emplacements autres que l’Europe</td> 
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

Si votre entreprise utilise le filtrage réseau sortant, ajoutez les domaines suivants à votre liste autorisée pour permettre à votre système d’accéder à Workfront.

>[!NOTE]
>
>Le filtrage de réseau sortant n’est pas monnaie courante. Vérifiez auprès de l’administration réseau si vous devez mettre à jour votre liste autorisée pour autoriser le trafic sortant.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/
* *.static.workfront.com

  Il s’agit d’un domaine statique qui étend tous les domaines suivants. Vous pouvez ajouter des domaines individuels si vous préférez :

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com


## URL à ajouter pour tous les cluster Workfront {#urls-to-add-for-all-clusters-workfront}

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
   <td role="rowheader">Pour permettre à Workfront Proof d’accéder à Workfront sur un cluster, ajoutez-les à tous les environnements.</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Obligatoire pour afficher les épreuves dans Workfront</li> 
     <li>*.proofhq.com - Obligatoire pour afficher les épreuves dans Workfront Proof</li> 
     <li>*.proofhq.eu - Obligatoire pour afficher les épreuves dans Workfront Proof</li> 
    </ul> <p><b>REMARQUE</b> :  <p>L’ajout d’adresses IP à votre liste autorisée pour Workfront Proof n’est pas pris en charge. Elles sont devenues dynamiques après le déplacement de Workfront déplacé dans AWS. Nous vous recommandons plutôt d’autoriser les domaines Workfront Proof uniquement.</p> <p>En cas de problème lors de l’ajout de ces domaines à votre liste autorisée et si vous avez besoin d’une adresse IP à la place, contactez le service clientèle de Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Adresses IP et URL à ajouter pour accéder à Workfront Proof

Vous devez ajouter les adresses IP suivantes à votre liste autorisée pour pouvoir utiliser différentes fonctions.

* [Pour les rappels et les épreuves de capture web](#for-callbacks-and-webcapture-proofs)
* [Pour les e-mails sortants](#for-outgoing-email)

### Pour les rappels et les épreuves de capture web {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (clusters 1, 2, 3, 5 et 7)</td> 
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
    </ul> <p><b>REMARQUE</b> : les options du serveur DNS ne sont plus prises en charge.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pour les e-mails sortants {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (clusters 1, 2, 3, 5 et 7)</p> </td> 
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

## Ports à ouvrir pour de meilleures performances Workfront Proof

Ouvrez les ports suivants si vous rencontrez des problèmes de chargement des épreuves ou si vous ne travaillez pas dans Workfront Proof :

* 5671
* 5672
* 15671

## Ports à ouvrir pour les e-mails chiffrés

Les e-mails de l’application Workfront sont chiffrés à l’aide des ports 465 et 587. Si votre serveur de messagerie ne prend pas en charge les e-mails chiffrés, les e-mails sont diffusés sans chiffrement à l’aide du port 25.

## Notifications par e-mail du support Workfront

Si vous ne recevez pas d’e-mails du support Workfront, veillez à ajouter les adresses IP et domaines Salesforce dont vous avez besoin. Pour plus d’informations, consultez l’article d’aide de Salesforce sur les adresses IP et domaines Salesforce à autoriser.
