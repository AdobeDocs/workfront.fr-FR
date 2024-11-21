---
title: Soumettre des demandes de planification Adobe Workfront
description: Une fois qu’une personne a partagé avec vous un lien vers un formulaire de demande à partir d’une page de type enregistrement dans Adobe Workfront Planning, vous pouvez ajouter une requête pour créer des enregistrements pour le type d’enregistrement associé au formulaire de demande.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 13%

---

# Soumettre des demandes de planification Adobe Workfront pour créer des enregistrements

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

{{planning-important-intro}}

Une fois qu’une personne a partagé avec vous un lien vers un formulaire de demande à partir d’une page de type enregistrement dans Adobe Workfront Planning, vous pouvez ajouter une requête pour créer des enregistrements pour le type d’enregistrement associé au formulaire de demande.

Les utilisateurs de Workfront et les utilisateurs externes peuvent envoyer des requêtes à Planification des types d’enregistrement et créer des enregistrements. <!--double check on the external users-->

Cet article décrit comment envoyer une demande d’ajout de nouveaux enregistrements à un type d’enregistrement.

Pour plus d’informations sur la façon dont un gestionnaire d’espace de travail peut créer un formulaire de requête et l’associer à un type d’enregistrement, voir [Création et gestion d’un formulaire de requête dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produits</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Planification d’Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td>
   <td>
<p>L’un des projets Workfront suivants est prévu :</p>
<ul><li>Sélectionner</li>
<li>Principal</li>
<li>Final</li></ul>
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p>
   </td>
<tr>
   <td role="rowheader"><p>Package de planification Adobe Workfront*</p></td>
   <td>
<p>Tous </p>  
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </td>
<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Licence externe, contributeur, légère ou standard</p>
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td>
   <p>Affichage ou autorisations supérieures à un espace de travail si vous êtes un utilisateur Workfront</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Pour accéder à la zone Planning dans Workfront, vous devez disposer d’un modèle de mise en page comprenant la zone Planning dans le menu principal. </p>
   <p> Toutefois, l’accès à la zone Planification n’est pas nécessaire pour envoyer des requêtes à Workfront Planning. </p>  
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Les éléments suivants doivent être en place avant de pouvoir envoyer une requête à un formulaire de demande de planification Workfront :

* Les éléments suivants doivent exister dans la planification Workfront :

   * Un espace de travail
   * Type d’enregistrement associé à un formulaire de demande. Pour plus d’informations, voir [Création d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Le formulaire de demande doit être partagé avec un lien d’une manière accessible. Les scénarios suivants sont possibles :

   * Si vous disposez d’un compte Workfront, le lien a été partagé uniquement avec les personnes internes et vous avez accès à l’espace de travail. Les personnes en dehors de Workfront ne peuvent pas accéder à un lien partagé en interne.
   * Si vous ne disposez pas d’un compte Workfront, le lien a été partagé avec des personnes externes. Les utilisateurs de Workfront peuvent également accéder à un lien partagé avec des personnes externes.

* Le lien vers le formulaire ne doit pas avoir expiré.

## Observations relatives à l’envoi de requêtes à la planification Workfront

* Vous ne pouvez pas accéder aux formulaires de requêtes de planification Workfront sans lien spécifique vers les formulaires.
* Vous ne pouvez pas modifier une requête une fois que vous l’avez envoyée à Workfront Planning.
* Chaque requête envoyée crée un enregistrement pour le type d’enregistrement associé au formulaire que vous utilisez.
* Les enregistrements créés lors de l’envoi de formulaires de demande ne peuvent pas être différenciés des enregistrements ajoutés par une autre méthode. Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

## Envoi d’une requête à Workfront Planning

1. Accédez au lien partagé avec vous à partir d’un type d’enregistrement Workfront Planning .

1. Mettez à jour les champs disponibles dans le formulaire. Les champs avec un astérisque sont obligatoires.

   >[!TIP]
   >
   >   Si le champ Workfront **Objet** est disponible, il peut ne pas être visible dans la planification Workfront. Nous vous recommandons de mettre à jour autant de champs que possible dans votre requête afin de rendre le nouvel enregistrement identifiable lorsqu’il est ajouté au type d’enregistrement.

1. Cliquez sur **Soumettre**.

   Votre formulaire est envoyé et un nouvel enregistrement est ajouté au type d’enregistrement associé au formulaire.
