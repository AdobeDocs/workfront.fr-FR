---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Stockage de champ de texte enrichi dans l’API
description: Si un objet tel qu’un projet, un problème ou une tâche contient du texte enrichi, il est stocké et accessible en tant que valeur de paramètre via l’API Workfront.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: 3f7f4557c18bbb91ece850f910350d926a9e84bf
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 95%

---

# Stockage de champs de texte enrichi dans l’API

Si un objet tel qu’un projet, un problème ou une tâche contient du texte enrichi, il est stocké et accessible en tant que valeur de paramètre via l’API Workfront.

La demande d’informations textuelles à partir d’un objet de projet contenant du texte enrichi peut être effectuée à l’aide du champ **parameterValues**.

Par exemple, une requête HTTP simple peut ressembler à ce qui suit :

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

Si cet exemple de projet contenait un formulaire personnalisé avec trois champs personnalisés : calc field, paragraph text, et rich 1 (champ calculé, texte de paragraphe et enrichi 1), alors, la requête ci-dessus renverrait une réponse qui ressemblerait à ce qui suit, où le champ « rich 1 » est un champ de paramètre de texte enrichi et la valeur de texte est « **Hello** *World!* » :

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
                "blocks":[
                {
                    "key":"7eibh",
                    "text":"Hello Word!",
                    "type":"unstyled",
                    "depth":0,
                    "inlineStyleRanges":[
                    {
                        "offset":0,
                        "length":6,
                        "style":"BOLD"
                    },
                    {
                        "offset":6,
                        "length":5,
                        "style":"ITALIC"
                    }
                    ],
                    "entityRanges":[
                    ],
                "data":{
                }
                }
                ],
            "entityMap":{
            }
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

Pour une analyse plus approfondie de la manière dont les informations de texte enrichi sont stockées et peuvent être récupérées via l’API Adobe Workfront, voir [Champs de texte enrichi dans l’API Adobe Workfront](../../../wf-api/general/rich-text-field-api.md).
