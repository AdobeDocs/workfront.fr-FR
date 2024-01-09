---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Mise à jour du travail
description: Vous pouvez ajouter une mise à jour sur un objet Adobe Workfront (projet, tâche ou problème) pour communiquer sur la progression de l’objet. Les utilisateurs affectés ou abonnés à l’objet peuvent afficher votre mise à jour. Vous pouvez également marquer les utilisateurs pour attirer leur attention sur la mise à jour.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: ba0dc486dfb104eb9fb8c964875f77cf24f520fd
workflow-type: tm+mt
source-wordcount: '4189'
ht-degree: 1%

---

# Mise à jour du travail

<!-- Audited: 1/2024 -->

<!--take "legacy" and "new commenting" references out when we remove the legacy - Jan 2024???-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. </span>

<span class="preview">Pour plus d’informations sur le calendrier de publication actuel, voir [Présentation de la version du premier trimestre 2024](../../product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

>[!IMPORTANT]
>
>Nous sommes en train de reconcevoir l’expérience de commentaire dans Adobe Workfront.
>
>Selon les objets pour lesquels vous accédez à l’expérience de commentaire, les fonctionnalités suivantes peuvent s’afficher dans la section Mises à jour :
>* La nouvelle expérience
>* L’expérience héritée
>* L’expérience nouvelle et héritée
>
>Pour plus d’informations sur la nouvelle expérience de commentaire et sa disponibilité, voir [Nouvelle expérience de commentaire](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>La nouvelle expérience de commentaire n’est disponible que pour la section Mises à jour des objets Workfront et n’est pas disponible lorsque vous accédez aux mises à jour des zones suivantes :
>
> * Page d’accueil
> * Panneau Résumé dans les listes
> * Panneau Résumé dans les feuilles de temps
> * Panneau Résumé de l’équilibreur de charge de travail

<!-- with October 26 release: add somewhere this, and decide where we need to keep information about the legacy commenting. Should we create an article about iterations comments like we have for goals and cards?!:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old message, before Auhust 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).
-->

## Observations relatives à la mise à jour du travail

* Vous pouvez ajouter des commentaires à la plupart des objets dans Adobe Workfront dans la section Mises à jour . Pour plus d’informations sur les objets qui affichent la section Mises à jour, voir [Présentation de la section Mises à jour](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

* Vous pouvez ajouter des commentaires aux objets Workfront à partir d’autres applications intégrées à Workfront ou à partir de l’application mobile Workfront.

  Toutes les applications intégrées à Workfront ne peuvent pas ajouter de commentaires aux objets Workfront.

  Toutes les fonctions disponibles dans la section Mises à jour d’un objet dans Workfront ne le sont pas dans d’autres applications lors de l’accès aux objets Workfront à partir de l’application. Par exemple, les fonctionnalités de texte enrichi ou la définition d’un commentaire privé pour la société d’une personne peuvent ne pas être disponibles lors de l’ajout de commentaires à un objet Workfront à partir d’une application tierce.

* Vous pouvez communiquer sur la progression d’un objet Workfront (projet, tâche ou problème) lorsque vous commentez l’objet. Les utilisateurs affectés ou abonnés à l’objet peuvent recevoir une notification à propos de votre mise à jour. Toute personne disposant de l’accès Afficher à l’objet peut afficher votre mise à jour.

* Vous pouvez marquer les utilisateurs pour attirer leur attention sur la mise à jour. Les utilisateurs balisés reçoivent une notification in-app et un e-mail concernant votre mise à jour.

  >[!TIP]
  >
  >   Dans la nouvelle expérience de commentaires, les propriétaires de commentaires sont automatiquement balisés. Pour plus d’informations, voir [Balisage des autres sur les mises à jour](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
  <!--take the "in the new commenting experience" out when this is the only experience-->

* Vous pouvez ajouter un commentaire à un objet que vous pouvez afficher ou vous connecter en tant qu’administrateur Workfront ou de groupe et ajouter un commentaire au nom d’un autre utilisateur. Pour plus d’informations, voir [Connexion en tant qu’autre utilisateur](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

* Vous pouvez ajouter une mise à jour aux projets, aux tâches et aux problèmes dans les zones suivantes de Workfront :

   * Dans la section Mises à jour d’un objet Workfront
   * Dans la zone Accueil (pour les tâches et les problèmes)
   * Dans le panneau Résumé d’une liste d’objets, d’une feuille de temps ou de l’équilibreur de charge de travail (pour les tâches et les problèmes)

Les informations de cette page expliquent comment ajouter des commentaires aux objets Workfront et comment mettre à jour des projets, des tâches et des problèmes lors de l’ajout de commentaires.

<!--take this out (below) when we remove legacy out of the application-->

Pour plus d’informations sur les commentaires sur les objectifs, voir [Gestion des commentaires d’objectif dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md). Vous devez disposer d’une licence supplémentaire pour accéder aux objectifs de Workfront.

Pour plus d’informations sur les commentaires sur les cartes dans la zone Panoramas, voir [Ajouter une carte ad hoc à un panorama](../../agile/get-started-with-boards/add-card-to-board.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> 
   <p>Actuel : demande ou version ultérieure pour les problèmes et les documents ; vérification ou version ultérieure pour tous les autres objets</p>
   <p>Nouveau : Contributeur ou version ultérieure pour les problèmes et les documents : clair ou supérieur pour tous les autres objets</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Accès à l’affichage ou à la modification de l’objet activé par la mise à jour</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Afficher l’accès à l’objet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>


&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Ajouter une mise à jour à un élément de travail

L’ajout d’une mise à jour à un élément de travail varie en fonction de la version de la section Mises à jour que vous utilisez.

Vous pouvez ajouter des mises à jour aux objets suivants :

* Projets
* Tâches
* Problèmes
* Programmes
* Portefeuilles
* Modèles
* Tâches de modèle
* Utilisateurs
* Feuilles de temps
* Équipes
* Objectifs
* Cartes dans la zone Panoramas
* Itérations

### Ajouter une mise à jour à un élément de travail dans la section Mises à jour héritées

>[!IMPORTANT]
>
>Les informations de cette page décrivent la mise à jour des projets, tâches et problèmes.

1. Accédez à l’élément de travail pour lequel vous souhaitez fournir une mise à jour (un projet, une tâche ou un problème, par exemple).
1. Cliquez sur le bouton **Mises à jour** .
1. (Conditionnel) Si cette option est activée, cliquez sur l’icône **Nouveaux commentaires** dans le coin supérieur droit de la section Mises à jour afin de la désactiver et d’activer l’expérience de commentaire héritée.
1. Cliquez sur **Démarrer une nouvelle mise à jour,** saisissez ensuite votre mise à jour.
1. (Facultatif) Utilisez les options de la barre d’outils Texte enrichi pour mettre en forme votre texte, ajouter des émoticônes, des liens ou des images à votre mise à jour, afin d’améliorer votre contenu. Pour plus d’informations, voir [Utilisation de texte enrichi dans une mise à jour Workfront](#use-rich-text-in-a-workfront-update) dans cet article.
1. (Facultatif) Mettez à jour l’une des informations suivantes sur l’élément de travail :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notifier </strong></td> 
      <td>Identifiez les utilisateurs qui doivent être informés de la mise à jour. Les utilisateurs affectés ou abonnés à l’objet reçoivent automatiquement une notification lorsqu’une mise à jour est effectuée.<br><p>Pour plus d’informations sur la manière d’inclure d’autres personnes à une mise à jour, voir <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Balisage des autres sur les mises à jour</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Date d'engagement</strong></td> 
      <td>Dans le sélecteur de date, sélectionnez la date de validation de la fin de l’élément de travail. Pour plus d’informations sur la date de validation, voir <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Présentation de la date de validation</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition</strong></td> 
      <td>Sélectionnez une nouvelle condition pour la tâche ou le problème. Pour plus d’informations sur la sélection d’une condition, voir <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Mise à jour de la condition pour les tâches et les problèmes</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Statut</strong></td> 
      <td>Cliquez sur la flèche en regard de l’état actuel, puis sélectionnez l’état de votre choix dans le menu déroulant. Pour plus d’informations sur la définition d’un état, voir <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Mettre à jour le statut des tâches</a>.<p>La mise à jour de l’état d’un élément de travail ne modifie pas automatiquement l’état d’un projet. Selon la configuration de votre projet, vous pouvez mettre à jour séparément l’état du projet. Pour plus d’informations sur les différents types de mise à jour de projet, voir <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Sélectionnez le type de mise à jour du projet. </a>.</p><p><b>NOTE</b>

   Vous ne pouvez pas modifier l’état d’un élément de travail lorsqu’il est dans un état d’approbation en attente.</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Barre d’achèvement</strong></td> 
      <td>(Uniquement disponible sur les tâches) Indiquez le pourcentage de travail réalisé en glissant la barre de progression sur le pourcentage souhaité. Vous pouvez également double-cliquer sur la barre d’achèvement et saisir le pourcentage de remplissage.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Réservé à mon entreprise</strong></td> 
      <td> <p>Désactivez cette option pour empêcher les utilisateurs en dehors de votre entreprise d’avoir accès à cette mise à jour.</p> 
      <p><b>NOTE</b></p>
      <p>Cette option s’affiche uniquement lorsque l’utilisateur est associé à une entreprise.</p>
      <p>Cette option n’est pas disponible dans toutes les zones à partir desquelles vous pouvez ajouter des mises à jour. Par exemple, cela n’est pas disponible dans les applications tierces à partir desquelles vous pouvez ajouter des mises à jour. </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Mettre à jour** pour ajouter la mise à jour à l’objet Workfront.

   >[!NOTE]
   >
   >Une petite fenêtre contextuelle s’affiche pendant sept secondes après avoir cliqué sur **Mettre à jour**, ce qui vous permet d’annuler la mise à jour et de revenir au volet d’édition avant la publication de la mise à jour. La mise à jour est publiée si vous ignorez la fenêtre contextuelle Annuler, attendez qu’elle disparaisse ou quittez la page.
   >
   >Si votre administrateur Workfront sélectionne le paramètre &quot;Ne jamais autoriser les utilisateurs à supprimer les commentaires&quot; dans votre niveau d’accès, vous ne pouvez pas annuler un commentaire. Pour plus d’informations, voir [Création et modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. Pour répondre à une mise à jour, voir [Répondre aux mises à jour](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

### Ajouter une mise à jour à un élément de travail à l’aide de la nouvelle expérience de commentaire

1. Recherchez l’objet à mettre à jour (projet, tâche ou problème), puis cliquez sur son nom pour ouvrir la page de l’objet.
1. Cliquez sur  **Mises à jour** dans le panneau de gauche.
1. (Conditionnel) Si la variable **Nouveaux commentaires** est désactivée, cliquez sur pour l’activer.

   Cela permet la nouvelle expérience de commentaire. La variable **Commentaires** est sélectionné par défaut.
1. Commencez à saisir un commentaire dans la variable **Nouveau commentaire** de la boîte.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Lorsque vous quittez la section Mises à jour avant de terminer la saisie, un commentaire est envoyé afin de conserver le commentaire sur la page en mode préliminaire, même après vous être déconnecté et vous être reconnecté. Toutes les images ajoutées au commentaire sont également enregistrées dans le brouillon. Les brouillons sont enregistrés pendant 7 jours, après quoi ils sont ignorés et ne peuvent pas être récupérés. Les commentaires préliminaires ne sont visibles que par l’utilisateur qui les saisit.

1. (Facultatif) Pour annuler ou rétablir une modification, utilisez les raccourcis clavier suivants :
   * Ctrl + Z ( ⌘ + z pour Mac) pour annuler une modification.
   * Ctrl + Y ( ⌘ + y pour Mac) pour rétablir la modification
1. (Facultatif) Dans la variable **Balisage de personnes ou d’équipes** , commencez à saisir le nom ou l’adresse électronique d’un utilisateur ou d’une équipe que vous souhaitez inclure dans ce commentaire, puis sélectionnez-la lorsqu’elle s’affiche dans la liste.
1. (Facultatif) Utilisez les options de la barre d’outils Texte enrichi pour mettre en forme votre texte, ajouter des émoticônes, des liens ou des images à votre mise à jour, afin d’améliorer votre contenu. Pour plus d’informations, voir [Utilisation de texte enrichi dans une mise à jour Workfront](#use-rich-text-in-a-workfront-update) dans cet article.

   >[!TIP]
   >
   >Si un autre utilisateur envoie un commentaire au même élément que celui que vous mettez à jour, une ligne rouge avec un indicateur &quot;Nouveau&quot; s’affiche pour vous informer des commentaires les plus récents.
   >
   >L’indicateur s’affiche uniquement après l’envoi du commentaire sur l’élément, et non lorsque le commentaire est toujours composé.
   >
   >L’indicateur &quot;Nouveau&quot; s’affiche uniquement lorsque l’utilisateur qui a saisi une nouvelle mise à jour, ainsi que celui qui a saisi une mise à jour, utilisent tous deux la nouvelle expérience de commentaire.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. Cliquez sur **Envoyer** pour ajouter la mise à jour à l’objet Workfront.
1. (Facultatif) Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) dans le coin supérieur droit du commentaire, puis cliquez sur **Modifier**.

   >[!IMPORTANT]
   >
   >Vous ne pouvez modifier votre commentaire que dans les 15 minutes suivant son envoi.

1. Modifiez les informations du commentaire, ajoutez ou supprimez des images ou supprimez l’un des utilisateurs balisés. Un indicateur &quot;Modifié&quot; est ajouté à gauche de l’horodatage qui s’affiche lorsque le commentaire a été saisi.

   >[!TIP]
   >
   >Les commentaires de l’année en cours n’affichent pas l’année dans l’horodatage. Le survol d’un horodatage affiche la date complète, y compris l’année.


   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >* Un message électronique est généré pour informer les utilisateurs de votre mise à jour uniquement lorsque vous envoyez la mise à jour d’origine. Aucun email n&#39;est généré après avoir modifié votre mise à jour.
   >* L’horodatage en regard du commentaire correspond à la date du commentaire d’origine, et non à celle de la dernière modification.
   >* Lorsque vous ajoutez un commentaire au nom d’un autre utilisateur (lorsque vous vous connectez en tant qu’autre utilisateur en tant qu’administrateur Workfront ou de groupe), vous ne pouvez pas le modifier si vous êtes connecté en tant qu’autre utilisateur. Vous ne pouvez modifier le commentaire qu’après vous être déconnecté en tant qu’utilisateur et vous être reconnecté vous-même.


1. (Facultatif) Cliquez sur **Répondre** ou commencez à saisir un commentaire dans la variable **Ajouter une réponse ...** , pour répondre à un commentaire existant, puis suivez les étapes 4 à 8 ci-dessus. <!--(**************insure this stays accurate***********)--> Pour plus d’informations sur la réponse à une mise à jour, voir [Répondre aux mises à jour](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

1. (Conditionnel et facultatif) Si d’autres utilisateurs ont ajouté des commentaires qui s’affichent en dehors de la zone visible dans la section Mises à jour pendant que vous ajoutiez vos commentaires, cliquez sur **Affichage** à l’intérieur du bleu **nouvelle bannière de commentaires** en bas de l’écran pour afficher ces commentaires.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   D’autres commentaires s’affichent en bas de l’écran.


   >[!NOTE]
   >
   >   L’indicateur &quot;nouveaux commentaires&quot; et le bouton &quot;Afficher&quot; s’affichent uniquement lorsque les utilisateurs qui ont saisi les nouvelles mises à jour, ainsi que l’utilisateur qui examine actuellement la section Mises à jour, utilisent tous deux la nouvelle expérience de commentaire.

1. (Facultatif) Cliquez sur le **Comme** icon![](assets/like-icon.png). L’icône se met à jour avec le nombre de mentions &quot;J’aime&quot;.
1. (Conditionnel et facultatif) Si vous avez inclus des personnes supplémentaires dans votre commentaire, cliquez sur le nombre de membres inclus dans la mise à jour pour afficher une liste des entités avec lesquelles le commentaire que vous avez saisi est partagé.

   ![](assets/members-icons-expanded-unshimmed.png)

   >[!TIP]
   >
   >Les noms des deux premières entités balisées s’affichent en regard de leurs avatars. Si plus de deux entités ne sont balisées que le nom du premier et que le nombre d’entités supplémentaires s’affiche.

1. (Facultatif) Cliquez sur le **Activité du système** pour afficher les mises à jour enregistrées par le système. Lorsque l’objet ou l’un de ses enfants est mis à jour, Workfront génère une note à ce sujet et l’affiche dans l’onglet Activité du système .

   Pour plus d’informations, voir [Présentation de la section Mises à jour](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >Vous ne pouvez pas ajouter de commentaire à une mise à jour du système.

## Utilisation de texte enrichi dans une mise à jour Workfront{#use-rich-text-in-a-workfront-update}

<!--October 2023: remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.-->

>[!NOTE]
>
>Les informations suivantes décrivent l’utilisation du texte enrichi dans la nouvelle expérience de commentaire, sauf indication contraire.

Vous pouvez améliorer vos mises à jour en utilisant du texte enrichi ou en y ajoutant divers éléments, tels que des émoticônes, des liens ou des images.

1. Accédez au **Mises à jour** d’un objet Workfront et commencez à saisir un commentaire.
1. (Facultatif) Pour ajouter un formatage de texte enrichi à votre mise à jour, utilisez n’importe quel attribut de la variable **Texte enrichi** au fur et à mesure que vous tapez.

   ![](assets/rich-text-toolbar.png)

   <!--October 2023: the individual icons in the toolbar will need replacing-->

   | **Attribut** | **Bouton Barre d’outils** | **Raccourcis clavier Mac** | **Raccourcis clavier Windows** |
   |---|---|---|---|
   | Gras | ![](assets/mceclip10.png) | épargner+b | Ctrl+B |
   | Italique | ![mceclip9.png](assets/mceclip9.png) | %+i | Ctrl+I |
   | Souligner | ![mceclip8.png](assets/mceclip8.png) | %+u | Ctrl+U |
   | Lien hypertexte | ![mceclip7.png](assets/mceclip7.png) | <br>Pour ouvrir le champ Ajouter des liens , procédez comme suit : CAS+K</br> <br>Pour coller un lien sur le texte sélectionné : jamais + V</br> | <br>Pour ouvrir la boîte de dialogue Ajouter des liens : Ctrl+K</br> <br>Pour coller un lien sur le texte sélectionné : Ctrl+V</br> |
   | Liste à puces | ![mceclip6.png](assets/mceclip6.png) | Greatest + Maj + 8 | Ctrl+Maj+8 |
   | Liste numérotée | ![mceclip5.png](assets/mceclip5.png) | Greatest + Maj + 7 | Ctrl+Maj+7 |
   | Citation | ![](assets/block-quote-icon-large.png) | Greatest + Maj + 9 | <br>Ctrl+Maj+9</br> <br>Cette option n’est pas disponible dans la nouvelle expérience de commentaire. </br> |

   <!--remove the last row when we remove legacy from the system-->

   Pour arrêter le formatage du texte, désélectionnez l’attribut sur la **Texte enrichi** barre d’outils.


   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment - with October 2023-->

   >[!NOTE]
   >
   >* Le formatage s’affiche également dans toutes les notifications électroniques que les utilisateurs reçoivent contenant votre mise à jour.
   >* Le formatage de texte enrichi appliqué à une mise à jour dans un email ne s’affiche pas sur la mise à jour lors de son affichage dans l’onglet Mises à jour .
   >* Si votre entreprise utilise Workfront avec Internet Explorer, tout texte formaté collé dans une mise à jour perd sa mise en forme de texte enrichi et s’affiche en tant que texte brut. Vous pouvez reformater le texte à l’aide des attributs de la barre d’outils Texte enrichi.
   >* La mise en forme de texte enrichi n’est pas disponible pour les mises à jour effectuées dans la zone Fiches horaires ou pour les objets Remarque et Dernière condition affichés dans un rapport.

1. (Facultatif et conditionnel) Si vous souhaitez inclure du texte provenant de mises à jour précédentes ou d’autres sources et le distinguer de votre propre mise à jour, vous pouvez le marquer comme une citation de bloc. Cliquez sur le bouton **Blocs de citations** icon ![](assets/block-quote-small.png) et tapez le texte que vous souhaitez citer. Le texte entre guillemets s’affiche avec une ligne grise verticale. Cliquez sur le bouton **Blocs de citations** pour revenir à la mise en forme normale. Cette option n’est pas disponible dans la nouvelle expérience de commentaire.

   <!--remove this picture below and the bullet above when we remove legacy-->

   ![](assets/block-quote-marked-350x144.png)</span>

1. (Facultatif) Cliquez sur le **émoji** icon ![](assets/emoji-icon.png) pour ajouter des émoticônes à votre mise à jour.

   >[!NOTE]
   >
   >* Workfront ne remplace pas les émoticônes de ponctuation telles que :) par des émoticônes.
   >* Les émoticônes ne sont pas disponibles pour les objets Remarque et Dernière condition affichés dans un rapport.
   >* La fonction d’émoticône de Workfront utilise des caractères Unicode et, en tant que tels, s’affiche uniquement sur les navigateurs et les systèmes d’exploitation qui prennent en charge les points de code Unicode. Les utilisateurs utilisant une plateforme, un navigateur ou une version de système d’exploitation différente de la vôtre peuvent ne pas avoir accès aux mêmes émoticônes.
   >* Une émoticône non prise en charge est représentée par une boîte noire ou blanche.
   >* Windows 7 ne prend en charge que les émoticônes en noir et blanc.
   >* Les émoticônes qui sont appliqués à une mise à jour effectuée par courrier électronique ne s’affichent pas sur la mise à jour lors de l’affichage dans la zone Mises à jour .

1. (Facultatif) Pour ajouter un lien URL vers des sources d’informations supplémentaires :

   1. Cliquez dans la mise à jour où vous souhaitez insérer un lien.
   1. Sur le **Texte enrichi** , cliquez sur **Lien hypertexte** icon ![](assets/link-icon.png).

   1. Dans le **Créer un lien** s’affiche, sous **URL**, saisissez ou collez l’URL de la source à laquelle vous souhaitez créer un lien.

   1. Sous **Texte à afficher**, saisissez ou collez le texte du lien.
   1. Cliquer sur **Enregistrer**.

1. (Facultatif) Pour joindre une image à votre mise à jour, effectuez l’une des opérations suivantes :

   * <span class="preview">Enregistrez l’image sur votre ordinateur, puis faites-la glisser et déposez-la dans la zone Nouveau commentaire.</span>
     <span class="preview">Cette option n’est pas disponible dans l’environnement de production pour la nouvelle expérience de commentaire. Vous pouvez faire glisser et déposer une image dans un commentaire dans l’expérience de commentaire héritée dans Production. </span>

   * <span class="preview">Copiez une capture d’écran de votre ordinateur, puis collez-la dans le commentaire. </span>
   * Cliquez sur le bouton **Ajouter une image** icon ![](assets/add-image-mountain-with-plus-icon.png) et accédez à l’image sur votre ordinateur.


   >[!NOTE]
   >
   >* Votre administrateur Workfront doit activer l’ajout d’images dans la section Mettre à jour les préférences des flux de la zone Interface de Workfront avant de pouvoir voir les icônes Image ou Ajouter une pièce jointe. Pour plus d’informations, voir [Configuration des préférences pour les mises à jour des utilisateurs](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* La taille maximale du fichier image est de 7 Mo. Les types de fichiers image pris en charge sont .jpg, .gif et .png.
   >* Les images sont accessibles à partir de la section Mises à jour d’un objet et elles sont également disponibles dans la zone Documents sous le menu principal.
   >* <span class="preview">Vous pouvez coller l’image en cliquant avec le bouton droit dans le nouveau commentaire, ou en appuyant sur Ctrl + V pour Windows (ou CMD + V pour Mac) sur votre clavier.</span>
   >* Vous pouvez envoyer une mise à jour avec une image et sans texte.
   >* Lorsque vous supprimez un commentaire qui contient une image, les scénarios suivants existent selon l’expérience choisie :
   >
   >     * Dans l’expérience de commentaire héritée, l’image reste dans la zone Documents, mais n’est plus visible dans la section Mises à jour .
   >     * Dans la nouvelle expérience de commentaire, l’image est supprimée de la section Mises à jour , ainsi que de la zone Documents . L’image est également supprimée de la zone Documents lorsque vous modifiez un commentaire et supprimez l’image.
   >* Lorsqu’une personne supprime une image jointe à un commentaire de la zone Documents, elle est également supprimée du commentaire.

   <!--remove the statement above about legacy, when we remove the legacy environment.-->

1. (Facultatif) Pour afficher une image dans la mise à jour existante, effectuez l’une des opérations suivantes :

   * Cliquez sur le bouton **Aperçu** icon <span class="preview">![](assets/previewimageicon-31x31.png)</span> sur la miniature de l’image pour ouvrir l’image en taille réelle dans un nouvel onglet du navigateur.
   * Cliquez sur le bouton **Télécharger** icon ![](assets/downloadimageicon.png) sur la miniature de l’image pour télécharger l’image.

1. Cliquez sur **Envoyer** pour ajouter votre commentaire.

<div class="preview">

## Rechercher une mise à jour

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement pour l’onglet Commentaires de la nouvelle expérience de commentaire. Cette option n’est pas disponible pour l’onglet Activité du système de la section Mises à jour .

Vous pouvez rechercher un commentaire ou une réponse dans la section Mises à jour d’un objet.

1. Accédez au **Mises à jour** d’un objet.
1. Commencer à saisir un mot-clé <!--or a user's name --> dans le **Rechercher** dans le coin supérieur droit de la **Commentaires** .

   <!--Add this tip when it'll be possible: You can search for users who have been tagged or for comment owners.-->

   ![](assets/search-field-in-updates-tab.png)

   Le mot-clé <!--or user--> La recherche effectuée est mise en surbrillance et les commentaires qui la contiennent s’affichent en haut de la section Mises à jour .

   Workfront recherche l’intégralité du flux de mise à jour de l’objet, en dehors des commentaires visibles à l’écran.

1. Cliquez sur le bouton **x** dans le champ de recherche pour effacer les résultats de la recherche et revenir à tous les commentaires.

</div>

<!-- when we release search to production, check above and make sure you don't have to add that the users tagged/ owners are also searchable-->

## Copie des informations de mise à jour

Il existe plusieurs façons de copier une mise à jour. Après avoir copié un lien, vous pouvez le partager avec d’autres personnes afin de les rediriger vers la mise à jour.

La copie d’une mise à jour varie en fonction de l’expérience de commentaire que vous utilisez.

### Copier une mise à jour dans la nouvelle expérience de commentaire

Pour plus d’informations sur les fonctionnalités disponibles pour la nouvelle expérience de commentaire et pour les objets, voir [Nouvelle expérience de commentaire](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--when we remove and deprecate the legacy stream, add screen shots in the sections below- October 2023-->

Vous pouvez copier des informations d’un commentaire existant en effectuant l’une des opérations suivantes :

* [Copier le lien](#copy-link)
* [Copier le texte du message](#copy-body-text)
* [Réponse entre guillemets](#quote-reply-1)

![](assets/copy-comment-ways-from-more-menu-on-comment.png)

#### Copier le lien

L’option Copier le lien copie le lien du commentaire ou du fil dans le Presse-papiers afin que vous puissiez partager le commentaire ou l’intégralité du fil avec d’autres utilisateurs.

1. Accédez à la mise à jour du lien dont vous souhaitez copier le lien.

1. Cliquez sur le bouton **Plus** , puis cliquez sur **Copier le lien**.

1. Collez le lien que vous avez copié à l’étape précédente dans un email ou dans une autre application pour le partager avec d’autres personnes. Le lien partagé ouvre le commentaire à partir duquel vous avez partagé le lien.

   >[!TIP]
   >
   >Lorsque vous partagez le lien d’une conversation sur un objet enfant à partir d’un objet de rang supérieur, le lien ouvre le thread dans la zone Mises à jour de l’objet de rang supérieur.
   >
   >Par exemple, si vous copiez le lien d’un commentaire de tâche dans la zone Mises à jour du projet, le commentaire ouvre la page du projet.

#### Copier le texte du message

L’option Copier le texte du corps copie le texte d’une mise à jour spécifique dans le Presse-papiers.

1. Accédez à la mise à jour ou à la réponse que vous souhaitez copier.
1. Cliquez sur le bouton **Plus** , puis cliquez sur **Copier le texte du corps**.

#### Réponse entre guillemets

L&#39;option Réponse entre guillemets copie le commentaire d&#39;origine dans une nouvelle réponse sous forme de citation bloquée.

1. Accédez à la mise à jour ou à la réponse que vous souhaitez copier.
1. Cliquez sur le bouton **Plus** , puis cliquez sur **Réponse entre guillemets**.

   Une nouvelle zone de commentaire s’ouvre et la réponse entre guillemets est incluse dans le nouveau commentaire et est marquée comme une citation bloquée.

   ![](assets/block-quote-highlighted-mid-comment-before-submit.png)

   <!--ensure the screen shot above is correct - missing he block quote icon in rich text -->

1. Continuez à ajouter votre mise à jour et cliquez sur **Envoyer** pour ajouter le commentaire.

### Copie d’une mise à jour dans l’expérience de commentaire héritée

<!--remove legacy when removed from the UI-->

* [Copier la mise à jour](#copy-the-update)
* [Copier le lien du thread](#copy-the-thread-link)
* [Copier le lien de mise à jour](#copy-the-update-link)
* [Citer la réponse](#quote-reply)

  >[!TIP]
  >
  >Lorsque vous copiez et partagez le lien d’une conversation sur un objet enfant à partir d’un objet de rang supérieur, le lien ouvre le thread dans la zone Mises à jour de l’objet enfant.
  >
  >Par exemple, si vous copiez le lien d’un commentaire de tâche dans la zone Mises à jour du projet, le commentaire ouvre la page de la tâche.

#### Copier la mise à jour {#copy-the-update}

Cette option copie le texte d’une mise à jour spécifique dans le Presse-papiers.

1. Accédez à la mise à jour ou à la réponse que vous souhaitez copier.
1. Cliquez sur le bouton **Plus** , puis cliquez sur **Copier le texte du corps**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### Copier le lien du thread {#copy-the-thread-link}

Cette option copie le lien de thread complet dans le Presse-papiers afin que vous puissiez partager le thread avec d’autres utilisateurs.

1. Accédez au thread de mise à jour que vous souhaitez copier.

1. Cliquez sur le bouton **Plus** , puis cliquez sur **Copier le lien du thread**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Collez le lien que vous avez copié à l’étape précédente dans un email ou dans une autre application pour le partager avec d’autres personnes. Le lien partagé ouvre le commentaire à partir duquel vous avez partagé le lien.

#### Copier le lien de mise à jour {#copy-the-update-link}

Cette option copie un lien de mise à jour spécifique dans le Presse-papiers. Lorsque vous partagez le lien de mise à jour, l’utilisateur qui le suit voit une bordure autour de la mise à jour.

1. Accédez à la mise à jour ou à la réponse que vous souhaitez copier.
1. Cliquez sur le bouton **Plus** en regard de la mise à jour, cliquez sur **Copier le lien de mise à jour**.

   ![](assets/copy-update-link-old-ui.png)

1. Collez le lien que vous avez copié à l’étape précédente dans un email ou dans une autre application pour le partager avec d’autres personnes. Le lien partagé ouvre le commentaire à partir duquel vous avez partagé le lien.

#### Citer la réponse

L’option Réponse à la citation copie le commentaire d’origine dans une nouvelle réponse sous forme de citation bloquée.

1. Accédez à la mise à jour ou à la réponse que vous souhaitez copier.
1. Cliquez sur le bouton **Plus** , puis cliquez sur **Réponse de devis**.

   Une nouvelle zone de commentaire s’ouvre et la réponse entre guillemets est incluse dans le nouveau commentaire et est marquée comme une citation bloquée.

1. Continuez à ajouter votre mise à jour et cliquez sur **Répondre** pour ajouter le commentaire.

## Supprimer une mise à jour ou une réponse

Selon l’accès que votre administrateur Workfront vous donne, vous pouvez supprimer les mises à jour que vous avez ajoutées dans l’onglet Mises à jour d’un objet . Pour plus d’informations, voir [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) dans l’article [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Aucun utilisateur Workfront (y compris l’administrateur Workfront) ne peut supprimer les mises à jour effectuées par un autre utilisateur. Cependant, si le niveau d’accès d’un utilisateur lui permet de supprimer ses propres mises à jour, l’administrateur Workfront peut se connecter en tant qu’utilisateur et supprimer les mises à jour qu’il a effectuées. Pour plus d’informations, voir [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) et [Connexion en tant qu’autre utilisateur](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Accédez à la mise à jour ou à la réponse que vous souhaitez supprimer.
1. Cliquez sur le bouton **Plus** en regard de la mise à jour ou de la réponse que vous souhaitez supprimer, puis cliquez sur **Supprimer**. <!--October 2023 - replace screen shot here-->

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Dans le message qui apparaît, cliquez sur **Supprimer**.

   >[!NOTE]
   >
   >La suppression d’une mise à jour avec une image jointe supprime à la fois le commentaire et l’image. Pour plus d’informations, voir [Utilisation de texte enrichi dans une mise à jour Workfront](#use-rich-text-in-a-workfront-update) dans cet article.

   Lorsque des réponses sont associées au commentaire que vous supprimez, il est indiqué que le commentaire a été supprimé avec le nom de l’utilisateur qui l’a supprimé.

   ![](assets/removed-comment-indicator-new-experience.png)

   Les commentaires supprimés sont immédiatement supprimés de Workfront. Un utilisateur qui utilise la section Mises à jour voit un commentaire supprimé par un autre utilisateur en temps réel.

   <!--when we remove the beta, take out the first part of the sentence above about only when commenting in beta experience. Leave the rest though-->

<!--this is no longer needed - adding timesheet comments is just like adding comments to any other object now

## Add an update on a Timesheet

1. Go to a Timesheet on which you want to make an update.
1. Click the Timesheet to open it.
1. At the bottom of the Timesheet, click **Include a comment**.
1. In the box that displays at the bottom of the Timesheet, type an update.

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (Conditional) To save your update without submitting the Timesheet for approval, click **Save for Later**.

   Or

   To save your update and submit the Timesheet for approval, click **Submit for Approval**.

   Or

   If your Timesheet is not set up with an approver, click **Save and Close Timesheet** to save your update.

-->



## Activation ou désactivation des mises à jour système

<!--update this section when we remove legacy, to just point to the article in green below and rename this section as "Review system activity updates" or something-->

<!--October 2023: when the new stream goes to all objects production, consider updating this article also, to say there is no System Activity tab to be disabled for objects anymore: help\quicksilver\administration-and-setup\set-up-workfront\system-tracked-update-feeds\system-tracked-update-feeds.md-->

>[!NOTE]
>
>Il n’est pas possible de désactiver les mises à jour système lors de l’utilisation de la nouvelle expérience de commentaire.
>Les informations de cette section se rapportent uniquement aux fonctionnalités disponibles dans la section Mises à jour héritées . &lt;!—Supprimez cette section lorsque nous supprimons les éléments hérités du système->
>Pour plus d’informations sur les mises à jour du système dans la nouvelle expérience de commentaire, voir [Présentation de la section Mises à jour](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

La section Mises à jour d’un objet Workfront affiche deux types d’informations :

* **Mises à jour de l’utilisateur :** Les mises à jour des utilisateurs sont des commentaires que vous et d’autres utilisateurs de votre système saisissez. <!--October 2023 - new screen shot -->

  ![](assets/user-update-cl-350x277.png)

* **Mises à jour système :** Le système met à jour l’enregistrement de suppression des ressources, d’ajout ou de suppression de versions, de pièce jointe ou de suppression d’une demande d’approbation, ainsi que des modifications ou modifications apportées aux documents sur l’objet. <!--October 2023 - new screen shot -->

  ![](assets/system-updates-cl-350x277.png)

  Selon votre licence Workfront, les mises à jour système peuvent être activées par défaut. Les administrateurs de Workfront peuvent déterminer ce qui est suivi dans les mises à jour du système, comme expliqué dans la section [Mises à jour suivies par le système](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). Vous pouvez également filtrer les mises à jour système ou les activités afin de n’afficher que les mises à jour utilisateur pour tous les objets.

  Les objets suivants ne comportent pas de mises à jour générées par le système :

   * Équipe
   * Modèle
   * Tâche de modèle

Pour activer ou désactiver les mises à jour du système :

1. Cliquez sur le bouton **Mises à jour** sur un objet.
1. Cliquez sur **Afficher les mises à jour du système** pour faire glisser le commutateur vers la gauche (désactivé) ou la droite (activé).

   ![](assets/show-system-updates-qs-350x55.png)

   Cette option est persistante dans tous les objets de Workfront et reste à l’emplacement sélectionné, même si vous vous déconnectez de Workfront.

   >[!TIP]
   >
   >   Les objets qui n’enregistrent pas les mises à jour système n’ont pas l’option Afficher les mises à jour système dans leur zone Mises à jour.

   <!--when Anna adds the new updates stream to ALL objects, she will remove the System Activity tab from the objects that don't record system updates - add another line to the TIP above to say: The System Activity tab is not available for objects that don't record system-generated updates.*************** OR: maybe make this part of the statement where we list which objects these are, above???  -->


