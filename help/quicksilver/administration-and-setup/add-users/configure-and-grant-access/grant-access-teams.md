---
title: Accorder l’accès aux équipes
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux équipes dans Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 4%

---

# Accorder l’accès aux équipes

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux équipes dans Workfront, comme expliqué dans la section [Présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurer l’accès des utilisateurs à la modification des utilisateurs à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d’accès, comme expliqué dans la section [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le **Affichage** ou **Modifier** à droite du bouton Equipes, puis sélectionnez les fonctionnalités sous lesquelles vous souhaitez accorder **Ajuster vos paramètres**.

   * **Affichage**: Si vous configurez la manière dont les utilisateurs disposant d’une licence peuvent afficher les équipes, modifiez l’une des options suivantes :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Afficher les équipes associées à mes groupes</td>
         <td>
          <p><b>Activé</b>: Lorsque les utilisateurs recherchent des équipes dans un champ anticipé de type Équipe , les utilisateurs peuvent voir les équipes associées à leurs groupes, qu’elles soient ou non membres de l’équipe. </p>
          <p><b>Désactivé</b>: Lorsque les utilisateurs recherchent des équipes dans un champ de type Equipe , les utilisateurs peuvent voir les équipes associées à leurs groupes uniquement là où ils sont membres de l’équipe.</p><p>Cette option est activée par défaut.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Afficher toutes les équipes</td>
         <td><p>Lorsque cette option est activée et que les utilisateurs recherchent des équipes dans un champ de type Équipe , les utilisateurs peuvent voir et sélectionner n’importe quelle équipe.</p><p>Cette option est activée par défaut. </p></td>
        </tr>
       </tbody>
      </table>

   * **Modifier**: Si vous configurez la façon dont les utilisateurs disposant d’une licence Plan et d’une licence de travail peuvent gérer les équipes, modifiez l’une des options suivantes :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Créer</td>
         <td><p>Permet aux utilisateurs disposant d’une licence Plan ou d’une licence de travail de créer des équipes.</p><p>Cette option est activée par défaut.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Supprimer</td>
         <td><p> Permet aux utilisateurs disposant d’une licence Plan de supprimer les équipes qu’ils ont accès à la modification (indisponible pour les utilisateurs disposant d’une licence de travail).</p><p>Cette option est activée par défaut.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Modifier les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</td>
         <td><p>Permet aux utilisateurs de la licence Plan qui sont désignés comme administrateurs de groupe de modifier les équipes associées aux groupes qu’ils gèrent.</p><p>Cette option est activée par défaut.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Éditer les équipes sur lesquelles je suis</td>
         <td><p>Permet aux utilisateurs de planifier une licence ou une licence de travail pour modifier les équipes auxquelles ils appartiennent.</p><p>Cette option est désactivée par défaut.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Afficher les équipes associées à mes groupes</td>
         <td>
         <p><b>Activé</b> Lorsque les utilisateurs recherchent des équipes dans un champ anticipé de type Équipe , les utilisateurs peuvent voir les équipes associées à leurs groupes, qu’elles soient ou non membres de l’équipe. </p>
         <p><b>Désactivé</b>: Lorsque les utilisateurs recherchent des équipes dans un champ de type Equipe , les utilisateurs peuvent voir les équipes associées à leurs groupes uniquement là où ils sont membres de l’équipe.</p><p>Cette option est activée par défaut.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Afficher toutes les équipes</td>
         <td><p>Lorsque cette option est activée et que les utilisateurs recherchent des équipes dans un champ de type Équipe , les utilisateurs peuvent voir et sélectionner n’importe quelle équipe.</p><p>Cette option est activée par défaut. </p></td>
        </tr>
       </tbody>
      </table>

1. Cliquez sur le X pour fermer la **Ajuster vos paramètres** de la boîte.
1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans la section [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), par exemple [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

>[!NOTE]
>
>* Les conditions suivantes sont vraies, quels que soient les paramètres de niveau d’accès :
   >
   >   * Les propriétaires d’équipes peuvent toujours afficher et modifier leurs équipes.
   >   * Les utilisateurs ont toujours accès à l’affichage des équipes sur lesquelles ils se trouvent.
>
* La configuration de toute option disponible pour Afficher et Modifier (par exemple, &quot;Afficher les équipes associées à mes groupes&quot;) est conservée si vous décidez de sélectionner Afficher au lieu de Modifier ou Modifier au lieu de Afficher au niveau d’accès.
>


## Accès aux équipes par type de licence

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec les problèmes, voir la section [Équipes](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
