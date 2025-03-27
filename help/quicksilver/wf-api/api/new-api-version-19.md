---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 19 de l’API
description: Adobe Workfront a publié la version 19 de l’API le jeudi 6 avril 2022. La version 19 de l’API présente les changements suivants par rapport à la version 18.
author: Becky
feature: Workfront API
role: Developer
exl-id: 84909dea-7ce1-4ad3-90f5-9dbdb354eaa4
source-git-commit: 1c1f9f46ea25ffa7d01c1a762b0478a5edb3339e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 50%

---

# Nouveautés de la version 19 de l’API

Adobe Workfront a publié la version 19 de l’API le mardi 8 avril 2024. La version 19 de l’API présente les changements suivants par rapport à la version 18.

## Ressources ajoutées

Aucune ressource n’a été ajoutée pour la version 19 de l’API.

## Ressources supprimées

Aucune ressource n’a été supprimée pour l’API version 19.

## Ressources modifiées

### AccessLevel (ACSLVL)

Un objet AccessLevel est associé à des personnes et décrit le jeu d’autorisations AccessLevelPermissions qui déterminent ce à quoi la personne peut accéder.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestrictions</b><p>Ajout des valeurs possibles suivantes :
            </p>
            <ul>
              <li>
                <p>Désactiver l’assistant d’IA pour Workfront (AIOFF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Assignment (ASSGN)

Un objet Affectation représente le lien entre un élément de travail et l&#39;utilisateur, l&#39;équipe ou le groupe affecté à ce travail.

L&#39;objet Assignment a ajouté l&#39;indicateur **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Ajout des champs directs suivants :
        <ul>
          <li>
            <p><b>categoryID</b><p>Une catégorie est un formulaire personnalisé. Ce champ permet d’ajouter un formulaire personnalisé à une affectation.
            </p>
          </li>
          <li>
            <p><b>priorité</b><p>Ce champ autorise les valeurs suivantes :
            <ul>
              <li>0 (Aucun)</li>
              <li>1 (Faible)</li>
              <li>2 (Normal)</li>
              <li>3 (Élevé)</li>
              <li>4 (Urgent)</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>Ajout des champs de référence suivants :
        <ul>
          <li>
            <p><b>catégorie</b><p>Une catégorie est un formulaire personnalisé. Ce champ permet d’ajouter un formulaire personnalisé à une affectation.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>Ajout des champs de collection suivants :
        <ul>
          <li>
            <p><b>objectCategories</b><p>Une catégorie est un formulaire personnalisé. Ce champ permet d’ajouter un formulaire personnalisé à une affectation.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### Catégorie (CTGY)

Un objet Category est un formulaire personnalisé.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été ajoutés pour permettre d’ajouter un formulaire personnalisé à une affectation.
        <ul>
          <li>
            <p><b>catObjCode</b><p>Ajout des valeurs possibles suivantes :
            </p>
            <ul>
              <li>
                <p>Assignment (ASSGN)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objTypes</b><p>Ajout des valeurs possibles suivantes :
            </p>
            <ul>
              <li>
                <p>Assignment (ASSGN)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Classificateur (CLSF)

Un classificateur est un emplacement.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>Ajout des actions suivantes :
        <ul>
          <li>
            <b>activateClassifiers</b>
          </li>
          <li>
            <b>deactivateClassifiers</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Client

Un objet Customer représente une organisation qui utilise une instance de Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumTypes</b><p>Ajout des valeurs possibles suivantes :
            </p>
            <ul>
              <li>
                <p>Priorités d'affectation (PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>L’objet CustomEnum permet de convertir les codes de statut en texte lisible par une personne.</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### CustomerPreferences (CUSTPR)

Un objet CustomerPreferences représente l’ensemble des préférences définies par un client ou une cliente pour son instance de Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>name</b><p>Suppression des valeurs possibles suivantes :
            </p>
            <ul>
              <li>
                <p>Activer l’intégration du zoom dans le flux de mises à jour (mot de passe : zoomIntegrationEnabled)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Document (DOCU)

Un objet Document représente un fichier (tel qu’un support écrit, des images ou d’autres formes d’informations).

<table>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>Ajout de la <code>folderID</code> de champs .</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>Ajout.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### ExchangeRate (EXRATE)

Un objet ExchangeRate représente un taux de change de devise configuré dans Workfront. Les objets ExchangeRate ne sont pas dynamiques.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
      <ul>
      <li>Les champs suivants ont ajouté le <code>REQUIRED</code> de validation :
        <ul>
          <li><p><b>currency</b></li>
          <li><p><b>taux</b></li></ul>
      <li>Les champs suivants ont été ajoutés :
        <ul>
          <li><p><b>enteredByID</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>
      <ul>
        <li>Les champs suivants ont été ajoutés :
        <ul>
          <li><p><b>enteredBy</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Groupe (GROUP)

Un objet Group représente un ensemble d’utilisateurs et utilisatrices et d’équipes. Les groupes représentent souvent la structure des services.

L’objet Group a ajouté l’indicateur **PARTAGEABLE**.

### Hour (HOUR)

Un objet Hour représente une heure enregistrée par un utilisateur ou une utilisatrice sur une feuille de temps.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
      Les champs suivants ont été ajoutés :
        <ul>
          <li><p><b>assignedApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>isBilling</b></li>
          <li><p><b>changedByID</b></li>
          <li><p><b>failedOnDate</b></li>
          <li><p><b>rejetCommentaire</b></li>
          <li><p><b>submittedByID</b></li>
          </ul>
          <p>Les modifications suivantes ont été apportées au champ <b>heures</b>.</p>
          <ul> 
          <li> Validateur supprimé <b>GREATER_THAN</b></li>
          <li> Validateur ajouté <b>NOT_EQUAL</b></li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
      Les actions suivantes ont été ajoutées :
        <ul>
          <li><p><b>approuver</b></li>
          <li><p><b>désapprouver</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

L’objet JournalEntry peut être configuré pour enregistrer des informations sur des champs d’objet spécifiques chaque fois que ces champs sont modifiés. Lorsqu’un champ est configuré pour être enregistré dans le cadre de l’objet JournalEntry, une entrée de journal correspondante est créée chaque fois que ce champ est modifié.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>drapeaux</b><p>Ajout des valeurs possibles suivantes :
            </p>
            <ul>
              <li>
                <p>Est un taux de coût (CR)
                </p>
              </li>
              <li>
                <p>Est un taux de facturation (BR)
                </p>
              </li>
              <li>
                <p>Est la finance générale (GF)
                </p>
              </li>
              <li>
                <p>Est un financement combiné (FC)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Paramètre (PARAM)

Un objet de paramètre est un champ personnalisé.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b></p><p>Ajout de la valeur possible suivante :
            <ul>
            <li>Durée (DRTN)</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>Pour créer un système plus convivial et plus flexible, le type de champ <b>Widget (WIDGET)</b> a été abandonné et divisé en plusieurs types de champs :
            <ul>
            <li>Adobe XD (ADOBE XD)</li>
            <li>Image (IMAGE)</li>
            <li>PDF (PDF)</li>
            <li>Vidéo (VIDEO)</li>
            <li>Recherche externe (EXTRA)</li>
            <li>Recherche externe multi-sélection (MULTI-EXTRAIT)</li>
            <li>Champ natif (WFNATIVE)</li>
            <li>Champ Planning (WFPLANNING)</li>
            <li>KPI par étapes (chronologique)</li>
            <li>Cumul (ROLLUP)</li>
            <li>Documents (DOCUMENT)</li>
           </ul>
          </li>
          <li>
            <p><b>configurations</b><p>Ajout.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Rôle (ROLE)

Un objet Rôle (fonction) représente une capacité fonctionnelle ou un ensemble de compétences qu’un utilisateur ou une utilisateur peut remplir, tel que Designer ou Chef ou Cheffe de produits.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
    Les champs suivants ont été ajoutés :
        <ul>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>
        Les champs suivants ont été ajoutés :
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion {#scorecardquestion}

Un objet ScoreCardQuestion représente une question qui a été ajoutée à une carte de performance. Ces questions sont généralement définies par la personne gestionnaire du portfolio et leurs réponses lui permettent de comprendre dans quelle mesure un projet s’aligne sur les objectifs du portfolio.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
            <p><b>displayType</b></p><p>Pour créer un système plus convivial et plus flexible, le type de champ <b>Widget (WIDGET)</b> a été abandonné et divisé en plusieurs types de champs :
            <ul>
            <li>Adobe XD (ADOBE XD)</li>
            <li>Image (IMAGE)</li>
            <li>PDF (PDF)</li>
            <li>Vidéo (VIDEO)</li>
            <li>Recherche externe (EXTRA)</li>
            <li>Recherche externe multi-sélection (MULTI-EXTRAIT)</li>
            <li>Champ natif (WFNATIVE)</li>
            <li>Champ Planning (WFPLANNING)</li>
            <li>KPI par étapes (chronologique)</li>
            <li>Cumul (ROLLUP)</li>
            <li>Documents (DOCUMENT)</li>
           </ul>
      </td>
  </tbody>
</table>

### TemplateAssignment (TÂCHE)

Un objet TemplateAssignment représente le lien entre une tâche de modèle et l&#39;utilisateur, l&#39;équipe ou le groupe affecté à cette tâche. Lorsque le modèle est utilisé pour un projet, cet utilisateur, cette équipe ou ce groupe est affecté à la tâche.

L&#39;objet TemplateAssignment a ajouté l&#39;indicateur **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Ajout des champs directs suivants :
        <ul>
          <li>
            <p><b>categoryID</b><p>Une catégorie est un formulaire personnalisé. Ce champ permet d’ajouter un formulaire personnalisé à une affectation.
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>Ajout des champs de référence suivants :
        <ul>
          <li>
            <p><b>catégorie</b><p>Une catégorie est un formulaire personnalisé. Ce champ permet d’ajouter un formulaire personnalisé à une affectation.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>Ajout des champs de collection suivants :
        <ul>
          <li>
            <p><b>objectCategories</b><p>Une catégorie est un formulaire personnalisé. Ce champ permet d’ajouter un formulaire personnalisé à une affectation.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Timesheet (TSHET)

Un objet Timesheet représente une feuille de temps virtuelle qui permet aux utilisateurs et utilisatrices de saisir les heures effectives travaillées pour les tâches, les projets et les types d’heures supplémentaires.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b></p><p>Supprimé.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>
