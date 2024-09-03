---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Mapper les attributs d'utilisateur
description: Grâce à l’authentification unique (SSO), vous pouvez transmettre des attributs de l’Active Directory de votre fournisseur d’identité à vos utilisateurs et utilisatrices Adobe Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 100%

---

# Mapper les attributs utilisateur

<!--Audited 2/2024-->

Grâce à l’authentification unique (SSO), vous pouvez transmettre des attributs de l’Active Directory de votre fournisseur d’identité à vos utilisateurs et utilisatrices Adobe Workfront.

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
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p><p>Ou</p><p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conseils pour le mappage des attributs

Tenez compte des points suivants lors du mappage des attributs :

* Testez toujours dans un sandbox de prévisualisation ou un sandbox d’actualisation client (CR).
* Testez avec des comptes administratif et non-administratif pour confirmer que vous avez correctement mappé les attributs.
* Les attributs mappés sont appliqués à chaque fois qu’un utilisateur ou une utilisatrice se connecte via l’authentification unique.

  Exemple : si vous mappez le « nom » et que vous mettez à jour son nom dans Workfront sans mettre à jour la valeur dans son fournisseur d’identité, le nom sera écrasé pour correspondre à la valeur du fournisseur d’identité la prochaine fois que l’utilisateur ou l’utilisatrice se connectera.

## Mapper les attributs utilisateur pour votre organisation

La procédure de mappage des attributs diffère selon que votre organisation utilise ou non Adobe Unified Experience.

Pour déterminer si votre organisation est sur Adobe Unified Experience, examinez l’URL que vous utilisez pour accéder à Workfront.

| URL | Adobe Experience |
|---|---|
| (Nom de l’entreprise).my.workfront.com | Expérience Classic |
| experience.adobe.com | Adobe Unified Experience |

* [Mapper les attributs utilisateur dans l’expérience Classic](#map-user-attributes-in-the-classic-experience)
* [Mapper les attributs utilisateur dans Adobe Unified Experience](#map-user-attributes-in-the-adobe-unified-experience)

### Mapper les attributs utilisateur dans l’expérience Classic

1. Cliquez sur l’icône **Menu principal**![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Authentification unique (SSO)**.

1. Dans le menu déroulant **Type**, cliquez sur **SAML 2.0**.

1. Cliquez sur **Mapper les attributs utilisateur**.

   ![](assets/map-user-attributes.png)

1. Dans la ligne d’options qui s’affiche, mappez les attributs dont vous avez besoin pour vos utilisateurs et utilisatrices Workfront.

   Vous pouvez mapper des attributs tels que l’adresse, la personne gestionnaire, la fonction, le groupe principal, etc.

   Les mappages d’attributs fonctionnent selon un rapport 1:1. Par exemple, vous ne pouvez pas définir tous les groupes auxquels appartient un utilisateur ou une utilisatrice ; vous ne pouvez en définir qu’un seul par utilisateur ou utilisatrice.

   >[!IMPORTANT]
   >
   >Il n’est pas recommandé de mapper les niveaux d’accès dans les mappages d’attributs. Si vous le faites, faites attention lorsque vous définissez la valeur par défaut de ne pas supprimer l’accès administratif par inadvertance.

   Le tableau suivant explique les champs que vous pouvez utiliser pour mapper des attributs :

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Attribut utilisateur Workfront</td> 
      <td>Choisissez le nom de l’attribut que vous mappez.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attribut de répertoire</td> 
      <td>Saisissez le libellé de l’attribut SSO que vous souhaitez utiliser.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Valeur par défaut</td> 
      <td> <p>Après avoir choisi un attribut utilisateur Workfront, si la valeur est NULL lors de la connexion, ce champ se remplit avec la valeur par défaut correspondante dans le système. Ne saisissez une valeur ici que si vous prévoyez d’appliquer des règles de mappage d’attributs (voir l’étape 7). La valeur par défaut constitue une exception à ces règles.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Cliquez sur **Règles** pour ajouter une règle à l’attribut.

   1. Dans la liste déroulante, choisissez le modificateur d’attribut que vous souhaitez utiliser.
   1. Dans les deux champs à droite, saisissez la valeur de l’attribut du répertoire et la valeur par laquelle vous souhaitez le remplacer.

      ![](assets/rule-fields.png)

   Vous pouvez cliquer sur **Ajouter une règle** pour ajouter d’autres règles à l’attribut.

1. (Facultatif) Pour mapper d’autres attributs utilisateur, cliquez sur **Ajouter un mappage** et répétez les étapes 6 à 7.
1. Cliquer sur **Enregistrer**.

### Mapper les attributs utilisateur dans Adobe Unified Experience

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-left.png) dans le coin supérieur gauche d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Authentification unique (SSO)**.

1. Sélectionnez l’onglet **Adobe**.

1. (Facultatif et le cas échéant) Si votre entreprise a configuré le mappage d’attributs dans l’expérience Classic et que vous souhaitez le copier dans Adobe Unified Experience, cliquez sur **Migrer les mappages**. Vous pouvez ensuite ignorer, supprimer ou modifier ces mappages.

   >[!NOTE]
   >
   >Nous recommandons de migrer les mappages la première fois que vous configurez des mappages dans Adobe Unified Experience. Vous pouvez les migrer à nouveau plus tard sans problème, mais il n’est pas nécessaire de les migrer plus d’une fois.

1. Pour créer un nouveau mappage d’attributs, cliquez sur **Ajouter un mappage**.

1. Cliquez sur la flèche située à côté du nom du champ Workfront et sélectionnez le champ [!DNL Workfront] auquel vous souhaitez le mapper.

1. (Facultatif) Si vous souhaitez créer plusieurs règles pour un champ donné, cliquez sur la flèche située à côté de **Toujours** et sélectionnez l’opérateur que la règle doit utiliser.

1. (Le cas échéant) Si vous avez sélectionné un opérateur autre que Toujours, sélectionnez le champ Workfront et la valeur auxquels l’opérateur s’applique.

   >[!NOTE]
   >
   >Les opérateurs `Is Truthy` et `Is Falsy` n’ont pas besoin de valeurs.

1. Indiquez si vous souhaitez appliquer la valeur d’un attribut de votre gestionnaire d’identité au champ Workfront ou si vous souhaitez appliquer une valeur constante spécifique.

1. Saisissez le nom du champ du gestionnaire d’identité que vous souhaitez appliquer ou saisissez le texte de la valeur constante que vous souhaitez appliquer.

1. (Facultatif) Pour ajouter d’autres règles au même champ Workfront, cliquez sur **Ajouter une nouvelle règle**, et suivez les étapes 4 à 9.

   >[!IMPORTANT]
   >
   > * Toute règle inférieure à « Toujours » sera ignorée. Si vous avez une règle Toujours, vous devez la déplacer au bas de la liste des règles. Vous pouvez déplacer les règles dans la liste en cliquant sur le menu à trois points à droite de la règle et en déplaçant la règle vers le haut ou vers le bas.
   > * Pour créer une règle au milieu de la liste, cliquez sur le menu à trois points situé à côté de la règle qui sera située au-dessus ou au-dessous de la nouvelle règle, puis sélectionnez **Ajouter la règle ci-dessus** ou **Ajouter la règle ci-dessous**.

1. Pour supprimer une règle, cliquez sur le menu à trois points situé à côté de la règle à supprimer et sélectionnez **Supprimer**.
1. Pour supprimer un mappage, cliquez sur l’icône **Supprimer** qui se trouve sur la carte de ce mappage.

1. Pour enregistrer, faites défiler la page jusqu’en haut et cliquez sur **Enregistrer**.


