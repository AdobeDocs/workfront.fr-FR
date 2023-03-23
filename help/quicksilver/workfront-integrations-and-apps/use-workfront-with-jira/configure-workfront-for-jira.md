---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configurer [!DNL Adobe Workfront for Jira]
description: Vous pouvez utiliser [!DNL Adobe Workfront for Jira] pour intégrer votre [!DNL Jira] et [!DNL Workfront] systèmes.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: d2c366a69b986bd8d559a18994810011c6d33441
workflow-type: tm+mt
source-wordcount: '2413'
ht-degree: 0%

---

# Configurer [!DNL Adobe Workfront for Jira]

Vous pouvez utiliser [!DNL Adobe Workfront for Jira] pour intégrer votre [!DNL Jira] et [!DNL Workfront] systèmes.

Après l’installation du module complémentaire, vous pouvez définir des workflows qui créent des [!DNL Jira] se déclenche automatiquement lorsque [!DNL Workfront] les tâches sont créées. Les éléments des deux applications sont liés et certaines de leurs informations sont automatiquement mises à jour dans les deux systèmes.

Tous les utilisateurs de [!DNL Workfront] et [!DNL Jira] peuvent bénéficier de cette intégration. Ils n&#39;ont besoin d&#39;une licence que pour le système dans lequel ils travaillent le plus, et non pour les deux systèmes.

Ce module complémentaire est disponible pour les deux [!UICONTROL Serveur] et [!UICONTROL OnDemand] (ou [!UICONTROL Cloud]) [!DNL Jira] Logiciel.

Pour une liste de [!DNL Jira] versions qui [!DNL Workfront for Jira] actuellement pris en charge, voir [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) à l’adresse [!DNL Atlassian Marketplace].

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] Présentation des licences</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accès</td> 
   <td> <p>Accès administrateur système</p> <p>Important : Nous vous recommandons de créer des comptes d’administrateur système distincts dans [!DNL Jira] et [!DNL Workfront] pour dédier à cette intégration, plutôt que d’utiliser des qui peuvent être associés à des utilisateurs existants.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Avant de pouvoir configurer [!DNL Workfront for Jira], vous devez

* Installer [!DNL Workfront for Jira]\
   Pour obtenir des instructions sur l’installation [!DNL Workfront for Jira], voir [Installer [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configurer [!DNL Workfront for Jira]

En configurant [!DNL Workfront for Jira] vous pouvez :

* Définir les déclencheurs qui vont créer [!DNL Jira] éléments lorsque [!DNL Workfront] sont créés.
* Spécifiez les champs à synchroniser entre les éléments liés. [!DNL Jira] et [!DNL Workfront].

>[!NOTE]
>
>* Après avoir configuré [!DNL Workfront for Jira] sur votre [!DNL Jira] environnement, tout [!DNL Jira] les utilisateurs voient une [!DNL Workfront] panneau droit pour tous [!DNL Jira] éléments. Le panneau contient des informations sur les éléments pouvant être liés à partir de [!DNL Workfront] ou spécifie que [!DNL Workfront] éléments liés à [!DNL Jira] éléments.
>* Lors de l’utilisation de la variable [!DNL Jira Server] , seuls les problèmes associés aux projets identifiés comme déclencheurs de l’intégration Workfront affichent le panneau Workfront. Pour plus d’informations sur la configuration des déclencheurs pour la variable [!DNL Workfront to Jira] workflow, voir [Configuration de déclencheurs pour la liaison automatique d’éléments entre [!DNL Jira] et [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>




Pour configurer [!DNL Workfront for Jira]:

1. Se connecter [!DNL Jira] as a [!DNL Jira] administrateur.
1. Cliquez sur **[!UICONTROL Paramètres]** dans l’objet principal [!DNL Jira] .
1. Cliquez sur **[!UICONTROL Modules complémentaires]**, puis cliquez sur **[!UICONTROL Gestion des modules complémentaires]**.

1. Développez l’objet **[!DNL Workfront]** module complémentaire .
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Suivez les invites pour vous connecter à [!DNL Workfront].

   >[!NOTE]
   >
   >L’utilisateur doit disposer d’un `apiKey` in [!UICONTROL Workfront] pour créer une connexion réussie.

   Vous devez vous connecter à [!DNL Workfront] as a [!DNL Workfront] pour poursuivre la configuration.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] se connecte à [!DNL Jira] en utilisant OAuth 2.0, une norme utilisée par la plupart des intégrations web pour l’authentification et l’autorisation des utilisateurs.
   >* Lorsque vous êtes invité à saisir le domaine de votre [!DNL Workfront] compte, saisissez-le au format suivant : *yourCompany&#39;sDomain.my.workfront.com*. Le domaine de votre société correspond généralement au nom de votre société.
   >* L’authentification améliorée n’est pas disponible tant qu’un [!DNL Workfront] L’administrateur l’active pour cette intégration.



1. Sélectionnez la **[!UICONTROL Triggers]** pour configurer la création automatique de [!DNL Jira] éléments en tant que nouveaux [!DNL Workfront] sont créés.

   Pour plus d’informations sur la configuration des déclencheurs pour Workfront sur [!DNL Jira] workflow, voir [Configuration de déclencheurs pour la liaison automatique d’éléments entre [!DNL Jira] et [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Sélectionnez la **[!UICONTROL Configuration]** pour paramétrer la synchronisation des champs entre les champs liés [!DNL Jira] et [!DNL Workfront] éléments.

   Pour plus d’informations sur la configuration de la synchronisation des champs entre [!DNL Jira] et [!DNL Workfront], voir [Configurer la synchronisation des champs entre [!DNL Jira] et [!DNL Workfront] Éléments](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Après avoir défini les déclencheurs et la synchronisation des champs entre les deux applications, toute [!DNL Workfront] Un utilisateur qui peut créer des tâches ou des problèmes peut potentiellement déclencher la création d’un élément dans [!DNL Jira]. L’utilisateur peut créer un élément si les critères de l’élément qu’il crée correspondent aux déclencheurs dans [!DNL Jira], même si l’utilisateur n’a pas de [!DNL Jira] licence. Aussi, n’importe quel [!DNL Jira] l’utilisateur peut immédiatement commencer à travailler sur la fonction [!DNL Jira] et leurs mises à jour sont visibles dans [!DNL Workfront], sans qu’ils aient un [!DNL Workfront] licence. Toutes les mises à jour dans [!DNL Workfront] sont également visibles dans la variable [!DNL Jira] éléments.

1. (Facultatif) Sélectionnez le **[!UICONTROL Journal d’activité]** pour examiner les erreurs qui se sont produites pendant l’intégration.

   Pour plus d’informations sur la variable [!UICONTROL Journal d’activité], voir [Afficher la variable [!DNL Jira] [!UICONTROL Journal d’activité]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configuration de déclencheurs pour la liaison automatique d’éléments entre [!DNL Jira] et [!DNL Workfront]

Comme la variable [!DNL Jira] administrateur système, vous pouvez définir des déclencheurs qui créeraient automatiquement des problèmes dans [!DNL Jira] lorsqu’un élément dans [!DNL Workfront] répond à certains critères.

>[!NOTE]
>
>L’intégration peut prendre jusqu’à 10 minutes pour créer de nouveaux problèmes dans [!DNL Jira].

Tenez compte de ce qui suit lors de la configuration du déclenchement de la création de [!DNL Jira] éléments en tant que [!DNL Workfront] les éléments sont créés :

* L’intégration est unidirectionnelle : Vous ne pouvez déclencher que les éléments que vous créez dans [!DNL Workfront] à créer automatiquement dans [!DNL Jira]. Vous ne pouvez pas déclencher des éléments que vous créez dans [!DNL Jira] pour être automatiquement créé dans [!DNL Workfront].
* Le nombre de déclencheurs que vous pouvez avoir n’est pas limité.
* Si un élément est créé dans [!DNL Workfront] correspond à plusieurs déclencheurs, un seul élément est créé dans [!DNL Jira]. L’élément est créé dans [!DNL Jira] selon le premier déclencheur (dans l’ordre dans lequel ils ont été définis dans [!DNL Jira]). Tous les autres déclencheurs sont ignorés.
* Un seul élément dans [!DNL Workfront] peut être lié à un élément dans Jira. Vous ne pouvez jamais lier un lien. [!DNL Workfront] élément à plusieurs [!DNL Jira] problèmes ou un [!DNL Jira] publication sur plusieurs [!DNL Workfront] éléments.

Pour configurer des triggers pour la création automatique d’éléments dans [!DNL Jira]:

1. Se connecter [!DNL Jira] en tant qu’administrateur système.
1. Cliquez sur **[!UICONTROL Paramètres]** dans l’objet principal [!DNL Jira] .
1. Cliquez sur **[!UICONTROL Modules complémentaires]**, puis **[!UICONTROL Gestion des modules complémentaires]**.

1. Développez l’objet **[!DNL Workfront]** module complémentaire .
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur système.

   Le **[!UICONTROL Triggers]** est sélectionné par défaut.

1. Cliquez sur **[!UICONTROL Ajouter un déclencheur]** pour ajouter un nouveau déclencheur.
1. Dans le **[!UICONTROL Équipe/utilisateur/rôle Workfront]** , indiquez le nom d’un champ [!DNL Workfront] équipe, utilisateur ou rôle de tâche, puis cliquez pour le sélectionner lorsqu’il s’affiche dans la liste.

   >[!NOTE]
   >
   >Vous ne pouvez pas avoir plusieurs déclencheurs pour une même équipe, un même utilisateur ou un même rôle.

   Lorsqu’une personne crée une tâche ou un problème et l’affecte à l’une de ces entités, un problème est automatiquement créé dans [!DNL] [!DNL Jira]].

1. Dans le **[!UICONTROL [!DNL Jira]project]** , commencez à saisir le nom d’un champ [!DNL Jira] , puis cliquez pour la sélectionner lorsqu’elle s’affiche dans la liste.

   Lorsque la variable [!DNL Jira] est créé, il est placé sur le projet que vous spécifiez ici.

1. Sélectionnez une **I[!UICONTROL type de problème]** dans le menu déroulant.

   Cela indique le type de problème créé dans [!DNL Jira] lorsque les conditions de ce déclencheur sont remplies, en fonction de vos paramètres pour ce projet spécifique dans [!DNL Jira].

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Avec cette configuration, chaque fois qu’une [!DNL Workfront] l’utilisateur crée un élément correspondant aux déclencheurs spécifiés, un nouveau problème est créé dans [!DNL Jira].

## Configurer la synchronisation des champs entre [!DNL Jira] et [!DNL Workfront] Éléments

Comme la variable [!DNL Jira] administrateur, vous pouvez définir les champs à synchroniser automatiquement sur les éléments liés entre [!DNL Workfront] et Jira. Certains champs peuvent se synchroniser à partir du [!DNL Workfront] au [!DNL Jira] et d’autres synchronisent de Jira vers Workfront.

Pour définir les champs à synchroniser automatiquement sur les éléments liés entre les deux applications :

1. Se connecter [!DNL Jira] en tant qu’administrateur Jira.
1. Cliquez sur **[!UICONTROL Paramètres]** dans l’objet principal [!DNL Jira] .
1. Cliquez sur **[!UICONTROL Modules complémentaires]**, puis **[!UICONTROL Gestion des modules complémentaires]**.

1. Développez l’objet **[!DNL Workfront]** module complémentaire .
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur Workfront.
1. Cliquez sur le bouton **[!UICONTROL Configuration]** .

1. Dans le **[!UICONTROL Synchronisation de Jira vers Workfront]** , sélectionnez les champs que vous souhaitez mettre à jour dans [!DNL Jira] lorsqu’elles sont mises à jour dans Workfront.

   1. Sélectionnez l&#39;une des fréquences avec lesquelles les champs sont synchronisés :

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL À La Création]</td>
              <td>Les champs que vous spécifiez sont synchronisés entre Workfront et [!DNL Jira] lors de la création de l’élément dans Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Toujours]</td>
              <td>Les champs que vous spécifiez sont synchronisés entre Workfront et [!DNL Jira] éléments lorsque les champs sont mis à jour dans Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Jamais]</td>
              <td>Les champs que vous spécifiez ne sont jamais synchronisés entre les [!DNL Workfront] et [!DNL Jira] éléments. Il n’y a aucune indication dans [!DNL Jira] que le champ a été mis à jour dans [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Sélectionnez cette option pour synchroniser l’un des champs suivants dans [!DNL Workfront] to [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Nom d’une tâche ou d’un problème dans [!DNL Workfront] devient le nom du problème auquel il est lié dans [!DNL Jira].</p><p>Remarque : Lorsque de nouveaux éléments sont créés dans [!DNL Jira] automatiquement, la variable [!DNL Workfront] Le nom est toujours mis à jour sur la variable [!DNL Jira] , que ce champ soit activé ou non ici. Lorsqu’une [!DNL Jira] est lié manuellement à un élément [!DNL Workfront] item, le Nom de la [!DNL Workfront] mises à jour des éléments uniquement dans [!DNL Jira] lorsque vous sélectionnez <strong>Toujours</strong> synchronisez ce champ. Pour plus d’informations sur la liaison manuelle ou automatique d’éléments, voir <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Lier des éléments entre [!DNL Adobe Workfront] et [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Description]</td>
         <td>Description d’une tâche ou d’un problème dans [!DNL Workfront] devient la description du problème auquel il est lié dans [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documents</td>
         <td><p>Documents joints à une tâche ou à un problème dans [!DNL Workfront] sont également liées à la question à laquelle il est lié en Jira. Nouvelles versions de document à partir de [!DNL Workfront] sont ajoutés en tant que documents distincts à Jira et sont ajoutés avec <i>_v&lt;version number=""&gt;</i> pour indiquer la version numérotée dans Workfront. </p><p>Par exemple, si le nom d’un document dans [!DNL Workfront] is <strong>Publicité principale</strong>, et vous y ajoutez une nouvelle version dans [!DNL Workfront], la nouvelle version est transférée à [!DNL Jira] en tant que nouveau document portant le nom <strong>Main Ad_v2</strong>.</p><p>Important: <p>Tenez compte des points suivants lors de la synchronisation de documents :</p>
           <ul>
            <li><p>Les documents de plus de 5 Mo ne sont pas synchronisés. Si la synchronisation d’un document échoue car le document est trop volumineux, une erreur est consignée dans le journal d’activité, </p><p>Pour plus d’informations sur le journal des activités, voir <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Afficher le journal d’activité Jira</a>.</p></li>
            <li><p>Les documents liés à des tâches et des problèmes provenant de serveurs externes ne sont pas transférés vers [!DNL Jira] éléments. Seuls les documents chargés directement sur la tâche ou le problème dans [!DNL Workfront] sont transférées vers le problème lié dans [!DNL Jira].</p></li>
            <li><p>Pour créer un BAT à partir d’un document, vous devez générer le BAT dans [!DNL Workfront]. </p><p>Pour plus d’informations sur la génération d’un BAT, voir <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create" class="MCXref xref">Créer un BAT pour un document existant </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Création d’un BAT pour un document</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Date d’achèvement prévue]</td>
         <td><p>La [!UICONTROL Date d’achèvement planifiée] d’une tâche ou d’un problème dans [!DNL Workfront] devient la [!UICONTROL Date d’échéance] du problème auquel il est lié dans [!DNL Jira].</p><p>Remarque : Assurez-vous d’afficher <strong>[!UICONTROL Échéance]</strong> on [!DNL Jira] problèmes, pour que cette valeur se synchronise.</p></td>
        </tr>
       </tbody>
      </table>

1. Dans le **[!UICONTROL Synchroniser à partir de [!DNL Jira] to[!DNL Workfront]]** , sélectionnez les champs que vous souhaitez mettre à jour dans [!DNL Workfront] lorsqu’elles sont mises à jour dans [!DNL Jira].

   1. Sélectionnez l&#39;une des fréquences avec lesquelles les champs sont synchronisés :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Toujours]</td>
         <td>Les champs que vous spécifiez sont toujours synchronisés entre les [!DNL Workfront] et [!DNL Jira] éléments lorsque les champs sont mis à jour dans [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Jamais]</td>
         <td><p>Les champs que vous spécifiez ne sont jamais synchronisés entre les [!DNL Workfront] et [!DNL Jira] éléments. Il n’y a aucune indication dans [!DNL Workfront] que le champ a été mis à jour dans [!DNL Jira]. </p><p>Remarque : Lorsque vous sélectionnez Jamais, [!DNL Workfront] Les champs peuvent toujours être mis à jour manuellement à partir de [!DNL Jira] à gauche [!DNL Workfront] du panneau [!DNL Jira] problème. Ces mises à jour n’apparaissent que sur [!DNL Workfront] éléments dans [!DNL Jira] et [!DNL Workfront] et non [!DNL Jira] éléments.</p></td>
        </tr>
       </tbody>
      </table>

   1. Sélectionnez cette option pour synchroniser l’un des champs suivants dans [!DNL Jira] to [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>[!UICONTROL Status] d’un problème dans [!DNL Jira] devient l’[!UICONTROL État] de la tâche ou du problème auquel elle est liée. [!DNL Workfront].<br>Pour plus d’informations sur [!DNL Workfront] états, voir <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Création ou modification d’un état</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Cessionnaire]</td>
         <td><p>Le [!UICONTROL Cessionnaire] d’un problème dans [!DNL Jira] devient le [!UICONTROL cessionnaire] de la tâche ou du problème auquel il est lié. [!DNL Workfront].</p><p>Important : Lorsque vous affectez un élément dans [!DNL Jira] à un utilisateur qui n’a pas de [!DNL Workfront] , l’intégration crée un utilisateur principal dans [!DNL Workfront] uniquement lorsque la variable <strong>Création automatique d’un utilisateur dans [!DNL Workfront] si la variable [!DNL Jira] L’utilisateur n’a pas de [!DNL Workfront] account</strong> est défini sur <strong>[!UICONTROL Toujours]</strong>. Cet utilisateur n’occupe pas un [!DNL Workfront] licence. Les utilisateurs principaux peuvent être affectés à des tâches dans [!DNL Workfront], mais ne peuvent pas être inclus dans les mises à jour. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Pièces jointes]</td>
         <td>Pièces jointes d’un problème dans [!DNL Jira] sont également associées à la tâche ou au problème auquel elles sont liées. [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>Un commentaire sur un [!DNL Jira] Ce problème est également publié sur le lien [!DNL Workfront] dans la zone [!UICONTROL Mises à jour]. Inversement, un commentaire publié dans la zone [!UICONTROL Mises à jour] pour une [!DNL Workfront] synchroniser les tâches ou les problèmes [!DNL Jira]flux de commentaires natif de pour le problème lié. </p><p>Défini sur <strong>[!UICONTROL Toujours]</strong> par défaut. Si vous sélectionnez <strong>[!UICONTROL Jamais]</strong> ici, vous pouvez toujours publier des commentaires manuellement sur un élément lié dans [!DNL Workfront] ou [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. Dans le **[!UICONTROL AUTRES]** , sélectionnez les champs supplémentaires à mettre à jour entre les éléments liés.

   1. Sélectionnez une option pour déterminer si les champs spécifiés **[!UICONTROL Toujours]** ou **[!UICONTROL Jamais]** mettre à jour dans [!DNL Jira] ou [!DNL Workfront] lorsqu’elles sont modifiées.

   1. Sélectionnez l’un des champs et mises à jour suivants :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Copie [!UICONTROL [!DNL Workfront] Données personnalisées dans le panneau de droite de [!DNL Jira]]</td>
         <td><p>Affiche la variable [!DNL Workfront] Données personnalisées d’un élément dans la variable [!DNL Workfront] panneau droit.</p><p>Remarque : Les sections Formulaire personnalisé s’affichent dans la [!DNL Workfront] panneau droit avec le niveau d’accès de la propriété [!DNL Workfront] Administrateur système.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Copie [!UICONTROL [!DNL Workfront] Priorité dans le panneau de droite de [!DNL Jira]]</td>
         <td>Affiche la variable [!DNL Workfront] Priorité d’un élément dans la variable [!DNL Workfront] panneau droit.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Ajoutez une mise à jour dans la variable [!DNL Workfront] Onglet Mises à jour concernant les changements de date d’échéance dans [!DNL Jira]]</td>
         <td>Ajoute un commentaire dans l’onglet [!UICONTROL Mettre à jour] de la variable [!DNL Workfront] lorsque le paramètre [!UICONTROL Échéance] change dans les liens [!DNL Jira] élément .</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Créer automatiquement un utilisateur dans [!DNL Workfront] si la variable [!DNL Jira] L’utilisateur n’a pas de [!DNL Workfront] account]</td>
         <td><p>Les scénarios suivants existent :</p>
          <ul>
           <li>Lorsque vous sélectionnez <strong>[!UICONTROL Toujours]</strong> vous activez l’intégration pour créer un utilisateur Workfront chaque fois qu’une [!DNL Jira] utilisateur sans [!DNL Workfront] effectue les actions suivantes sur un lien [!DNL Jira] Problème :
            <ul>
             <li>Est affecté à une [!DNL Jira] issue</li>
             <li><p>Consigne l’heure dans un [!DNL Jira] issue</p><p>Ce nouvel utilisateur n’occupe pas un [!DNL Workfront] licence. Le paramètre par défaut est Toujours. L’utilisateur a créé cette manière dans [!DNL Workfront] "[!UICONTROL Jira]" a été ajouté à leur nom.</p></li>
            </ul></li>
           <li>Lorsque vous sélectionnez <strong>[!UICONTROL Jamais]</strong>, les événements suivants se produisent :
            <ul>
             <li>Vous ne pouvez pas voir les [!DNL Jira] sur l’objet [!DNL Workfront] éléments. Dans ce cas, seules les affectations effectuées dans [!DNL Workfront] s’affiche sur la [!DNL Workfront] éléments.</li>
             <li>Heure de connexion à un lien [!DNL Jira] d’un utilisateur sans [!DNL Workfront] Le compte n’est pas automatiquement transféré vers le lien [!DNL Workfront] élément . Vous pouvez toujours journaliser l’heure sur la variable [!DNL Workfront] dans le panneau de droite de l’objet [!DNL Jira] problème.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Désormais, chaque fois qu’un utilisateur met à jour l’un des champs spécifiés dans cette configuration pour un élément dans [!DNL Jira] ou [!DNL Workfront], l’élément lié dans l’autre application est également mis à jour.

## Dépannage

### Les éléments ne peuvent pas être créés dans [!DNL Jira] en raison des champs déclencheurs marqués &quot;[!UICONTROL Impossible de trouver]&quot;

#### Problème

Lorsque une erreur se produit avec notre [!DNL Workfront for Jira] application, [!DNL Workfront] désactive les déclencheurs pour éviter d’autres complications. Lorsque ces déclencheurs sont désactivés, ils s’affichent sous la forme &quot;[!UICONTROL Impossible de trouver]&quot;.

#### Solution

Recherchez l’erreur qui a désactivé les déclencheurs. Vous pouvez trouver l’erreur dans la variable [!DNL Workfront for Jira] &quot;[!UICONTROL Journal d’activité]&quot;.

La cause la plus courante de ce comportement est l’erreur &quot;[!UICONTROL Le champ &quot;duedate&quot; ne peut pas être défini. Il ne se trouve pas sur l’écran approprié, ou il est inconnu.]&quot;

Cette erreur signifie que vous tentez de synchroniser le[!UICONTROL Date d’achèvement prévue]&quot; de [!DNL Workfront] to [!DNL Jira]. Pour ce faire, vous devez vous assurer que la variable [!DNL Jira] les objets ont un champ appelé &quot;[!UICONTROL Date d’échéance]&quot;. S&#39;ils ne disposent pas de ce champ, [!DNL Workfront] ne peut pas synchroniser la date d’achèvement prévue à partir de [!DNL Workfront] et désactive vos déclencheurs.

Pour résoudre cette erreur, essayez l’une des méthodes suivantes :

* Demandez à votre [!DNL Jira] l’administrateur pour mettre à jour les [!DNL Jira] afin de s’assurer qu’ils disposent d’un champ de date d’échéance.
* Désactivation de la synchronisation des [!DNL Workfront]Date d’achèvement prévue dans Workfront &quot;[!UICONTROL Configuration]page &quot;
