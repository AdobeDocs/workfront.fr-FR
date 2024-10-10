---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 19 de l’API
description: Adobe Workfront a publié la version 19 de l’API le jeudi 6 avril 2022. La version 19 de l’API présente les changements suivants par rapport à la version 18.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: e3f50efa03a43c44e9defd0a724b0516504b0e83
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 53%

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
                <p>Désactivation de l’assistant Workfront AI (AIOFF)
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

Un objet d’affectation représente la connexion entre un élément de travail et l’utilisateur, l’équipe ou le groupe affecté pour y travailler.

L’objet Assignment a ajouté l’indicateur **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Ajout des champs directs suivants :
        <ul>
          <li>
            <p><b>categoryID</b><p>Une catégorie est un formulaire personnalisé. Ce champ prend en charge la possibilité d’ajouter un formulaire personnalisé à une affectation.
            </p>
          </li>
          <li>
            <p><b>priorité</b><p>Ce champ autorise les valeurs suivantes :
            <ul>
              <li>0 (Aucun)</li>
              <li>1 (Faible)</li>
              <li>2 (Normal)</li>
              <li>3 (élevé)</li>
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
            <p><b>category</b><p>Une catégorie est un formulaire personnalisé. Ce champ prend en charge la possibilité d’ajouter un formulaire personnalisé à une affectation.
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
            <p><b>objectCategories</b><p>Une catégorie est un formulaire personnalisé. Ce champ prend en charge la possibilité d’ajouter un formulaire personnalisé à une affectation.
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
      <td>Les champs suivants ont été ajoutés pour prendre en charge la possibilité d’ajouter un formulaire personnalisé à une affectation.
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
                <p>Priorités d’affectation (PRIORITY_ASSIGNMENT)
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
                <p>Activez l’intégration Zoom dans le flux de mises à jour (password:zoomIntegrationEnabled).
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
            <p><b>createLargeDocument</b><p>Ajout du champ <code>folderID</code>.</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>Ajout.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### ExchangeRate (EXRATE)

Un objet ExchangeRate représente un taux d’exchange de devise configuré dans Workfront. Les objets ExchangeRate ne sont pas dynamiques.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
      <ul>
      <li>Les champs suivants ont ajouté le programme de validation <code>REQUIRED</code> :
        <ul>
          <li><p><b>currency</b></li>
          <li><p><b>rate</b></li></ul>
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

L’objet Group a ajouté l’indicateur **SHARABLE**.

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
          <li><p><b>isBill</b></li>
          <li><p><b>rejectByID</b></li>
          <li><p><b>rejectOnDate</b></li>
          <li><p><b>rejetComment</b></li>
          <li><p><b>submittedByID</b></li>
          </ul>
          <p>Les modifications suivantes ont été apportées au champ <b>hours</b> .</p>
          <ul> 
          <li> Suppression du programme de validation <b>GREATER_THAN</b></li>
          <li> Ajout du programme de validation <b>NOT_EQUAL</b></li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
      Les actions suivantes ont été ajoutées :
        <ul>
          <li><p><b>valider</b></li>
          <li><p><b>unapprove</b></li>
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
            <p><b>flags</b><p>Ajout des valeurs possibles suivantes :
            </p>
            <ul>
              <li>
                <p>Est le taux de coût (CR)
                </p>
              </li>
              <li>
                <p>Taux de facturation (BR)
                </p>
              </li>
              <li>
                <p>Is general finance (GF)
                </p>
              </li>
              <li>
                <p>Est le financement combiné (CF)
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
            <li>Durée (RTN)</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>Ajout des valeurs possibles suivantes :
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Image (IMAGE)</li>
            <li>PDF (PDF)</li>
            <li>Vidéo (VIDEO)</li>
            <li>Recherche externe (EXTRNL)</li>
            <li>Recherche externe multi-sélection (MULTEXTRNL)</li>
            <li>Champ natif (WFNATIVE)</li>
            <li>Champ de planification (WFPLANNING)</li>
            <li>IPC par étapes (TIMEPHASED)</li>
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
            <p><b>displayType</b></p><p>Ajout des valeurs possibles suivantes :
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Image (IMAGE)</li>
            <li>PDF (PDF)</li>
            <li>Vidéo (VIDEO)</li>
            <li>Recherche externe (EXTRNL)</li>
            <li>Recherche externe multi-sélection (MULTEXTRNL)</li>
            <li>Champ natif (WFNATIVE)</li>
            <li>Champ de planification (WFPLANNING)</li>
            <li>IPC par étapes (TIMEPHASED)</li>
            <li>Cumul (ROLLUP)</li>
            <li>Documents (DOCUMENT)</li>
           </ul>
      </td>
  </tbody>
</table>

### TemplateAssignment (TASSGN)

Un objet TemplateAssignment représente la connexion entre une tâche de modèle et l’utilisateur, l’équipe ou le groupe qui est affecté pour y travailler. Lorsque le modèle est utilisé pour un projet, cet utilisateur, cette équipe ou ce groupe est affecté à la tâche.

L’objet TemplateAssignment a ajouté l’indicateur **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Ajout des champs directs suivants :
        <ul>
          <li>
            <p><b>categoryID</b><p>Une catégorie est un formulaire personnalisé. Ce champ prend en charge la possibilité d’ajouter un formulaire personnalisé à une affectation.
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>Ajout des champs de référence suivants :
        <ul>
          <li>
            <p><b>category</b><p>Une catégorie est un formulaire personnalisé. Ce champ prend en charge la possibilité d’ajouter un formulaire personnalisé à une affectation.
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
            <p><b>objectCategories</b><p>Une catégorie est un formulaire personnalisé. Ce champ prend en charge la possibilité d’ajouter un formulaire personnalisé à une affectation.
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
            <p><b>objCode</b></p><p>Supprimée.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


