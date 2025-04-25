---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Résoudre les problèmes d’intégration d’Adobe Experience Manager
description: 'Problème : les ressources ne sont pas enregistrées dans Adobe Experience Manager'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 99%

---

# Résoudre les problèmes d’intégration d’Adobe Experience Manager

## Problème : les ressources ne sont pas enregistrées dans Adobe Experience Manager

Lorsqu’un utilisateur ou une utilisatrice sélectionne une ressource ou un dossier à exporter vers Experience Manager Assets et clique sur Sélectionner, la fenêtre du sélecteur se ferme, mais les ressources ne sont pas enregistrées dans Experience Manager Assets. Il n’y a aucune indication dans Workfront que les ressources n’ont pas été enregistrées dans Experience Manager Assets.

### Cause

Cela peut se produire en raison de la liste autorisée dans Adobe Cloud Manager. Si la liste autorisée Adobe Cloud Manager d’une organisation est vide, les adresses IP ne sont pas limitées et Workfront peut accéder aux dossiers et ressources de l’organisation dans Adobe Experience Manager. Toutefois, si même une seule adresse IP est ajoutée à la liste autorisée Cloud Manager, la liste autorisée suppose que toute adresse IP qui ne figure pas dans la liste n’est pas autorisée. Par conséquent, si la liste autorisée Cloud Manager inclut des adresses IP, les adresses IP Workfront doivent également être ajoutées à la liste autorisée pour permettre à Workfront d’envoyer des ressources vers Experience Manager Assets.

### Solution :

Ajoutez les adresses IP Workfront à la liste autorisée Adobe Cloud Manager.

* Pour plus d’informations sur l’ajout d’adresses IP à Adobe Cloud Manager, voir [Présentation des listes autorisées d’adresses IP](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction) dans la documentation d’Adobe Experience Manager.
* Pour obtenir la liste des adresses IP Workfront à ajouter à la liste autorisée, voir [Configurer votre pare-feu](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
