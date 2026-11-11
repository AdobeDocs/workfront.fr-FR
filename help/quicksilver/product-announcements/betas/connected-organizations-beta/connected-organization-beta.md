---
product-area: betas
title: Programme de Beta des fonctionnalités des organisations connectées
description:
author: Alina
feature: Product Announcements
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 98410f6d8632eb9842fdbcff88b52f4bc6a87b2e
workflow-type: tm+mt
source-wordcount: '2214'
ht-degree: 1%
---
# Programme bêta des fonctionnalités des organisations connectées

>[!IMPORTANT]
>
>La fonctionnalité Organisations connectées est actuellement en phase Beta fermée et ouverte à un petit nombre de clients.
>
>La version bêta sera disponible jusqu’à la fin de 2026.
>
>Pour toute question, contactez votre responsable de programme Adobe Beta.

La fonctionnalité Organisations connectées permet à une société et à ses partenaires de collaborer au travail lorsque les deux organisations ont acheté Adobe Workfront.

Par exemple, une société cliente peut soumettre une demande à la société du fournisseur pour que le travail soit effectué.

Chaque société peut continuer à travailler dans sa propre instance de Workfront, avec ses propres utilisateurs, autorisations et workflows.

Les objets de travail sont mis en miroir entre les deux instances et seules les données que les deux parties acceptent de partager sont synchronisées.

Le résultat est une vue partagée des requêtes, des statuts et des décisions sans connexions d&#39;invités supplémentaires, licences en double ou longs threads d&#39;e-mail.

## Présentation du workflow multi-organisation d’aujourd’hui

Lorsque deux sociétés investissent toutes deux dans Workfront, elles devraient être en mesure de travailler ensemble sans que l&#39;une paie deux fois ou passe dans le système de l&#39;autre.

Aujourd’hui, lorsque les deux sociétés travaillent dans deux systèmes distincts, leur collaboration peut inclure certains des workflows suivants :

* Les demandes et les notes sont transmises par le biais de fils de discussion difficiles à suivre.

* Les remises sont manuelles, avec peu de possibilité d’audit.

* Travailler dans le système d’une autre entreprise implique des connexions d’invités, des licences supplémentaires ou les deux.

* Plusieurs copies de fichiers circulent et personne ne sait avec certitude quelle est la source de vérité.

* Le statut étant difficile à suivre, les chargés de compte passent du temps à créer des présentations et à planifier des réunions de mise à jour.

## Présentation de la solution Organisation connectée

Lorsque vous utilisez la fonctionnalité Organisation connectée , les deux sociétés continuent à travailler dans deux systèmes distincts et leur collaboration inclut certains des workflows suivants :

* Aucune organisation n’accède à un objet dans l’instance de l’autre.
* Un objet tel qu’une demande de l’organisation cliente est dupliqué et publié dans l’instance du fournisseur.
* Seules les métadonnées configurées pour la synchronisation sont mises à jour entre les deux copies.
* Chaque société gère ses propres utilisateurs, autorisations et workflows au-delà de cet objet.

Le principe directeur est de partager le minimum nécessaire pour faire le travail et de garder le reste confidentiel.

<table>
<tbody>
<tr class="odd">
<td><strong>Éléments partagés</strong></td>
<td><strong>Ce qui reste privé</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Briefs et détails de la demande</p></li>
<li><p>Dates limites et jalons convenus</p></li>
<li><p>Consulter les commentaires</p></li>
<li><p>Décisions d’approbation</p></li>
<li><p>Ressources approuvées finales</p></li>
</ul></td>
<td><ul>
<li><p>Relations avec d'autres clients ou d'autres agences</p></li>
<li><p>Données financières, taux et frais facturés au client</p></li>
<li><p>Planification des ressources et capacité</p></li>
<li><p>Structure interne du projet, tâches et tout champ non sélectionné pour le partage</p></li>
</ul></td>
</tr>
</tbody>
</table>

## Fonctionnalités disponibles en version bêta

La première phase du programme bêta vous permet de connecter les deux instances et de lancer le travail.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Fonctionnalité** | **Fonctions** |
| **Organisations connectées** | Associe les deux instances Workfront entre les deux organisations. Pendant la phase bêta, Adobe configure la connexion. Une configuration en libre-service est actuellement en cours de développement. |
| **Formulaires de demande** | La société cliente crée un formulaire de demande, le publie et le partage avec une société de fournisseurs à partir des paramètres de partage du formulaire. |
| **Réception de demandes assistée par l’IA** | Le demandeur du client peut utiliser la fonctionnalité de remplissage de formulaire de l’IA pour saisir une invite et joindre des fichiers au lieu de remplir un formulaire long. Le système mappe ce contenu aux champs du formulaire et affiche le mappage pour révision. Le demandeur accepte le résultat et envoie le formulaire. |
| **Requêtes mises en miroir** | La demande envoyée apparaît dans la zone Demandes de l’entreprise du fournisseur sous la forme d’une copie en lecture seule, y compris les valeurs de champ personnalisé. |
| **Conversion de demande en projet** | Le fournisseur convertit la demande en projet et sélectionne le portfolio, le programme et le modèle pour lancer le travail. Le nouvel objet dans l’instance du fournisseur est lié à la demande d’origine du client. Les détails du travail réel du côté du fournisseur ne sont pas visibles pour la société requérante. |
| **Commentaires bidirectionnels** | Les commentaires sur la demande sont visibles des deux côtés et arrivent presque immédiatement, de sorte que les deux parties peuvent s&#39;entendre au même endroit. |
| **Acceptation de la demande** | Une fois que les deux parties sont d&#39;accord, le fournisseur accepte la demande et le client peut voir qu&#39;elle a été acceptée. |
| **Mises à jour de statut rédigées par l’IA** | Lorsqu’un demandeur demande l’état d’un commentaire, le fournisseur peut utiliser des commandes d’IA pour générer rapidement et de manière cohérente un brouillon de réponse. <br> Le brouillon comprend des informations provenant des objets liés à la demande, telles que la date d&#39;achèvement prévue, la condition et les heures consignées par rapport aux heures prévues. <br> Il s’agit d’un résumé des informations les plus importantes, et non d’une exportation champ par champ. Une personne la révise et la modifie avant d’envoyer une réponse au client. |

## Participer au programme Beta

Adressez-vous au responsable de programme de la version bêta d’Adobe pour participer à la version bêta.

### Ce que nous demandons aux participants

* Participez à un appel de commentaires hebdomadaire.

* Réservez environ une heure par semaine pour effectuer des tests pratiques par vous-même. Des sessions de travail en direct sur l’appel sont une option.

* Amener les deux points de vue des partenaires aux réunions, dans la mesure du possible.

* Identifiez les environnements Workfront à connecter et configurez les comptes d’administration pour un petit nombre d’ingénieurs Adobe afin qu’ils puissent valider la connexion.

### Ce que nous voulons apprendre

* La mise en miroir d’un objet et la synchronisation des données sélectionnées uniquement constituent-elles le modèle de partage approprié ? Est-il suffisamment souple pour chaque côté?

* Le séquencement des phases est-il correct ou une fonctionnalité ultérieure doit-elle intervenir plus tôt ?

* Quels points de contact sont absents de la collaboration ?

* Comment les noms de champs et le mappage doivent-ils fonctionner entre les deux instances ?

  Aujourd’hui, le formulaire et la demande appartiennent au client et le fournisseur les voit en lecture seule avec les noms de champ du client.

* De quoi le service informatique a-t-il besoin pour approuver et administrer une connexion ?

## Workflow de bout en bout

Cette section décrit le workflow pour deux parties impliquées dans cette intégration.

Nous utilisons un workflow de client et de fournisseur comme exemples.

Le workflow comprend les étapes suivantes :

1. [Création d’une connexion à une instance](#1-create-an-instance-connection)
1. [Confirmation de la connexion](#2-acknowledge-the-connection)
1. [Partager un formulaire de demande avec l’organisation connectée](#3-share-a-request-form-with-the-connected-organization)
1. [Envoyez une demande](#4-submit-a-request)
1. [Examinez la demande et créez un projet](#5-review-the-request-and-create-a-project)
1. [Collaborer dans la conversation intersociétés](#6-collaborate-in-the-cross-company-conversation)

### Avant de commencer

* Vous devez être un administrateur système disposant d&#39;un accès complet à la zone **Configuration** dans les deux instances.
* L&#39;instance requérante a besoin du client unique **GUID** de l&#39;instance de réception.
* Le formulaire que vous souhaitez partager doit être publié.

### &#x200B;1. Création d’une connexion à une instance

Configurez les éléments suivants dans l’instance requérante (le client) :

1. Connectez-vous à l’environnement du client et accédez à **Configuration** > **Connexions d’instance**. La page répertorie toutes les connexions et est vide si aucune n’existe encore.
1. Cliquez sur **Créer une connexion**.
1. Dans la zone **Créer une connexion**, ajoutez le **GUID de l&#39;instance de réception**. Ce champ est obligatoire.
1. (Facultatif) Définissez une **Date d’expiration**. La connexion cesse de fonctionner après cette date.
1. Cliquez sur **Créer une connexion**.

   La nouvelle connexion s’affiche dans la liste des connexions avec le statut **En attente**.
1. Sélectionnez la nouvelle connexion pour afficher ses détails.

   >[!TIP]
   >
   >Une connexion en attente ne partage rien. L’instance de réception doit d’abord l’acquitter.


### &#x200B;2. Confirmation de la connexion

Configurez les éléments suivants dans l’instance de réception (le fournisseur) :

1. Connectez-vous à l&#39;instance du fournisseur et accédez au **Menu principal** > **Configuration** > **Connexions d&#39;instance**.
1. Cliquez sur le nom pour ouvrir la connexion à partir de l’instance de réception. Une bannière affiche le message suivant : **Une instance souhaite se connecter à la vôtre. Sélectionnez au moins un destinataire éligible, puis acquittez la connexion. Rien n&#39;est partagé tant que vous ne l&#39;avez pas fait.**
1. Sous **Destinataires éligibles**, ouvrez la liste **Groupes de recherche et utilisateurs** et choisissez qui peut recevoir du travail de l’instance à l’origine de la demande. Vous pouvez sélectionner des groupes et des utilisateurs individuels. <!--asking Anna K if this should be teams and users, instead of groups; it's groups in the UI-->
1. Cliquez sur **Accepter** pour accepter la connexion ou cliquez sur l&#39;une des options suivantes :

   * **Refuser** la connexion.
   * **Fermez** pour le laisser en attente.

   Un message « Modifications enregistrées » apparaît et le statut de la connexion passe à **Actif**. La liste affiche désormais les destinataires éligibles, la date de création et la date d’expiration.

   >[!TIP]
   >
   >**Accepter** reste grisé jusqu&#39;à ce que vous choisissiez au moins un destinataire éligible.

### &#x200B;3. Partager un formulaire de demande avec l’organisation demandeuse

À partir de l’instance Workfront du client :

1. Accédez au **Menu principal** > **Demandes** et cliquez sur **Formulaires de demande**.
1. Ouvrez le formulaire publié que vous souhaitez partager.
1. Cliquez sur **Partager**.

   Notez les onglets suivants dans la zone **Partager** :

   * **Partage interne**
   * **Partage public**
   * **Organisations connectées**
1. Ouvrez l’onglet **Organisations connectées**.
1. Dans le champ **Organisation**, sélectionnez l’instance du fournisseur connecté.
1. Dans le champ **Utilisateurs et groupes**, choisissez qui, dans cette organisation, peut utiliser le formulaire. Ajoutez des utilisateurs, des utilisatrices et des groupes.
1. Cliquer sur **Enregistrer**.

Un message **Vos modifications ont bien été enregistrées** confirme le partage. <!--need to submit a UI text change - remove "successfully"-->

### &#x200B;4. Envoyez une demande

En tant qu’utilisateur de l’instance du client, envoyez une requête en procédant comme suit :

1. Connectez-vous à l’instance Workfront du client et accédez à **Menu principal** > **Demandes**.

   La page **Envoyer une nouvelle demande** répertorie les formulaires récents, y compris celui que vous venez de partager.

   Une note en haut affiche **Demande intersociétés : les demandes soumises avec ce formulaire sont visibles pour l&#39;organisation connectée.**
1. Remplissez le formulaire manuellement ou utilisez **Remplir le formulaire** pour que l’IA le fasse pour vous.
1. (Facultatif) Pour utiliser Remplir le formulaire, procédez comme suit :

   1. Cliquez sur **Remplir le formulaire**.
   1. Décrivez votre demande, collez un e-mail associé ou cliquez sur **Joindre des fichiers** pour charger un fichier. L’IA trouve les détails pertinents et les applique au formulaire.
   1. Cliquez sur **Appliquer au formulaire**. Une barre de progression indique **Remplir le formulaire** pendant la génération des valeurs de champ.
   1. Pour ignorer l’étape de l’IA, cliquez sur **Ignorer**.
1. Passez en revue les valeurs générées et modifiez tout ce qui doit être modifié.
1. Cliquez sur **Soumettre** pour soumettre la demande.

   Un message **Demande envoyée avec succès** s’affiche avec un lien **Afficher votre demande**.

   La nouvelle demande est ajoutée à la liste des demandes avec le nom du formulaire et un statut de **Nouveau**.

   >[!TIP]
   >
   >Les réponses de l’IA peuvent être inexactes. Vérifiez toujours deux fois les valeurs renseignées avant d’envoyer.

### &#x200B;5. Examinez la demande et créez un projet

1. Connectez-vous à l&#39;instance Workfront du fournisseur et accédez à **Menu principal** > **Demandes**.

La demande entrante s’affiche dans la liste.

Le **Type** de la requête est marqué comme **Externe : &lt; nom de l&#39;instance du client >**, ce qui le marque comme provenant de l&#39;organisation connectée.

1. Ouvrez la requête. Un badge **Partagé avec : &lt; nom de l’instance du client >** s’affiche en regard du titre et le panneau des commentaires affiche l’avis de **conversation intersociétés** suivant : **Cette discussion est visible pour &lt; nom de l’organisation du client >.**
1. Vérifiez les informations de la demande et les réponses du formulaire.
1. Cliquez sur le menu **Plus** à droite du nom de la requête, puis sur **Créer un objet**.
1. Dans la boîte de dialogue **Créer un objet**, mettez à jour les champs suivants :
   * **Action** : sélectionnez une action dans le menu. Par exemple, **Créez un seul projet**
   * **Modèle de projet** : sélectionnez un modèle disponible.
   * **Propriétaire du projet** : ajoutez un propriétaire de projet.
   * **Module** : choisissez un produit où l&#39;objet s&#39;affichera. Si vous choisissez **Workflow**, un projet est créé dans l’instance de Workfront du fournisseur.
   * **Formulaires personnalisés** : si nécessaire, joignez des formulaires personnalisés.
   * **Portfolio** et **Programme** : ajoutez des portfolios ou des programmes pour le nouveau projet.
1. Cliquez sur **Créer**.

   La demande dans l&#39;instance du fournisseur est désormais liée au nouveau projet et le statut de la demande passe à **En cours**. L’instance demandeuse du client voit le changement de statut sur sa propre copie de la requête.

### &#x200B;6. Collaborer dans la conversation intersociétés

Les utilisateurs et utilisatrices des deux organisations peuvent commenter leurs requêtes respectives. La bannière **Conversation intersociétés** rappelle que tout ce qui est écrit ici est visible pour l’autre organisation.

Utilisez l’une des méthodes suivantes :

1. Pour demander une mise à jour à partir de l’instance du client :

   1. Ouvrez la requête et accédez au panneau **Commentaires**.
   1. Cliquez sur **Nouveau commentaire**, saisissez votre message, puis cliquez sur **Envoyer**.

1. Pour mettre à jour la requête de l’instance du fournisseur :

   1. Ouvrez la requête. Le nouveau commentaire est surligné avec un libellé **Nouveau**.
   1. Cliquez sur **Répondre**, écrivez la réponse, puis cliquez sur **Envoyer**.

1. Pour effectuer un suivi à partir de l’instance du client :

   1. Ouvrez la requête. La réponse du fournisseur apparaît sous le commentaire d&#39;origine.
   1. Cliquez sur **J&#39;aime** pour l&#39;accuser réception ou sur **Ajouter une réponse** pour poursuivre la discussion.




<!--
### Client's workflow

As a requestor in the client's organization, you can do the following:  

1. Create or ask an administrator to create a request form, publish it, and share it with the connected provider's organization.

2. Open the published form from the Requests area, enter a prompt, and attach any files.

3. Review how the content maps to the form fields, accept, and submit.

### Provider's workflow

As a work manager in the provider's organization, do the following: 

1. Receive the request in your Requests area as a read-only copy.

2. Discuss the request through comments until both sides are aligned, then accept it.

3. Convert the request into a project, choosing the portfolio, program, and template, if needed.

4. Choose which project fields are mirrored back to the client's request. 

5. Answer status questions in comments, or generate a draft status update, review it, and publish to your request. It will also display on the client's original request. 

    From that point on, the request on the provider's side acts as a replica of the client's original request, so comments and agreed-upon data stay in sync.
-->

## Sécurité et gouvernance

La protection des données de chaque organisation est une exigence de conception essentielle.

L’une des lignes de base que nous voulons que la version bêta établisse est la facilité avec laquelle les équipes informatiques et de sécurité peuvent approuver et administrer une connexion entre les instances.

Voici les avantages du workflow d’organisation connecté :

* **Pas d&#39;accès inter-instances** : aucun utilisateur de l&#39;organisation partenaire n&#39;est nécessaire dans votre instance, il n&#39;y a donc pas de connexions invitées ni de licences supplémentaires.

* **Partage minimum nécessaire** : seules les données configurées pour la synchronisation sont partagées. Le reste reste dans son instance d’origine.

* **Contrôles indépendants** : chaque organisation conserve ses propres utilisateurs, autorisations et workflows.

* **Définition de la portée au niveau de l’équipe** : les requêtes sont destinées à atteindre uniquement les équipes de l’agence configurées pour travailler avec ce client, à l’aide des contrôles d’accès Workfront existants.

## Perspectives de la feuille de route

Les phases ci-dessous décrivent notre plan de développement et de publication actuel. Le séquencement peut changer en fonction de ce que nous apprenons pendant la phase bêta. Les phases ultérieures ne sont pas des engagements.

<table>
<tbody>
<tr class="odd">
<td><strong>Phase</strong></td>
<td><strong>Focus et fonctionnalités planifiées</strong></td>
<td><strong>Statut</strong></td>
</tr>
<tr class="even">
<td><strong>Phase 1</strong></td>
<td>Connectez les instances et lancez le travail : formulaires de demande, réception assistée par l’IA, demandes mises en miroir, conversion de projet, commentaires et rédaction de l’état.</td>
<td>En version bêta</td>
</tr>
<tr class="odd">
<td><strong>Phase 2</strong></td>
<td><ul>
<li><p>Révision et approbation à l’aide de Frame et de l’expérience de révision et d’approbation unifiée</p></li>
<li><p>Les révisions en attente apparaissent dans Workfront ou Frame, quel que soit l’endroit où travaille le ou la partenaire</p></li>
<li><p>Les annotations restent liées au fichier de travail afin que les équipes créatives puissent envoyer leurs commentaires au même endroit</p></li>
</ul></td>
<td>Prévu</td>
</tr>
<tr class="even">
<td><strong>Phase 3</strong></td>
<td><ul>
<li><p>Affectation de travail basée sur une tâche en plus des demandes</p></li>
<li><p>Statut plus automatisé, basé sur des champs partagés ou non partagés</p></li>
<li><p>Un nouveau type d'objet livrable, avec des métadonnées définies pendant la session d'information et héritées par la ressource finale approuvée</p></li>
<li><p>Diffusion directe des ressources finales approuvées dans AEM de la marque, ce qui réduit la saisie manuelle des métadonnées</p></li>
</ul></td>
<td>Prévu</td>
</tr>
<tr class="odd">
<td><strong>Phase 4</strong></td>
<td><ul>
<li><p>Contexte partagé entre les partenaires</p></li>
<li><p>Utilisation de Adobe Brand Intelligence <!--by the agency--> avant révision, avec un accès contrôlé par l'équipe</p></li>
<li><p>Fonctionnalités basées sur le contexte, telles que l’estimation</p></li>
</ul></td>
<td>Long terme</td>
</tr>
</tbody>
</table>






<!--

Original pdf from team:

**ADOBE WORKFRONT | BETA PROGRAM**

**Agency Brand Connectors**

Product overview for beta participants

# **Overview**

Agency Brand Connectors lets a brand and its agency collaborate on work when both organizations run Adobe Workfront. Each side keeps working in its own Workfront instance, with its own users, permissions, and workflows. Work objects are mirrored between the two instances, and only the data both sides agree to share is synchronized.

The result is a shared view of requests, status, and decisions without guest logins, duplicate licenses, or long email threads.

# **The challenge this addresses**

When a brand and an agency are both invested in Workfront, they should be able to work together without either one paying twice or moving into the other's system. Today the collaboration usually looks like this:

  - Requests and briefs travel through email threads that are hard to follow.

  - Handoffs are manual, with little auditability.

  - Working inside a partner's system means guest logins, extra licenses, or both.

  - Multiple copies of files circulate, and no one is sure which is the source of truth.

  - Status is hard to see, so producers and account managers spend time building decks and scheduling update meetings.

# **How it works: the sharing model**

Neither organization accesses an object in the other's instance. Instead, an object such as a request is duplicated and published into the partner's instance, and only the metadata configured for sync is kept up to date between the two copies. Each side manages its own users, permissions, and workflows downstream of that object.

The guiding principle is to share the minimum needed to get the work done, and to keep everything else confidential.

<table>
<tbody>
<tr class="odd">
<td><strong>What is shared</strong></td>
<td><strong>What stays private</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Briefs and request details</p></li>
<li><p>Agreed deadlines and milestones</p></li>
<li><p>Review comments</p></li>
<li><p>Approval decisions</p></li>
<li><p>Final approved assets</p></li>
</ul></td>
<td><ul>
<li><p>Relationships with other clients or other agencies</p></li>
<li><p>Financials, rates, and what is charged to the client</p></li>
<li><p>Resource planning and capacity</p></li>
<li><p>Internal project structure, tasks, and any fields not selected for sharing</p></li>
</ul></td>
</tr>
</tbody>
</table>

# **Features available in the beta**

The first phase of the beta covers connecting two instances and kicking off work.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Feature**                       | **What it does**                                                                                                                                                                                                                                                                                                                      |
| **Connected organizations**       | Links a brand instance and an agency instance. During the beta, Adobe configures the connection. A self-serve setup is being worked on.                                                                                                                                                                                               |
| **Request forms**                 | The brand creates a request form, publishes it, and shares it with a connected organization from the form's Share settings.                                                                                                                                                                                                           |
| **AI-assisted request intake**    | The requester types a prompt and attaches files instead of filling out a long form. The system maps that content to the form fields and shows the mapping for review. The requester accepts the result and submits. This uses Workfront's existing form-filling technology.                                                           |
| **Mirrored requests**             | The submitted request appears in the agency's request area as a read-only copy, including custom field values.                                                                                                                                                                                                                        |
| **Request-to-project conversion** | The agency converts the request into a project and selects the portfolio, program, and template. The new object is linked back to the request. Downstream work on the agency side is not visible to the brand.                                                                                                                        |
| **Two-way comments**              | Comments on the request are visible on both sides and arrive almost immediately, so both parties can work toward agreement in one place.                                                                                                                                                                                              |
| **Request acceptance**            | Once both sides agree, the agency accepts the request and the brand sees that it has been accepted.                                                                                                                                                                                                                                   |
| **AI-drafted status updates**     | When a brand asks for status in a comment, the agency can use a slash command to generate a draft reply. The draft draws on connected objects, such as planned completion date, condition, and hours logged against hours planned. It is a summary, not a field-by-field export, and a person reviews and edits it before publishing. |

# **End-to-end workflow**

## **Brand side**

1.  Create a request form, publish it, and share it with the connected agency.

2.  Open the published form, enter a prompt, and attach any files.

3.  Review how the content maps to the form fields, accept, and submit.

## **Agency side**

1.  Receive the request in the request area as a read-only copy.

2.  Discuss the request through comments until both sides are aligned, then accept it.

3.  Convert the request into a project, choosing the portfolio, program, and template.

4.  Choose which project data is mirrored back to the brand.

5.  Answer status questions in comments, or generate a draft status update, review it, and publish.

From that point on, the request on the agency side acts as a replica of the request on the brand side, so comments and agreed data stay in step.

# **Security and governance**

Keeping each organization's data protected is a core design requirement, and one of the baselines we want the beta to establish is how easily IT and security teams can approve and administer a connection between instances.

  - **No cross-instance access.** No users from the partner organization are needed in your instance, so there are no guest logins and no additional licenses.

  - **Minimum necessary sharing.** Only the data configured for sync is shared. Everything else stays in the originating instance.

  - **Independent controls.** Each organization keeps its own users, permissions, and workflows.

  - **Team-level scoping.** Requests are intended to reach only the agency teams set up to work on that brand, using existing Workfront access controls.

# **Roadmap**

The phases below describe our current plan. Sequencing may change based on what we learn in the beta, and later phases are not commitments.

<table>
<tbody>
<tr class="odd">
<td><strong>Phase</strong></td>
<td><strong>Focus and planned capabilities</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>Phase 1</strong></td>
<td>Connect instances and kick off work: request forms, AI-assisted intake, mirrored requests, project conversion, comments, and status drafting.</td>
<td>In beta</td>
</tr>
<tr class="odd">
<td><strong>Phase 2</strong></td>
<td><ul>
<li><p>Review and approval using Frame and the unified review and approval experience</p></li>
<li><p>Pending reviews appear in Workfront or Frame, wherever the stakeholder works</p></li>
<li><p>Annotations stay tied to the working file so creative teams see feedback in one place</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="even">
<td><strong>Phase 3</strong></td>
<td><ul>
<li><p>Task-based work assignment in addition to requests</p></li>
<li><p>More automated status, informed by shared or unshared fields</p></li>
<li><p>A new deliverable object type, with metadata defined during briefing and inherited by the final approved asset</p></li>
<li><p>Direct delivery of approved final assets into the brand's AEM, reducing manual metadata entry</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="odd">
<td><strong>Phase 4</strong></td>
<td><ul>
<li><p>Shared context between brand and agency</p></li>
<li><p>Use of Adobe Brand Intelligence by the agency before review, with access controlled by team</p></li>
<li><p>Context-informed capabilities such as estimating</p></li>
</ul></td>
<td>Longer term</td>
</tr>
</tbody>
</table>

# **Participating in the beta**

## **What we ask of participants**

  - Join a weekly feedback call.

  - Set aside about one hour per week for hands-on testing. Live working sessions on the call are an option if time is tight.

  - Bring both the brand and the agency perspective where possible.

  - Identify the Workfront environments to connect, and provision admin accounts for a small number of Adobe engineers so they can validate the connection.

## **What we want to learn**

  - Is mirroring an object and syncing only selected data the right sharing model, and is it flexible enough for each side?

  - Is the phase sequencing right, or should a later capability come sooner?

  - What touchpoints are missing from the collaboration?

  - How should field naming and mapping work between brand and agency instances? Today, the form and request are owned by the brand, and the agency sees them read-only with the brand's field names.

  - What does IT need to approve and administer a connection?

The beta runs through the end of the year. For questions or blockers, contact your Adobe beta program manager.


-->