---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Résolution des problèmes d’intégration d’Adobe Experience Manager
description: "Problème : les ressources ne sont pas enregistrées dans Adobe Experience Manager"
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: a73ebfe8c735eb9e103b01a201a8f71d6ab7bda2
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# Résolution des problèmes d’intégration d’Adobe Experience Manager

## Problème : les ressources ne sont pas enregistrées dans Adobe Experience Manager

Lorsqu’un utilisateur sélectionne une ressource ou un dossier à exporter vers Experience Manager Assets et clique sur Sélectionner, la fenêtre du sélecteur se ferme, mais les ressources ne sont pas enregistrées dans Experience Manager Assets. Il n’y a aucune indication dans Workfront que les ressources n’ont pas été enregistrées dans Experience Manager Assets.

### Cause

Cela peut se produire en raison de la liste autorisée dans Adobe Cloud Manager. Si la liste autorisée Adobe Cloud Manager d’une organisation est vide, les adresses IP ne sont pas limitées et Workfront peut accéder aux dossiers et ressources de l’organisation dans Adobe Experience Manager. Toutefois, si une seule adresse IP est ajoutée à la liste autorisée Cloud Manager, la liste autorisée suppose que toute adresse IP qui ne figure pas dans la liste n’est pas autorisée. Par conséquent, si la liste autorisée Cloud Manager inclut des adresses IP, les adresses IP Workfront doivent également être ajoutées à la liste autorisée pour permettre à Workfront d’envoyer des ressources vers Experience Manager Assets.

### Solution :

Ajoutez les adresses IP Workfront à la liste autorisée Adobe Cloud Manager.

* Pour plus d’informations sur l’ajout d’adresses IP à Adobe Cloud Manager, voir [Présentation des Listes autorisées IP](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) dans la documentation Adobe Experience Manager.
* Pour obtenir la liste des adresses IP Workfront à ajouter à la liste autorisée, voir [Configuration de votre pare-feu](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).


