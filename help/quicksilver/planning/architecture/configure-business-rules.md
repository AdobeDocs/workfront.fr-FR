---
title: Configurer les règles métier de type d’enregistrement
description: Vous pouvez configurer des règles métier de type enregistrement qui définissent la manière dont les enregistrements de ce type sont gérés dans Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 31db7a4ef190793558bcb2fa10beb2585e1068e4
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 2%

---


# Configurer des règles métier de type enregistrement

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Vous pouvez configurer des règles métier de type enregistrement qui définissent la manière dont les enregistrements de ce type sont gérés dans Adobe Workfront Planning.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès afin d’effectuer les étapes de cet article :  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Tout Workfront ou workflow avec un package Planning</p></li>
Ou
<li><p>Tout package Planning lorsqu’il est acheté en tant que produit autonome</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Norme de workflow</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Norme de planification</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Vous devez ajouter un workflow et un type de licence Planning au niveau d'accès lorsque vous disposez à la fois d'un workflow et d'un package Planning</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations sur un espace de travail et sur un type d’enregistrement</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant la configuration des règles métier

* Vous pouvez configurer des règles indiquant le moment où les enregistrements peuvent être modifiés ou supprimés, selon les conditions que vous définissez.

  Par exemple, vous pouvez créer des conditions pour que certains champs aient une valeur. Si la valeur est absente de ces champs, les utilisateurs ne peuvent pas modifier ni supprimer cet enregistrement.
* Vous ne pouvez pas ajouter de règles métier aux types d’enregistrements globaux dans leurs espaces de travail principaux ou secondaires.
* Vous ne pouvez pas configurer de règles pour le moment où les enregistrements sont créés. Toute personne disposant d’autorisations de niveau Gérer pour le type d’enregistrement peut créer des enregistrements.
* Vous pouvez créer une condition pour votre règle métier qui fait référence à tous les types de champ, à l’exception des suivants :
  * Champs de formule
  * Champs de recherche
  * Champs de référence

## Configuration des règles métier

1. Accédez à un type d’enregistrement.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur Règles métier.


**&#x200B;**&#x200B;**&#x200B;**&#x200B;*** DE CLAUDE - CI-DESSOUS - DOIT MODIFIER &#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;***

## Configuration de règles métier dans Workfront Planning : guide détaillé

Avez-vous déjà effectué un transfert record vers « Prêt pour l’exécution » pour découvrir plus tard que la moitié des champs requis (marque, indication, dates de lancement) n’ont jamais été remplis ? Quand quelqu&#39;un s&#39;en aperçoit, il y a déjà un projet en aval avec des données manquantes, et quelqu&#39;un doit retrouver les détails et les renvoyer manuellement.

Les règles métier corrigent ce problème. Ils permettent de mettre en place un point de contrôle simple : **avant qu&#39;un enregistrement puisse passer à un statut spécifique, certains champs doivent être renseignés.** Si ce n&#39;est pas le cas, la personne qui apporte la modification voit exactement ce qui manque et ne peut pas procéder tant que la situation n&#39;est pas corrigée.

Ce guide décrit le fonctionnement des règles métier, comment en configurer une et ce que votre équipe vivra une fois qu’elles seront disponibles en ligne.

### À quoi servent les règles métier ?

Les règles métier attachent une condition à un **changement de statut**. Au lieu d’appliquer des données complètes au moment où une personne crée un enregistrement (ce qui ralentirait tout le monde), la règle ne se déclenche qu’à un moment spécifique et délibéré : lorsqu’un statut est sur le point de passer à un statut que vous avez configuré.

Voici à quoi ressemble une règle en langage clair :

> « Avant qu’un enregistrement puisse passer à **Prêt pour l’exécution**, le champ **Marque** doit avoir une valeur. »

Si le champ est vide, le changement de statut est bloqué et la personne reçoit un message clair lui indiquant ce qu’elle doit corriger. Une fois qu’il l’a renseignée et qu’il a réessayé, la modification est effectuée.

Voici quelques points importants *pas* :

* **Cela ne bloque pas la création d’enregistrements.** Les utilisateurs peuvent toujours créer un nouvel enregistrement instantanément et le remplir au fil du temps, exactement comme aujourd’hui.
* **Il ne remplit pas automatiquement les champs ou ne modifie pas automatiquement les statuts.** Une personne doit toujours faire changer le statut elle-même.
* **Il ne signale pas rétroactivement les anciens enregistrements.** Les enregistrements dont le statut est déjà défini sur la cible ne sont pas affectés : la vérification ne s&#39;exécute que la prochaine fois qu&#39;un utilisateur tente de déplacer un enregistrement *vers* ce statut.



### Avant de commencer

Avant de pouvoir configurer des règles, deux ou trois choses doivent être vraies :

1. **La fonctionnalité doit être activée pour votre organisation.** Cela s’effectue du côté d’Adobe (via un indicateur de fonctionnalité), et non d’une manière que vous activez vous-même. Si la section règles métier décrite ci-dessous ne s’affiche pas, contactez votre contact Adobe pour confirmer qu’elle a été activée pour votre client.
2. **Vous avez besoin d’autorisations admin ou workspace-configurator.** Les planificateurs réguliers ne peuvent pas créer ni modifier de règles — seules les personnes qui gèrent la configuration de l&#39;espace de travail peuvent le faire.

### Étape 1 : ouvrir la zone de configuration des règles métier

Les règles métier cohabitent avec votre autre configuration d’administration : vous n’avez pas besoin de rechercher un panneau « Planification » distinct. Dans la zone Configuration du workflow :

1. Accédez à la zone principale **configuration du workflow/configuration de l’administration** pour votre espace de travail.
2. Recherchez la section **règles métier** pour le type d’enregistrement que vous souhaitez configurer (par exemple, « Matériaux » ou « Campagnes »).


### Etape 2 : sélection du type d&#39;enregistrement

Les règles sont configurées par type d’enregistrement. Sélectionnez donc celle à laquelle vous souhaitez ajouter une règle. Par exemple, si vous souhaitez vous assurer que chaque enregistrement Matières comporte des champs clés remplis avant l&#39;exécution, sélectionnez **Matières**.



### Étape 3 : créer une règle

Pour chaque règle, vous spécifiez trois éléments :

| Ce que vous avez défini | Exemple |
|---|---|
| **Type d’enregistrement** | Matériaux |
| **Statut cible** | Prêt pour l’exécution |
| **Champ obligatoire** | Marque |

En d’autres termes : « Lorsque le statut d’un enregistrement Matières est modifié en **Prêt pour l’exécution**, le champ **Marque** doit comporter une valeur. »

Vous pouvez ajouter plusieurs règles pour le même statut. Par exemple, vous pouvez exiger que la marque, la zone thérapeutique, l&#39;indication et la date de lancement estimée soient toutes renseignées avant qu&#39;un enregistrement puisse passer à « Prêt pour l&#39;exécution » — chacune d&#39;elles étant sa propre règle et toutes vérifiées ensemble.

**Quels champs pouvez-vous exiger ?**
&#x200B;- Champs d’enregistrement connectés (par exemple, un enregistrement de marque ou d’indication lié) : la règle passe dès qu’au moins un enregistrement est lié.
&#x200B;- Champs de texte standard (une seule ligne ou paragraphe) : la règle est transmise lorsqu’il existe une valeur.
&#x200B;- Champs de date : la règle est acceptée une fois qu&#39;une date est définie.

**Ce que vous ne pouvez pas encore utiliser :** les champs de formule et de recherche ne sont pas pris en charge en tant que cibles de règle dans cette version, car ils sont calculés en arrière-plan plutôt que renseignés directement par une personne.

### Étape 4 : Écrivez le message que les gens verront

Lorsque vous créez une règle, vous fournissez également le message qui s’affiche si quelqu’un tente d’effectuer la modification sans remplir le champ . Veillez à ce qu’il soit spécifique et exploitable, par exemple :

> « La marque est requise. »

Vous n&#39;avez pas à vous soucier de la mise en forme d&#39;une bannière d&#39;erreur entière — le système gère la combinaison des messages si plusieurs règles sont violées à la fois (voir ci-dessous).

### Étape 5 : enregistrer la règle

Une fois enregistrée, la règle prend effet **immédiatement** pour tous les utilisateurs de l’espace de travail. Nul besoin de se déconnecter, d’actualiser ou d’attendre un déploiement. La prochaine fois que quelqu’un tentera de déplacer un enregistrement vers ce statut, la règle sera vérifiée.

### Ce que votre équipe vivra réellement

Voici ce qui change pour les personnes qui utilisent Planning au jour le jour, une fois qu&#39;une règle est active.

#### Si un champ obligatoire est vide

1. Un planificateur ouvre un enregistrement et change son statut en statut de point de contrôle (par exemple, « Prêt pour l’exécution »).
2. Le système vérifie toutes les règles liées à ce statut.
3. Si un champ obligatoire est vide, la modification est **rejetée** — le statut revient à ce qu’il était.
4. Un message toast s’affiche, indiquant exactement le ou les champs manquants :
   > *« Changement de statut bloqué : &#39;Marque&#39; et &#39;Date de lancement estimée&#39; doivent être renseignées avant de passer à &#39;Prêt pour l&#39;exécution&#39;.«*
5. Le planificateur remplit le ou les champs manquants et tente à nouveau de modifier le statut.
6. Cette fois, la règle est acceptée et l’état est mis à jour normalement.

#### Si tout est déjà renseigné

Rien ne change. Le statut est mis à jour instantanément, sans étapes ou fenêtres contextuelles supplémentaires. Les règles de gestion sont invisibles jusqu&#39;à ce qu&#39;elles soient réellement nécessaires.

#### Si plusieurs champs sont manquants à la fois

Toutes les règles enfreintes sont vérifiées ensemble, et le message répertorie tous les champs manquants en une seule fois. Les planificateurs n&#39;ont pas à corriger un champ, à réessayer, à se faire informer du suivant et à répéter.

### Étape 6 : modifier ou supprimer une règle ultérieurement

Les règles ne sont pas immuables. Pour apporter des modifications :

1. Revenez à la zone de configuration des règles métier pour le type d’enregistrement.
2. Recherchez la règle que vous souhaitez modifier.
3. Modifiez le champ, le statut de la cible ou le message requis, ou supprimez entièrement la règle.
4. Enregistrez. La modification s’applique immédiatement aux modifications de statut futures.

Gardez à l’esprit que la modification ou la suppression d’une règle **affecte uniquement les transitions dans les années à venir.** Les enregistrements qui ont déjà atteint le statut cible avant la modification ne sont pas réévalués.
3## Quelques choses à savoir

* **Ceci est distinct du verrouillage des enregistrements après un changement de statut.** Les règles métier (comme décrit ici) vérifient uniquement l’exhaustivité des champs *avant* qu’un changement de statut ne soit effectué. Une autre fonctionnalité liée détermine si un enregistrement est complètement verrouillé des modifications/suppressions une fois qu&#39;il atteint un certain statut - ce n&#39;est pas ce qui est couvert ici.
* Les **modifications de statut en bloc** (modification du statut sur de nombreux enregistrements à la fois) ne sont pas encore entièrement définies pour la manière dont elles interagissent avec les règles métier. Si votre équipe s’appuie fortement sur des actions en bloc, vérifiez auprès de votre contact Adobe le comportement actuel.
* **Si une règle ne peut pas être évaluée** en raison d’une erreur système, la transition est bloquée plutôt que silencieusement autorisée. Vous ne vous retrouverez jamais avec un enregistrement incomplet qui glisse au-delà d’une règle en raison d’un problème de serveur principal.
* La **désactivation de la fonctionnalité** ne supprime pas les règles configurées, elles sont simplement suspendues. Le fait de le réactiver les restaure exactement comme ils étaient, aucune reconfiguration n’était nécessaire.

### Référence rapide : configuration de votre première règle

1. Vérifiez que la fonctionnalité est activée pour votre client .
2. Accédez à Configuration du workflow → Règles métier pour votre type d’enregistrement.
3. Choisissez le type d&#39;enregistrement (par exemple, Matériaux).
4. Créez une règle : statut de la cible + champ obligatoire.
5. Rédigez un message d’erreur clair et spécifique.
6. Sauvegarde — c&#39;est en ligne immédiatement.
7. Répétez l’opération pour chaque champ à exiger.
8. Testez-le vous-même : essayez de modifier le statut d’un enregistrement avec le champ vide, confirmez que le message attendu s’affiche, remplissez le champ, puis confirmez que le changement de statut est maintenant terminé.

C&#39;est ça - à partir de maintenant, toute personne convertissant un enregistrement aura un coup de pouce clair si quelque chose manque, au lieu d&#39;un projet en aval qui se montrera silencieusement incomplet.