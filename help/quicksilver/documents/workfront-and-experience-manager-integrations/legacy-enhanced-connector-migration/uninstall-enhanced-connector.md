---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Désinstallation de Workfront pour Adobe Experience Manager Enhanced Connector
description: Vous devez désinstaller Workfront avec le connecteur amélioré Adobe Experience Manager vers la dernière intégration native connectant Workfront et Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Désinstallation de Workfront avec Adobe Experience Manager Enhanced Connector

Vous devez désinstaller Workfront avec le connecteur amélioré Adobe Experience Manager vers la dernière intégration native connectant Workfront et Adobe Experience Manager Assets as a Cloud Service.

## Conditions préalables

* (Facultatif) Si nécessaire, annulez les modifications apportées à la configuration du pare-feu Workfront et aux paramètres du dispatcher AEM.

## Désinstaller le connecteur amélioré

1. Accédez à votre référentiel as a Cloud Service AEM et clonez-le à partir de Cloud Manager.

1. Ouvrez votre référentiel git cloné dans l’IDE de votre choix.

1. Extrayez la branche dans laquelle le connecteur amélioré est installé.

1. Accédez au chemin d’accès suivant et supprimez le fichier zip du connecteur amélioré :

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
   >Assurez-vous que la version référencée dans le bloc de code ci-dessus, c’est-à-dire la version 1.8.0, reflète la version en cours de désinstallation du code.

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
1. Supprimez l’élément suivant incorporé du fichier pom.xml du sous-module du projet nommé all.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. (Conditionnel) Supprimez la configuration du référentiel du fichier pom.xml de la racine du projet.


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. (Conditionnel) Supprimez la configuration du serveur du fichier settings.xml, situé dans le chemin suivant./cloudmanager/maven/settings.xml à la racine du projet.&#39;

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

1. Validez les modifications et envoyez le code vers le référentiel Cloud Manager.

1. Exécutez le pipeline Cloud Manager pour déployer les modifications sur votre instance Cloud Services.
