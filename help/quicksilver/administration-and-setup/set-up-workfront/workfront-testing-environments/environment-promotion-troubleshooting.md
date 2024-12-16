---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Résolution des problèmes liés à la promotion de l’environnement
description: Résolution des problèmes courants liés à la promotion de l’environnement.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 830dd573-d954-4ba2-a1d3-d1645b3fbac8
source-git-commit: c3c9a423bd60b26b2605a1b52bd706c9bc6acdec
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Résolution des problèmes liés à la promotion de l’environnement

Cet article décrit comment résoudre les problèmes liés à la promotion de l’environnement.

## Problème : le package de promotion de l’environnement est en cours de blocage ou d’échec.

Si votre package de promotion d’environnement est en cours de blocage ou échoue, essayez les méthodes suivantes :

* Si l’installation d’un package s’arrête après 10 à 15 minutes, ou si l’installation d’un package échoue, réassemblez le package existant ou créez-en un nouveau.

* Si l’installation d’un package échoue, un problème lié à un ou plusieurs objets peut se produire. Vérifiez les messages d’erreur, qui identifient l’objet et peuvent vous aider à identifier le problème. Après avoir résolu le problème avec l’objet , réassemblez le package et retentez l’installation.

* Si vous rencontrez toujours des problèmes avec une installation, essayez de répliquer l’installation dans un autre environnement cible. Restez aussi proche que possible de l’installation d’origine, y compris des objets et des actions d’installation sélectionnés.

* Nous vous recommandons de toujours vérifier le contenu du package une fois qu’il a été assemblé afin de confirmer qu’il contient les objets attendus.


## Problème : la promotion du formulaire personnalisé échoue

Cela peut se produire, car le formulaire personnalisé comprend un champ calculé. Si un champ calculé fait référence à un champ qui n’est pas référencé dans un formulaire personnalisé, le package contenant ce formulaire n’effectue pas de promotion et le message suivant peut s’afficher :

« Les champs suivants ne sont pas valides : Expression personnalisée non valide : Expression personnalisée non valide. »

Ce problème peut se produire lors du référencement d’un champ existant qui n’est joint à aucun formulaire personnalisé dans l’environnement cible, ou avec un champ nouvellement créé.

Pour résoudre ce problème, effectuez l’une des opérations suivantes :

* Créez un package avec un formulaire personnalisé de type projet contenant le champ référencé. Après avoir promu ce package dans l’environnement cible, convertissez le package prévu à l’origine contenant le champ calculé.
* Créez manuellement le champ référencé dans l’environnement cible et associez-le à un formulaire personnalisé de type projet. Une fois cette opération effectuée, le champ est reconnu et vous pouvez convertir le package sans rencontrer l’erreur.
