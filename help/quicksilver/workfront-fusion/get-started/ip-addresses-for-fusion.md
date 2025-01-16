---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adresses IP pour accéder à Adobe Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 3983d811a849c01b3c34b1cd6ee895e5552225a6
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 43%

---

# Adresses IP pour accéder à [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Configuration des adresses IP pour Fusion dans la place sur la liste autorisée de données de votre entreprise](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/set-up-ip-addresses-for-fusion.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une licence [!DNL Adobe Workfront Fusion] en plus d’une [!DNL Adobe Workfront license].

Si votre pare-feu ou serveur de messagerie est configuré pour autoriser l’accès à certains fournisseurs uniquement, vous devez ajouter certaines adresses IP à sa liste autorisée afin d’autoriser une communication ouverte entre votre environnement et [!DNL Adobe Workfront Fusion].

Placer sur la liste autorisée Vous pouvez ajouter tous les domaines et adresses IP Fusion à votre cluster, ou vous pouvez localiser votre cluster Fusion et ajouter uniquement les domaines et adresses IP de ce cluster.

## Ajouter tous les domaines et adresses IP Fusion

Ajoutez les adresses IP suivantes à votre place sur la liste autorisée :

* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 100.20.126.137
* 34.223.32.4
* 52.39.176.220
* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

De même, si votre entreprise utilise le filtrage de réseau sortant, ajoutez le domaine suivant à votre place sur la liste autorisée pour permettre à votre système d’accéder à Workfront Fusion. Ils sont utilisés pour les Webhooks.

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## Ajoutez des adresses IP et des domaines Fusion pour votre cluster uniquement

### Identification de votre centre de données

Les adresses IP varient en fonction de l’emplacement de stockage de vos données.

Si vous accédez à Fusion par le biais d’une URL, vous pouvez examiner l’URL pour localiser votre centre de données.

| URL | Datacenter |
| --- | --- |
| `https://app.workfrontfusion.com/` | centre de données des États-Unis |
| `https://app-eu.workfrontfusion.com/` | centre de données de l&#39;UE |
| `https://app-az.workfrontfusion.com/` | Centre de données Azure |

Si vous accédez à Fusion via experience.adobe.com, vous pouvez vérifier l’onglet réseau dans votre navigateur pour identifier le centre de données.

| URL | Datacenter |
| --- | --- |
| Appels à `https://fusion.adobe.com` | centre de données des États-Unis |
| Appels à `https://eu.fusion.adobe.com` | centre de données de l&#39;UE |
| Appels à `https://az.fusion.adobe.com` | Centre de données Azure |

### Ajouter des adresses IP et des domaines pour votre centre de données

Ajoutez les adresses IP suivantes à votre liste autorisée pour permettre à [!DNL Workfront Fusion] d’accéder à votre système.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Centre de données de l’UE</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Centre de données des États-Unis</p> </td> 
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

En outre, si votre organisation utilise le filtrage réseau sortant, ajoutez le domaine suivant à votre liste autorisée pour permettre à votre système d’accéder à Workfront Fusion.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Centre de données de l’UE</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Centre de données des États-Unis</p> </td> 
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

Pour plus d’informations sur la configuration de la liste autorisée de votre organisation, voir [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
