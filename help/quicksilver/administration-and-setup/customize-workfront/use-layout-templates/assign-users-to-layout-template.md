---
title: Affectation d’utilisateurs à un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez affecter un modèle de mise en page que vous avez créé à tout utilisateur ou utilisatrice, fonction, équipe ou groupe qui doit l’utiliser.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 92%

---

# Affecter des utilisateurs et utilisatrices à un modèle de mise en page

Vous pouvez affecter un modèle de mise en page que vous avez créé à tout utilisateur ou utilisatrice, fonction, équipe ou groupe qui doit l’utiliser.

Pour les personnes auxquelles aucun modèle de mise en page n’est affecté, la mise en page par défaut est utilisée. Pour en savoir plus sur la mise en page par défaut, voir [À propos de la mise en page Adobe Workfront par défaut](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Les utilisateurs et utilisatrices peuvent également s’affecter un modèle de mise en page, comme décrit dans la section Modifier les zones Mon travail et Demandes de travail avec des modèles de mise en page.

Vous pouvez attribuer plusieurs modèles de mise en page différents au même nom. Pour plus d’informations sur le modèle de mise en page en vigueur pour une personne, un rôle, un groupe ou une équipe, voir [Priorité d’affectation du modèle de mise en page](#layout-template-assignment-priority) plus loin dans cet article.

Pour plus d’informations sur les modèles de mise en page, voir [Modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Pour plus d’informations sur les modèles de mise en page pour les groupes, voir [Créer et modifier des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.</p>
        <p>Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Affecter un modèle de mise en page aux utilisateurs et utilisatrices

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >Lorsque vous êtes satisfait de votre modèle de mise en page, nous vous recommandons de le tester, comme décrit dans la section [Tester un nouveau modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Cliquez sur **Affecter ceci à** dans la section supérieure de la page.
1. Dans la zone qui s’affiche, cliquez sur **Ajouter un utilisateur ou une utilisatrice, une fonction, une équipe ou un groupe**, commencez à saisir le nom d’un utilisateur ou d’une utilisatrice, d’une fonction, d’une équipe ou d’un groupe, puis cliquez sur le nom qui s’affiche dans la liste déroulante.

   Les noms récemment ajoutés s’affichent avec un arrière-plan bleu. Cela s’avère utile lorsque vous modifiez un modèle de mise en page existant, car vous pouvez distinguer les noms que vous venez d’ajouter de ceux qui étaient déjà dans la liste.

   Une icône d’informations ![icône d’informations](assets/info-icon.png) s’affiche à droite du nom de tout utilisateur, fonction, équipe ou groupe déjà affecté à un autre modèle de mise en page. Vous pouvez pointer sur l’icône pour afficher le nom de ce modèle de mise en page et décider si vous souhaitez remplacer l’affectation existante.

1. Répétez les deux étapes précédentes pour affecter le modèle de mise en page à d’autres personnes, fonctions, équipes ou groupes, si nécessaire.

   Vous pouvez affecter jusqu’à 100 personnes à la fois.

1. Cliquez sur **Terminé**, puis sur **Enregistrer et fermer** dans le coin inférieur gauche.

   Cette étape complète le processus de création et d’attribution d’un modèle de mise en page.

## Priorité d’affectation du modèle de mise en page {#layout-template-assignment-priority}

Vous et d’autres administrateurs et administratrices Workfront pouvez affecter plusieurs modèles de mise en page différents à une même personne de quatre manières différentes :

* À l’utilisateur ou utilisatrice individuel
* À une fonction particulière que l’utilisateur ou utilisatrice occupe
* À une certaine équipe dont fait partie l’utilisateur ou utilisatrice
* À un certain groupe dans lequel se trouve l’utilisateur ou utilisatrice

Cependant, un seul modèle de mise en page est visible à tout moment par la personne. Le modèle visible est déterminé par la hiérarchie de priorité suivante :

* **Utilisateur ou utilisatrice individuel** : le modèle de mise en page affecté à la personne en tant qu’utilisateur ou utilisatrice individuel remplace tous les autres. Vous pouvez remplacer une affectation précédente effectuée pour un utilisateur ou une utilisatrice individuel en effectuant une nouvelle affectation ; la plus récente est prioritaire.
* **Fonction principale** : si aucun modèle de mise en page n’est affecté à la personne en tant qu’utilisateur ou utilisatrice unique, elle voit le modèle affecté à leur fonction principale.

  Seul le modèle de mise en page affecté à la fonction principale d’une personne est visible par la personne. Les modèles affectés à des fonctions secondaires occupées par la personne ne sont pas visibles.

* **Équipe principale** : si aucun modèle de mise en page n’est affecté à la personne en tant qu’utilisateur ou utilisatrice individuel ou en tant qu’utilisateur ou utilisatrice avec une fonction principale, elle voit le modèle affecté à son équipe principale.

  Seul le modèle affecté à l’équipe principale d’une personne est visible par la personne. Les modèles attribués à d’autres équipes dont fait partie un utilisateur ou une utilisatrice ne sont pas visibles.

* **Groupe principal** : si aucun modèle de mise en page n’est affecté à cette personne en tant qu’utilisateur individuel ou utilisatrice individuelle, en tant qu’utilisateur ou utilisatrice avec une fonction principale ou en tant que membre de l’équipe interne, le modèle affecté à son groupe principal s’affiche.

  Seul le modèle affecté au groupe principal d’un utilisateur ou d’une utilisatrice est visible par l’utilisateur ou l’utilisatrice. Les modèles affectés à ses autres groupes ne sont pas visibles.

## Si un grand nombre de personnes sont affectées à un modèle de mise en page

<!--If you edit a layout template which is assigned to more than 2000 users and make changes to it, only the first 2000 users will be retained on the layout template and will see the changes you made. The layout template is removed from all others.
-->
Si vous avez plus de 2 000 utilisateurs et utilisatrices à affecter à un modèle de mise en page, nous vous recommandons d’effectuer l’une des opérations suivantes :

* Organisez les utilisateurs et utilisatrice en groupes ou en équipes et affectez le modèle de mise en page à ces groupes ou équipes. Pour plus d’informations, voir [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) et [Créer et gérer des équipes](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Affectez des fonctions aux utilisateurs et utilisatrices et affectez le modèle de mise en page à leur fonction principale. Pour plus d’informations, voir [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
