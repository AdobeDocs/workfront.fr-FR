---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configuration de la liste autorisée de votre pare-feu
description: Si votre pare-feu ou serveur de messagerie est configuré pour autoriser l’accès à certains fournisseurs uniquement, vous devez ajouter certaines adresses IP à sa liste autorisée. Cela ouvre la communication entre votre environnement et les serveurs Adobe Workfront et permet à vos utilisateurs d’envoyer des messages depuis Workfront et d’utiliser la fonction SSO avec Active Directory ou LDAP.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 8a8a36732800d0f48026b616cc16e4ff30e0ad41
workflow-type: tm+mt
source-wordcount: '1598'
ht-degree: 0%

---

# Configuration de la liste autorisée de votre pare-feu

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées au Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, vous devez effectuer cette action via Adobe Admin Console.
>
>Pour configurer votre liste autorisée si votre organisation a été intégrée à Adobe Admin Console, voir [Domaines autorisés pour les applications et services d’Adobe](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Admin Console, voir [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>La manière dont une organisation configure sa liste autorisée est propre à chaque organisation. Collaborez avec votre équipe informatique pour identifier la procédure de votre entreprise et mettre en oeuvre ces ajouts.

Si votre pare-feu ou serveur de messagerie est configuré pour autoriser l’accès à certains fournisseurs uniquement, vous devez ajouter certaines adresses IP à sa liste autorisée. Cela permet la communication entre votre environnement et les serveurs Adobe Workfront et permet les processus suivants :

* Envoi de messages depuis l’application Workfront

  >[!NOTE]
  >
  >Cette option n’est pas disponible si l’instance Workfront de votre entreprise est activée avec Adobe IMS. Si vous avez besoin d’informations supplémentaires, contactez votre administrateur réseau ou informatique.

* Utilisation des webhooks de document lors de la configuration des intégrations de documents personnalisées
* Utilisation d’abonnements à des événements Workfront

  Pour plus d’informations, voir [API d’abonnement à un événement](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

Vous devez également ouvrir certains ports pour que les emails soient cryptés lors de leur diffusion.

## listes autorisées Workfront utilisables

Si votre entreprise dispose du plan Enterprise, vous pouvez également configurer deux listes autorisées Workfront :

* **Liste autorisée de courrier électronique**: vous permet de contrôler où les utilisateurs peuvent envoyer par e-mail des données stockées dans Workfront. Pour plus d’informations, voir [Configuration de votre liste autorisée de messagerie](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **LISTE AUTORISÉE IP**: limite l’accès à Workfront à 45 adresses IP ou plages d’adresses que vous spécifiez, fournissant ainsi une couche de sécurité supplémentaire pour l’application Workfront. Pour plus d’informations, voir [Limitation de l’accès à Adobe Workfront par adresse IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Localisation de la grappe Workfront

Les adresses IP que vous devez ajouter à votre liste autorisée sur votre pare-feu dépendent de la grappe sur laquelle s’exécute votre environnement de production.

Pour localiser la grappe de votre entreprise :

1. En tant qu’administrateur Workfront, cliquez sur le bouton **Menu Principal** icon ![Menu Principal](assets/main-menu-icon.png), puis cliquez sur **Configuration**.
1. Dans la navigation de gauche, cliquez sur **Système**, puis sélectionnez **Informations sur le client**.
1. Recherchez la variable **Configuration en grappe** dans le coin supérieur droit de la page. La grappe de votre entreprise est répertoriée ici.

   CL01 fait référence au cluster 1, CL02 est le cluster 2, etc.

Pour plus d’informations, voir la section [Affichage de la grappe et du plan Workfront de votre entreprise](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) dans l’article [Présentation du pare-feu](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## Adresses IP à ajouter à la liste autorisée

>[!IMPORTANT]
>
>Certaines intégrations Workfront ne fonctionnent pas lorsque la liste autorisée est activée, car elles ne peuvent pas être configurées avec une adresse IP statique. Pour utiliser les intégrations suivantes, vous devez désactiver la liste autorisée.
>
>* Workfront pour G Suite
>* Workfront pour Outlook
>* Workfront pour Salesforce

* [Adresses IP pour permettre les clusters 1, 2, 3, 5, 7, 8 et 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [Adresses IP à autoriser pour la grappe 4](#ip-addresses-to-allow-for-cluster-4)
* [Adresses IP à autoriser pour la grappe 6](#ip-addresses-to-allow-for-cluster-6)
* [Adresses IP pour permettre un test de lecteur](#IP%20Addre2)
* [Adresses IP à autoriser lors de l’implémentation des abonnements aux événements](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Adresses IP pour permettre une authentification améliorée](#ip-addresses-to-allow-for-enhanced-authentication)
* [Adresses IP à ajouter pour accéder à Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Adresses IP à ajouter pour l’utilisation de Workfront pour Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [URL à ajouter pour toutes les grappes Workfront](#urls-to-add-for-all-clusters-workfront)

### Adresses IP pour permettre les clusters 1, 2, 3, 5, 7, 8 et 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Si votre environnement de production se trouve sur les clusters 1, 2, 3, 5 ou 7, vous devez autoriser les adresses IP suivantes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pour la connexion unique, les webhooks de documents ou d’autres fonctionnalités</td> 
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
   <td role="rowheader">Pour recevoir un courrier électronique de l’application Workfront</td> 
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
    </ul> <p>Pour plus d’informations sur les adresses IP suivantes, voir <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md" class="MCXref xref">Nouvelles adresses IP pour les emails Adobe Workfront avec la version 21.1</a></p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Adresses IP à autoriser pour la grappe 4 {#ip-addresses-to-allow-for-cluster-4}

Si votre environnement de production se trouve sur la grappe 4, ajoutez les adresses IP suivantes pour la connexion unique, les intégrations webhook de document et pour recevoir des courriers électroniques de l’application Workfront :

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69,169. 230,232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34 252 250 191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32

Pour plus d’informations sur les adresses IP suivantes, voir [Nouvelles adresses IP pour les emails Adobe Workfront avec la version 21.1](../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)

* 23.251.239.98
* 23.251.239.99

### Adresses IP à autoriser pour la grappe 6 {#ip-addresses-to-allow-for-cluster-6}

Si votre environnement de production se trouve sur la grappe 6, ajoutez les adresses IP suivantes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pour recevoir un courrier électronique de l’application Workfront</td> 
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
   <td role="rowheader">Pour utiliser le service de messagerie AWS</td> 
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
 </tbody> 
</table>

### Adresses IP pour permettre un test de lecteur

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pour recevoir un courrier électronique de l’application Workfront lors de l’utilisation d’un test de lecteur</td> 
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
     <li> <p>69.42.126.188 :</p> <p>Cette adresse doit également être ajoutée à votre liste autorisée pour que vos utilisateurs puissent recevoir des courriers électroniques de Workfront.</p> </li> 
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
   <td role="rowheader"> Pour les clients en Europe</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34 252 250 191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pour les clients situés à des endroits autres que l’Europe</td> 
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

### Adresses IP pour permettre une authentification améliorée {#ip-addresses-to-allow-for-enhanced-authentication}

Ajoutez les adresses IP suivantes pour utiliser une authentification améliorée pour l’aperçu ou la production.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Si votre environnement se trouve sur les clusters 1, 2, 3, 5, 7, 8 ou 9</td> 
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
     <li>18 232 225 224</li> 
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
   <td role="rowheader">Si votre environnement se trouve sur la grappe 4</td> 
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

### Adresses IP à ajouter pour accéder à Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Ajoutez les adresses IP suivantes à votre liste autorisée pour permettre à Workfront Fusion d’accéder à votre système.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] sur la grappe Microsoft Azure</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

En outre, si votre entreprise utilise le filtrage réseau sortant, ajoutez le domaine suivant à votre liste autorisée pour permettre à votre système d’accéder à Workfront Fusion.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] sur la grappe Microsoft Azure</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Le filtrage de réseau sortant est rare. Vérifiez auprès de votre administrateur réseau si vous devez mettre à jour votre liste autorisée pour l’adapter.

### Adresses IP à ajouter pour l’utilisation de Workfront pour Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Ajoutez les adresses IP suivantes à votre liste autorisée pour utiliser l’intégration Workfront for Jira.

Le domaine jira.workfront.com doit également être accessible à partir des serveurs de votre entreprise. Ce domaine est requis, car il sert de middleware entre Workfront et Jira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Pour les clients en Europe</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34 252 250 191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pour les clients situés à des endroits autres que l’Europe</td> 
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

## Domaines à ajouter pour l’accès à Workfront

Si votre entreprise utilise le filtrage réseau sortant, ajoutez les domaines suivants à votre liste autorisée pour permettre à votre système d’accéder à Workfront.

>[!NOTE]
>
>Le filtrage de réseau sortant est rare. Vérifiez auprès de votre administrateur réseau si vous devez mettre à jour votre liste autorisée pour l’adapter.

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

## URL à ajouter pour toutes les grappes Workfront {#urls-to-add-for-all-clusters-workfront}

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
   <td role="rowheader">Pour permettre à Workfront Proof d’accéder à Workfront sur une grappe, ajoutez-les à tous les environnements.</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Obligatoire pour afficher les bons à tirer dans Workfront</li> 
     <li>*.proofhq.com - Obligatoire pour afficher les bons à tirer dans Workfront Proof</li> 
     <li>*.proofhq.eu - Obligatoire pour afficher les bons à tirer dans Workfront Proof</li> 
    </ul> <p><b>REMARQUE</b>:  <p>L’ajout d’adresses IP à votre liste autorisée pour Workfront Proof n’est pas pris en charge. Ils ont été dynamiques une fois Workfront déplacé vers AWS. Nous vous recommandons plutôt d’autoriser les domaines Workfront Proof uniquement.</p> <p>En cas de problème lors de l’ajout de ces domaines à votre liste autorisée et si vous avez besoin d’une adresse IP à la place, contactez le service clientèle de Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Adresses IP et URL à ajouter pour l’accès à Workfront Proof

Vous devez ajouter les adresses IP suivantes à votre liste autorisée pour pouvoir utiliser différentes fonctions.

* [Pour les rappels et les BAT de capture web](#for-callbacks-and-webcapture-proofs)
* [Pour l’email sortant](#for-outgoing-email)

### Pour les rappels et les BAT de capture web {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (clusters 1, 2, 3, 5 et 7)</td> 
   <td> 
    <ul> 
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
   <td role="rowheader">Prod-EU (Grappe 4)</td> 
   <td> 
    <ul> 
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34 252 250 191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>REMARQUE</b>: les options du serveur DNS ne sont plus prises en charge.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Pour l’email sortant {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (clusters 1, 2, 3, 5 et 7)</p> </td> 
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
   <td role="rowheader">Prod-EU (Grappe 4)</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Ports à ouvrir pour de meilleures performances Workfront Proof

Ouvrez les ports suivants si vous rencontrez des problèmes de chargement des bons à tirer ou si vous ne travaillez pas dans Workfront Proof :

* 5671
* 5672
* 15671

## Ports à ouvrir pour les emails chiffrés

Les emails de l’application Workfront sont cryptés à l’aide des ports 465 et 587. Si votre serveur de messagerie ne prend pas en charge les emails chiffrés, les emails sont diffusés sans cryptage à l’aide du port 25.

## Notifications par e-mail de l’assistance Workfront

Si vous ne recevez pas de courriers électroniques du support Workfront, veillez à ajouter les adresses IP et domaines Salesforce dont vous avez besoin. Pour plus d’informations, reportez-vous à l’article d’aide de Salesforce sur les adresses IP et domaines Salesforce à autoriser.
