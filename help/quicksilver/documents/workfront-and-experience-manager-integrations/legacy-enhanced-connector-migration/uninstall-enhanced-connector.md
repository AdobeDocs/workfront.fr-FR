---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Désinstaller le connecteur amélioré Workfront pour Adobe Experience Manager
description: Vous devez désinstaller le connecteur amélioré de Workfront avec Adobe Experience Manager pour passer à la dernière intégration native reliant Workfront et Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
TQID: https://experienceleague.adobe.com/CeCyF8zbwp4tVcxQebq0EdaJqagDyppVuCL6ilqEvJA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 260
ht-degree: 92%

---

# Désinstaller le connecteur amélioré Workfront with Adobe Experience Manager

Vous devez désinstaller le connecteur amélioré de Workfront avec Adobe Experience Manager pour passer à la dernière intégration native reliant Workfront et Adobe Experience Manager Assets as a Cloud Service.

## Conditions préalables

* (Facultatif) Si nécessaire, annulez les modifications apportées à la configuration du pare-feu Workfront et aux paramètres du dispatcher AEM.

## Désinstaller le connecteur amélioré

1. Accédez à votre référentiel AEM as a Cloud Service et clonez-le à partir de Cloud Manager.

1. Ouvrez votre dépôt git cloné dans l’IDE de votre choix.

1. Extrayez la branche où le connecteur amélioré est installé.

1. Naviguez jusqu’au chemin suivant et supprimez le fichier zip du connecteur amélioré :

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. Supprimez la dépendance suivante du fichier pom.xml de la racine du projet.

   ```
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >Veuillez vous assurer que la version référencée dans le bloc de code ci-dessus, c’est-à-dire 1.8.0, correspond à la version qui est désinstallée du code.

1. Supprimez la dépendance suivante du fichier pom.xml du sous-module du projet nommé **all**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. Supprimez l’élément suivant intégré au fichier pom.xml du sous-module du projet nommé all.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. (Ld cas échéant) Supprimez la configuration du référentiel du fichier pom.xml de la racine du projet.


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. (Conditionnel) Supprimez la configuration du serveur du fichier settings.xml, présent dans le chemin suivant ./cloudmanager/maven/settings.xml dans la racine du projet.&#39;

   ```
           <server>
           <id>hoodoo-maven</id>
           <configuration>
               <httpHeaders>
                   <property>
                       <name>Deploy-Token</name>
                       <value>*********************</value>
                   </property>
               </httpHeaders>
           </configuration>
       </server>
   ```

1. Valider les modifications et pousser le code vers le référentiel Cloud Manager.

1. Exécutez le pipeline Cloud Manager pour déployer les modifications sur votre instance Cloud Services.
