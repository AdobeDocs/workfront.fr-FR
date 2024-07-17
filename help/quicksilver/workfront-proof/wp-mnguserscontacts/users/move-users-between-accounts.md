---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: Déplacer des utilisateurs entre les comptes à l’aide de  [!DNL Workfront Proof]
description: Si vous êtes administrateur  [!DNL Workfront Proof] et qu'un ou plusieurs comptes satellites sont connectés à votre compte principal, vous pouvez déplacer les utilisateurs entre tous ces comptes.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Déplacer des utilisateurs entre des comptes à l’aide de [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Si vous êtes administrateur de BAT [!DNL Workfront] et qu&#39;un ou plusieurs comptes satellites sont connectés à votre compte principal, vous pouvez déplacer les utilisateurs entre tous ces comptes.

## Déplacement d’utilisateurs entre des comptes connectés

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]**.

1. Ouvrez l’onglet **[!UICONTROL Utilisateurs]** .
1. Cliquez sur l’icône **[!UICONTROL Déplacer l’utilisateur]** (1). ![Move_user2.png](assets/move-user2-350x95.png)

1. Dans la zone Déplacer l’utilisateur qui s’affiche, confirmez l’utilisateur à déplacer (1).
1. Sélectionnez un compte de destination dans la liste des comptes connectés (2).
1. Attribuez l’autorisation de profil (3) que cet utilisateur doit posséder sur le nouveau compte.
1. Sélectionnez un utilisateur (4) qui doit prendre en charge les éléments qui ne seront pas déplacés.
Cela inclut les éléments que vous décidez de laisser sur l’ancien compte et les éléments qui ne peuvent pas être déplacés (voir [Éléments qui ne peuvent pas être déplacés](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) ci-dessous).

1. Cochez les cases si vous souhaitez déplacer les bons à tirer (5) et les fichiers (6) avec l’utilisateur.
1. Créez un nom pour le dossier (7) dans lequel tous les éléments déplacés seront placés sur le nouveau compte.
1. Cliquez sur **[!UICONTROL Déplacer l’utilisateur]** (8) pour lancer le processus.
   ![Moving_users_pop-up.png](assets/moving-users-pop-up-350x380.png)

Si vous choisissez de déplacer l’utilisateur sans ses bons à tirer et ses fichiers, cette action sera exécutée immédiatement. Si vous choisissez de déplacer l’utilisateur avec ses bons à tirer et ses fichiers, le profil de l’utilisateur sera immédiatement réaffecté, mais les bons à tirer et les fichiers apparaîtront progressivement sur le compte de destination, car cette opération nécessite du temps pour transférer les données.

Selon le nombre de fichiers et le processus de déplacement des BAT, le temps de déplacement peut aller de quelques minutes à quelques heures.

>[!NOTE]
>
>Si vous pensez que le processus prend plus de temps que prévu ou que les bons à tirer et/ou les fichiers déplacés n’apparaissent pas sur le nouveau compte, contactez notre équipe d’assistance.

## Éléments qui ne peuvent pas être déplacés

### Dossiers créés ou détenus par l’utilisateur déplacé

En raison de la nature des différentes autorisations appliquées aux dossiers et à leur contenu (par exemple, ils peuvent être partagés avec d’autres utilisateurs et comptes), nous ne pouvons pas déplacer les structures de dossiers avec l’utilisateur.

Si un dossier appartient à l’utilisateur déplacé, la propriété est transférée à l’utilisateur sélectionné (4) dans la fenêtre contextuelle &quot;Déplacer l’utilisateur&quot;.

>[!NOTE]
>
>Si un dossier a été créé par l’utilisateur déplacé, il reste son créateur ; seule la propriété est transférée. Le dossier reste visible pour l’utilisateur déplacé dans la barre latérale de son nouveau compte. L’utilisateur déplacé disposera toujours d’un accès en lecture seule aux éléments placés dans ces dossiers.

Si vous ne souhaitez pas que l’utilisateur déplacé conserve ces autorisations ou que l’utilisateur déplacé ne souhaite pas voir ses anciens dossiers sur l’ancien compte, la solution ici serait de supprimer les dossiers comme suit :

1. Créez un dossier sur l’ancien compte.
1. Déplacez tous les éléments des dossiers de l’utilisateur déplacé vers le dossier nouvellement créé.
1. Supprimez tous les dossiers laissés par l’utilisateur déplacé.

### Jeux de versions avec différents propriétaires

Si un BAT comporte quelques versions et que chacune d’elles appartient à un utilisateur différent, les versions détenues par l’utilisateur déplacé ne seront pas déplacées. La propriété de ces versions sera transférée à un autre utilisateur selon votre choix (4) dans la zone Déplacer l’utilisateur . (Pour plus d’informations, voir .)

>[!NOTE]
>
>Un utilisateur déplacé doit posséder toutes les versions de BAT dans le jeu pour que le BAT soit déplacé.

### Groupes

Les groupes devront être recréés par l’utilisateur déplacé sur son nouveau compte. Pour plus d’informations, voir [Création de groupes de vérification à l’aide de [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### Vues personnalisées

Les vues personnalisées personnelles devront être recréées par l’utilisateur déplacé sur son nouveau compte. Pour plus d’informations, voir [Créer et gérer des vues personnalisées dans [!DNL Workfront Proof] Bon à tirer](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### Champs personnalisés

Les champs personnalisés ne peuvent pas être déplacés et les données des champs personnalisés seront perdues. Veillez donc à générer les rapports sur les éléments requis avant le déplacement.

### Modèles de workflow automatisés

Les modèles de workflow automatisés doivent être recréés sur le nouveau compte, mais les étapes seront conservées sur les bons à tirer déplacés créés avec les modèles.

### Actions sur les commentaires

Les actions sur les commentaires restent sur les bons à tirer, mais il ne sera plus possible de les filtrer. La solution serait de créer des actions correspondantes sur le nouveau compte et de marquer à nouveau les commentaires avec les nouvelles actions si nécessaire.
