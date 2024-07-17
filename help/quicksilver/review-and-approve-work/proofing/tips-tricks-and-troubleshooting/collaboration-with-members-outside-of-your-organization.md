---
title: Vérification des limites de collaboration avec des personnes extérieures à votre entreprise
description: Vérification des limites de collaboration avec des personnes extérieures à votre entreprise
author: Courtney
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Vérification des limites de collaboration avec des personnes extérieures à votre entreprise

Il existe certaines limites à connaître lors de la communication avec des personnes à l’extérieur de votre organisation lorsqu’elles sont ajoutées à un BAT, en particulier si la personne à l’extérieur de votre organisation dispose d’un accès de vérification dans un environnement distinct.

## Contacts avec la distinction des membres

Il existe trois types de contacts dans un environnement de vérification :

* **Utilisateurs** : les utilisateurs disposent d’une connexion Workfront Proof dans l’environnement de votre entreprise.
* **Membres** : les membres disposent de leur propre connexion Workfront Proof dans l’environnement d’une autre organisation (et non le vôtre). Vous ne pouvez pas convertir les membres en utilisateurs dans votre environnement.
* **Invités** : les invités n’ont pas leur propre connexion Workfront Proof dans l’environnement de votre entreprise, mais vous avez ajouté leurs détails à votre compte (par exemple, les réviseurs invités sur les bons à tirer). Vous pouvez convertir les invités en utilisateurs.

Comme les membres ne peuvent pas être convertis en utilisateurs, leur capacité à baliser les personnes dans les commentaires de BAT est limitée aux utilisateurs de *leur organisation d’origine*.

**Exemple :** La société A invite un utilisateur externe à passer en revue un BAT. Cet utilisateur existe déjà dans un environnement de BAT distinct, Société B.

 

Lorsque la Société A invite l’utilisateur externe au BAT, l’utilisateur externe est ajouté en tant que membre à la liste de contacts de la Société A. Les réviseurs du workflow du BAT de la Société A peuvent marquer l’utilisateur externe dans les commentaires du BAT, car ils se trouvent désormais dans le répertoire de contacts de la Société A.

 

L’utilisateur extérieur ne peut pas baliser les utilisateurs de la Société A, même s’ils se trouvent dans le même workflow de BAT, car les utilisateurs de la Société A n’ont pas été ajoutés en tant que contacts à la Société B.

 

L’utilisateur externe de la Société B peut marquer d’autres utilisateurs de la Société B s’ils se trouvent dans le workflow de BAT ou s’il est autorisé à partager le BAT avec de nouveaux utilisateurs, car ces utilisateurs existent en tant que contacts dans la Société B.
