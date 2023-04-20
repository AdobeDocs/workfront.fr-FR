---
title: Fichier de test masqué
author: Bob
description: Masqué de la recherche et dans le volet de navigation de gauche
hidefromtoc: true
hide: true
exl-id: b6b0f429-b619-4b8e-ab81-ad190dae5a0b
source-git-commit: cedc10b67911365b20027926f840f4ec27212c04
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---


# Fichier de test masqué - TEST DE BRANCHE DE FONCTIONNALITÉS

Ce fichier est masqué de la recherche (`hide: yes`) et depuis le volet de navigation de gauche (`hidefromtoc: yes`).

<span class="preview">Ce fichier est **hidden** à partir de la recherche (`hide: yes`) et depuis le volet de navigation de gauche (`hidefromtoc: yes`).</span>

<p class="preview">Ce fichier est **masqué** de la recherche (`masquer : oui`) et depuis le volet de navigation de gauche (`hidefromtoc: oui).</p>

## Test d’image

![test d’image](assets/get-started.png){width="50" align="center"}

## Test de mise en surbrillance de l’aperçu

**Utilisez DIV pour les blocs de composants.**

DIV commence ci-dessous.

<div class="preview">

Début de DIV.

>[!NOTE]
>
>C&#39;est une note.
>
>J’ai une demande pour mettre en évidence le fond de la note.

![image](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/assets/add-admin-1.png)

Dernier élément en surbrillance.

</div>

La balise DIV se termine au-dessus.

**Utilisation de SPAN pour les paragraphes ou les expressions**

C&#39;est un paragraphe. <span class="preview">Je suis un texte jaune.</span> N’oubliez pas de fermer correctement votre syntaxe, sinon la page risque d’afficher un rendu bizarre.

Les DIV et SPAN sont également utiles dans les tableaux de HTML.

**Autres éléments de HTML pris en charge**

Vous pouvez également spécifier la variable `class="preview"` syntaxe dans `<p>`, `<td>`, `<tr>`, etc. Assurez-vous de tester l’aperçu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr class="preview"> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Formule Adobe Workfront</a>*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"></td> 
   <td> <p class="preview">Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accès Jira</td> 
   <td> <p><span class="preview">Accès administrateur système</p> <p>Important : Nous vous recommandons de créer des comptes d’administrateur système distincts dans Jira et Workfront afin de vous consacrer à cette intégration, plutôt que d’utiliser des comptes existants qui peuvent être joints aux utilisateurs. </span></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un administrateur Workfront. Pour plus d’informations sur les administrateurs Workfront, voir .</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Vidéo avec qualité = 12

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=12)

Vidéo avec qualité = 6

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=6)

Vidéo dans un tableau de HTML

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  </tr> 
  <tr> 
   <td role="rowheader">Cette vidéo fonctionne-t-elle ?</td> 
   <td>Non ce n’est pas le cas </td> 
  </tr> 
 </tbody> 
</table>

Vidéo dans le tableau Markdown

| Colonne 1 | Colonne 2 |
|---|---|
| Cela fonctionne-t-il ? | Aussi non |


