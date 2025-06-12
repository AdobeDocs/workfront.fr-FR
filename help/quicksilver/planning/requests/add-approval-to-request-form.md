---
title: Ajout d’une approbation à un formulaire de demande dans Adobe Workfront Planning
description: Vous pouvez ajouter un processus d’approbation à un formulaire de demande Adobe Workfront Planning, afin de lancer une approbation pour chaque demande soumise, avant la création d’un enregistrement.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 14%

---

# Ajouter une approbation à un formulaire de demande dans Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez ajouter un processus d’approbation à un formulaire de demande Adobe Workfront Planning, afin de lancer une approbation pour chaque demande soumise, avant la création d’un enregistrement.

Cet article décrit comment un responsable d’espace de travail peut ajouter une approbation à un formulaire de demande associé à un type d’enregistrement.

Pour plus d’informations sur la création d’un formulaire de demande dans Workfront Planning, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Pour plus d’informations sur la soumission d’une demande à un type d’enregistrement pour créer un enregistrement, voir [ Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

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
<p>L’un des plans Workfront suivants :</p>
<ul><li>Sélectionner</li>
<li>Principal</li>
<li>Final</li></ul>
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p>
   </td>

<tr>
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td>
   <td>
<p>Tous </p>  
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </td>

<tr>
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td>
   <td>
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p>
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
   <ul>
   <li><p>Gérer les autorisations pour un espace de travail <span class="preview">et le type d’enregistrement</span></p></li>
    <li><p>L’administration système peut gérer les espaces de travail qu’elle n’a pas créés. </p></li>
    </ul>
   <p>Pour plus d’informations sur les autorisations de partage pour les objets Workfront Planning, voir <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning</a>. 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Dans l’environnement de production, tous les utilisateurs, y compris les administrateurs système, doivent être affectés à un modèle de mise en page qui inclut Planning.</p>
<p><span class="preview">Dans l’environnement de Prévisualisation, les utilisateurs et utilisatrices standard et les administrateurs et administratrices système ont Planning activé par défaut.</span></p>
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à l’ajout d’approbations à un formulaire de demande

* Vous pouvez ajouter un ou plusieurs approbateurs à un formulaire de demande. Vous ne pouvez ajouter que des utilisateurs en tant qu’approbateurs.
* Lorsque vous ajoutez plusieurs approbateurs à un formulaire de demande, tous les approbateurs doivent accepter la demande avant la création d&#39;un enregistrement dans Workfront Planning.
* Si tous les approbateurs approuvent la demande, un enregistrement est créé pour le type d&#39;enregistrement associé au formulaire de demande.
* Si au moins un approbateur rejette la demande et que tous les autres l&#39;approuvent, une demande est créée pour la zone Demandes de Workfront, mais aucun enregistrement n&#39;est créé pour le type d&#39;enregistrement associé au formulaire de demande.
* L’ajout d’approbations à un formulaire de demande est facultatif. Workfront Planning crée immédiatement un enregistrement lorsqu&#39;une demande est soumise, si le formulaire de demande n&#39;est pas associé à une approbation.

## Ajouter une approbation à un formulaire de demande

1. Commencez à créer un formulaire de demande pour un type d’enregistrement, comme décrit dans la section [Créer et gérer un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Cliquez sur **Configuration**.

   La zone **Configuration** s’affiche.

   ![Onglet Configuration](assets/configuration-tab.png)
1. Dans le champ **Approbateurs**, cliquez sur l&#39;icône déroulante et sélectionnez un ou plusieurs noms dans la liste

   Ou

   Commencez à saisir le nom d’un approbateur, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Vous pouvez ajouter un ou plusieurs approbateurs à un formulaire de demande.
   >
   >* Si vous ajoutez plusieurs approbateurs, tous doivent approuver la demande avant que Workfront Planning ne crée un enregistrement.
   >
   >* Si au moins un approbateur rejette la demande, celle-ci est rejetée et l&#39;enregistrement n&#39;est pas créé. La demande reste dans l’onglet Planification de la section Soumis de la zone Demandes de Workfront.
   >
   >* Tous les approbateurs doivent prendre une décision avant qu&#39;une demande ne soit approuvée ou rejetée.


1. (Facultatif) Cliquez sur **Publier** si vous n’avez jamais partagé le formulaire de demande auparavant

   Ou

   Cliquez sur **Partager** pour partager le formulaire, puis sur **Copier le lien**.
1. (Facultatif) Lorsqu’un utilisateur utilise le lien que vous partagez et soumet une demande, Workfront Planning envoie une notification d’approbation in-app et un e-mail aux approbateurs.

   >[!NOTE]
   >
   >   L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour que les utilisateurs puissent recevoir des notifications par e-mail et in-app.


   Pour plus d’informations sur l’approbation des demandes, voir [ Approuver une demande ](/help/quicksilver/planning/requests/approve-request.md).
