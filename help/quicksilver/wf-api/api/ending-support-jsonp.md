---
content-type: api
navigation-topic: api-navigation-topic
title: Fin de la prise en charge de JSONP
description: Fin de la prise en charge de JSONP
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 100%

---

# Fin de la prise en charge de JSONP

JSONP (JavaScript with Padding) étant une ancienne norme avec des vulnérabilités de sécurité connues, Adobe Workfront ne prendra plus en charge JSONP à compter de novembre 2018. Cette décision s’inscrit dans le cadre de notre initiative plus large de modernisation de la plateforme Workfront.

JSONP est une norme qui permet d’effectuer des requêtes interorigines ou intersites. De nombreuse personnes clientes et partenaires Workfront utilisent JSONP pour accéder à Workfront à partir d’un système sur leur propre domaine dans le cadre d’une intégration. JSONP permet le traitement des requêtes provenant de domaines autres que Workfront par l’application Workfront.

Si vous utilisez JSONP dans le cadre de l’une de vos intégrations Workfront, vous devez mettre à jour votre intégration afin d’utiliser la norme CORS (Cross-Origin Resource Sharing). Cette mise à jour requiert que vous procédiez comme suit :

1. Envoyez une demande à l’équipe de support de Workfront afin que tous les domaines utilisés pour effectuer des demandes d’origine croisée vers notre liste autorisée soient envoyés.

   Pour que vos domaines soient ajoutés à la liste autorisée pour CORS, contactez l’assistance clientèle de Workfront au numéro 844-306-HELP(4357) ou en envoyant un ticket d’assistance en ligne.

   >[!NOTE]
   >
   >L’ajout de domaines à la liste autorisée pour CORS n’est pris en charge que pour les clientes et clients qui utilisaient JSONP avant le 1er août 2018.


1. Apportez des modifications au code d’intégration pour utiliser CORS.
