---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Ajout d’options de vérification avancées à l’aide de l’API Adobe Workfront
description: Ajout d’options de vérification avancées à l’aide de l’API Adobe Workfront
author: John
feature: Workfront API, Workfront Proof
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---


# Ajout d’options de vérification avancées lors de la création d’un BAT via l’API Adobe Workfront

Lors de la création d’un BAT dans l’API Workfront, vous pouvez ajouter des options de vérification avancées.

Utilisez l’un des workflows suivants pour ajouter des options de vérification à un BAT à l’aide de l’API :

* (Recommandé) Créez un BAT simple à l’aide de l’API Workfront, puis ajoutez des options de vérification avancées au BAT à l’aide de l’API ProofHQ.

* Création d’un BAT avec des options de vérification avancées à l’aide de JSON dans l’API Workfront

## Créer un BAT à l’aide des API Workfront et ProofHQ (recommandé) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

Cette section décrit comment créer un BAT avec des options de vérification avancées via l’API Workfront, à l’aide d’une combinaison d’API Workfront et de BATHQ.

L’API ProofHQ inclut diverses actions qui ne sont pas disponibles pour les bons à tirer dans l’API Workfront. En utilisant ces actions, vous pouvez modifier ou configurer le BAT avec plus de précision que ne l’est l’API Workfront.

Pour un aperçu de l’API ProofHQ, reportez-vous à la section [Présentation de PoofHQ](../../proofhq-api/general/overview.md). Vous pouvez également consulter la section [Documentation de ProofHQ](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* L’API Workfront est une API REST-ful. L’API ProofHQ est une API SOAP.
>* Les bons à tirer créés dans l’API ProofHQ ne sont pas automatiquement liés à Workfront. Par conséquent, nous vous recommandons de créer des bons à tirer dans l’API Workfront avant de les mettre à jour avec l’API ProofHQ.
>


### Créer un BAT avec des options de vérification avancées

1. Créez un BAT à l’aide de la fonction `Document createProof` dans l’API Workfront.

   >[!NOTE]
   Lors de la création du BAT, n’incluez pas de valeur pour le paramètre advancedProofingOptions .

1. Une fois le BAT créé, utilisez l’API ProofHQ pour ajouter toutes les options avancées.

### Exemples

Cette section présente des exemples de mises à jour que vous pouvez effectuer avec l’API ProofHQ.

**Exemples:**

* [Un Bon à tirer peut être téléchargé, comporte un message et est partagé publiquement.](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [Mettre à jour une étape afin qu’elle ne soit pas privée, pas obligatoire et ne nécessite qu’une seule validation](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [Ajouter deux destinataires à un BAT sans décideur Principal](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**Un Bon à tirer peut être téléchargé, comporte un message et est partagé publiquement.**

La documentation de ce point de terminaison se trouve sur la page [Mise à jour de l’API ProofHQProof](https://api.proofhq.com/home/proofs/updateproof.html) page.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**Mettre à jour une étape afin qu’elle ne soit pas privée, pas obligatoire et ne nécessite qu’une seule validation**

La documentation de ce point de terminaison se trouve sur la page [API ProofHQ updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) page.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**Ajouter deux destinataires à un BAT sans décideur Principal**

La documentation de ce point de terminaison se trouve sur la page [API ProofHQ addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) page.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## Création d’un BAT à l’aide de JSON dans l’API Workfront

Cette section décrit comment créer un BAT avec des options de vérification avancées via l’API Workfront, en utilisant JSON comme valeur de paramètre dans l’API Workfront

### Créer un BAT avec des options de vérification avancées

Vous pouvez créer des bons à tirer à l’aide de l’API Workfront à l’aide du `Document createProof` action. Cette action accepte la variable `advancedProofingOptions` qui possède le type de valeur `string`. Pour inclure des options de vérification avancées dans votre `createProof` , vous devez saisir les options dans la variable `advancedProofingOptions` au format JSON.

>[!NOTE]
Il peut être difficile de prévoir les champs à inclure dans votre fichier JSON advancedProofingOptions. Vous pouvez examiner les données réseau de votre entreprise tout en utilisant la vérification avancée dans Workfront et baser votre code JSON sur les champs et les valeurs couramment utilisés par votre entreprise.
Comme ces champs peuvent être difficiles à prédire, nous vous recommandons de créer un BAT à l’aide de l’API Workfront, puis de le mettre à jour à l’aide de l’API ProofHQ. Pour plus d’informations, voir [Créer un BAT à l’aide des API Workfront et ProofHQ (recommandé)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) dans cet article

### Exemple

Cet exemple présente les champs et la mise en forme que vous pouvez utiliser lors de la création de votre fichier JSON pour le `advancedProofingOptions` . Votre `advancedProofingOptions` Le fichier JSON peut comporter plus ou moins de champs que celui illustré ici.

**Exemple:**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
