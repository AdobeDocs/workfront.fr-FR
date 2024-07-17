---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configurer [!DNL Adobe Workfront for Jira]
description: Vous pouvez utiliser  [!DNL Adobe Workfront for Jira] pour intégrer vos systèmes  [!DNL Jira] et [!DNL Workfront] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '2384'
ht-degree: 2%

---

# Configurer [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->

Vous pouvez utiliser [!DNL Adobe Workfront for Jira] pour intégrer vos systèmes [!DNL Jira] et [!DNL Workfront].

Après l’installation du module complémentaire, vous pouvez définir des workflows qui créent automatiquement des problèmes [!DNL Jira] lors de la création d’éléments de travail [!DNL Workfront]. Les éléments des deux applications sont liés et certaines de leurs informations sont automatiquement mises à jour dans les deux systèmes.

Tous les utilisateurs de [!DNL Workfront] et [!DNL Jira] peuvent bénéficier de cette intégration. Ils n&#39;ont besoin d&#39;une licence que pour le système dans lequel ils travaillent le plus, et non pour les deux systèmes.

Ce module complémentaire est disponible pour les versions [!UICONTROL Server] et [!UICONTROL OnDemand] (ou [!UICONTROL Cloud]) du logiciel [!DNL Jira].

Pour obtenir la liste des [!DNL Jira] versions actuellement prises en charge par [!DNL Workfront for Jira], voir [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) sur le [!DNL Atlassian Marketplace].

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] plan]</td> 
   <td><p>Nouveau : Tous</p>
       <p>ou</p>
       <p>Actuel : [!UICONTROL Pro] ou version ultérieure</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard] </p>
       <p>ou</p> 
       <p>Actuelle : [!UICONTROL Plan] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Accès administrateur système</p> <p>Important : Nous vous recommandons de créer des comptes d’administrateur système distincts dans [!DNL Jira] et [!DNL Workfront] afin de vous consacrer à cette intégration, plutôt que d’utiliser des comptes existants pouvant être joints aux utilisateurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de pouvoir configurer [!DNL Workfront for Jira], vous devez :

* Installez [!DNL Workfront for Jira].
Pour plus d&#39;informations sur l&#39;installation de [!DNL Workfront for Jira], voir [Installation [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configurer [!DNL Workfront for Jira]

En configurant [!DNL Workfront for Jira], vous pouvez :

* Définissez des déclencheurs qui créeront [!DNL Jira] éléments lors de la création de [!DNL Workfront] éléments.
* Spécifiez les champs à synchroniser entre les éléments liés entre [!DNL Jira] et [!DNL Workfront].

>[!NOTE]
>
>* Une fois que vous avez configuré [!DNL Workfront for Jira] sur votre environnement [!DNL Jira], tous les utilisateurs [!DNL Jira] voient un panneau de droite [!DNL Workfront] sur tous les éléments [!DNL Jira]. Le panneau contient des informations sur les éléments qui peuvent être liés à partir de [!DNL Workfront] ou indique qu’aucun élément [!DNL Workfront] n’est lié à des éléments [!DNL Jira].
>* Lors de l’utilisation de l’installation [!DNL Jira Server], seuls les problèmes associés aux projets identifiés comme déclencheurs de l’intégration Workfront affichent le panneau Workfront. Pour plus d’informations sur la configuration des déclencheurs pour le workflow [!DNL Workfront to Jira], voir [Configuration des déclencheurs pour la liaison automatique d’éléments entre [!DNL Jira] et [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Pour configurer [!DNL Workfront for Jira] :

1. Connectez-vous à [!DNL Jira] en tant qu’administrateur [!DNL Jira].
1. Cliquez sur **[!UICONTROL Paramètres]** dans le menu principal [!DNL Jira].
1. Cliquez sur **[!UICONTROL Add-ons]**, puis sur **[!UICONTROL Gérer les modules complémentaires]**.

1. Développez le module complémentaire **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Suivez les invites pour vous connecter à [!DNL Workfront].

   >[!NOTE]
   >
   >L’utilisateur doit disposer d’un `apiKey` valide dans [!UICONTROL Workfront] pour créer une connexion réussie.

   Vous devez vous connecter à [!DNL Workfront] en tant qu&#39;administrateur [!DNL Workfront] pour continuer la configuration.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] se connecte à [!DNL Jira] à l’aide d’OAuth 2.0, une norme utilisée par la plupart des intégrations web pour l’authentification et l’autorisation des utilisateurs.
   >* Lorsque vous êtes invité à saisir le domaine de votre compte [!DNL Workfront], saisissez-le au format suivant : *yourCompany&#39;sDomain.my.workfront.com*. Le domaine de votre société correspond généralement au nom de votre société.
   >* L’authentification améliorée n’est pas disponible tant qu’un administrateur [!DNL Workfront] ne l’a pas activée pour cette intégration.

1. Dans Jira, sélectionnez l’onglet **[!UICONTROL Triggers]** pour configurer la création automatique de [!DNL Jira] éléments à mesure que de nouveaux [!DNL Workfront] éléments sont créés.

   Pour plus d’informations sur la configuration des déclencheurs pour le processus Workfront vers [!DNL Jira], voir [Configuration des déclencheurs pour la liaison automatique d’éléments entre [!DNL Jira] et [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Sélectionnez l&#39;onglet **[!UICONTROL Setup]** pour configurer la synchronisation des champs entre les éléments [!DNL Jira] et [!DNL Workfront] liés.

   Pour plus d’informations sur la configuration de la synchronisation des champs entre [!DNL Jira] et [!DNL Workfront], voir [Configuration de la synchronisation des champs entre [!DNL Jira] et [!DNL Workfront] Éléments](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Après avoir défini les déclencheurs et la synchronisation des champs entre les deux applications, tout utilisateur [!DNL Workfront] pouvant créer des tâches ou des problèmes peut potentiellement déclencher la création d’un élément dans [!DNL Jira]. L’utilisateur peut créer un élément si les critères qu’il crée correspondent aux déclencheurs dans [!DNL Jira], même si l’utilisateur ne dispose pas d’une licence [!DNL Jira]. En outre, tout utilisateur de [!DNL Jira] peut immédiatement commencer à travailler sur l’élément [!DNL Jira] et ses mises à jour sont visibles dans [!DNL Workfront], sans disposer d’une licence [!DNL Workfront]. Toutes les mises à jour de [!DNL Workfront] sont également visibles sur les éléments [!DNL Jira] .

1. (Facultatif) Sélectionnez l’onglet **[!UICONTROL Journal d’activité]** pour passer en revue les erreurs qui se sont produites pendant l’intégration.

   Pour plus d’informations sur le [!UICONTROL journal des activités], voir [Affichage du [!DNL Jira] [!UICONTROL journal des activités]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configuration de déclencheurs pour la liaison automatique d’éléments entre [!DNL Jira] et [!DNL Workfront]

En tant qu&#39;administrateur système [!DNL Jira], vous pouvez définir des déclencheurs qui créeraient automatiquement des problèmes dans [!DNL Jira] lorsqu&#39;un élément de [!DNL Workfront] répond à certains critères.

>[!NOTE]
>
>L’intégration peut prendre jusqu’à 10 minutes pour créer de nouveaux problèmes dans [!DNL Jira].

Tenez compte de ce qui suit lors de la configuration du déclenchement de la création de [!DNL Jira] éléments lorsque [!DNL Workfront] éléments sont créés :

* L’intégration est unidirectionnelle : vous pouvez uniquement déclencher la création automatique d’éléments que vous créez dans [!DNL Workfront] dans [!DNL Jira]. Vous ne pouvez pas déclencher la création automatique d’éléments que vous créez dans [!DNL Jira] dans [!DNL Workfront].
* Le nombre de déclencheurs que vous pouvez avoir n’est pas limité.
* Si un élément que vous créez dans [!DNL Workfront] correspond à plusieurs des déclencheurs, un seul élément est créé dans [!DNL Jira]. L’élément est créé dans [!DNL Jira] en fonction du premier déclencheur (dans l’ordre dans lequel il a été défini dans [!DNL Jira]). Tous les autres déclencheurs sont ignorés.
* Un seul élément de [!DNL Workfront] peut être lié à un élément de Jira. Vous ne pouvez jamais lier un élément [!DNL Workfront] à plusieurs problèmes [!DNL Jira] ou un problème [!DNL Jira] à plusieurs éléments [!DNL Workfront].

Pour configurer des déclencheurs pour la création automatique d’éléments dans [!DNL Jira] :

1. Connectez-vous à [!DNL Jira] en tant qu’administrateur système.
1. Cliquez sur **[!UICONTROL Paramètres]** dans le menu principal [!DNL Jira].
1. Cliquez sur **[!UICONTROL Add-ons]**, puis **[!UICONTROL Gérer les modules complémentaires]**.
1. Développez le module complémentaire **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur système.

   L’onglet **[!UICONTROL Triggers]** est sélectionné par défaut dans Jira.

1. Cliquez sur **[!UICONTROL Ajouter un déclencheur]** pour ajouter un nouveau déclencheur.
1. Dans le champ **[!UICONTROL Équipe de Workfront/utilisateur/rôle]**, indiquez le nom d’une équipe [!DNL Workfront], d’un utilisateur ou d’un rôle de tâche, puis cliquez pour le sélectionner lorsqu’il s’affiche dans la liste.

   >[!NOTE]
   >
   >Vous ne pouvez pas avoir plusieurs déclencheurs pour une même équipe, un même utilisateur ou un même rôle.

   Lorsqu’une personne crée une tâche ou un problème et l’affecte à l’une de ces entités, un problème est automatiquement créé dans [!DNL [!DNL Jira]].

1. Dans le champ **[!UICONTROL [!DNL Jira]project]** , commencez à saisir le nom d’un projet [!DNL Jira], puis cliquez pour le sélectionner lorsqu’il s’affiche dans la liste.

   Lorsque le problème [!DNL Jira] est créé, il est placé sur le projet que vous avez choisi ici.

1. Sélectionnez un **I[!UICONTROL type de thème]** dans le menu déroulant.

   Cela indique le type de problème créé dans [!DNL Jira] lorsque les conditions de ce déclencheur sont remplies, en fonction de vos paramètres pour ce projet spécifique dans [!DNL Jira].

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Avec cette configuration, chaque fois qu’un utilisateur [!DNL Workfront] crée un élément correspondant aux déclencheurs spécifiés, un nouveau problème est créé dans [!DNL Jira].

## Configurer la synchronisation des champs entre [!DNL Jira] et [!DNL Workfront] éléments

En tant qu&#39;administrateur [!DNL Jira], vous pouvez définir les champs à synchroniser automatiquement sur les éléments liés entre [!DNL Workfront] et Jira. Certains champs peuvent se synchroniser de l’élément [!DNL Workfront] vers l’élément [!DNL Jira], tandis que d’autres se synchronisent de Jira vers Workfront.

Pour définir les champs à synchroniser automatiquement sur les éléments liés entre les deux applications :

1. Connectez-vous à [!DNL Jira] en tant qu’administrateur Jira.
1. Cliquez sur **[!UICONTROL Paramètres]** dans le menu principal [!DNL Jira].
1. Cliquez sur **[!UICONTROL Add-ons]**, puis **[!UICONTROL Gérer les modules complémentaires]**.
1. Développez le module complémentaire **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur Workfront.
1. Dans Jira, cliquez sur l’onglet **[!UICONTROL Setup]** .
1. Dans la section **[!UICONTROL Synchroniser de Workfront à Jira]** , sélectionnez les champs que vous souhaitez mettre à jour dans [!DNL Jira] lorsqu’ils sont mis à jour dans Workfront.

   1. Sélectionnez l&#39;une des fréquences avec lesquelles les champs sont synchronisés :

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL À La Création]</td>
              <td>Les champs que vous spécifiez sont synchronisés entre les éléments Workfront liés et [!DNL Jira] lorsque l’élément est créé dans Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Toujours]</td>
              <td>Les champs que vous spécifiez sont synchronisés entre les éléments Workfront liés et [!DNL Jira] lorsque les champs sont mis à jour dans Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Jamais]</td>
              <td>Les champs que vous spécifiez ne sont jamais synchronisés entre les éléments [!DNL Workfront] et [!DNL Jira] liés. Il n’y a aucune indication dans [!DNL Jira] que le champ a été mis à jour dans [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Sélectionnez l’une des options suivantes pour synchroniser les champs de [!DNL Workfront] à [!DNL Jira] :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Le nom d'une tâche ou d'un problème dans [!DNL Workfront] devient le nom du problème auquel il est lié dans [!DNL Jira].</p><p>Remarque : Lorsque de nouveaux éléments sont créés automatiquement dans [!DNL Jira], le nom [!DNL Workfront] est toujours mis à jour sur l’élément [!DNL Jira], que ce champ soit activé ou non dans ce champ. Lorsqu’un élément [!DNL Jira] est lié manuellement à un élément [!DNL Workfront], le nom de l’élément [!DNL Workfront] n’est mis à jour que dans [!DNL Jira] lorsque vous sélectionnez <strong>Toujours</strong> pour synchroniser ce champ. Pour plus d’informations sur la liaison manuelle ou automatique d’éléments, voir <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Liaison d’éléments entre [!DNL Adobe Workfront] et [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Description]</td>
         <td>La description d'une tâche ou d'un problème dans [!DNL Workfront] devient la description du problème auquel elle est liée dans [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documents</td>
         <td><p>Les documents joints à une tâche ou à un problème dans [!DNL Workfront] sont également joints au problème auquel il est lié dans Jira. Les nouvelles versions de documents de [!DNL Workfront] sont ajoutées en tant que documents distincts à Jira et sont ajoutées avec <i>_v&lt;numéro de version&gt;</i> pour indiquer la version numérotée dans Workfront. </p><p>Par exemple, si le nom d’un document dans [!DNL Workfront] est <strong>Main Ad</strong> et que vous y ajoutez une nouvelle version dans [!DNL Workfront], la nouvelle version est transférée vers [!DNL Jira] en tant que nouveau document portant le nom <strong>Main Ad_v2</strong>.</p><p>Important : <p>Tenez compte des points suivants lors de la synchronisation de documents :</p>
           <ul>
            <li><p>Les documents de plus de 5 Mo ne sont pas synchronisés. Si la synchronisation d’un document échoue car le document est trop volumineux, une erreur est consignée dans le journal d’activité. </p><p>Pour plus d’informations sur le journal des activités, voir <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Affichage du journal des activités Jira</a>.</p></li>
            <li><p>Les documents liés à des tâches et des problèmes provenant de serveurs externes ne sont pas transférés vers les éléments [!DNL Jira]. Seuls les documents chargés directement sur la tâche ou le problème dans [!DNL Workfront] sont transférés vers le problème lié dans [!DNL Jira].</p></li>
            <li><p>Pour créer un BAT à partir d’un document, vous devez générer le BAT dans [!DNL Workfront]. </p><p>Pour plus d'informations sur la génération d'un BAT, voir <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Création d'un BAT pour un document existant </a> dans <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Création d'un BAT pour un document</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Date d’achèvement prévue]</td>
         <td><p>La [!UICONTROL Date d’achèvement planifiée] d’une tâche ou d’un problème dans [!DNL Workfront] devient la [!UICONTROL Date d’échéance] du problème auquel elle est liée dans [!DNL Jira].</p><p>Remarque : Assurez-vous d’afficher <strong>[!UICONTROL Échéance]</strong> sur les problèmes [!DNL Jira] pour que cette valeur soit synchronisée.</p></td>
        </tr>
       </tbody>
      </table>

1. Dans la section **[!UICONTROL Synchroniser de [!DNL Jira] à[!DNL Workfront]]** , sélectionnez les champs que vous souhaitez mettre à jour dans [!DNL Workfront] lorsqu&#39;ils sont mis à jour dans [!DNL Jira].

   1. Sélectionnez l&#39;une des fréquences avec lesquelles les champs sont synchronisés :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Toujours]</td>
         <td>Les champs que vous spécifiez sont toujours synchronisés entre les éléments [!DNL Workfront] et [!DNL Jira] liés lorsque les champs sont mis à jour dans [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Jamais]</td>
         <td><p>Les champs que vous spécifiez ne sont jamais synchronisés entre les éléments [!DNL Workfront] et [!DNL Jira] liés. Il n’y a aucune indication dans [!DNL Workfront] que le champ a été mis à jour dans [!DNL Jira]. </p><p>Remarque : Lorsque vous sélectionnez Jamais, les champs [!DNL Workfront] peuvent toujours être mis à jour manuellement à partir de [!DNL Jira] dans le panneau de gauche [!DNL Workfront] du problème [!DNL Jira]. Ces mises à jour s’affichent uniquement sur les éléments [!DNL Workfront] de [!DNL Jira] et [!DNL Workfront] et non sur les éléments [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

   1. Sélectionnez pour synchroniser l’un des champs suivants de [!DNL Jira] à [!DNL Workfront] :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>L’[!UICONTROL Status] d’un problème dans [!DNL Jira] devient l’[!UICONTROL Status] de la tâche ou du problème auquel il est lié dans [!DNL Workfront].<br>Pour plus d’informations sur les états [!DNL Workfront], voir <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Création ou modification d’un état</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Cessionnaire]</td>
         <td><p>Le [!UICONTROL cessionnaire] d’un problème dans [!DNL Jira] devient le [!UICONTROL cessionnaire] de la tâche ou du problème auquel il est lié dans [!DNL Workfront].</p><p>Important : Lorsque vous affectez un élément dans [!DNL Jira] à un utilisateur qui n’a pas de compte [!DNL Workfront], l’intégration crée un nouvel utilisateur actif dans [!DNL Workfront] uniquement lorsque <strong> Créer automatiquement un utilisateur dans [!DNL Workfront] si l’utilisateur [!DNL Jira] n’a pas de compte [!DNL Workfront]</strong> est défini sur <strong>[!UICONTROL Toujours]</strong>. Cet utilisateur n’utilise pas de licence [!DNL Workfront]. Les utilisateurs actifs peuvent être affectés à des tâches dans [!DNL Workfront], mais ne peuvent pas être inclus dans les mises à jour. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Pièces jointes]</td>
         <td>Les pièces jointes d'un problème dans [!DNL Jira] sont également jointes à la tâche ou au problème auquel il est lié dans [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>Un commentaire sur un problème [!DNL Jira] est également publié sur l’élément [!DNL Workfront] lié dans la zone [!UICONTROL Mises à jour]. Inversement, un commentaire publié dans la zone [!UICONTROL Mises à jour] pour une tâche [!DNL Workfront] ou émet des synchronisations avec le flux de commentaires natif de [!DNL Jira] pour le problème lié. </p><p>Il est défini sur <strong>[!UICONTROL Toujours]</strong> par défaut. Si vous sélectionnez <strong>[!UICONTROL Jamais]</strong> ici, vous pouvez toujours publier des commentaires manuellement sur un élément lié, que ce soit dans [!DNL Workfront] ou dans [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. Dans la section **[!UICONTROL AUTRE]** , sélectionnez les champs supplémentaires à mettre à jour entre les éléments liés.

   1. Sélectionnez une option pour déterminer si les champs que vous spécifiez **[!UICONTROL Toujours]** ou **[!UICONTROL Jamais]** se mettent à jour dans [!DNL Jira] ou [!DNL Workfront] lorsqu’ils sont modifiés.

   1. Sélectionnez l’un des champs et mises à jour suivants :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copier [!DNL Workfront] des données personnalisées dans le panneau de droite de [!DNL Jira]]</td>
         <td><p>Affiche les [!DNL Workfront] données personnalisées d’un élément dans le panneau de droite de [!DNL Workfront].</p><p>Remarque : les sections Formulaire personnalisé s’affichent dans le panneau de droite [!DNL Workfront] avec le niveau d’accès de l’administrateur système [!DNL Workfront].</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copie [!DNL Workfront] Priorité dans le panneau de droite de [!DNL Jira]]</td>
         <td>Affiche la priorité [!DNL Workfront] d’un élément dans le panneau de droite [!DNL Workfront].</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Ajout d’une mise à jour dans l’onglet [!DNL Workfront] Mises à jour concernant les changements de date d’échéance dans [!DNL Jira]]</td>
         <td>Ajoute un commentaire dans l’onglet [!UICONTROL Mettre à jour] de l’élément [!DNL Workfront] lorsque la [!UICONTROL Date d’échéance] change dans l’élément [!DNL Jira] lié.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Créer automatiquement un utilisateur dans [!DNL Workfront] si l’utilisateur [!DNL Jira] n’a pas de compte [!DNL Workfront]]</td>
         <td><p>Les scénarios suivants sont possibles :</p>
          <ul>
           <li>Lorsque vous sélectionnez <strong>[!UICONTROL Toujours]</strong>, vous activez l’intégration pour créer un utilisateur Workfront chaque fois qu’un utilisateur [!DNL Jira] sans compte [!DNL Workfront] effectue les actions suivantes sur un problème [!DNL Jira] lié :
            <ul>
             <li>Est affecté à un problème [!DNL Jira]</li>
             <li><p>Consigne le temps d’un problème [!DNL Jira]</p><p>Ce nouvel utilisateur n’utilise pas de licence [!DNL Workfront]. Le paramètre par défaut est Toujours. "[!UICONTROL Jira]" a été ajouté à son nom pour l’utilisateur créé de cette manière dans [!DNL Workfront].</p></li>
            </ul></li>
           <li>Lorsque vous sélectionnez <strong>[!UICONTROL Jamais]</strong>, les événements suivants se produisent :
            <ul>
             <li>Vous ne pouvez pas voir d’affectations [!DNL Jira] sur les éléments [!DNL Workfront]. Dans ce cas, seules les affectations effectuées dans [!DNL Workfront] s’affichent sur les éléments [!DNL Workfront].</li>
             <li>L’heure connectée à un problème [!DNL Jira] lié par un utilisateur sans compte [!DNL Workfront] ne se transfère pas automatiquement vers l’élément [!DNL Workfront] lié. Vous pouvez toujours consigner l’heure sur l’élément [!DNL Workfront] dans le panneau droit du problème [!DNL Jira].</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Désormais, chaque fois qu’un utilisateur met à jour l’un des champs spécifiés dans cette configuration sur un élément dans [!DNL Jira] ou [!DNL Workfront], l’élément lié dans l’autre application est également mis à jour.

## Dépannage

### Les éléments ne peuvent pas être créés dans [!DNL Jira] en raison des champs déclencheurs marqués &quot;[!UICONTROL Impossible de trouver]&quot;

#### Problème

Lorsqu&#39;une erreur se produit avec l&#39;application [!DNL Workfront for Jira], [!DNL Workfront] désactive les déclencheurs pour éviter d&#39;autres complications. Lorsque ces déclencheurs sont désactivés, ils s’affichent comme &quot;[!UICONTROL Impossible de trouver]&quot;.

#### Solution

Recherchez l’erreur qui a désactivé les déclencheurs. Vous pouvez trouver l’erreur dans le [!DNL Workfront for Jira] [!UICONTROL Journal d’activité].

La cause la plus courante de ce comportement est l’erreur &quot;[!UICONTROL Field ’duedate’ ne peut pas être définie. Il ne se trouve pas sur l’écran approprié, ou inconnu.]&quot;

Cette erreur signifie que vous tentez de synchroniser la &quot;[!UICONTROL date d’achèvement prévue]&quot; de [!DNL Workfront] à [!DNL Jira]. Pour ce faire, vous devez vous assurer que vos objets [!DNL Jira] ont un champ appelé &quot;[!UICONTROL Date d’échéance]&quot;. Si ce champ n’est pas disponible, [!DNL Workfront] ne peut pas synchroniser la date d’achèvement prévue à partir de [!DNL Workfront] et désactive vos déclencheurs.

Pour résoudre cette erreur, essayez l’une des méthodes suivantes :

* Demandez à votre administrateur [!DNL Jira] de mettre à jour les objets [!DNL Jira] concernés pour vous assurer qu&#39;ils disposent d&#39;un champ de date d&#39;échéance.
* Désactivez la synchronisation de la date d&#39;achèvement prévue de [!DNL Workfront] dans la page [!UICONTROL Configuration] de Workfront.
