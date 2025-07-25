---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Planifier la remise automatique d’un rapport
description: Planifier la remise automatique d’un rapport
author: Courtney
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 62f56486ccc590921b7dc8227d46cdede84df32d
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 66%

---

# Planifier la remise automatique d’un rapport

<!-- Audited: 4/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Vous pouvez planifier la remise automatique des rapports aux utilisateurs et aux utilisatrices selon un calendrier défini ou envoyer manuellement et ponctuellement des rapports. Lorsque vous envoyez un rapport à partir de Adobe Workfront, la personne reçoit un e-mail contenant le rapport Workfront dans une pièce jointe séparée.

Pour plus d’informations, y compris les limites de taille qui peuvent affecter la remise de vos rapports, voir [Vue d’ensemble des remises de rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
      <td> 
      <p>Nouveau : Standard</p>
      <p>Ou</p>

<p>Actuel : formule</p>

</td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et regroupements</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer, vous devez créer un rapport. Pour en savoir plus sur la création de rapports, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Planifier la diffusion d’un rapport


Pour planifier la diffusion automatique d&#39;un rapport, procédez comme suit &#x200B;

{{step1-to-reports}}

>[!NOTE]
>
>Les remises de rapports ne contiennent pas d’invites. Si vous souhaitez limiter des données dans une remise de rapport, nous vous conseillons d’appliquer des filtres au rapport que vous souhaitez envoyer.

1. Sélectionnez un rapport sur la page **Rapports**.
1. Dans la partie supérieure de l’écran, cliquez sur **Actions du rapport**, puis **Envoyer le rapport** dans la liste déroulante qui s’affiche. La boîte de dialogue **Envoyer le rapport** s’affiche.

   >[!TIP]
   >
   >Pour envoyer manuellement un rapport à tout moment, accédez au rapport, puis cliquez sur **Actions de rapport** > **Envoyer le rapport** > **Envoyer maintenant**.

1. Cliquez sur l’onglet **Remises répétées**.
1. (Conditionnel) Pour modifier une diffusion de rapport répétée existante, sélectionnez la diffusion de rapport dans la section **Diffusions répétées** sur le côté droit de la boîte de dialogue.
1. Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Envoyer à</p> </td> 
      <td> <p>Commencez à saisir le nom de l’utilisateur, de l’utilisatrice, du groupe, de l’équipe ou du rôle à qui vous souhaitez envoyer le rapport, puis cliquez sur le nom quand il s’affiche dans la liste déroulante.</p> <p>Ou</p> <p>Saisissez l’adresse e-mail d’une personne externe au système Workfront à laquelle vous souhaitez accorder l’accès au rapport.</p> <p>Répétez cette procédure pour envoyer le rapport à plusieurs utilisateurs, utilisatrices, groupes, équipes ou rôles.</p> <p>Note :  <p>Tenez compte des points suivants lors de l’ajout de personnes destinataires de remises de rapports :</p> 
        <ul> 
         <li><p>Si votre entreprise limite les notifications Workfront à des domaines d’e-mail spécifiques, vous ne pourrez peut-être envoyer des rapports qu’aux adresses e-mail répertoriées dans la place sur la liste autorisée e-mail.</p> <p>Par exemple, lorsque l’utilisateur est défini comme destinataire de rapport et possède une adresse e-mail qui était précédemment autorisée, et que la place sur la liste autorisée est mise à jour pour ne plus diffuser d’e-mails vers ce domaine, l’utilisateur ne recevra plus les rapports diffusés.</p><p>Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront met à jour la liste autorisée des adresses e-mails, voir la section <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Configurer votre liste autorisée d’adresses e-mail</a>.</p></li> 
         <li> <p>L’ajout d’un grand nombre d’utilisateurs et d’utilisatrices en tant que destinataires peut entraîner un échec de la remise. Si vous rencontrez des échecs de remise, vous pouvez planifier plusieurs remises de rapports avec des groupes d’utilisateurs et d’utilisatrices plus petits.</p> </li> 
        </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Objet de l'e-mail</p> </td> 
      <td> <p>Saisissez l’objet de l’e-mail de notification.</p> <p>Par défaut, l’objet de l’e-mail est :</p> <p><em>Rapport Workfront : [Nom du rapport] [Date]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Message électronique</p> </td> 
      <td> <p>Saisissez un message à inclure dans l’e-mail.</p> <p>Par défaut, le message e-mail est :</p> <p><em>Vous trouverez ci-joint le rapport [fréquence du rapport] [nom du rapport] généré par Workfront le [date].</em> </p> <p>Note : pour les rapports remis sous forme de fichier Excel uniquement, le message suivant est également ajouté à l’e-mail : « Gardez à l’esprit qu’avec les types de fichiers MS Excel (XLS), une limite s’applique (65 530) au nombre de liens hypertexte pris en charge par ces types de fichiers. Si vous dépassez ces limites, votre fichier ne s’ouvrira pas et il est recommandé de le renvoyer sans les liens hypertexte. Revenez au planificateur de rapports pour supprimer les liens hypertexte et renvoyer le rapport. » L’expression « Revenez au planificateur de rapports » est un lien renvoyant au rapport.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Remettre ce rapport avec les droits d’accès suivants</p> </td> 
      <td> <p>Commencez à saisir le nom d’une personne ayant accès au rapport, puis cliquez sur le nom qui apparaît dans la liste déroulante. Les personnes qui reçoivent le rapport auront le même niveau d’accès à ce dernier que la personne spécifiée ici.<br> Pour plus d’informations, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Exécuter et diffuser un rapport avec les droits d’accès d’un autre utilisateur ou d’une autre utilisatrice</a>.</p> <p>Note : ce champ ne prend pas en charge les caractères génériques. Par exemple, le caractère générique <em>$$User.ID</em> n’exécute pas le rapport avec les droits d’accès de l’utilisateur qui reçoit le rapport.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Format</p> </td> 
      <td> <p>Sélectionnez le format souhaité pour le rapport remis :</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Si vous sélectionnez PDF, vous pouvez mettre en forme la sortie à l’aide des options supplémentaires <strong>Format du papier</strong> et <strong>Orientation</strong> qui s’affichent.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Inclure des liens</p> </td> 
      <td> <p>Cette option est disponible uniquement lorsque <strong>MS Excel</strong> est sélectionné dans le menu déroulant <strong>Format</strong>. Lorsque cette option est activée, tous les liens hypertexte sont inclus dans le document Excel exporté.</p> <p>Les documents contenant plus de 65 530 liens ne peuvent pas être ouverts. Si le document exporté contient plus de 65 530 liens, désélectionnez cette option.</p> <p>Cette option est activée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Résumé</p> </td> 
      <td> <p>Affiche un résumé du moment où la remise se répète.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se répète</p> </td> 
      <td> <p>Indiquez la fréquence de remise du rapport : quotidienne, hebdomadaire, mensuelle ou annuelle.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se répète tous les</p> </td> 
      <td> <p>Sélectionnez la fréquence de répétition de la remise. La valeur que vous sélectionnez pour cette option est basée sur l’option sélectionnée dans la liste déroulante <strong>Répéter</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Heure</p> </td> 
      <td> <p>Sélectionnez l’heure de la journée à laquelle vous souhaitez envoyer la remise.</p> <p>Conseil : les chargements du système pouvant affecter les délais de livraison des rapports, il peut y avoir un délai de jusqu'à 24 heures entre l'heure planifiée et l'heure réelle de livraison. Si vous devez remettre un rapport à une heure spécifique, nous vous recommandons de planifier la remise au préalable. En règle générale, nous vous recommandons de planifier la diffusion au moins un jour avant la date à laquelle elle est nécessaire.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se répète le</p> </td> 
      <td> <p>Cette option est disponible lorsque l’option <strong>Répéter</strong> est définie sur <strong>Hebdomadaire</strong> ou <strong>Mensuel</strong> :</p> 
       <ul> 
        <li> <p>Lorsque l’option <strong>Répéter</strong> est définie sur <strong>Hebdomadaire</strong> : sélectionnez les jours de la semaine où la remise est envoyée.</p> </li> 
        <li> <p>Lorsque l’option <strong>Répéter</strong> est définie sur <strong>Mensuel</strong> : choisissez si la remise est envoyée le jour du mois, le jour de la semaine ou le dernier jour du mois (ces options utilisent la date que vous avez sélectionnée dans le champ <strong>Commence le</strong>).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Commence le</p> </td> 
      <td>Sélectionnez la date de début de la remise planifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se termine le</p> </td> 
      <td>Sélectionnez la date de fin de la remise planifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Jamais</p> </td> 
      <td>Sélectionnez <strong>Jamais</strong> si vous souhaitez que la remise planifiée dure indéfiniment.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer** pour enregistrer la diffusion du rapport. Le rapport s’affiche dans la section **Diffusions répétées** de la boîte de dialogue **Envoyer le rapport** et sera envoyé à l’heure planifiée.

   Pour plus d’informations sur les limitations de taille qui peuvent affecter la remise de vos rapports, consultez les sections [Limitations des remises de rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) et [Limitations d’export](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

>[!IMPORTANT]
>
>Les rapports planifiés sont soumis à un délai interne lors de leur traitement pour diffusion. Dans le cas où un rapport dépasse la limite d&#39;envoi, vous recevrez une notification et le rapport ne sera plus diffusé indépendamment des autres diffusions planifiées. Pour continuer à envoyer le rapport, essayez d’abord de réduire sa taille à l’aide de filtres et de vues, puis créez une diffusion planifiée.
>
>Si vous utilisez une diffusion de rapports planifiée pour analyser les données de Workfront par le biais d’un outil BI, nous vous recommandons d’utiliser plutôt Workfront Data Connect. Pour plus d&#39;informations, consultez [Présentation de Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

## Supprimer une diffusion de rapports planifiée

Pour supprimer une diffusion de rapports planifiée, procédez comme suit &#x200B;

{{step1-to-reports}}

1. Sélectionnez un rapport sur la page **Rapports**.

1. Dans la partie supérieure de l’écran, cliquez sur **Actions du rapport**, puis **Envoyer le rapport** dans la liste déroulante qui s’affiche. La boîte de dialogue **Envoyer le rapport** s’affiche.

1. Cliquez sur l’onglet **Remises répétées**.
1. Dans la section **Diffusions répétées** sur le côté droit de la boîte de dialogue, cliquez sur la diffusion planifiée à supprimer.
1. Dans la section détaillée **Diffusions répétées**, cliquez sur **Supprimer**.

1. Cliquez sur **Supprimer** pour confirmer.

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![Video walkthrough of report delivery](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
