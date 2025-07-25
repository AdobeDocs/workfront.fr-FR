---
title: Octroi d’un accès administratif pour un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: En tant que membre de l’administration d’Adobe Workfront, vous pouvez accorder un accès administratif pour un modèle de mise en page aux administrateurs et aux administratrices de groupes d’un groupe particulier afin que le modèle puisse être modifié. Cette opération n’affecte pas le modèle aux utilisateurs et utilisatrices du groupe.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 98%

---

# Octroyer un accès d’administration à un modèle de disposition

En tant que membre de l’administration d’Adobe Workfront, vous pouvez accorder un accès administratif pour un modèle de mise en page aux administrateurs et aux administratrices de groupes d’un groupe particulier afin que le modèle puisse être modifié. Cette opération n’affecte pas le modèle aux utilisateurs et utilisatrices du groupe.

Pour plus d’informations sur l’affectation d’utilisateurs et d’utilisatrices à un modèle de mise en page, consultez la section [Affecter des utilisateurs et des utilisatrices à un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

Pour plus d’informations sur les modèles de mise en page, consultez la section [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de disposition pour les groupes, consultez [Création et modification des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td><p>Nouveau : Standard</p>
  <p> Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.
Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Octroyer un accès d’administration à un modèle de disposition

1. Commencez à travailler sur un modèle de disposition, comme décrit dans la section [Créer et gérer des modèles de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur **Accorder l’accès à** dans la section supérieure de la page.
1. Dans la zone qui s’affiche, cliquez sur **Ajouter un groupe**, commencez à saisir le nom du groupe, cliquez sur le nom qui s’affiche, puis cliquez sur **Terminé**.

   L’ensemble des utilisateurs et des utilisatrices qui ont reçu un mandat d’administration pour le groupe que vous avez spécifié peuvent administrer le modèle de mise en page. Cependant, le modèle n’est pas affecté aux membres du groupe pour qu’ils puissent l’utiliser. Pour plus d’informations sur l’affectation d’un modèle de mise en page à un groupe, consultez dans cet article la section [Attribuer un modèle de mise en page aux utilisateurs et aux utilisatrices](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign).

   >[!NOTE]
   >
   >* Lorsqu’un administrateur ou une administratrice de groupes crée un modèle de mise en page, l’attribution d’un accès administratif est obligatoire. Le modèle de mise en page est destiné au groupe spécifié et n’est visible que par lui. Pour plus d’informations, consultez la section [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). Pour plus d’informations sur les administrateurs et administratrices de groupes, voir [Administrateurs et administratrices de groupes](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* Si vous n’accordez pas un accès administratif aux administrateurs et aux administratrices de groupes d’un groupe particulier, toutes les personnes pouvant modifier des comptes d’utilisateurs et d’utilisatrices disposent d’un accès administratif au modèle de mise en page. Certains administrateurs et certaines administratrices de Workfront choisissent volontairement de ne pas accorder l’accès administratif à un modèle de mise en page afin de le transformer en modèle de mise en page de niveau système.

1. Vous pouvez cliquer sur **Enregistrer** à tout moment pour enregistrer votre progression, puis continuer à modifier le modèle ultérieurement.
