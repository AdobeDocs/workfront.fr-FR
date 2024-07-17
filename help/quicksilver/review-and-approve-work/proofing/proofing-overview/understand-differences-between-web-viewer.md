---
content-type: reference
product-area: documents
navigation-topic: proofing-overview
title: Vue d’ensemble des différences entre la visionneuse de relecture web et la visionneuse de relecture de bureau
description: Découvrez les différences entre les visionneuses de test pour ordinateur et web.
author: Courtney
feature: Digital Content and Documents
exl-id: 72ce147b-29c9-4c3b-a03c-2da0758bc178
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 14%

---

# Vue d’ensemble des différences entre la visionneuse de relecture web et la visionneuse de relecture de bureau

Adobe Workfront fournit deux visionneuses de vérification :

* **Visionneuse de test Web :** conçue principalement pour la vérification de fichiers statiques et vidéo. S’exécute dans Google Chrome, Firefox ou Safari.
* **Visionneuse de vérification de l’appli de bureau :** conçue pour la vérification de fichiers interactifs ainsi que de fichiers vidéo et statiques. S’exécute en tant qu’application autonome sur votre poste de travail. Pour plus d’informations, voir [Présentation de la visionneuse de vérification de l’appli de bureau](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)

* Si votre entreprise ne peut pas utiliser l’application Visionneuse de vérification de l’appli de bureau pour des raisons de sécurité, votre administrateur Workfront peut configurer votre système afin que vous puissiez consulter le contenu interactif, regroupé dans un fichier d’archive ZIP, dans la visionneuse de vérification de l’application Web. Pour plus d’informations, voir  [Configurez la vérification de contenu interactif dans la visionneuse de vérification de contenu web](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

La liste suivante peut vous aider à comprendre la visionneuse de vérification que vous pouvez utiliser pour vérifier certains types de contenu :

* **Contenu web interactif - URL** : si vous créez un BAT pour le contenu web à l’aide d’une URL et que vous souhaitez tester le contenu de manière interactive, vous devez utiliser la visionneuse de vérification de l’appli de bureau.
* **Contenu web interactif - fichier ZIP** : si vous créez un BAT pour le contenu web à l’aide d’un fichier ZIP, vous pouvez utiliser soit la visionneuse de test Web (avec certaines restrictions), soit la visionneuse de vérification de l’appli de bureau. Pour plus d’informations sur les limites liées à l’utilisation de la visionneuse de vérification de l’intégrité web pour le contenu interactif, voir [ Configuration de la vérification de l’intégrité du contenu interactif dans la visionneuse de vérification de l’intégrité web](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/interactive-content-in-web-viewer.md).

* **Contenu statique et vidéo** : si vous créez un BAT contenant du contenu statique, vous pouvez utiliser la visionneuse de vérification de l’intégrité Web ou la visionneuse de vérification de l’intégrité de bureau.

## BAT statique

| **Fonctionnalité** | **Visionneuse de proxy web** | **Visionneuse de vérification de l’appli de bureau** |
|---|---|---|
| Ouvrir les bons à tirer statiques | ✓ | ✓&#42; |
| Affichages uniques, de magazines et continus | ✓ | ✓&#42; |
| Panoramique | ✓ | ✓&#42; |
| Zoom | ✓ | ✓&#42; |
| Rotation | ✓ | ✓&#42; |
| Outil de mesure | ✓ (définissez une zone de taille personnalisée) | ✓&#42; |
| Mode Miniature | ✓ | ✓&#42; |
| Navigateur de BAT statique | ✓ | ✓&#42; |
| Recherche de documents | ✓ | ✓&#42; |
| Commentaire Post sur plusieurs pages | ✓ (disponible sur toutes les vues) | ✓&#42; (disponible sur toutes les vues) |
| Raccourcis de BAT statique avancés | ✓ (pour plus d’informations, voir [Raccourcis clavier dans la visionneuse de correctifs](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;(pour plus d’informations, voir [Raccourcis clavier dans la visionneuse de vérification de correction](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) |

{style="table-layout:auto"}

&#42; Cette fonctionnalité fonctionne uniquement si votre administrateur Workfront a configuré la visionneuse de vérification de l’appli de bureau en tant que visionneuse par défaut pour tous les bons à tirer.

## BAT vidéo

| **Fonctionnalité**  | **Visionneuse de proxy web** | **Visionneuse de vérification de l’appli de bureau** |
|---|---|---|
| BAT vidéo ouvert | ✓ | ✓&#42; |
| Mise en mémoire tampon | ✓ | ✓&#42; |
| Révision à l’aide du temps | ✓ | ✓&#42; |
| Vérification à l’aide d’images ou de code temporel | ✓ | ✓&#42; |
| Révision plus rapide ou plus lente | ✓ | ✓&#42; |
| Régulation des volumes | ✓ | ✓&#42;  |
| mode plein écran | ✓ | ✓&#42;  |
| Commentaires sur la plage | ✓ | ✓&#42;  |
| BAT vidéo en boucle (les vidéos se terminent et démarrent automatiquement) | ✓ | ✓&#42;  |
| Raccourcis vidéo avancés | ✓ (pour plus d’informations, voir [Raccourcis clavier dans la visionneuse de correctifs](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/keyboard-shortcuts-proof.md)) | ✓&#42;  |

{style="table-layout:auto"}

&#42; Cette fonctionnalité fonctionne uniquement si la visionneuse de vérification de l’appli de bureau est configurée comme visionneuse par défaut pour tous les bons à tirer.

## BAT interactif

| **Fonctionnalité**  | **Visionneuse de proxy web** | **Visionneuse de vérification de l’appli de bureau** |
|---|---|---|
| Ouvrir les BAT interactifs créés à partir de contenu regroupé dans un fichier ZIP | ✓ | ✓ (recommandé) |
| Ouvrir un BAT interactif créé à partir d’une URL | Non pris en charge | ✓ |
| Affichage de BAT interactifs (créés à partir de contenu regroupé dans un fichier ZIP) dans différentes tailles d’écran | ✓ | ✓ |
| Affichage de BAT interactifs (créés à partir de contenu regroupé dans un fichier ZIP) pour divers appareils | Non pris en charge | ✓ |
| Vérifier les sites non sécurisés (HTTP) | Non pris en charge | ✓ |
| Vérification des sites protégés par un iFrame (sites protégés contre l’affichage dans un iFrame) | Non pris en charge | ✓ |

{style="table-layout:auto"}

## Commentaires

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Fonctionnalité</th> 
   <th>Visionneuse de test Web </th> 
   <th>Visionneuse de relecture de bureau </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Ajouter, supprimer et modifier des commentaires</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ajouter et supprimer des réponses</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Outils de marquage Rectangle, flèche, ligne, main libre et surlignage</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Outil Polyligne</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Outils de balisage de masque de recadrage</p> </td> 
   <td>Non pris en charge</td> 
   <td>Non pris en charge</td> 
  </tr> 
  <tr> 
   <td> <p>Outil Balisage de sélection de texte</p> </td> 
   <td>✓ BAT statique uniquement</td> 
   <td>✓ BAT statique uniquement</td> 
  </tr> 
  <tr> 
   <td> <p>Modifier la couleur du balisage</p> </td> 
   <td>✓ (32 couleurs disponibles) </td> 
   <td>✓ (32 couleurs disponibles) </td> 
  </tr> 
  <tr> 
   <td> <p>Modifier l’opacité des balises</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Modifier l’épaisseur des balises</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Couper, copier et coller des balises</p> </td> 
   <td> Non pris en charge</td> 
   <td> Non pris en charge</td> 
  </tr> 
  <tr> 
   <td> <p>Annuler et rétablir la dernière opération</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Balises en double</p> </td> 
   <td> Non pris en charge</td> 
   <td> Non pris en charge</td> 
  </tr> 
  <tr> 
   <td>Définition des actions dans les commentaires</td> 
   <td>✓ (les actions sont visibles sur les commentaires immédiatement après la définition de l’action)</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Définir la couleur du balisage par défaut</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Résoudre les commentaires</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Verrouillage de commentaires</p> </td> 
   <td>Non pris en charge</td> 
   <td> Non pris en charge</td> 
  </tr> 
  <tr> 
   <td> <p>Balisage des utilisateurs</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Reprendre les commentaires</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Affichage de la liste de commentaires dans une vue compacte</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>Affichage de la liste de commentaires dans une vue standard, complète ou unique</p> </td> 
   <td>Planifié pour le futur</td> 
   <td>Planifié pour le futur</td> 
  </tr> 
  <tr> 
   <td> <p>Commentaires sur la recherche</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Filtrage des commentaires par utilisateur</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Filtrage des commentaires et réponses par utilisateur</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Tri des commentaires</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Mises à jour automatiques des commentaires</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Décisions

| Fonctionnalité | Visionneuse de test Web | Visionneuse de relecture de bureau |
|---|---|---|
| Prendre des décisions | ✓ | ✓ |
| Personnalisation des décisions | ✓ | ✓ |

{style="table-layout:auto"}

## Comparer les épreuves

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Fonctionnalité</th> 
   <th>Visionneuse de test Web </th> 
   <th>Visionneuse de relecture de bureau </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Comparaison de différentes versions de BAT</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
  <tr> 
   <td>Comparaison de BAT distincts</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

## Opérations de BAT

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Fonctionnalité</th> 
   <th>Visionneuse de test Web </th> 
   <th>Visionneuse de relecture de bureau </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Modifier la version du BAT </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td>Création d’une version</td> 
   <td> <p>Disponible uniquement dans Workfront Proof (prévu pour le futur lors de la vérification dans Workfront)<br></p> </td> 
   <td>Disponible uniquement dans Workfront Proof (prévu pour le futur lors de la vérification dans Workfront)</td> 
  </tr> 
  <tr> 
   <td>Vérification des détails du BAT </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Vérifier les workflows du BAT</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modification des étapes de workflow</td> 
   <td>Non pris en charge</td> 
   <td>Non pris en charge</td> 
  </tr> 
  <tr> 
   <td>Partage de bons à tirer</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Obtenir l’URL de l’équipe</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modifier les notifications par email</td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Télécharger le fichier d’origine</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Verrouillage et déverrouillage des bons à tirer et des scènes</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Résumé du BAT d'impression</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Suppression de BAT</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Gestion des BAT à partir du même dossier</td> 
   <td><strong>Disponible uniquement dans Workfront Proof</strong> </td> 
   <td><strong>Disponible uniquement dans Workfront Proof</strong> </td> 
  </tr> 
  <tr> 
   <td>Marques (logos personnalisés)</td> 
   <td>✓</td> 
   <td> ✓<br> (logo Workfront sur la page de lancement) </td> 
  </tr> 
  <tr> 
   <td>Liens personnalisés (Workfront Proof uniquement)</td> 
   <td>Non pris en charge</td> 
   <td> Non pris en charge </td> 
  </tr> 
  <tr> 
   <td>Intégrations Basecamp (Workfront Proof uniquement) </td> 
   <td>Prévu pour le futur</td> 
   <td>Prévu pour le futur</td> 
  </tr> 
  <tr> 
   <td>Indicateur de présence </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Mises à jour automatiques du BAT (modifications des autorisations et nouvelles versions)</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

## Miniviewer

| **Fonctionnalité**  | **Visionneuse de proxy web**  | **Visionneuse de vérification de l’appli de bureau** |
|---|---|---|
| Code incorporé | Prévu pour le futur des BAT vidéo statiques et natifs | Non pris en charge  |

{style="table-layout:auto"}

## Traductions

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Fonctionnalité</strong> </th> 
   <th><strong>Visionneuse de proxy web</strong> </th> 
   <th><strong>Visionneuse de vérification de l’appli de bureau</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Langues de prise en charge autres que l’anglais</td> 
   <td>✓</td> 
   <td>✓<br></td> 
  </tr> 
 </tbody> 
</table>
